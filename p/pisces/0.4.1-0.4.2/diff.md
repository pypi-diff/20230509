# Comparing `tmp/pisces-0.4.1.tar.gz` & `tmp/pisces-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisces-0.4.1.tar", last modified: Fri Apr 28 21:58:59 2023, max compression
+gzip compressed data, was "pisces-0.4.2.tar", last modified: Tue May  9 16:55:48 2023, max compression
```

## Comparing `pisces-0.4.1.tar` & `pisces-0.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-04-28 21:58:45.000000 pisces-0.4.1/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-04-28 21:58:45.000000 pisces-0.4.1/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-28 21:58:45.000000 pisces-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-28 21:58:59.545687 pisces-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-28 21:58:45.000000 pisces-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.541687 pisces-0.4.1/pisces/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4997 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/pisces/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/db2db.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/drop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7781 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/mseed2db.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/sac2db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/commands/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/crud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/pisces/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/mseed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/readwaveform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28825 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/sac.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/trace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1965 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/io/util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20951 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/pisces/schema/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29149 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/antelope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31325 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/css3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36653 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/kbcore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15417 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/schema/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/pisces/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/tables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2080 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/tables/antelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/tables/css3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/tables/kbcore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23709 2023-04-28 21:58:45.000000 pisces-0.4.1/pisces/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.541687 pisces-0.4.1/pisces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 21:58:59.000000 pisces-0.4.1/pisces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:58:59.545687 pisces-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-04-28 21:58:45.000000 pisces-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:58:59.545687 pisces-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-28 21:58:45.000000 pisces-0.4.1/tests/test_readwaveform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8220 2023-04-28 21:58:45.000000 pisces-0.4.1/tests/test_schema_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-28 21:58:45.000000 pisces-0.4.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:48.684055 pisces-0.4.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-05-09 16:55:35.000000 pisces-0.4.2/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-05-09 16:55:35.000000 pisces-0.4.2/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-05-09 16:55:35.000000 pisces-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-09 16:55:48.684055 pisces-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-09 16:55:35.000000 pisces-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:48.680055 pisces-0.4.2/pisces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4997 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:48.684055 pisces-0.4.2/pisces/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/commands/db2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/commands/drop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7781 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/commands/mseed2db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/commands/sac2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/commands/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/crud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:48.684055 pisces-0.4.2/pisces/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/io/mseed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/io/readwaveform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28825 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/io/sac.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/io/trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1965 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/io/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20951 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:48.684055 pisces-0.4.2/pisces/schema/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/schema/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28291 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/schema/antelope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30373 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/schema/css3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35759 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/schema/kbcore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15417 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/schema/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:48.684055 pisces-0.4.2/pisces/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/tables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2080 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/tables/antelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/tables/css3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/tables/kbcore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23709 2023-05-09 16:55:35.000000 pisces-0.4.2/pisces/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:48.680055 pisces-0.4.2/pisces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-09 16:55:48.000000 pisces-0.4.2/pisces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-09 16:55:48.000000 pisces-0.4.2/pisces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:55:48.000000 pisces-0.4.2/pisces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-09 16:55:48.000000 pisces-0.4.2/pisces.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 16:55:48.000000 pisces-0.4.2/pisces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 16:55:48.000000 pisces-0.4.2/pisces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:55:48.684055 pisces-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-05-09 16:55:35.000000 pisces-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:55:48.684055 pisces-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-09 16:55:35.000000 pisces-0.4.2/tests/test_readwaveform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8220 2023-05-09 16:55:35.000000 pisces-0.4.2/tests/test_schema_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-09 16:55:35.000000 pisces-0.4.2/tests/test_util.py
```

### Comparing `pisces-0.4.1/LICENSE.txt` & `pisces-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/MANIFEST.in` & `pisces-0.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/PKG-INFO` & `pisces-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pisces
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Practical Seismological Database Library in Python.
 Home-page: https://github.com/LANL-Seismoacoustics/pisces
-Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.3.2
+Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.4.2
 Author: Jonathan MacCarthy
 Author-email: jkmacc@lanl.gov
 License: LANL-MIT
 Keywords: seismology,geophysics,database
 Platform: Mac OS X
 Platform: Linux/Unix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pisces-0.4.1/README.md` & `pisces-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/__init__.py` & `pisces-0.4.2/pisces/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
 The ultimate goal of Pisces is to allow the user to write code that will not 
 eventually have to be abandoned due to different project scales, system 
 architectures, or licensing concerns.  
 
 """
 
-__version__ = '0.3.2'
+__version__ = '0.4.2'
 
 from pisces.util import db_connect, get_tables, travel_times, make_table
 from pisces.schema.util import string_formatter
 from pisces.io.trace import wfdisc2trace
 from pisces.schema import kbcore
 from pisces.io.readwaveform import read_waveform
```

### Comparing `pisces-0.4.1/pisces/client.py` & `pisces-0.4.2/pisces/client.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/commands/main.py` & `pisces-0.4.2/pisces/commands/main.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/commands/mseed2db.py` & `pisces-0.4.2/pisces/commands/mseed2db.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/commands/sac2db.py` & `pisces-0.4.2/pisces/commands/sac2db.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/commands/util.py` & `pisces-0.4.2/pisces/commands/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/crud.py` & `pisces-0.4.2/pisces/crud.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/io/mseed.py` & `pisces-0.4.2/pisces/io/mseed.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/io/readwaveform.py` & `pisces-0.4.2/pisces/io/readwaveform.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/io/sac.py` & `pisces-0.4.2/pisces/io/sac.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/io/trace.py` & `pisces-0.4.2/pisces/io/trace.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/io/util.py` & `pisces-0.4.2/pisces/io/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/request.py` & `pisces-0.4.2/pisces/request.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/schema/antelope.py` & `pisces-0.4.2/pisces/schema/css3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,760 +1,940 @@
+# Converted to Python 3.5.2 on 01-25-17
+# by: Jeremy Webster
+
 # coding: utf-8
 """
