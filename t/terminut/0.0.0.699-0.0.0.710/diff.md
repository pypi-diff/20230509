# Comparing `tmp/terminut-0.0.0.699.tar.gz` & `tmp/terminut-0.0.0.710.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminut-0.0.0.699.tar", last modified: Mon May  8 23:22:02 2023, max compression
+gzip compressed data, was "terminut-0.0.0.710.tar", last modified: Mon May  8 23:58:37 2023, max compression
```

## Comparing `terminut-0.0.0.699.tar` & `terminut-0.0.0.710.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:22:02.438660 terminut-0.0.0.699/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.699/LICENSE
--rw-rw-rw-   0        0        0     1996 2023-05-08 23:22:02.437665 terminut-0.0.0.699/PKG-INFO
--rw-rw-rw-   0        0        0      816 2023-05-08 01:53:38.000000 terminut-0.0.0.699/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.699/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 23:22:02.438660 terminut-0.0.0.699/setup.cfg
--rw-rw-rw-   0        0        0     1600 2023-05-08 23:21:40.000000 terminut-0.0.0.699/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:22:02.420879 terminut-0.0.0.699/terminut/
--rw-rw-rw-   0        0        0      335 2023-05-08 02:35:20.000000 terminut-0.0.0.699/terminut/__init__.py
--rw-rw-rw-   0        0        0     2629 2023-05-08 23:20:47.000000 terminut-0.0.0.699/terminut/console.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:22:02.436665 terminut-0.0.0.699/terminut.egg-info/
--rw-rw-rw-   0        0        0     1996 2023-05-08 23:22:02.000000 terminut-0.0.0.699/terminut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-08 23:22:02.000000 terminut-0.0.0.699/terminut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:22:02.000000 terminut-0.0.0.699/terminut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-08 23:22:02.000000 terminut-0.0.0.699/terminut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 23:22:02.000000 terminut-0.0.0.699/terminut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 23:58:37.206208 terminut-0.0.0.710/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.710/LICENSE
+-rw-rw-rw-   0        0        0     1996 2023-05-08 23:58:37.206208 terminut-0.0.0.710/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2023-05-08 01:53:38.000000 terminut-0.0.0.710/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.710/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 23:58:37.206208 terminut-0.0.0.710/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2023-05-08 23:58:26.000000 terminut-0.0.0.710/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:58:37.193597 terminut-0.0.0.710/terminut/
+-rw-rw-rw-   0        0        0      363 2023-05-08 23:41:45.000000 terminut-0.0.0.710/terminut/__init__.py
+-rw-rw-rw-   0        0        0     3786 2023-05-08 23:58:14.000000 terminut-0.0.0.710/terminut/console.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:58:37.205210 terminut-0.0.0.710/terminut.egg-info/
+-rw-rw-rw-   0        0        0     1996 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/top_level.txt
```

### Comparing `terminut-0.0.0.699/LICENSE` & `terminut-0.0.0.710/LICENSE`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.699/PKG-INFO` & `terminut-0.0.0.710/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.699
+Version: 0.0.0.710
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
```

### Comparing `terminut-0.0.0.699/README.md` & `terminut-0.0.0.710/README.md`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.699/setup.py` & `terminut-0.0.0.710/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.699"
+vers = "0.0.0.710"
     
 setup(name="terminut",
       version=vers,
       description="Terminut // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `terminut-0.0.0.699/terminut.egg-info/PKG-INFO` & `terminut-0.0.0.710/terminut.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.699
+Version: 0.0.0.710
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
```

