# Comparing `tmp/spotipy_anon-1.0.tar.gz` & `tmp/spotipy_anon-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotipy_anon-1.0.tar", last modified: Tue May  9 15:32:19 2023, max compression
+gzip compressed data, was "spotipy_anon-1.1.tar", last modified: Tue May  9 16:14:18 2023, max compression
```

## Comparing `spotipy_anon-1.0.tar` & `spotipy_anon-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 15:32:19.523458 spotipy_anon-1.0/
--rw-rw-rw-   0        0        0     1082 2023-05-09 15:14:25.000000 spotipy_anon-1.0/LICENSE
--rw-rw-rw-   0        0        0     1843 2023-05-09 15:32:19.523458 spotipy_anon-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-05-09 15:14:25.000000 spotipy_anon-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 15:32:19.523458 spotipy_anon-1.0/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-05-09 15:25:55.000000 spotipy_anon-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:32:19.507408 spotipy_anon-1.0/spotipy_anon/
--rw-rw-rw-   0        0        0       58 2023-05-09 15:25:55.000000 spotipy_anon-1.0/spotipy_anon/__init__.py
--rw-rw-rw-   0        0        0     3991 2023-05-09 15:14:25.000000 spotipy_anon-1.0/spotipy_anon/oauth2.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:32:19.523458 spotipy_anon-1.0/spotipy_anon.egg-info/
--rw-rw-rw-   0        0        0     1843 2023-05-09 15:32:19.000000 spotipy_anon-1.0/spotipy_anon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-09 15:32:19.000000 spotipy_anon-1.0/spotipy_anon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 15:32:19.000000 spotipy_anon-1.0/spotipy_anon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 15:32:19.000000 spotipy_anon-1.0/spotipy_anon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-09 15:32:19.000000 spotipy_anon-1.0/spotipy_anon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 16:14:18.535687 spotipy_anon-1.1/
+-rw-rw-rw-   0        0        0     1102 2023-05-09 16:13:32.000000 spotipy_anon-1.1/LICENSE
+-rw-rw-rw-   0        0        0     1843 2023-05-09 16:14:18.535687 spotipy_anon-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2023-05-09 16:13:32.000000 spotipy_anon-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 16:14:18.535687 spotipy_anon-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      650 2023-05-09 16:13:32.000000 spotipy_anon-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:14:18.519165 spotipy_anon-1.1/spotipy_anon/
+-rw-rw-rw-   0        0        0       56 2023-05-09 16:13:32.000000 spotipy_anon-1.1/spotipy_anon/__init__.py
+-rw-rw-rw-   0        0        0     3991 2023-05-09 16:13:32.000000 spotipy_anon-1.1/spotipy_anon/oauth2.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:14:18.535687 spotipy_anon-1.1/spotipy_anon.egg-info/
+-rw-rw-rw-   0        0        0     1843 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/top_level.txt
```

### Comparing `spotipy_anon-1.0/LICENSE` & `spotipy_anon-1.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Niko
+Copyright (c) 2023 dieser-niko (dieserniko)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `spotipy_anon-1.0/PKG-INFO` & `spotipy_anon-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotipy_anon
-Version: 1.0
+Version: 1.1
 Summary: An extension to Spotipy for anonymous access to the Spotify Web API
 Home-page: https://github.com/dieser-niko/spotipy-anon
 Author: @dieserniko
 Author-email: dieserniko@gmx.de
 License: MIT
 Project-URL: Source, https://github.com/dieserniko/spotipy-anon
 Description: # SpotipyAnon
```

### Comparing `spotipy_anon-1.0/README.md` & `spotipy_anon-1.1/README.md`

 * *Files identical despite different names*

### Comparing `spotipy_anon-1.0/setup.py` & `spotipy_anon-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 
 setup(
     name='spotipy_anon',
-    version='1.0',
+    version='1.1',
     description='An extension to Spotipy for anonymous access to the Spotify Web API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="@dieserniko",
     author_email="dieserniko@gmx.de",
     url='https://github.com/dieser-niko/spotipy-anon',
     project_urls={
```

### Comparing `spotipy_anon-1.0/spotipy_anon/oauth2.py` & `spotipy_anon-1.1/spotipy_anon/oauth2.py`

 * *Files identical despite different names*

### Comparing `spotipy_anon-1.0/spotipy_anon.egg-info/PKG-INFO` & `spotipy_anon-1.1/spotipy_anon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotipy-anon
-Version: 1.0
+Version: 1.1
 Summary: An extension to Spotipy for anonymous access to the Spotify Web API
 Home-page: https://github.com/dieser-niko/spotipy-anon
 Author: @dieserniko
 Author-email: dieserniko@gmx.de
 License: MIT
 Project-URL: Source, https://github.com/dieserniko/spotipy-anon
 Description: # SpotipyAnon
```