-Antelope v4.11 Datascope database schema
+Center for Seismic Studies relational database schema 3.0 (CSS3.0)
 
 
 """
 from datetime import datetime
-from sqlalchemy import Date, DateTime, Float, Numeric, String, Integer
-from sqlalchemy import Column, Table, func
-from sqlalchemy import PrimaryKeyConstraint, UniqueConstraint, Index
+from sqlalchemy import DateTime, Float, String, Integer
+from sqlalchemy import Column
+from sqlalchemy import PrimaryKeyConstraint, UniqueConstraint
 from sqlalchemy.orm import declarative_base
 from sqlalchemy.ext.declarative import declared_attr
 
 from obspy.core import UTCDateTime
 from pisces.schema.util import PiscesMeta
 from pisces.schema.util import parse_int, parse_float, parse_str
 
 from pisces.io.trace import wfdisc2trace
+from copy import deepcopy as dc
 
 Base = declarative_base(metaclass=PiscesMeta, constructor=None)
 
 # COLUMN DEFINITIONS
 # Generic SQLA types, compatible with different backends
 # !! info dictionary defines the external representations (NumPy, text files)
 #   and default values for the mapped class representation.
+#
 # XXX: for numeric types, maximum width is not enforced!
+#
 # NOTE: info['dtype'] for floats/ints should match the system default for Python
 #       "{:f}".format(numpyfloat/int) to work, b/c it can use the builtin float
 #       __format__().  use 'float' or 'int'
 #       See:
 #       http://stackoverflow.com/questions/16928644/floats-in-numpy-structured-array-and-native-string-formatting-with-format
 
+
 def strip(s):
     return str(s).strip()
 
+
 DATEFMT = '%y-%m-%d %H:%M:%S'
+
+
 def dtfn(s):
     try:
         dt = datetime.strptime(s.strip(), DATEFMT)
     except ValueError:
         # Antelope convention
         dt = UTCDateTime(float(s)).datetime
     return dt
 
 
 algorithm = Column(String(15),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+                   info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+
 amp = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 10, 'format': '10.1f'})
+             info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 10, 'format': '10.1f'})
+
 ampid = Column(Integer, nullable=False,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
-amptime = Column(Float(53), info={'default': -9999999999.999,
-        'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
+               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
+
+amptime = Column(Float(53),
+                 info={'default': -9999999999.999, 'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
+
 amptype = Column(String(8),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+
 arid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 auth = Column(String(15),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15s'})
+              info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15s'})
+
 azdef = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 azimuth = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+                 info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 azres = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.1f'})
+               info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.1f'})
+
 band = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+              info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 belief = Column(Float(24),
-        info={'default': -9.99, 'parse': parse_float, 'dtype': 'float', 'width': 4, 'format': '4.2f'})
+                info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 4, 'format': '4.2f'})
+
 calib = Column(Float(24),
-        info={'default': 0.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.9f'})
+               info={'default': 1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+
 calper = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+                info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+
 calratio = Column(Float(24),
-        info={'default': 1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+                  info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+
 chan = Column(String(8),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+              info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+
 chanid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 clip = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+              info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 commid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 conf = Column(Float(24),
-        info={'default': 0, 'parse': parse_float, 'dtype': 'float', 'width': 5, 'format': '5.3f'})
+              info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 5, 'format': '5.3f'})
+
 ctype = Column(String(4),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
+
 datatype = Column(String(2),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a2', 'width': 2, 'format': '2.2s'})
+                  info={'default': '-', 'parse': parse_str, 'dtype': 'a2', 'width': 2, 'format': '2.2s'})
+
 deast = Column(Float(24),
-        info={'default': 0.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+               info={'default': 0.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 delaz = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+               info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 delslo = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+                info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 delta = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8.3f'})
+               info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8.3f'})
+
 deltaf = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.3f'})
+                info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.3f'})
+
 deltim = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.3f'})
+                info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.3f'})
+
 depdp = Column(Float(24),
-        info={'default': -999, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+               info={'default': -999, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 depth = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+               info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 descrip = Column(String(50),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a50', 'width': 50, 'format': '50.50s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a50', 'width': 50, 'format': '50.50s'})
+
 dfile = Column(String(32),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a32', 'width': 32, 'format': '32.32s'})
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a32', 'width': 32, 'format': '32.32s'})
+
 digital = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 dir = Column(String(64),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a64', 'width': 64, 'format': '64.64s'})
+             info={'default': '-', 'parse': parse_str, 'dtype': 'a64', 'width': 64, 'format': '64.64s'})
+
+dist = Column(Float(24),
+              info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 dnorth = Column(Float(24),
-        info={'default': 0.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+                info={'default': 0.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 dtype = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 duration = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+                  info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 edepth = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+                info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 elev = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+              info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 ema = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+             info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 emares = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.1f'})
-endtime = Column(Float(53), info={'default':  9999999999.999,
-        'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
+                info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.1f'})
+
+endtime = Column(Float(53),
+                 info={'default': 9999999999.999, 'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
+
 esaz = Column(Float(24),
-        info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
-etype = Column(String(2),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a2', 'width': 2, 'format': '2.2s'})
+              info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
+etype = Column(String(7),
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a7', 'width': 7, 'format': '7.7s'})
+
 evid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 evname = Column(String(15),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+
 fm = Column(String(2),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a2', 'width': 2, 'format': '2.2s'})
+            info={'default': '-', 'parse': parse_str, 'dtype': 'a2', 'width': 2, 'format': '2.2s'})
+
 foff = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 10, 'format': '10d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 10, 'format': '10d'})
+
 grn = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+             info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 grname = Column(String(40),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a40', 'width': 40, 'format': '40.40s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a40', 'width': 40, 'format': '40.40s'})
+
 hang = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.1f'})
+              info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.1f'})
+
+imb = Column(Float(24),
+             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
+iml = Column(Float(24),
+             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
+ims = Column(Float(24),
+             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 inarrival = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+                   info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 inid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 insname = Column(String(50),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a50', 'width': 50, 'format': '50.50s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a50', 'width': 50, 'format': '50.50s'})
+
 instant = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 instype = Column(String(6),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+
 iphase = Column(String(8),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+
 jdate = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 keyname = Column(String(15),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+
 keyvalue = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
-lat = Column(Float(53),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+                  info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
+lat = Column(Float(24),
+             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 lddate = Column(DateTime, nullable=False, onupdate=datetime.now,
-        info={'default': datetime.now, 'parse': dtfn, 'dtype': 'O', 'width': 17, 'format': DATEFMT})
+                info={'default': datetime.now, 'parse': dtfn, 'dtype': 'O', 'width': 17, 'format': DATEFMT})
+
 lineno = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
+location = Column(String(32),
+                  info={'default': '-', 'parse': parse_str, 'dtype': 'a32', 'width': 32, 'format': '32.32s'})
+
 logat = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
-lon = Column(Float(53),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+               info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
+lon = Column(Float(24),
+             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 magid = Column(Integer, nullable=False,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 magnitude = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+                   info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 magres = Column(Float(24),
-        info={'default': -999, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+                info={'default': -999, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 magdef = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 magtype = Column(String(6),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+
 mb = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+            info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 mbid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 ml = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+            info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 mlid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 ms = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+            info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 msid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 mmodel = Column(String(15),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+
 nass = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 4, 'format': '4d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 4, 'format': '4d'})
+
 ncalib = Column(Float(24),
-        info={'default': 1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+                info={'default': 1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+
 ncalper = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+                 info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.6f'})
+
 ndef = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 4, 'format': '4d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 4, 'format': '4d'})
+
 ndp = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 4, 'format': '4d'})
+             info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 4, 'format': '4d'})
+
 net = Column(String(8),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+             info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+
 netname = Column(String(80),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a80', 'width': 80, 'format': '80.80s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a80', 'width': 80, 'format': '80.80s'})
+
 nettype = Column(String(4),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
+
 nsamp = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 nsta = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 offdate = Column(Integer,
-        info={'default': 2286324, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                 info={'default': 2286324, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 ondate = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 orid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 parid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
+
 per = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+             info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 phase = Column(String(8),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+
 prefor = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 qual = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+              info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 rect = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.3f'})
+              info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.3f'})
+
 refsta = Column(String(6),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+
 remark = Column(String(80),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a80', 'width': 80, 'format': '80.80s'})
-review =  Column(String(4),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a80', 'width': 80, 'format': '80.80s'})
+
 rsptype = Column(String(6),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+
 samprate = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 11, 'format': '11.7f'})
+                  info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 11, 'format': '11.7f'})
+
 sdepth = Column(Float(24),
-        info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+                info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 sdobs = Column(Float(24),
-        info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+               info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 seaz = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+              info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 segtype = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 slodef = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 slores = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+                info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 slow = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float','width': 7, 'format': '7.2f'})
+              info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
 smajax = Column(Float(24),
-        info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+                info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 sminax = Column(Float(24),
-        info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+                info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+
 snr = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 10, 'format': '10.5f'})
+             info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 10, 'format': '10.2f'})
+
 srn = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+             info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 srname = Column(String(40),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a40', 'width': 40, 'format': '40.40s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a40', 'width': 40, 'format': '40.40s'})
+
 sta = Column(String(6),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+             info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+
 staname = Column(String(50),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a50', 'width': 50, 'format': '50.50s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a50', 'width': 50, 'format': '50.50s'})
+
 stassid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                 info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 statype = Column(String(4),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
+
 stime = Column(Float(24),
-        info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8.2f'})
+               info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8.2f'})
+
 strike = Column(Float(24),
-        info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.2f'})
+                info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.2f'})
+
 stt = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 stx = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 sty = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 stype = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 stz = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 sxx = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 sxy = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 sxz = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 syy = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 syz = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 szz = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+             info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
+
 tagid = Column(Integer,
-        info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8d'})
+               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 tagname = Column(String(8),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
+
 time = Column(Float(53),
-        info={'default': -9999999999.999, 'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
-timedef = Column(String(1),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+              info={'default': -9999999999.999, 'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
+
+timedef = Column(String(1), info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+
 timeres = Column(Float(24),
-        info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8.3f'})
+                 info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8.3f'})
+
 tshift = Column(Float(24),
-        info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.2f'})
+                info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.2f'})
+
 uncertainty = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
-units = Column(String(12),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a12', 'width': 12, 'format': '12.12s'})
+                     info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
+
+units = Column(String(15),
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+
 vang = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.1f'})
+              info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.1f'})
+
 vmodel = Column(String(15),
-        info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+
 wfid = Column(Integer,
-        info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+
 wgt = Column(Float(24),
-        info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.3f'})
+             info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.3f'})
+
 
 class Affiliation(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('net', 'sta', 'time'),)
+        return (PrimaryKeyConstraint('net', 'sta'),)
 
-    net = net.copy()
-    sta = sta.copy()
-    lddate = lddate.copy()
+    net = dc(net)
+    sta = dc(sta)
+    lddate = dc(lddate)
 
 
 class Amplitude(Base):
-    __abstract__ =True
+    __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('ampid'),)
 
-    ampid = ampid._copy()
-    arid = arid._copy()
-    parid = parid._copy()
-    chan = chan._copy()
-    amp = amp._copy()
-    per = per._copy()
-    snr = snr._copy()
-    amptime = amptime._copy()
-    time = time._copy()
-    duration = duration._copy()
-    deltaf = deltaf._copy()
-    amptype = amptype._copy()
-    units = units._copy()
-    clip = clip._copy()
-    inarrival = inarrival._copy()
-    auth = auth._copy()
-    lddate = lddate._copy()
+    ampid = dc(ampid)
+    arid = dc(arid)
+    parid = dc(parid)
+    chan = dc(chan)
+    amp = dc(amp)
+    per = dc(per)
+    snr = dc(snr)
+    amptime = dc(amptime)
+    time = dc(time)
+    duration = dc(duration)
+    deltaf = dc(deltaf)
+    amptype = dc(amptype)
+    units = dc(units)
+    clip = dc(clip)
+    inarrival = dc(inarrival)
+    auth = dc(auth)
+    lddate = dc(lddate)
 
 
 class Arrival(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('arid'),
-                UniqueConstraint(u'sta', u'time', u'chan', u'iphase', u'auth'),)
+                UniqueConstraint('sta', 'time', 'chan', 'iphase', 'auth'),)
 
-    sta = sta._copy()
-    time = time._copy()
-    arid = arid._copy()
-    jdate = jdate._copy()
-    stassid = stassid._copy()
-    chanid = chanid._copy()
-    chan = chan._copy()
-    iphase = iphase._copy()
-    stype = stype._copy()
-    deltim = deltim._copy()
-    azimuth = azimuth._copy()
-    delaz = delaz._copy()
-    slow = slow._copy()
-    delslo = delslo._copy()
-    ema = ema._copy()
-    rect = rect._copy()
-    amp = amp._copy()
-    per = per._copy()
-    logat = logat._copy()
-    clip = clip._copy()
-    fm = fm._copy()
-    snr = snr._copy()
-    qual = qual._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    time = dc(time)
+    arid = dc(arid)
+    jdate = dc(jdate)
+    stassid = dc(stassid)
+    chanid = dc(chanid)
+    chan = dc(chan)
+    iphase = dc(iphase)
+    stype = dc(stype)
+    deltim = dc(deltim)
+    azimuth = dc(azimuth)
+    delaz = dc(delaz)
+    slow = dc(slow)
+    delslo = dc(delslo)
+    ema = dc(ema)
+    rect = dc(rect)
+    amp = dc(amp)
+    per = dc(per)
+    logat = dc(logat)
+    clip = dc(clip)
+    fm = dc(fm)
+    snr = dc(snr)
+    qual = dc(qual)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Assoc(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('arid','orid'),
-                UniqueConstraint('arid'),)
+        return (PrimaryKeyConstraint('arid', 'orid'), UniqueConstraint('arid'), )
 
-    arid = arid._copy()
-    orid = orid._copy()
-    sta = sta._copy()
-    phase = phase._copy()
-    belief = belief._copy()
-    delta = delta._copy()
-    seaz = seaz._copy()
-    esaz = esaz._copy()
-    timeres = timeres._copy()
-    timedef = timedef._copy()
-    azres = azres._copy()
-    azdef = azdef._copy()
-    slores = slores._copy()
-    slodef = slodef._copy()
-    emares = emares._copy()
-    wgt = wgt._copy()
-    vmodel = vmodel._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    arid = dc(arid)
+    orid = dc(orid)
+    sta = dc(sta)
+    phase = dc(phase)
+    belief = dc(belief)
+    delta = dc(delta)
+    seaz = dc(seaz)
+    esaz = dc(esaz)
+    timeres = dc(timeres)
+    timedef = dc(timedef)
+    azres = dc(azres)
+    azdef = dc(azdef)
+    slores = dc(slores)
+    slodef = dc(slodef)
+    emares = dc(emares)
+    wgt = dc(wgt)
+    vmodel = dc(vmodel)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Event(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('evid'),
-                UniqueConstraint('prefor'),)
+        return (PrimaryKeyConstraint('evid'), UniqueConstraint('prefor'),)
 
-    evid = evid._copy()
-    evname = evname._copy()
-    prefor = prefor._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    evid = dc(evid)
+    evname = dc(evname)
+    prefor = dc(prefor)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Gregion(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('grn'),)
 
-    grn = grn._copy()
-    grname = grname._copy()
-    lddate = lddate._copy()
+    grn = dc(grn)
+    grname = dc(grname)
+    lddate = dc(lddate)
 
 
 class Instrument(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('inid'),)
 
-    inid = inid._copy()
-    insname = insname._copy()
-    instype = instype._copy()
-    band = band._copy()
-    digital = digital._copy()
-    samprate = samprate._copy()
-    ncalib = ncalib._copy()
-    ncalper = ncalper._copy()
-    dir = dir._copy()
-    dfile = dfile._copy()
-    rsptype = rsptype._copy()
-    lddate = lddate._copy()
+    inid = dc(inid)
+    insname = dc(insname)
+    instype = dc(instype)
+    band = dc(band)
+    digital = dc(digital)
+    samprate = dc(samprate)
+    ncalib = dc(ncalib)
+    ncalper = dc(ncalper)
+    dir = dc(dir)
+    dfile = dc(dfile)
+    rsptype = dc(rsptype)
+    lddate = dc(lddate)
 
 
 class Lastid(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('keyname'),
-                UniqueConstraint(u'keyname', u'keyvalue'),)
+        return (PrimaryKeyConstraint('keyname'), UniqueConstraint('keyname', 'keyvalue'),)
 
-    keyname = keyname._copy()
-    keyvalue = keyvalue._copy()
-    lddate = lddate._copy()
+    keyname = dc(keyname)
+    keyvalue = dc(keyvalue)
+    lddate = dc(lddate)
 
 
 class Netmag(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('magid'),
                 UniqueConstraint('magid', 'orid'),)
 
-    magid = magid._copy()
-    net = net._copy()
-    orid = orid._copy()
-    evid = evid._copy()
-    magtype = magtype._copy()
-    nsta = nsta._copy()
-    magnitude = magnitude._copy()
-    uncertainty = uncertainty._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    magid = dc(magid)
+    net = dc(net)
+    orid = dc(orid)
+    evid = dc(evid)
+    magtype = dc(magtype)
+    nsta = dc(nsta)
+    magnitude = dc(magnitude)
+    uncertainty = dc(uncertainty)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Network(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('net'),)
 
-    net = net.copy()
-    netname = netname._copy()
-    nettype = nettype._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    net = dc(net)
+    netname = dc(netname)
+    nettype = dc(nettype)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Origerr(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('orid'),)
 
-    orid = orid._copy()
-    sxx = sxx._copy()
-    syy = syy._copy()
-    szz = szz._copy()
-    stt = stt._copy()
-    sxy = sxy._copy()
-    sxz = sxz._copy()
-    syz = syz._copy()
-    stx = stx._copy()
-    sty = sty._copy()
-    stz = stz._copy()
-    sdobs = sdobs._copy()
-    smajax = smajax._copy()
-    sminax = sminax._copy()
-    strike = strike._copy()
-    sdepth = sdepth._copy()
-    stime = stime._copy()
-    conf = conf._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    orid = dc(orid)
+    sxx = dc(sxx)
+    syy = dc(syy)
+    szz = dc(szz)
+    stt = dc(stt)
+    sxy = dc(sxy)
+    sxz = dc(sxz)
+    syz = dc(syz)
+    stx = dc(stx)
+    sty = dc(sty)
+    stz = dc(stz)
+    sdobs = dc(sdobs)
+    smajax = dc(smajax)
+    sminax = dc(sminax)
+    strike = dc(strike)
+    sdepth = dc(sdepth)
+    stime = dc(stime)
+    conf = dc(conf)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Origin(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (UniqueConstraint('lat','lon','depth','time','auth'),
-                PrimaryKeyConstraint('orid'),)
+        return (UniqueConstraint('lat', 'lon', 'depth', 'time', 'auth'), PrimaryKeyConstraint('orid'))
 
-    lat = lat._copy()
-    lon = lon._copy()
-    depth = depth._copy()
-    time = time._copy()
-    orid = orid._copy()
-    evid = evid._copy()
-    jdate = jdate._copy()
-    nass = nass._copy()
-    ndef = ndef._copy()
-    ndp = ndp._copy()
-    grn = grn._copy()
-    srn = srn._copy()
-    etype = etype._copy()
-    review = review._copy()
-    depdp = depdp._copy()
-    dtype = dtype._copy()
-    mb = mb._copy()
-    mbid = mbid._copy()
-    ms = ms._copy()
-    msid = msid._copy()
-    ml = ml._copy()
-    mlid = mlid._copy()
-    algorithm = algorithm._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    lat = dc(lat)
+    lon = dc(lon)
+    depth = dc(depth)
+    time = dc(time)
+    orid = dc(orid)
+    evid = dc(evid)
+    jdate = dc(jdate)
+    nass = dc(nass)
+    ndef = dc(ndef)
+    ndp = dc(ndp)
+    grn = dc(grn)
+    srn = dc(srn)
+    etype = dc(etype)
+    depdp = dc(depdp)
+    dtype = dc(dtype)
+    mb = dc(mb)
+    mbid = dc(mbid)
+    ms = dc(ms)
+    msid = dc(msid)
+    ml = dc(ml)
+    mlid = dc(mlid)
+    algorithm = dc(algorithm)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Remark(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('commid','lineno'),)
+        return (PrimaryKeyConstraint('commid', 'lineno'),)
 
-    commid = commid._copy()
-    lineno = lineno._copy()
-    remark = remark._copy()
-    lddate = lddate._copy()
+    commid = dc(commid)
+    lineno = dc(lineno)
+    remark = dc(remark)
+    lddate = dc(lddate)
 
 
 class Sensor(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('sta','chan','time','endtime'),)
+        return (PrimaryKeyConstraint('sta', 'chan', 'time', 'endtime'),)
 
-    sta = sta._copy()
-    chan = chan._copy()
-    time = time._copy()
-    endtime = endtime._copy()
-    inid = inid._copy()
-    chanid = chanid._copy()
-    jdate = jdate._copy()
-    calratio = calratio._copy()
-    calper = calper._copy()
-    tshift = tshift._copy()
-    instant = instant._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    chan = dc(chan)
+    time = dc(time)
+    endtime = dc(endtime)
+    inid = dc(inid)
+    chanid = dc(chanid)
+    jdate = dc(jdate)
+    calratio = dc(calratio)
+    calper = dc(calper)
+    tshift = dc(tshift)
+    instant = dc(instant)
+    lddate = dc(lddate)
 
 
 class Site(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('sta','ondate'),)
+        return (PrimaryKeyConstraint('sta', 'ondate'),)
 
-    sta = sta._copy()
-    ondate = ondate._copy()
-    offdate = offdate._copy()
-    lat = lat._copy()
-    lon = lon._copy()
-    elev = elev._copy()
-    staname = staname._copy()
-    statype = statype._copy()
-    refsta = refsta._copy()
-    dnorth = dnorth._copy()
-    deast = deast._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    ondate = dc(ondate)
+    offdate = dc(offdate)
+    lat = dc(lat)
+    lon = dc(lon)
+    elev = dc(elev)
+    staname = dc(staname)
+    statype = dc(statype)
+    refsta = dc(refsta)
+    dnorth = dc(dnorth)
+    deast = dc(deast)
+    lddate = dc(lddate)
 
 
 class Sitechan(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (UniqueConstraint('sta','chan','ondate'),
-                PrimaryKeyConstraint('sta','chan','ondate','offtime'),)
+        return (UniqueConstraint('sta', 'chan', 'ondate'),
+                PrimaryKeyConstraint('chanid'),)
 
-    sta = sta._copy()
-    chan = chan._copy()
-    ondate = ondate._copy()
-    chanid = chanid._copy()
-    offdate = offdate._copy()
-    ctype = ctype._copy()
-    edepth = edepth._copy()
-    hang = hang._copy()
-    vang = vang._copy()
-    descrip = descrip._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    chan = dc(chan)
+    ondate = dc(ondate)
+    chanid = dc(chanid)
+    offdate = dc(offdate)
+    ctype = dc(ctype)
+    edepth = dc(edepth)
+    hang = dc(hang)
+    vang = dc(vang)
+    descrip = dc(descrip)
+    lddate = dc(lddate)
 
 
 class Sregion(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('srn'),)
 
-    srn = srn.copy()
-    srname = srname._copy()
-    lddate = lddate.copy()
+    srn = dc(srn)
+    srname = dc(srname)
+    lddate = dc(lddate)
 
 
 class Stamag(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('magid', 'sta', 'arid'),)
-
-    magid = magid.copy()
-    sta = sta.copy()
-    arid = arid.copy()
-    orid = orid.copy()
-    evid = evid.copy()
-    phase = phase.copy()
-    magtype = magtype.copy()
-    magnitude = magnitude.copy()
-    uncertainty = uncertainty.copy()
-    auth = auth.copy()
-    commid = commid.copy()
-    lddate = lddate._copy()
+        return (PrimaryKeyConstraint('magid', 'sta'),)
 
+    magid = dc(magid)
+    sta = dc(sta)
+    arid = dc(arid)
+    orid = dc(orid)
+    evid = dc(evid)
+    phase = dc(phase)
+    delta = dc(delta)
+    magtype = dc(magtype)
+    magnitude = dc(magnitude)
+    uncertainty = dc(uncertainty)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
+    
+    
+class Stassoc(Base):
+    __abstract__ = True
+    
+    @declared_attr
+    def __table_args__(cls):
+        return (PrimaryKeyConstraint('stassid'),)
+        
+    stassid = dc(stassid)
+    sta = dc(sta)
+    etype = dc(etype)
+    location = dc(location)
+    dist = dc(dist)
+    azimuth = dc(azimuth)
+    lat = dc(lat)
+    lon = dc(lon)
+    depth = dc(depth)
+    time = dc(time)
+    imb = dc(imb)
+    ims = dc(ims)
+    iml = dc(iml)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
+        
 
 class Wfdisc(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (UniqueConstraint('wfid','dir','dfile'),
-                PrimaryKeyConstraint('wfid'),)
+        return (UniqueConstraint('wfid', 'dir', 'dfile'), PrimaryKeyConstraint('wfid'),)
 
     def to_trace(self):
-         """
-         Read the wfdisc line into a Trace instance.  Minimal header.
+        """
+        Read the wfdisc line into a Trace instance.  Minimal header.
 
-         Returns
-         -------
-         obspy.Trace
-
-         """
-         return wfdisc2trace(self)
-
-    sta = sta._copy()
-    chan = chan._copy()
-    time = time._copy()
-    wfid = wfid._copy()
-    chanid = chanid._copy()
-    jdate = jdate._copy()
-    endtime = endtime._copy()
-    nsamp = nsamp._copy()
-    samprate = samprate._copy()
-    calib = calib._copy()
-    calper = calper._copy()
-    instype = instype._copy()
-    segtype = segtype._copy()
-    datatype = datatype._copy()
-    clip = clip._copy()
-    dir = dir._copy()
-    dfile = dfile._copy()
-    foff = foff._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+        Returns
+        -------
+        obspy.Trace
+
+        """
+        return wfdisc2trace(self)
+
+    sta = dc(sta)
+    chan = dc(chan)
+    time = dc(time)
+    wfid = dc(wfid)
+    chanid = dc(chanid)
+    jdate = dc(jdate)
+    endtime = dc(endtime)
+    nsamp = dc(nsamp)
+    samprate = dc(samprate)
+    calib = dc(calib)
+    calper = dc(calper)
+    instype = dc(instype)
+    segtype = dc(segtype)
+    datatype = dc(datatype)
+    clip = dc(clip)
+    dir = dc(dir)
+    dfile = dc(dfile)
+    foff = dc(foff)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Wftag(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('tagid'),
-                UniqueConstraint('tagname','tagid','wfid'),)
-
-    tagname = tagname._copy()
-    tagid = tagid._copy()
-    wfid = wfid._copy()
-    lddate = lddate._copy()
-
+        return (PrimaryKeyConstraint('tagname', 'tagid', 'wfid'),)
 
+    tagname = dc(tagname)
+    tagid = dc(tagid)
+    wfid = dc(wfid)
+    lddate = dc(lddate)
```

### Comparing `pisces-0.4.1/pisces/schema/css3.py` & `pisces-0.4.2/pisces/schema/kbcore.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,140 @@
 # Converted to Python 3.5.2 on 01-25-17
 # by: Jeremy Webster
 
+
 # coding: utf-8
 """
