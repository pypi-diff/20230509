# Comparing `tmp/prettynumbers-0.2.1.tar.gz` & `tmp/prettynumbers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.2.1.tar", last modified: Mon May  8 13:03:34 2023, max compression
+gzip compressed data, was "prettynumbers-0.2.2.tar", last modified: Tue May  9 13:57:56 2023, max compression
```

## Comparing `prettynumbers-0.2.1.tar` & `prettynumbers-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 13:03:34.192640 prettynumbers-0.2.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14849 2023-05-08 13:03:28.000000 prettynumbers-0.2.1/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-08 13:03:28.000000 prettynumbers-0.2.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-08 13:03:34.192640 prettynumbers-0.2.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1199 2023-05-08 13:03:28.000000 prettynumbers-0.2.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-05-08 13:03:28.000000 prettynumbers-0.2.1/README.rst
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1981 2023-05-08 13:03:28.000000 prettynumbers-0.2.1/pretty_numbers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 13:03:34.192640 prettynumbers-0.2.1/prettynumbers.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-08 13:03:34.000000 prettynumbers-0.2.1/prettynumbers.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2023-05-08 13:03:34.000000 prettynumbers-0.2.1/prettynumbers.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-08 13:03:34.000000 prettynumbers-0.2.1/prettynumbers.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-08 13:03:34.000000 prettynumbers-0.2.1/prettynumbers.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 13:03:28.000000 prettynumbers-0.2.1/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-05-08 13:03:28.000000 prettynumbers-0.2.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-08 13:03:34.196640 prettynumbers-0.2.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-05-08 13:03:28.000000 prettynumbers-0.2.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14849 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1138 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/pretty_numbers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/pretty_numbers/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1915 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/pretty_numbers/pretty_numbers.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3303 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/pretty_numbers/test_pretty_numbers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/prettynumbers.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-09 13:57:56.000000 prettynumbers-0.2.2/prettynumbers.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-05-09 13:57:56.000000 prettynumbers-0.2.2/prettynumbers.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 13:57:56.000000 prettynumbers-0.2.2/prettynumbers.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-09 13:57:56.000000 prettynumbers-0.2.2/prettynumbers.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/setup.py
```

### Comparing `prettynumbers-0.2.1/LICENSE.txt` & `prettynumbers-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.1/PKG-INFO` & `prettynumbers-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.2.1
+Version: 0.2.2
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 Author: Gerard Keating
 Author-email: gerardk@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.2.1.tar.gz?raw=true
+Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.2.2.tar.gz?raw=true
 Description: |Build Status| |codecov.io| |Code Climate|
         
         .. |Build Status| image:: https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master
            :target: https://travis-ci.org/vfxGer/pretty-numbers
         .. |codecov.io| image:: https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master
            :target: https://codecov.io/gh/vfxGer/pretty-numbers
         .. |Code Climate| image:: https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg
```

### Comparing `prettynumbers-0.2.1/README.md` & `prettynumbers-0.2.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[![Build Status](https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master)](https://travis-ci.org/vfxGer/pretty-numbers)
+[![vfxGer](https://circleci.com/gh/vfxGer/pretty-numbers.svg?style=svg)](BUILD)
 [![codecov.io](https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master)](https://codecov.io/gh/vfxGer/pretty-numbers)
 [![Code Climate](https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg)](https://codeclimate.com/github/vfxGer/pretty-numbers)
 [![PYPI](https://img.shields.io/pypi/v/prettynumbers.svg)](https://pypi.python.org/pypi/prettynumbers)
 
-Pretty Numbers
-==============
+# Pretty Numbers
 
-Pretty Numbers is a simple Python package that displays long series of numbers in a more human readable way. 
+Pretty Numbers is a simple Python package that displays long series of numbers in a more human readable way.
 
 I have used it for displaying frames of a render in a more human readable way or issues of comic books. It allows the user to quickly see what is included and what is missing.
 
 ## Installation
-It is available on [PyPi](https://pypi.python.org/pypi/prettynumbers) meaning you can just:
 
-    pip install prettynumbers 
+It is available on [PyPi](https://pypi.python.org/pypi/prettynumbers) meaning you can just:
 
+    pip install prettynumbers
 
 ## Usage
+
 ```python
 import pretty_numbers
-pretty_numbers.getPrettyTextFromNumbers([1001, 99, 1004, 1005, 1003, 1008, 
+pretty_numbers.getPrettyTextFromNumbers([1001, 99, 1004, 1005, 1003, 1008,
                                          1002, 1007, 1010, 1006, 1111, 1009])
 ```
+
 Returns:
 
     "99,1001-1010,1111"
-
```

### Comparing `prettynumbers-0.2.1/pretty_numbers.py` & `prettynumbers-0.2.2/pretty_numbers/pretty_numbers.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-#!/usr/bin/env python
-########################################################
-__author__ = "Gerard Keating vfxger.com"
-########################################################
-from typing import Any, Sequence, Set
-
-
-def getPrettyTextFromSet(frames: Set[int]) -> str:
-    """
-    Given a set of integers returns a more human readable string
-    """
-    if not frames:
-        return ""
-    if len(frames) == 1:
-        framesSet = frames.copy()
-        return str(framesSet.pop())
-    framesList = list(frames)
-    framesList.sort(reverse=True)
-    lastNum = framesList.pop()
-    currentStrStart = lastNum
-    pStr = str(lastNum)
-    while framesList:
-        currNum = framesList.pop()
-        if not lastNum + 1 == currNum:
-            if not lastNum == currentStrStart:
-                pStr = pStr + "-" + str(lastNum)
-            pStr = pStr + "," + str(currNum)
-            currentStrStart = currNum
-        lastNum = currNum
-    if currentStrStart != currNum:
-        pStr = pStr + "-" + str(lastNum)
-    return pStr
-
-
-def getPrettyTextFromNumbers(frames: Sequence[int]) -> str:
-    """
-    Given iterable of integers returns a more human readable string
-    """
-    framesSet = set(frames)
-    return getPrettyTextFromSet(framesSet)
-
-
-def getPrettyNumbersText(list_of_strings: Sequence[Any]) -> str:
-    nums = set()
-    text_result = set()
-    for i in list_of_strings:
-        try:
-            is_digit = i.isdigit()
-        except AttributeError:
-            is_digit = True
-        if is_digit:
-            try:
-                nums.add(int(i))
-            except TypeError:
-                text_result.add(str(i))
-        else:
-            text_result.add(i)
-    result = getPrettyTextFromSet(nums)
-    if not text_result:
-        return result
-    texts = list(text_result)
-    texts.sort()
-    final_text = ",".join(texts)
-    if result:
-        return result + "," + final_text
-    return final_text
+#!/usr/bin/env python
+########################################################
+__author__ = "Gerard Keating vfxger.com"
+########################################################
+from typing import Any, Sequence, Set
+
+
+def getPrettyTextFromSet(frames: Set[int]) -> str:
+    """
+    Given a set of integers returns a more human readable string
+    """
+    if not frames:
+        return ""
+    if len(frames) == 1:
+        framesSet = frames.copy()
+        return str(framesSet.pop())
+    framesList = list(frames)
+    framesList.sort(reverse=True)
+    lastNum = framesList.pop()
+    currentStrStart = lastNum
+    pStr = str(lastNum)
+    while framesList:
+        currNum = framesList.pop()
+        if not lastNum + 1 == currNum:
+            if not lastNum == currentStrStart:
+                pStr = pStr + "-" + str(lastNum)
+            pStr = pStr + "," + str(currNum)
+            currentStrStart = currNum
+        lastNum = currNum
+    if currentStrStart != currNum:
+        pStr = pStr + "-" + str(lastNum)
+    return pStr
+
+
+def getPrettyTextFromNumbers(frames: Sequence[int]) -> str:
+    """
+    Given iterable of integers returns a more human readable string
+    """
+    framesSet = set(frames)
+    return getPrettyTextFromSet(framesSet)
+
+
+def getPrettyNumbersText(list_of_strings: Sequence[Any]) -> str:
+    nums = set()
+    text_result = set()
+    for i in list_of_strings:
+        try:
+            is_digit = i.isdigit()
+        except AttributeError:
+            is_digit = True
+        if is_digit:
+            try:
+                nums.add(int(i))
+            except TypeError:
+                text_result.add(str(i))
+        else:
+            text_result.add(i)
+    result = getPrettyTextFromSet(nums)
+    if not text_result:
+        return result
+    texts = list(text_result)
+    texts.sort()
+    final_text = ",".join(texts)
+    if result:
+        return result + "," + final_text
+    return final_text
```

### Comparing `prettynumbers-0.2.1/prettynumbers.egg-info/PKG-INFO` & `prettynumbers-0.2.2/prettynumbers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.2.1
+Version: 0.2.2
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 Author: Gerard Keating
 Author-email: gerardk@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.2.1.tar.gz?raw=true
+Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.2.2.tar.gz?raw=true
 Description: |Build Status| |codecov.io| |Code Climate|
         
         .. |Build Status| image:: https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master
            :target: https://travis-ci.org/vfxGer/pretty-numbers
         .. |codecov.io| image:: https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master
            :target: https://codecov.io/gh/vfxGer/pretty-numbers
         .. |Code Climate| image:: https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg
```

### Comparing `prettynumbers-0.2.1/pyproject.toml` & `prettynumbers-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.1/setup.py` & `prettynumbers-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# based on https://github.com/pypa/sampleproject/blob/master/setup.py
 from os import path
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 here = path.abspath(path.dirname(__file__))
 
-version = "0.2.1"
+version = "0.2.2"
+
 
 # Get the long description from the README file
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="prettynumbers",
@@ -17,15 +17,16 @@
     description="Display a range of numbers in a human readable way",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Gerard Keating",
     author_email="gerardk@gmail.com",
     license="GNU GENERAL PUBLIC LICENSE",
     url="https://github.com/vfxGer/pretty-numbers",
-    py_modules=["pretty_numbers"],
+    packages=find_packages(),
     download_url=f"https://pypi.python.org/packages/"
     f"source/d/"
     f"pretty_numbers-{version}.tar.gz?raw=true",
     platforms="Cross-platform",
     classifiers=["Programming Language :: Python :: 3"],
-    package_data={"prettynumbers": ["py.typed"]},
+    package_data={"pretty_numbers": ["py.typed"]},
+    include_package_data=True,
 )
```

