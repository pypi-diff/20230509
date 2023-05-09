# Comparing `tmp/pytweening-1.0.5.tar.gz` & `tmp/pytweening-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytweening-1.0.5.tar", last modified: Tue Apr 25 21:57:08 2023, max compression
+gzip compressed data, was "pytweening-1.0.7.tar", last modified: Tue May  9 16:50:05 2023, max compression
```

## Comparing `pytweening-1.0.5.tar` & `pytweening-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.360048 pytweening-1.0.5/
--rw-rw-rw-   0        0        0      117 2018-09-24 23:55:11.000000 pytweening-1.0.5/.gitignore
--rw-rw-rw-   0        0        0      463 2023-04-25 21:47:28.000000 pytweening-1.0.5/AUTHORS.txt
--rw-rw-rw-   0        0        0      248 2015-10-28 23:47:22.000000 pytweening-1.0.5/CHANGES.txt
--rw-rw-rw-   0        0        0     1514 2014-07-17 23:32:58.000000 pytweening-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      222 2021-09-14 17:31:54.000000 pytweening-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4868 2023-04-25 21:57:08.360048 pytweening-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1519 2021-09-01 21:18:54.000000 pytweening-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.298032 pytweening-1.0.5/docs/
--rw-rw-rw-   0        0        0     6778 2014-08-04 08:42:22.000000 pytweening-1.0.5/docs/Makefile
--rw-rw-rw-   0        0        0     8443 2014-08-04 08:42:22.000000 pytweening-1.0.5/docs/conf.py
--rw-rw-rw-   0        0        0      457 2014-08-04 08:42:22.000000 pytweening-1.0.5/docs/index.rst
--rwxrwxrwx   0        0        0     6709 2014-08-04 08:42:22.000000 pytweening-1.0.5/docs/make.bat
--rw-rw-rw-   0        0        0     1735 2023-04-25 21:52:51.000000 pytweening-1.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.302026 pytweening-1.0.5/pytweening/
--rw-rw-rw-   0        0        0    18638 2023-04-25 21:52:10.000000 pytweening-1.0.5/pytweening/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.326040 pytweening-1.0.5/pytweening.egg-info/
--rw-rw-rw-   0        0        0     4868 2023-04-25 21:57:08.000000 pytweening-1.0.5/pytweening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-04-25 21:57:08.000000 pytweening-1.0.5/pytweening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:57:08.000000 pytweening-1.0.5/pytweening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 21:57:08.000000 pytweening-1.0.5/pytweening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 21:57:08.364054 pytweening-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.356047 pytweening-1.0.5/tests/
--rw-rw-rw-   0        0        0     4989 2023-04-25 21:43:19.000000 pytweening-1.0.5/tests/basicTests.py
--rw-rw-rw-   0        0        0     3229 2015-09-09 18:30:07.000000 pytweening-1.0.5/tests/generateExcelGraphs.py
--rw-rw-rw-   0        0        0   606728 2015-09-09 18:30:07.000000 pytweening-1.0.5/tests/graphs.ipynb
--rw-rw-rw-   0        0        0   118762 2015-09-09 18:31:30.000000 pytweening-1.0.5/tests/graphs.xlsx
--rw-rw-rw-   0        0        0     1816 2023-04-25 16:35:05.000000 pytweening-1.0.5/tests/seeGraphs.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:50:05.498876 pytweening-1.0.7/
+-rw-rw-rw-   0        0        0      117 2018-09-24 23:55:11.000000 pytweening-1.0.7/.gitignore
+-rw-rw-rw-   0        0        0      463 2023-04-25 21:47:28.000000 pytweening-1.0.7/AUTHORS.txt
+-rw-rw-rw-   0        0        0      248 2015-10-28 23:47:22.000000 pytweening-1.0.7/CHANGES.txt
+-rw-rw-rw-   0        0        0     1514 2014-07-17 23:32:58.000000 pytweening-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      222 2021-09-14 17:31:54.000000 pytweening-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2833 2023-05-09 16:50:05.498876 pytweening-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1519 2021-09-01 21:18:54.000000 pytweening-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 16:50:05.456411 pytweening-1.0.7/docs/
+-rw-rw-rw-   0        0        0     6778 2014-08-04 08:42:22.000000 pytweening-1.0.7/docs/Makefile
+-rw-rw-rw-   0        0        0     8443 2014-08-04 08:42:22.000000 pytweening-1.0.7/docs/conf.py
+-rw-rw-rw-   0        0        0      457 2014-08-04 08:42:22.000000 pytweening-1.0.7/docs/index.rst
+-rwxrwxrwx   0        0        0     6709 2014-08-04 08:42:22.000000 pytweening-1.0.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-09 16:50:05.459408 pytweening-1.0.7/pytweening/
+-rw-rw-rw-   0        0        0    20995 2023-05-09 16:48:09.000000 pytweening-1.0.7/pytweening/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:50:05.481822 pytweening-1.0.7/pytweening.egg-info/
+-rw-rw-rw-   0        0        0     2833 2023-05-09 16:50:05.000000 pytweening-1.0.7/pytweening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-09 16:50:05.000000 pytweening-1.0.7/pytweening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 16:50:05.000000 pytweening-1.0.7/pytweening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 16:50:05.000000 pytweening-1.0.7/pytweening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 16:50:05.499876 pytweening-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2001 2023-05-09 16:49:53.000000 pytweening-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:50:05.495877 pytweening-1.0.7/tests/
+-rw-rw-rw-   0        0        0     4989 2023-04-25 21:43:19.000000 pytweening-1.0.7/tests/basicTests.py
+-rw-rw-rw-   0        0        0     3229 2015-09-09 18:30:07.000000 pytweening-1.0.7/tests/generateExcelGraphs.py
+-rw-rw-rw-   0        0        0   606728 2015-09-09 18:30:07.000000 pytweening-1.0.7/tests/graphs.ipynb
+-rw-rw-rw-   0        0        0   118762 2015-09-09 18:31:30.000000 pytweening-1.0.7/tests/graphs.xlsx
+-rw-rw-rw-   0        0        0     1816 2023-04-25 16:35:05.000000 pytweening-1.0.7/tests/seeGraphs.py
```

### Comparing `pytweening-1.0.5/LICENSE.txt` & `pytweening-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/README.md` & `pytweening-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/docs/Makefile` & `pytweening-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/docs/conf.py` & `pytweening-1.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/docs/make.bat` & `pytweening-1.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/pytweening/__init__.py` & `pytweening-1.0.7/pytweening/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import division
 
 import math