-Center for Seismic Studies relational database schema 3.0 (CSS3.0)
+Core columns and abstract classes representing the KB Core seismic schema.
+
+ORM classes that inherit from these classes are guaranteed primary and unique
+keys, column info dictionaries, and schema-qualified __tablename__ .
 
+Examples
+--------
+Define a site class that points to a 'TA_site' table.
+
+>>> import pisces.schema.kbcore as kb
+>>>
+>>> class Site(kb.Site):
+>>>     __tablename__ = 'TA_site'
+
+Define a site class that points to a 'jkmacc.my_site' table.
+
+>>> import pisces.schema.kbcore as kb
+>>>
+>>> class Site(kb.Site):
+>>>     __tablename__ = 'jkmacc.my_site'
+
+Create this table, if it doesn't exist.
+
+>>> import sqlalchemy as sa
+>>> e = sa.create_engine('sqlite:///my.sqlite')
+>>> if not Site.__table__.exists(e)
+>>>     Site.__table__.create(e)
+
+Define a new abstract class in this schema.
+
+>>> import sqlalchemy as sa
+>>> from sqlalchemy.ext.declarative import declared_attr
+>>> import pisces.schema.kbcore as kb
+>>> from copy import deepcopy as dc
+>>>
+>>> def strparse(s):
+>>>     return s.strip()
+>>>
+>>> class Beam(kb.Base):
+>>>     __abstract__ = True
+>>>     @declared_attr
+>>>     def __table_args__(cls):
+>>>         return (sa.PrimaryKeyConstraint('wfid'),)
+>>>
+>>>     wfid = kb.wfid._copy()
+>>>     azimuth = dc(kb.azimuth)
+>>>     slo = sa.Column(Float(24),
+>>>         info={'default': -1.0, 'parse': float, 'width': 7, 'format': '7.4f'})
+>>>     filter = sa.Column(String(30),
+>>>         info={'default': '-', 'parse': strparse, 'width': 30, 'format': '30.30s'})
+>>>     recipe = sa.Column(String(15),
+>>>         info={'default': '-', 'parse': strparse, 'width': 15, 'format': '15.15s'})
+>>>     algorithm = dc(kb.algorithm)
+>>>     auth = dc(kb.auth)
+>>>     lddate = dc(kb.lddate)
 
 """
 from datetime import datetime
+
 from sqlalchemy import DateTime, Float, String, Integer
 from sqlalchemy import Column
 from sqlalchemy import PrimaryKeyConstraint, UniqueConstraint
 from sqlalchemy.orm import declarative_base
 from sqlalchemy.ext.declarative import declared_attr
 
-from obspy.core import UTCDateTime
 from pisces.schema.util import PiscesMeta
-from pisces.schema.util import parse_int, parse_float, parse_str
-
+from pisces.schema.util import parse_str, parse_int, parse_float
 from pisces.io.trace import wfdisc2trace
+from copy import deepcopy as dc
+
+# TODO: check __table_args__ syntax for final empty {}
+# TODO: use http://docs.sqlalchemy.org/en/rel_0_8/orm/extensions/hybrid.html?
 
 Base = declarative_base(metaclass=PiscesMeta, constructor=None)
 
 # COLUMN DEFINITIONS
 # Generic SQLA types, compatible with different backends
 # !! info dictionary defines the external representations (NumPy, text files)
 #   and default values for the mapped class representation.
-#
 # XXX: for numeric types, maximum width is not enforced!
-#
 # NOTE: info['dtype'] for floats/ints should match the system default for Python
 #       "{:f}".format(numpyfloat/int) to work, b/c it can use the builtin float
 #       __format__().  use 'float' or 'int'
 #       See:
 #       http://stackoverflow.com/questions/16928644/floats-in-numpy-structured-array-and-native-string-formatting-with-format
-
-
-def strip(s):
-    return str(s).strip()
-
-
-DATEFMT = '%y-%m-%d %H:%M:%S'
+# NOTE: column names are not defined here, they are assigned during declarative
+#       table definitions.  i.e. amp.name is None until it is used later.  This
+#       allows recycling columns as different names, like sta1 = dc(sta1)).
+
+# TODO: write a parser that gets the width (and type?) from info['format']
+
+# specialized string parsing functions
+
+# TODO: use dateutil module to handle wildcard characters, etc.?
+# https://docs.python.org/2.7/library/datetime.html#strftime-strptime-behavior
+# https://docs.python.org/2/library/string.html#format-specification-mini-language
+DATEFMT = '%Y-%m-%d %H:%M:%S'
 
 
 def dtfn(s):
     try:
-        dt = datetime.strptime(s.strip(), DATEFMT)
+        val = datetime.strptime(s, DATEFMT)
     except ValueError:
-        # Antelope convention
-        dt = UTCDateTime(float(s)).datetime
-    return dt
+        val = None
+    return val
 
 
 algorithm = Column(String(15),
                    info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
 
 amp = Column(Float(24),
-             info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 10, 'format': '10.1f'})
+             info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 11, 'format': '11.2f'})
 
 ampid = Column(Integer, nullable=False,
                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
-amptime = Column(Float(53),
-                 info={'default': -9999999999.999, 'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
+amptime = Column(Float(53), info={'default': -9999999999.999, 'parse': parse_float,
+                                  'dtype': 'float', 'width': 17, 'format': '17.5f'})
 
 amptype = Column(String(8),
                  info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
 
 arid = Column(Integer,
-              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
-auth = Column(String(15),
-              info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15s'})
+auth = Column(String(20),
+              info={'default': '-', 'parse': parse_str, 'dtype': 'a20', 'width': 20, 'format': '20.20s'})
 
 azdef = Column(String(1),
                info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
 
 azimuth = Column(Float(24),
                  info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
@@ -103,21 +162,21 @@
 chanid = Column(Integer,
                 info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
 
 clip = Column(String(1),
               info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
 
 commid = Column(Integer,
-                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 conf = Column(Float(24),
               info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 5, 'format': '5.3f'})
 
 ctype = Column(String(4),
-               info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
+               info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
 
 datatype = Column(String(2),
                   info={'default': '-', 'parse': parse_str, 'dtype': 'a2', 'width': 2, 'format': '2.2s'})
 
 deast = Column(Float(24),
                info={'default': 0.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
 
@@ -150,17 +209,14 @@
 
 digital = Column(String(1),
                  info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
 
 dir = Column(String(64),
              info={'default': '-', 'parse': parse_str, 'dtype': 'a64', 'width': 64, 'format': '64.64s'})
 
-dist = Column(Float(24),
-              info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
-
 dnorth = Column(Float(24),
                 info={'default': 0.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
 
 dtype = Column(String(1),
                info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
 
 duration = Column(Float(24),
@@ -174,28 +230,28 @@
 
 ema = Column(Float(24),
              info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
 emares = Column(Float(24),
                 info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.1f'})
 
-endtime = Column(Float(53),
-                 info={'default': 9999999999.999, 'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
+endtime = Column(Float(53), info={'default': 9999999999.999,
+                                  'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
 
 esaz = Column(Float(24),
               info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
 etype = Column(String(7),
                info={'default': '-', 'parse': parse_str, 'dtype': 'a7', 'width': 7, 'format': '7.7s'})
 
 evid = Column(Integer,
-              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
-evname = Column(String(15),
-                info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
+evname = Column(String(32),
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a32', 'width': 32, 'format': '32.32s'})
 
 fm = Column(String(2),
             info={'default': '-', 'parse': parse_str, 'dtype': 'a2', 'width': 2, 'format': '2.2s'})
 
 foff = Column(Integer,
               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 10, 'format': '10d'})
 
@@ -204,23 +260,14 @@
 
 grname = Column(String(40),
                 info={'default': '-', 'parse': parse_str, 'dtype': 'a40', 'width': 40, 'format': '40.40s'})
 
 hang = Column(Float(24),
               info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.1f'})
 
-imb = Column(Float(24),
-             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
-
-iml = Column(Float(24),
-             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
-
-ims = Column(Float(24),
-             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
-
 inarrival = Column(String(1),
                    info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
 
 inid = Column(Integer,
               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
 
 insname = Column(String(50),
@@ -238,36 +285,33 @@
 jdate = Column(Integer,
                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
 
 keyname = Column(String(15),
                  info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
 
 keyvalue = Column(Integer,
-                  info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                  info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
-lat = Column(Float(24),
-             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+lat = Column(Float(53),
+             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 11, 'format': '11.6f'})
 
 lddate = Column(DateTime, nullable=False, onupdate=datetime.now,
-                info={'default': datetime.now, 'parse': dtfn, 'dtype': 'O', 'width': 17, 'format': DATEFMT})
+                info={'default': datetime.now, 'parse': dtfn, 'dtype': 'O', 'width': 19, 'format': DATEFMT})
 
 lineno = Column(Integer,
                 info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
 
-location = Column(String(32),
-                  info={'default': '-', 'parse': parse_str, 'dtype': 'a32', 'width': 32, 'format': '32.32s'})
-
 logat = Column(Float(24),
                info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
-lon = Column(Float(24),
-             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 9, 'format': '9.4f'})
+lon = Column(Float(53),
+             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 11, 'format': '11.6f'})
 
 magid = Column(Integer, nullable=False,
-               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 magnitude = Column(Float(24),
                    info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
 magres = Column(Float(24),
                 info={'default': -999, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
@@ -277,27 +321,27 @@
 magtype = Column(String(6),
                  info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
 
 mb = Column(Float(24),
             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
 mbid = Column(Integer,
-              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 ml = Column(Float(24),
             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
 mlid = Column(Integer,
-              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 ms = Column(Float(24),
             info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
 msid = Column(Integer,
-              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 mmodel = Column(String(15),
                 info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
 
 nass = Column(Integer,
               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 4, 'format': '4d'})
 
@@ -331,36 +375,36 @@
 offdate = Column(Integer,
                  info={'default': 2286324, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
 
 ondate = Column(Integer,
                 info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
 
 orid = Column(Integer,
-              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 parid = Column(Integer,
                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 per = Column(Float(24),
              info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
 phase = Column(String(8),
                info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
 
 prefor = Column(Integer,
-                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '9d'})
 
 qual = Column(String(1),
               info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
 
 rect = Column(Float(24),
               info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.3f'})
 
 refsta = Column(String(6),
-                info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
+                info={'default': '-', 'parse': parse_str, 'dtype': 'str', 'width': 6, 'format': '6.6s'})
 
 remark = Column(String(80),
                 info={'default': '-', 'parse': parse_str, 'dtype': 'a80', 'width': 80, 'format': '80.80s'})
 
 rsptype = Column(String(6),
                  info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
 
@@ -396,31 +440,31 @@
 
 snr = Column(Float(24),
              info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 10, 'format': '10.2f'})
 
 srn = Column(Integer,
              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
 
-srname = Column(String(40),
-                info={'default': '-', 'parse': parse_str, 'dtype': 'a40', 'width': 40, 'format': '40.40s'})
+srname = Column(String(80),
+                info={'default': '-', 'parse': parse_str, 'dtype': 'a80', 'width': 80, 'format': '80.80s'})
 
 sta = Column(String(6),
              info={'default': '-', 'parse': parse_str, 'dtype': 'a6', 'width': 6, 'format': '6.6s'})
 
 staname = Column(String(50),
                  info={'default': '-', 'parse': parse_str, 'dtype': 'a50', 'width': 50, 'format': '50.50s'})
 
 stassid = Column(Integer,
-                 info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+                 info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 statype = Column(String(4),
                  info={'default': '-', 'parse': parse_str, 'dtype': 'a4', 'width': 4, 'format': '4.4s'})
 
 stime = Column(Float(24),
-               info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8.2f'})
+               info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.2f'})
 
 strike = Column(Float(24),
                 info={'default': -1, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.2f'})
 
 stt = Column(Float(24),
              info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
 
@@ -451,444 +495,439 @@
 syz = Column(Float(24),
              info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
 
 szz = Column(Float(24),
              info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 15, 'format': '15.4f'})
 
 tagid = Column(Integer,
-               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+               info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 tagname = Column(String(8),
                  info={'default': '-', 'parse': parse_str, 'dtype': 'a8', 'width': 8, 'format': '8.8s'})
 
 time = Column(Float(53),
               info={'default': -9999999999.999, 'parse': parse_float, 'dtype': 'float', 'width': 17, 'format': '17.5f'})
 
-timedef = Column(String(1), info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
+timedef = Column(String(1),
+                 info={'default': '-', 'parse': parse_str, 'dtype': 'a1', 'width': 1, 'format': '1.1s'})
 
 timeres = Column(Float(24),
                  info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 8, 'format': '8.3f'})
 
 tshift = Column(Float(24),
-                info={'default': -999.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.2f'})
+                info={'default': -100000000, 'parse': parse_float, 'dtype': 'float', 'width': 16, 'format': '16.2f'})
 
 uncertainty = Column(Float(24),
                      info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 7, 'format': '7.2f'})
 
 units = Column(String(15),
                info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
 
 vang = Column(Float(24),
               info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.1f'})
 
 vmodel = Column(String(15),
                 info={'default': '-', 'parse': parse_str, 'dtype': 'a15', 'width': 15, 'format': '15.15s'})
 
 wfid = Column(Integer,
-              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 8, 'format': '8d'})
+              info={'default': -1, 'parse': parse_int, 'dtype': 'int', 'width': 9, 'format': '9d'})
 
 wgt = Column(Float(24),
              info={'default': -1.0, 'parse': parse_float, 'dtype': 'float', 'width': 6, 'format': '6.3f'})
 
 
 class Affiliation(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('net', 'sta'),)
+        return (PrimaryKeyConstraint('net', 'sta', 'time'),)
 
-    net = net._copy()
-    sta = sta._copy()
-    lddate = lddate._copy()
+    net = dc(net)
+    sta = dc(sta)
+    time = dc(time)
+    endtime = dc(endtime)
+    lddate = dc(lddate)
 
 
 class Amplitude(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('ampid'),)
 
-    ampid = ampid._copy()
-    arid = arid._copy()
-    parid = parid._copy()
-    chan = chan._copy()
-    amp = amp._copy()
-    per = per._copy()
-    snr = snr._copy()
-    amptime = amptime._copy()
-    time = time._copy()
-    duration = duration._copy()
-    deltaf = deltaf._copy()
-    amptype = amptype._copy()
-    units = units._copy()
-    clip = clip._copy()
-    inarrival = inarrival._copy()
-    auth = auth._copy()
-    lddate = lddate._copy()
+    ampid = dc(ampid)
+    arid = dc(arid)
+    parid = dc(parid)
+    chan = dc(chan)
+    amp = dc(amp)
+    per = dc(per)
+    snr = dc(snr)
+    amptime = dc(amptime)
+    time = dc(time)
+    duration = dc(duration)
+    deltaf = dc(deltaf)
+    amptype = dc(amptype)
+    units = dc(units)
+    clip = dc(clip)
+    inarrival = dc(inarrival)
+    auth = dc(auth)
+    lddate = dc(lddate)
 
 
 class Arrival(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('arid'),
                 UniqueConstraint('sta', 'time', 'chan', 'iphase', 'auth'),)
 
-    sta = sta._copy()
-    time = time._copy()
-    arid = arid._copy()
-    jdate = jdate._copy()
-    stassid = stassid._copy()
-    chanid = chanid._copy()
-    chan = chan._copy()
-    iphase = iphase._copy()
-    stype = stype._copy()
-    deltim = deltim._copy()
-    azimuth = azimuth._copy()
-    delaz = delaz._copy()
-    slow = slow._copy()
-    delslo = delslo._copy()
-    ema = ema._copy()
-    rect = rect._copy()
-    amp = amp._copy()
-    per = per._copy()
-    logat = logat._copy()
-    clip = clip._copy()
-    fm = fm._copy()
-    snr = snr._copy()
-    qual = qual._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    time = dc(time)
+    arid = dc(arid)
+    jdate = dc(jdate)
+    stassid = dc(stassid)
+    chanid = dc(chanid)
+    chan = dc(chan)
+    iphase = dc(iphase)
+    stype = dc(stype)
+    deltim = dc(deltim)
+    azimuth = dc(azimuth)
+    delaz = dc(delaz)
+    slow = dc(slow)
+    delslo = dc(delslo)
+    ema = dc(ema)
+    rect = dc(rect)
+    amp = dc(amp)
+    per = dc(per)
+    logat = dc(logat)
+    clip = dc(clip)
+    fm = dc(fm)
+    snr = dc(snr)
+    qual = dc(qual)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Assoc(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('arid', 'orid'), UniqueConstraint('arid'), )
+        return (PrimaryKeyConstraint('arid', 'orid'), UniqueConstraint('arid'),)
 
-    arid = arid._copy()
-    orid = orid._copy()
-    sta = sta._copy()
-    phase = phase._copy()
-    belief = belief._copy()
-    delta = delta._copy()
-    seaz = seaz._copy()
-    esaz = esaz._copy()
-    timeres = timeres._copy()
-    timedef = timedef._copy()
-    azres = azres._copy()
-    azdef = azdef._copy()
-    slores = slores._copy()
-    slodef = slodef._copy()
-    emares = emares._copy()
-    wgt = wgt._copy()
-    vmodel = vmodel._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    arid = dc(arid)
+    orid = dc(orid)
+    sta = dc(sta)
+    phase = dc(phase)
+    belief = dc(belief)
+    delta = dc(delta)
+    seaz = dc(seaz)
+    esaz = dc(esaz)
+    timeres = dc(timeres)
+    timedef = dc(timedef)
+    azres = dc(azres)
+    azdef = dc(azdef)
+    slores = dc(slores)
+    slodef = dc(slodef)
+    emares = dc(emares)
+    wgt = dc(wgt)
+    vmodel = dc(vmodel)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Event(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('evid'), UniqueConstraint('prefor'),)
-
-    evid = evid._copy()
-    evname = evname._copy()
-    prefor = prefor._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    
+    evid = dc(evid)
+    evname = dc(evname)
+    prefor = dc(prefor)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Gregion(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('grn'),)
 
-    grn = grn._copy()
-    grname = grname._copy()
-    lddate = lddate._copy()
+    grn = dc(grn)
+    grname = dc(grname)
+    lddate = dc(lddate)
 
 
 class Instrument(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('inid'),)
 
-    inid = inid._copy()
-    insname = insname._copy()
-    instype = instype._copy()
-    band = band._copy()
-    digital = digital._copy()
-    samprate = samprate._copy()
-    ncalib = ncalib._copy()
-    ncalper = ncalper._copy()
-    dir = dir._copy()
-    dfile = dfile._copy()
-    rsptype = rsptype._copy()
-    lddate = lddate._copy()
-
-
+    inid = dc(inid)
+    insname = dc(insname)
+    instype = dc(instype)
+    band = dc(band)
+    digital = dc(digital)
+    samprate = dc(samprate)
+    ncalib = dc(ncalib)
+    ncalper = dc(ncalper)
+    dir = dc(dir)
+    dfile = dc(dfile)
+    rsptype = dc(rsptype)
+    lddate = dc(lddate)
+
+
+# TODO: implement class-wide generator expressions on keyvalues.
+#   https://groups.google.com/forum/#!topic/sqlalchemy/XksPIVYOdSU
+# or something else
+# http://stackoverflow.com/questions/10494033/setting-sqlalchemy-autoincrement-start-value
+# @attr_generate
 class Lastid(Base):
+    """
+    Store last id values.
+
+    """
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('keyname'), UniqueConstraint('keyname', 'keyvalue'),)
 
-    keyname = keyname._copy()
-    keyvalue = keyvalue._copy()
-    lddate = lddate._copy()
+    def __next__(self):
+        self.keyvalue += 1
+        return self.keyvalue
+
+    keyname = dc(keyname)
+    keyvalue = dc(keyvalue)
+    lddate = dc(lddate)
 
 
 class Netmag(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('magid'),
                 UniqueConstraint('magid', 'orid'),)
 
-    magid = magid._copy()
-    net = net._copy()
-    orid = orid._copy()
-    evid = evid._copy()
-    magtype = magtype._copy()
-    nsta = nsta._copy()
-    magnitude = magnitude._copy()
-    uncertainty = uncertainty._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    magid = dc(magid)
+    net = dc(net)
+    orid = dc(orid)
+    evid = dc(evid)
+    magtype = dc(magtype)
+    nsta = dc(nsta)
+    magnitude = dc(magnitude)
+    uncertainty = dc(uncertainty)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Network(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('net'),)
 
-    net = net._copy()
-    netname = netname._copy()
-    nettype = nettype._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    net = dc(net)
+    netname = dc(netname)
+    nettype = dc(nettype)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Origerr(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('orid'),)
 
-    orid = orid._copy()
-    sxx = sxx._copy()
-    syy = syy._copy()
-    szz = szz._copy()
-    stt = stt._copy()
-    sxy = sxy._copy()
-    sxz = sxz._copy()
-    syz = syz._copy()
-    stx = stx._copy()
-    sty = sty._copy()
-    stz = stz._copy()
-    sdobs = sdobs._copy()
-    smajax = smajax._copy()
-    sminax = sminax._copy()
-    strike = strike._copy()
-    sdepth = sdepth._copy()
-    stime = stime._copy()
-    conf = conf._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    orid = dc(orid)
+    sxx = dc(sxx)
+    syy = dc(syy)
+    szz = dc(szz)
+    stt = dc(stt)
+    sxy = dc(sxy)
+    sxz = dc(sxz)
+    syz = dc(syz)
+    stx = dc(stx)
+    sty = dc(sty)
+    stz = dc(stz)
+    sdobs = dc(sdobs)
+    smajax = dc(smajax)
+    sminax = dc(sminax)
+    strike = dc(strike)
+    sdepth = dc(sdepth)
+    stime = dc(stime)
+    conf = dc(conf)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Origin(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (UniqueConstraint('lat', 'lon', 'depth', 'time', 'auth'), PrimaryKeyConstraint('orid'))
+        return (UniqueConstraint('lat', 'lon', 'depth', 'time', 'auth'), PrimaryKeyConstraint('orid'),)
 
-    lat = lat._copy()
-    lon = lon._copy()
-    depth = depth._copy()
-    time = time._copy()
-    orid = orid._copy()
-    evid = evid._copy()
-    jdate = jdate._copy()
-    nass = nass._copy()
-    ndef = ndef._copy()
-    ndp = ndp._copy()
-    grn = grn._copy()
-    srn = srn._copy()
-    etype = etype._copy()
-    depdp = depdp._copy()
-    dtype = dtype._copy()
-    mb = mb._copy()
-    mbid = mbid._copy()
-    ms = ms._copy()
-    msid = msid._copy()
-    ml = ml._copy()
-    mlid = mlid._copy()
-    algorithm = algorithm._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    lat = dc(lat)
+    lon = dc(lon)
+    depth = dc(depth)
+    time = dc(time)
+    orid = dc(orid)
+    evid = dc(evid)
+    jdate = dc(jdate)
+    nass = dc(nass)
+    ndef = dc(ndef)
+    ndp = dc(ndp)
+    grn = dc(grn)
+    srn = dc(srn)
+    etype = dc(etype)
+    depdp = dc(depdp)
+    dtype = dc(dtype)
+    mb = dc(mb)
+    mbid = dc(mbid)
+    ms = dc(ms)
+    msid = dc(msid)
+    ml = dc(ml)
+    mlid = dc(mlid)
+    algorithm = dc(algorithm)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Remark(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('commid', 'lineno'),)
 
-    commid = commid._copy()
-    lineno = lineno._copy()
-    remark = remark._copy()
-    lddate = lddate._copy()
+    commid = dc(commid)
+    lineno = dc(lineno)
+    remark = dc(remark)
+    lddate = dc(lddate)
 
 
 class Sensor(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('sta', 'chan', 'time', 'endtime'),)
 
-    sta = sta._copy()
-    chan = chan._copy()
-    time = time._copy()
-    endtime = endtime._copy()
-    inid = inid._copy()
-    chanid = chanid._copy()
-    jdate = jdate._copy()
-    calratio = calratio._copy()
-    calper = calper._copy()
-    tshift = tshift._copy()
-    instant = instant._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    chan = dc(chan)
+    time = dc(time)
+    endtime = dc(endtime)
+    inid = dc(inid)
+    chanid = dc(chanid)
+    jdate = dc(jdate)
+    calratio = dc(calratio)
+    calper = dc(calper)
+    tshift = dc(tshift)
+    instant = dc(instant)
+    lddate = dc(lddate)
 
 
 class Site(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('sta', 'ondate'),)
 
-    sta = sta._copy()
-    ondate = ondate._copy()
-    offdate = offdate._copy()
-    lat = lat._copy()
-    lon = lon._copy()
-    elev = elev._copy()
-    staname = staname._copy()
-    statype = statype._copy()
-    refsta = refsta._copy()
-    dnorth = dnorth._copy()
-    deast = deast._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    ondate = dc(ondate)
+    offdate = dc(offdate)
+    lat = dc(lat)
+    lon = dc(lon)
+    elev = dc(elev)
+    staname = dc(staname)
+    statype = dc(statype)
+    refsta = dc(refsta)
+    dnorth = dc(dnorth)
+    deast = dc(deast)
+    lddate = dc(lddate)
 
 
 class Sitechan(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (UniqueConstraint('sta', 'chan', 'ondate'),
-                PrimaryKeyConstraint('chanid'),)
+                PrimaryKeyConstraint('chanid'))
 
-    sta = sta._copy()
-    chan = chan._copy()
-    ondate = ondate._copy()
-    chanid = chanid._copy()
-    offdate = offdate._copy()
-    ctype = ctype._copy()
-    edepth = edepth._copy()
-    hang = hang._copy()
-    vang = vang._copy()
-    descrip = descrip._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    chan = dc(chan)
+    ondate = dc(ondate)
+    chanid = dc(chanid)
+    offdate = dc(offdate)
+    ctype = dc(ctype)
+    edepth = dc(edepth)
+    hang = dc(hang)
+    vang = dc(vang)
+    descrip = dc(descrip)
+    lddate = dc(lddate)
 
 
 class Sregion(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('srn'),)
 
-    srn = srn._copy()
-    srname = srname._copy()
-    lddate = lddate._copy()
+    srn = dc(srn)
+    srname = dc(srname)
+    lddate = dc(lddate)
 
 
 class Stamag(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
-        return (PrimaryKeyConstraint('magid', 'sta'),)
+        return (PrimaryKeyConstraint('magid', 'sta', 'arid'),)
+
+    magid = dc(magid)
+    ampid = dc(ampid)
+    sta = dc(sta)
+    arid = dc(arid)
+    orid = dc(orid)
+    evid = dc(evid)
+    phase = dc(phase)
+    delta = dc(delta)
+    magtype = dc(magtype)
+    magnitude = dc(magnitude)
+    uncertainty = dc(uncertainty)
+    magres = dc(magres)
+    magdef = dc(magdef)
+    mmodel = dc(mmodel)
+    auth = dc(auth)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
-    magid = magid._copy()
-    sta = sta._copy()
-    arid = arid._copy()
-    orid = orid._copy()
-    evid = evid._copy()
-    phase = phase._copy()
-    delta = delta._copy()
-    magtype = magtype._copy()
-    magnitude = magnitude._copy()
-    uncertainty = uncertainty._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
-    
-    
-class Stassoc(Base):
-    __abstract__ = True
-    
-    @declared_attr
-    def __table_args__(cls):
-        return (PrimaryKeyConstraint('stassid'),)
-        
-    stassid = stassid._copy()
-    sta = sta._copy()
-    etype = etype._copy()
-    location = location._copy()
-    dist = dist._copy()
-    azimuth = azimuth._copy()
-    lat = lat._copy()
-    lon = lon._copy()
-    depth = depth._copy()
-    time = time._copy()
-    imb = imb._copy()
-    ims = ims._copy()
-    iml = iml._copy()
-    auth = auth._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
-        
 
 class Wfdisc(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (UniqueConstraint('wfid', 'dir', 'dfile'), PrimaryKeyConstraint('wfid'),)
@@ -900,40 +939,132 @@
         Returns
         -------
         obspy.Trace
 
         """
         return wfdisc2trace(self)
 
