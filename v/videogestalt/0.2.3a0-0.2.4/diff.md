# Comparing `tmp/videogestalt-0.2.3a0.tar.gz` & `tmp/videogestalt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videogestalt-0.2.3a0.tar", last modified: Mon May  8 10:49:06 2023, max compression
+gzip compressed data, was "videogestalt-0.2.4.tar", last modified: Mon May  8 22:06:45 2023, max compression
```

## Comparing `videogestalt-0.2.3a0.tar` & `videogestalt-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:49:06.775918 videogestalt-0.2.3a0/
--rw-rw-rw-   0        0        0    16725 2023-05-07 23:32:02.000000 videogestalt-0.2.3a0/LICENSE
--rw-rw-rw-   0        0        0      194 2023-05-07 23:32:02.000000 videogestalt-0.2.3a0/MANIFEST.in
--rw-rw-rw-   0        0        0     6344 2023-05-08 10:49:06.768937 videogestalt-0.2.3a0/PKG-INFO
--rw-rw-rw-   0        0        0     4051 2023-05-08 00:12:49.000000 videogestalt-0.2.3a0/README.md
--rw-rw-rw-   0        0        0     4815 2023-05-08 10:48:29.000000 videogestalt-0.2.3a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 10:49:06.776916 videogestalt-0.2.3a0/setup.cfg
--rw-rw-rw-   0        0        0      455 2023-05-07 23:32:02.000000 videogestalt-0.2.3a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:49:06.684237 videogestalt-0.2.3a0/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 10:49:06.719070 videogestalt-0.2.3a0/src/videogestalt/
--rw-rw-rw-   0        0        0     7302 2023-05-07 23:32:02.000000 videogestalt-0.2.3a0/src/videogestalt/videogestalt.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:49:06.760958 videogestalt-0.2.3a0/src/videogestalt.egg-info/
--rw-rw-rw-   0        0        0     6344 2023-05-08 10:49:06.000000 videogestalt-0.2.3a0/src/videogestalt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-05-08 10:49:06.000000 videogestalt-0.2.3a0/src/videogestalt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:49:06.000000 videogestalt-0.2.3a0/src/videogestalt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-08 10:49:06.000000 videogestalt-0.2.3a0/src/videogestalt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2023-05-08 10:49:06.000000 videogestalt-0.2.3a0/src/videogestalt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 10:49:06.000000 videogestalt-0.2.3a0/src/videogestalt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 22:06:45.039221 videogestalt-0.2.4/
+-rw-rw-rw-   0        0        0    16725 2023-05-08 22:05:15.000000 videogestalt-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-05-08 22:05:15.000000 videogestalt-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6342 2023-05-08 22:06:45.039221 videogestalt-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4051 2023-05-08 22:05:15.000000 videogestalt-0.2.4/README.md
+-rw-rw-rw-   0        0        0     4814 2023-05-08 22:05:15.000000 videogestalt-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 22:06:45.039221 videogestalt-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-05-08 22:05:15.000000 videogestalt-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:06:45.023598 videogestalt-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 22:06:45.039221 videogestalt-0.2.4/src/videogestalt/
+-rw-rw-rw-   0        0        0     7302 2023-05-08 22:05:15.000000 videogestalt-0.2.4/src/videogestalt/videogestalt.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:06:45.039221 videogestalt-0.2.4/src/videogestalt.egg-info/
+-rw-rw-rw-   0        0        0     6342 2023-05-08 22:06:45.000000 videogestalt-0.2.4/src/videogestalt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-05-08 22:06:45.000000 videogestalt-0.2.4/src/videogestalt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 22:06:45.000000 videogestalt-0.2.4/src/videogestalt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-08 22:06:45.000000 videogestalt-0.2.4/src/videogestalt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2023-05-08 22:06:45.000000 videogestalt-0.2.4/src/videogestalt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 22:06:45.000000 videogestalt-0.2.4/src/videogestalt.egg-info/top_level.txt
```

### Comparing `videogestalt-0.2.3a0/LICENSE` & `videogestalt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `videogestalt-0.2.3a0/PKG-INFO` & `videogestalt-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videogestalt
-Version: 0.2.3a0
+Version: 0.2.4
 Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
 Author: Eamonn O'Brien-Strain
 Maintainer: Eamonn O'Brien-Strain
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: Mozilla Public License 2.0
 Project-URL: Homepage, https://github.com/eobrain/videogestalt
 Project-URL: Documentation, https://github.com/eobrain/videogestalt/blob/master/README.md
```

### Comparing `videogestalt-0.2.3a0/README.md` & `videogestalt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `videogestalt-0.2.3a0/pyproject.toml` & `videogestalt-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 # never uppercap requirements unless we have evidence it won't work https://iscinumpy.dev/post/bound-version-constraints/ 
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]  # beware if using setuptools: setup.py still gets executed, and even if pyproject.toml fields take precedence, if there is any code error in setup.py, building will fail!
 name = "videogestalt"
-version = "0.2.3a"  # see PEP 440 https://peps.python.org/pep-0440/#pre-releases and https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
+version = "0.2.4"  # see PEP 440 https://peps.python.org/pep-0440/#pre-releases and https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
 description = "Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!"
 authors = [
     {name = "Eamonn O'Brien-Strain"},
     ]
 maintainers = [
     {name = "Eamonn O'Brien-Strain"},
     {name = "Stephen Karl Larroque", email = "lrq3000@gmail.com"},
```

### Comparing `videogestalt-0.2.3a0/src/videogestalt/videogestalt.py` & `videogestalt-0.2.4/src/videogestalt/videogestalt.py`

 * *Files identical despite different names*

### Comparing `videogestalt-0.2.3a0/src/videogestalt.egg-info/PKG-INFO` & `videogestalt-0.2.4/src/videogestalt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videogestalt
-Version: 0.2.3a0
+Version: 0.2.4
 Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
 Author: Eamonn O'Brien-Strain
 Maintainer: Eamonn O'Brien-Strain
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: Mozilla Public License 2.0
 Project-URL: Homepage, https://github.com/eobrain/videogestalt
 Project-URL: Documentation, https://github.com/eobrain/videogestalt/blob/master/README.md
```