+try:
+    from typing import List, Tuple, Union
+except ImportError:
+    pass  # This is fine; it happens on Python 2.6 and before, but type hints aren't supported there anyway.
 
-__version__ = '1.0.5'
+__version__ = '1.0.7'
 
 
 # from http://www.roguebasin.com/index.php?title=Bresenham%27s_Line_Algorithm#Python
-def getLine(x1, y1, x2, y2):
+def getLine(x1, y1, x2, y2):  # type: (int, int, int, int) -> List[Tuple[int, int]]
     """Returns a list of (x, y) tuples of every point on a line between
     (x1, y1) and (x2, y2). The x and y values inside the tuple are integers.
 
     Line generated with the Bresenham algorithm.
 
     Args:
       x1 (int, float): The x coordinate of the line's start point.
@@ -60,24 +64,24 @@
             error += deltax
     # Reverse the list if the coordinates were reversed
     if rev:
         points.reverse()
     return points
 
 
-def getPointOnLine(x1, y1, x2, y2, n):
+def getPointOnLine(x1, y1, x2, y2, n):  # type: (Union[int, float], Union[int, float], Union[int, float], Union[int, float], Union[int, float]) -> Tuple[Union[int, float], Union[int, float]]
     """Returns the (x, y) tuple of the point that has progressed a proportion
     n along the line defined by the two x, y coordinates.
 
     Args:
       x1 (int, float): The x coordinate of the line's start point.
       y1 (int, float): The y coordinate of the line's start point.
       x2 (int, float): The x coordinate of the line's end point.
       y2 (int, float): The y coordiante of the line's end point.
-      n (float): Progress along the line. 0.0 is the start point, 1.0 is the end point. 0.5 is the midpoint. This value can be less than 0.0 or greater than 1.0.
+      n (int, float): Progress along the line. 0.0 is the start point, 1.0 is the end point. 0.5 is the midpoint. This value can be less than 0.0 or greater than 1.0.
 
     Returns:
       Tuple of floats for the x, y coordinate of the point.
 
     Example:
     >>> getPointOnLine(0, 0, 6, 6, 0)
     (0, 0)
@@ -95,21 +99,21 @@
     (-1.5, -1.5)
     """
     x = ((x2 - x1) * n) + x1
     y = ((y2 - y1) * n) + y1
     return (x, y)
 
 
-def _checkRange(n):
+def _checkRange(n):  # type: (Union[int, float]) -> None
     """Raises ValueError if the argument is not between 0.0 and 1.0."""
     if not 0.0 <= n <= 1.0:
         raise ValueError('Argument must be between 0.0 and 1.0.')
 
 
-def linear(n):
+def linear(n):  # type: (Union[int, float]) -> Union[int, float]
     """A linear tween function
 
     Example:
     >>> linear(0.0)
     0.0
     >>> linear(0.2)
     0.2
