# Comparing `tmp/clevertable-2.0.0.tar.gz` & `tmp/clevertable-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-2.0.0.tar", last modified: Thu May  4 18:21:54 2023, max compression
+gzip compressed data, was "clevertable-2.1.0.tar", last modified: Tue May  9 06:39:26 2023, max compression
```

## Comparing `clevertable-2.0.0.tar` & `clevertable-2.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 18:21:54.731578 clevertable-2.0.0/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.0.0/LICENSE
--rw-rw-rw-   0        0        0    28874 2023-05-04 18:21:54.731578 clevertable-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    27104 2023-05-04 17:35:13.000000 clevertable-2.0.0/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-04 18:15:33.000000 clevertable-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 18:21:54.732578 clevertable-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:21:54.667362 clevertable-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 18:21:54.719829 clevertable-2.0.0/src/clevertable/
--rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.0.0/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-01 14:12:57.000000 clevertable-2.0.0/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     2948 2023-05-04 17:33:19.000000 clevertable-2.0.0/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3691 2023-05-03 09:20:52.000000 clevertable-2.0.0/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     3672 2023-05-04 12:32:37.000000 clevertable-2.0.0/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.0.0/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.0.0/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.0.0/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.0.0/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     3864 2023-05-01 18:32:23.000000 clevertable-2.0.0/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.0.0/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.0.0/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.0.0/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.0.0/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.0.0/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.0.0/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.0.0/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.0.0/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.0.0/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     6334 2023-05-04 05:34:03.000000 clevertable-2.0.0/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.0.0/src/clevertable/Split.py
--rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.0.0/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0      312 2023-05-01 14:33:36.000000 clevertable-2.0.0/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2535 2023-05-04 10:32:03.000000 clevertable-2.0.0/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      672 2023-05-04 18:15:33.000000 clevertable-2.0.0/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.0.0/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2731 2023-05-02 18:50:19.000000 clevertable-2.0.0/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:21:54.729579 clevertable-2.0.0/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    28874 2023-05-04 18:21:54.000000 clevertable-2.0.0/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1010 2023-05-04 18:21:54.000000 clevertable-2.0.0/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 18:21:54.000000 clevertable-2.0.0/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-04 18:21:54.000000 clevertable-2.0.0/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-04 18:21:54.000000 clevertable-2.0.0/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-04 18:21:54.000000 clevertable-2.0.0/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 06:39:26.086484 clevertable-2.1.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0    28874 2023-05-09 06:39:26.086484 clevertable-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    27104 2023-05-04 17:35:13.000000 clevertable-2.1.0/README.md
+-rw-rw-rw-   0        0        0     1306 2023-05-09 06:34:18.000000 clevertable-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 06:39:26.086484 clevertable-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:39:26.023056 clevertable-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 06:39:26.071442 clevertable-2.1.0/src/clevertable/
+-rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.1.0/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-01 14:12:57.000000 clevertable-2.1.0/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     2948 2023-05-04 17:33:19.000000 clevertable-2.1.0/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.1.0/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     3672 2023-05-04 12:32:37.000000 clevertable-2.1.0/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.1.0/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.1.0/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.1.0/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.1.0/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     3864 2023-05-01 18:32:23.000000 clevertable-2.1.0/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.1.0/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.1.0/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.1.0/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.1.0/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.1.0/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.1.0/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.1.0/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.1.0/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.1.0/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     6334 2023-05-04 05:34:03.000000 clevertable-2.1.0/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.1.0/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.1.0/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0      312 2023-05-01 14:33:36.000000 clevertable-2.1.0/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2535 2023-05-04 10:32:03.000000 clevertable-2.1.0/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      672 2023-05-09 06:34:18.000000 clevertable-2.1.0/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.1.0/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2731 2023-05-02 18:50:19.000000 clevertable-2.1.0/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:39:26.086484 clevertable-2.1.0/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    28874 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1010 2023-05-09 06:39:26.000000 clevertable-2.1.0/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-2.0.0/LICENSE` & `clevertable-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/PKG-INFO` & `clevertable-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.0.0
+Version: 2.1.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clevertable-2.0.0/README.md` & `clevertable-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/pyproject.toml` & `clevertable-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "2.0.0"
+version = "2.1.0"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "2.0.0"
+current_version = "2.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-2.0.0/src/clevertable/Binary.py` & `clevertable-2.1.0/src/clevertable/Binary.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/ConversionProfile.py` & `clevertable-2.1.0/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Converter.py` & `clevertable-2.1.0/src/clevertable/Converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
 
 class Converter(ABC):
-    """A converter is used to convert a single column of data into multiple columns of data."""
+    """
+    Base class for all converters.
+    A converter is used to convert a single column of data into one or multiple columns of data."""
 
     def fit(self, rows: list[list]):
         """The converter is presented representative sample data.
         In this method, the converter should adapt its internal state so that there will
         be no errors when transform() is called with the same data.
         Implementations of this method can make the following assumptions:
 
@@ -71,7 +73,10 @@
         """
         Returns a string representation of this converter.
         If possible, this should be a string that can be used to create a new instance.
         If possible, a converter instantiated from this string should behave identical to this converter
         even if fitted with different data.
         """
         return repr(self)
+
+    def __add__(self, other):
+        return [self, other]
```

### Comparing `clevertable-2.0.0/src/clevertable/DataFrameProfile.py` & `clevertable-2.1.0/src/clevertable/DataFrameProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Enumerate.py` & `clevertable-2.1.0/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Float.py` & `clevertable-2.1.0/src/clevertable/Float.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/ForEach.py` & `clevertable-2.1.0/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Function.py` & `clevertable-2.1.0/src/clevertable/Function.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Infer.py` & `clevertable-2.1.0/src/clevertable/Infer.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Label.py` & `clevertable-2.1.0/src/clevertable/Label.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/List.py` & `clevertable-2.1.0/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Map.py` & `clevertable-2.1.0/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/OneHot.py` & `clevertable-2.1.0/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Parallel.py` & `clevertable-2.1.0/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Pipeline.py` & `clevertable-2.1.0/src/clevertable/Pipeline.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/RecordProfile.py` & `clevertable-2.1.0/src/clevertable/RecordProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Split.py` & `clevertable-2.1.0/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Strip.py` & `clevertable-2.1.0/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/Try.py` & `clevertable-2.1.0/src/clevertable/Try.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/__init__.py` & `clevertable-2.1.0/src/clevertable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-2.0.0/src/clevertable/__main__.py` & `clevertable-2.1.0/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable/_utils.py` & `clevertable-2.1.0/src/clevertable/_utils.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.0.0/src/clevertable.egg-info/PKG-INFO` & `clevertable-2.1.0/src/clevertable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.0.0
+Version: 2.1.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clevertable-2.0.0/src/clevertable.egg-info/SOURCES.txt` & `clevertable-2.1.0/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