-    sta = sta._copy()
-    chan = chan._copy()
-    time = time._copy()
-    wfid = wfid._copy()
-    chanid = chanid._copy()
-    jdate = jdate._copy()
-    endtime = endtime._copy()
-    nsamp = nsamp._copy()
-    samprate = samprate._copy()
-    calib = calib._copy()
-    calper = calper._copy()
-    instype = instype._copy()
-    segtype = segtype._copy()
-    datatype = datatype._copy()
-    clip = clip._copy()
-    dir = dir._copy()
-    dfile = dfile._copy()
-    foff = foff._copy()
-    commid = commid._copy()
-    lddate = lddate._copy()
+    sta = dc(sta)
+    chan = dc(chan)
+    time = dc(time)
+    wfid = dc(wfid)
+    chanid = dc(chanid)
+    jdate = dc(jdate)
+    endtime = dc(endtime)
+    nsamp = dc(nsamp)
+    samprate = dc(samprate)
+    calib = dc(calib)
+    calper = dc(calper)
+    instype = dc(instype)
+    segtype = dc(segtype)
+    datatype = dc(datatype)
+    clip = dc(clip)
+    dir = dc(dir)
+    dfile = dc(dfile)
+    foff = dc(foff)
+    commid = dc(commid)
+    lddate = dc(lddate)
 
 
 class Wftag(Base):
     __abstract__ = True
 
     @declared_attr
     def __table_args__(cls):
         return (PrimaryKeyConstraint('tagname', 'tagid', 'wfid'),)
 