@@ -122,41 +126,41 @@
     >>> linear(1.0)
     1.0
     """
     _checkRange(n)
     return n
 
 
-def easeInQuad(n):
+def easeInQuad(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quadratic tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return n**2
 
 
-def easeOutQuad(n):
+def easeOutQuad(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quadratic tween function that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return -n * (n - 2)
 
 
-def easeInOutQuad(n):
+def easeInOutQuad(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quadratic tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -165,42 +169,42 @@
     if n < 0.5:
         return 2 * n**2
     else:
         n = n * 2 - 1
         return -0.5 * (n * (n - 2) - 1)
 
 
-def easeInCubic(n):
+def easeInCubic(n):  # type: (Union[int, float]) -> Union[int, float]
     """A cubic tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return n**3
 
 
-def easeOutCubic(n):
+def easeOutCubic(n):  # type: (Union[int, float]) -> Union[int, float]
     """A cubic tween function that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     n -= 1
     return n**3 + 1
 
 
-def easeInOutCubic(n):
+def easeInOutCubic(n):  # type: (Union[int, float]) -> Union[int, float]
     """A cubic tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -210,42 +214,42 @@
     if n < 1:
         return 0.5 * n**3
     else:
         n -= 2
         return 0.5 * (n**3 + 2)
 
 
-def easeInQuart(n):
+def easeInQuart(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quartic tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return n**4
 
 
-def easeOutQuart(n):
+def easeOutQuart(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quartic tween function that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     n -= 1
     return -(n**4 - 1)
 
 
-def easeInOutQuart(n):
+def easeInOutQuart(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quartic tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -255,42 +259,42 @@
     if n < 1:
         return 0.5 * n**4
     else:
         n -= 2
         return -0.5 * (n**4 - 2)
 
 
-def easeInQuint(n):
+def easeInQuint(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quintic tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return n**5
 
 
-def easeOutQuint(n):
+def easeOutQuint(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quintic tween function that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     n -= 1
     return n**5 + 1
 
 
-def easeInOutQuint(n):
+def easeInOutQuint(n):  # type: (Union[int, float]) -> Union[int, float]
     """A quintic tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -300,45 +304,45 @@
     if n < 1:
         return 0.5 * n**5
     else:
         n -= 2
         return 0.5 * (n**5 + 2)
 
 
-def easeInPoly(n, degree=2):
+def easeInPoly(n, degree=2):  # type: (Union[int, float], Union[int, float]) -> Union[int, float]
     """A polynomial tween function of given degree that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     if not isinstance(degree, (int, float)) or degree < 0:
         raise ValueError('degree argument must be a positive number.')
     return n**degree
 
 
-def easeOutPoly(n, degree=2):
+def easeOutPoly(n, degree=2):  # type: (Union[int, float], Union[int, float]) -> Union[int, float]
     """A polynomial tween function of given degree that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     if not isinstance(degree, (int, float)) or degree < 0:
         raise ValueError('degree argument must be a positive number.')
     return 1 - abs((n - 1) ** degree)
 
 
-def easeInOutPoly(n, degree=2):
+def easeInOutPoly(n, degree=2):  # type: (Union[int, float], Union[int, float]) -> Union[int, float]
     """A polynomial tween function of given degree that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -351,54 +355,54 @@
     if n < 1:
         return 0.5 * n**degree
     else:
         n -= 2
         return 1 - 0.5 * abs(n**degree)
 
 
-def easeInSine(n):
+def easeInSine(n):  # type: (Union[int, float]) -> Union[int, float]
     """A sinusoidal tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return -1 * math.cos(n * math.pi / 2) + 1
 
 
-def easeOutSine(n):
+def easeOutSine(n):  # type: (Union[int, float]) -> Union[int, float]
     """A sinusoidal tween function that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return math.sin(n * math.pi / 2)
 
 
-def easeInOutSine(n):
+def easeInOutSine(n):  # type: (Union[int, float]) -> Union[int, float]
     """A sinusoidal tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return -0.5 * (math.cos(math.pi * n) - 1)
 
 
-def easeInExpo(n):
+def easeInExpo(n):  # type: (Union[int, float]) -> Union[int, float]
     """An exponential tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -406,15 +410,15 @@
     _checkRange(n)
     if n == 0:
         return 0
     else:
         return 2 ** (10 * (n - 1))
 
 
-def easeOutExpo(n):
+def easeOutExpo(n):  # type: (Union[int, float]) -> Union[int, float]
     """An exponential tween function that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -422,15 +426,15 @@
     _checkRange(n)
     if n == 1:
         return 1
     else:
         return -(2 ** (-10 * n)) + 1
 
 
-def easeInOutExpo(n):
+def easeInOutExpo(n):  # type: (Union[int, float]) -> Union[int, float]
     """An exponential tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -446,42 +450,42 @@
             return 0.5 * 2 ** (10 * (n - 1))
         else:
             n -= 1
             # 0.5 * (-() + 2)
             return 0.5 * (-1 * (2 ** (-10 * n)) + 2)
 
 
-def easeInCirc(n):
+def easeInCirc(n):  # type: (Union[int, float]) -> Union[int, float]
     """A circular tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return -1 * (math.sqrt(1 - n * n) - 1)
 
 
-def easeOutCirc(n):
+def easeOutCirc(n):  # type: (Union[int, float]) -> Union[int, float]
     """A circular tween function that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     n -= 1
     return math.sqrt(1 - (n * n))
 
 
-def easeInOutCirc(n):
+def easeInOutCirc(n):  # type: (Union[int, float]) -> Union[int, float]
     """A circular tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -491,28 +495,28 @@
     if n < 1:
         return -0.5 * (math.sqrt(1 - n**2) - 1)
     else:
         n -= 2
         return 0.5 * (math.sqrt(1 - n**2) + 1)
 
 
-def easeInElastic(n, amplitude=1, period=0.3):
+def easeInElastic(n, amplitude=1, period=0.3):  # type: (Union[int, float], Union[int, float], Union[int, float]) -> Union[int, float]
     """An elastic tween function that begins with an increasing wobble and then snaps into the destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return 1 - easeOutElastic(1 - n, amplitude=amplitude, period=period)
 
 
-def easeOutElastic(n, amplitude=1, period=0.3):
+def easeOutElastic(n, amplitude=1, period=0.3):  # type: (Union[int, float], Union[int, float], Union[int, float]) -> Union[int, float]
     """An elastic tween function that overshoots the destination and then "rubber bands" into the destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -524,15 +528,15 @@
         s = period / 4
     else:
         s = period / (2 * math.pi) * math.asin(1 / amplitude)
 
     return amplitude * 2 ** (-10 * n) * math.sin((n - s) * (2 * math.pi / period)) + 1
 
 
-def easeInOutElastic(n, amplitude=1, period=0.5):
+def easeInOutElastic(n, amplitude=1, period=0.5):  # type: (Union[int, float], Union[int, float], Union[int, float]) -> Union[int, float]
     """An elastic tween function wobbles towards the midpoint.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -541,42 +545,42 @@
     n *= 2
     if n < 1:
         return easeInElastic(n, amplitude=amplitude, period=period) / 2
     else:
         return easeOutElastic(n - 1, amplitude=amplitude, period=period) / 2 + 0.5
 
 
-def easeInBack(n, s=1.70158):
+def easeInBack(n, s=1.70158):  # type: (Union[int, float], Union[int, float]) -> Union[int, float]
     """A tween function that backs up first at the start and then goes to the destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return n * n * ((s + 1) * n - s)
 
 
-def easeOutBack(n, s=1.70158):
+def easeOutBack(n, s=1.70158):  # type: (Union[int, float], Union[int, float]) -> Union[int, float]
     """A tween function that overshoots the destination a little and then backs into the destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     n -= 1
     return n * n * ((s + 1) * n + s) + 1
 
 
-def easeInOutBack(n, s=1.70158):
+def easeInOutBack(n, s=1.70158):  # type: (Union[int, float], Union[int, float]) -> Union[int, float]
     """A "back-in" tween function that overshoots both the start and destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -588,28 +592,28 @@
         return 0.5 * (n * n * ((s + 1) * n - s))
     else:
         n -= 2
         s *= 1.525
         return 0.5 * (n * n * ((s + 1) * n + s) + 2)
 
 
-def easeInBounce(n):
+def easeInBounce(n):  # type: (Union[int, float]) -> Union[int, float]
     """A bouncing tween function that begins bouncing and then jumps to the destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     return 1 - easeOutBounce(1 - n)
 
 
-def easeOutBounce(n):
+def easeOutBounce(n):  # type: (Union[int, float]) -> Union[int, float]
     """A bouncing tween function that hits the destination and then bounces to rest.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
@@ -624,15 +628,15 @@
         n -= 2.25 / 2.75
         return 7.5625 * n * n + 0.9375
     else:
         n -= 2.65 / 2.75
         return 7.5625 * n * n + 0.984375
 
 
-def easeInOutBounce(n):
+def easeInOutBounce(n):  # type: (Union[int, float]) -> Union[int, float]
     """A bouncing tween function that bounces at the start and end.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
```

### Comparing `pytweening-1.0.5/tests/basicTests.py` & `pytweening-1.0.7/tests/basicTests.py`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/tests/generateExcelGraphs.py` & `pytweening-1.0.7/tests/generateExcelGraphs.py`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/tests/graphs.ipynb` & `pytweening-1.0.7/tests/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/tests/graphs.xlsx` & `pytweening-1.0.7/tests/graphs.xlsx`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.5/tests/seeGraphs.py` & `pytweening-1.0.7/tests/seeGraphs.py`

 * *Files identical despite different names*