-    tagname = tagname._copy()
-    tagid = tagid._copy()
-    wfid = wfid._copy()
-    lddate = lddate._copy()
+    tagname = dc(tagname)
+    tagid = dc(tagid)
+    wfid = dc(wfid)
+    lddate = dc(lddate)
+
+
+# possibly useful indexes
+# To add, use Index.create(engine)
+# ix_affiliation_stanet = Index(u'ix_affiliation_stanet',
+#                              Affiliation.__table__.c.sta,
+#                              Affiliation.__table__.c.net)
+#
+# ix_amplitude_uk = Index(u'ix_amplitude_uk',
+#                        Amplitude.__table__.c.arid,
+#                        Amplitude.__table__.c.amptime,
+#                        Amplitude.__table__.c.amptype,
+#                        Amplitude.__table__.c.auth,
+#                        Amplitude.__table__.c.chan,
+#                        Amplitude.__table__.c.deltaf,
+#                        Amplitude.__table__.c.duration,
+#                        Amplitude.__table__.c.parid,
+#                        Amplitude.__table__.c.per,
+#                        Amplitude.__table__.c.time)
+#
+# ix_arrival_uk = Index(u'ix_arrival_uk',
+#                      Arrival.__table__.c.time,
+#                      Arrival.__table__.c.sta,
+#                      Arrival.__table__.c.chan,
+#                      Arrival.__table__.c.iphase,
+#                      Arrival.__table__.c.auth)
+#
+# ix_event_evid_prefor = Index(u'ix_event_evid_prefor',
+#                             Event.__table__.c.evid,
+#                             Event.__table__.c.prefor)
+#
+# ix_instrument_uk = Index(u'ix_instrument_uk',
+#                         Instrument.__table__.c.dfile,
+#                         Instrument.__table__.c.dir,
+#                         Instrument.__table__.c.instype,
+#                         Instrument.__table__.c.ncalib,
+#                         Instrument.__table__.c.samprate)
+#
+# ix_netmaguk = Index(u'ix_netmaguk',
+#                    Netmag.__table__.c.orid,
+#                    Netmag.__table__.c.magtype,
+#                    Netmag.__table__.c.auth)
+#
+# ix_network_uk = Index(u'ix_network_uk',
+#                      Network.__table__.c.auth,
+#                      Network.__table__.c.netname)
+#
+# ix_originautheviduk = Index(u'ix_originautheviduk',
+#                            Origin.__table__.c.evid,
+#                            Origin.__table__.c.auth)
+#
+# ix_origin_uk = Index(u'origin_uk',
+#                     Origin.__table__.c.lat,
+#                     Origin.__table__.c.lon,
+#                     Origin.__table__.c.depth,
+#                     Origin.__table__.c.time,
+#                     Origin.__table__.c.auth)
+#
+# ix_b_newsite_onoff_ix = Index(u'ix_b_newsite_onoff',
+#                              Site.__table__.c.ondate,
+#                              Site.__table__.c.offdate)
+#
+# ix_site = Index(u'ix_site',
+#                Site.__table__.c.sta,
+#                Site.__table__.c.ondate,
+#                Site.__table__.c.offdate)
+#
+# ix_sitechan_uk = Index(u'ix_sitechan_uk',
+#                       Sitechan.__table__.c.sta,
+#                       Sitechan.__table__.c.chan,
+#                       Sitechan.__table__.c.ondate)
+#
+# ix_wfdisc_dirdfile = Index(u'ix_wfdisc_dirdfile',
+#                           Wfdisc.__table__.c.dfile,
+#                           Wfdisc.__table__.c.dir,
+#                           Wfdisc.__table__.c.foff)
+#
+# ix_wfdisc = Index(u'ix_wfdisc',
+#                  Wfdisc.__table__.c.sta,
+#                  Wfdisc.__table__.c.jdate,
+#                  Wfdisc.__table__.c.time,
+#                  Wfdisc.__table__.c.endtime,
+#                  Wfdisc.__table__.c.wfid)
+#
+# ix_wfdisc_uk = Index(u'ix_wfdisc_uk',
+#                     Wfdisc.__table__.c.sta,
+#                     Wfdisc.__table__.c.chan,
+#                     Wfdisc.__table__.c.time)
+#
+# ix_wfdisc_chanid_instype = Index(u'ix_wfdisc_chanid_instype',
+#                                 Wfdisc.__table__.c.chanid,
+#                                 Wfdisc.__table__.c.instype)
```

### Comparing `pisces-0.4.1/pisces/schema/util.py` & `pisces-0.4.2/pisces/schema/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/tables/antelope.py` & `pisces-0.4.2/pisces/tables/antelope.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/tables/css3.py` & `pisces-0.4.2/pisces/tables/css3.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/tables/kbcore.py` & `pisces-0.4.2/pisces/tables/kbcore.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces/util.py` & `pisces-0.4.2/pisces/util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/pisces.egg-info/PKG-INFO` & `pisces-0.4.2/pisces.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pisces
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Practical Seismological Database Library in Python.
 Home-page: https://github.com/LANL-Seismoacoustics/pisces
-Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.3.2
+Download-URL: https://github.com/LANL-Seismoacoustics/pisces/tarball/0.4.2
 Author: Jonathan MacCarthy
 Author-email: jkmacc@lanl.gov
 License: LANL-MIT
 Keywords: seismology,geophysics,database
 Platform: Mac OS X
 Platform: Linux/Unix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pisces-0.4.1/pisces.egg-info/SOURCES.txt` & `pisces-0.4.2/pisces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/setup.py` & `pisces-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 with open('README.md') as readme:
     # https://dustingram.com/articles/2018/03/16/markdown-descriptions-on-pypi
     long_description = readme.read()
 
 doclines = __doc__.split("\n")
 
 setup(name='pisces',
-      version='0.4.1',
+      version='0.4.2',
       description='A Practical Seismological Database Library in Python.',
       long_description=long_description,
       long_description_content_type="text/markdown", # setuptools >= 38.6.0
       author='Jonathan MacCarthy',
       author_email='jkmacc@lanl.gov',
       packages=['pisces','pisces.schema','pisces.io','pisces.tables',
                 'pisces.commands'],
       url='https://github.com/LANL-Seismoacoustics/pisces',
-      download_url='https://github.com/LANL-Seismoacoustics/pisces/tarball/0.3.2',
+      download_url='https://github.com/LANL-Seismoacoustics/pisces/tarball/0.4.2',
       keywords = ['seismology', 'geophysics', 'database'],
       install_requires=['numpy','obspy>=1.0','sqlalchemy>=1.4','Click'],
       extras_require={
          'e1': ["e1"],
       },
       entry_points = """
           [console_scripts]
```

### Comparing `pisces-0.4.1/tests/test_readwaveform.py` & `pisces-0.4.2/tests/test_readwaveform.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/tests/test_schema_util.py` & `pisces-0.4.2/tests/test_schema_util.py`

 * *Files identical despite different names*

### Comparing `pisces-0.4.1/tests/test_util.py` & `pisces-0.4.2/tests/test_util.py`

 * *Files identical despite different names*

