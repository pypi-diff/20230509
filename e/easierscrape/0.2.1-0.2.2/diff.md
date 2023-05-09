# Comparing `tmp/easierscrape-0.2.1.tar.gz` & `tmp/easierscrape-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierscrape-0.2.1.tar", last modified: Sat May  6 16:34:50 2023, max compression
+gzip compressed data, was "easierscrape-0.2.2.tar", last modified: Tue May  9 14:14:45 2023, max compression
```

## Comparing `easierscrape-0.2.1.tar` & `easierscrape-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.477454 easierscrape-0.2.1/
--rw-rw-rw-   0        0        0      550 2023-05-06 16:30:28.000000 easierscrape-0.2.1/.bumpversion.cfg
--rw-rw-rw-   0        0        0      289 2023-04-04 16:46:22.000000 easierscrape-0.2.1/.readthedocs.yml
--rw-rw-rw-   0        0        0     1105 2023-04-04 01:00:40.000000 easierscrape-0.2.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-04-04 01:00:40.000000 easierscrape-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      610 2023-04-04 17:02:03.000000 easierscrape-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2745 2023-04-11 20:59:45.000000 easierscrape-0.2.1/Makefile
--rw-rw-rw-   0        0        0    18493 2023-05-06 16:34:50.474191 easierscrape-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4461 2023-05-05 19:55:40.000000 easierscrape-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.380834 easierscrape-0.2.1/docs/
--rw-rw-rw-   0        0        0      654 2023-04-04 17:30:23.000000 easierscrape-0.2.1/docs/Makefile
--rw-rw-rw-   0        0        0     1098 2023-05-06 16:30:28.000000 easierscrape-0.2.1/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.390833 easierscrape-0.2.1/docs/images/
--rw-rw-rw-   0        0        0   242191 2023-05-06 16:10:24.000000 easierscrape-0.2.1/docs/images/cli_recording.gif
--rw-rw-rw-   0        0        0    92263 2023-05-06 16:10:24.000000 easierscrape-0.2.1/docs/images/demo_recording.gif
--rw-rw-rw-   0        0        0     2607 2023-05-06 16:10:24.000000 easierscrape-0.2.1/docs/index.md
--rwxrwxrwx   0        0        0      800 2023-04-04 17:30:23.000000 easierscrape-0.2.1/docs/make.bat
--rw-rw-rw-   0        0        0      109 2023-05-06 16:30:28.000000 easierscrape-0.2.1/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.398790 easierscrape-0.2.1/docs/source/
--rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.2.1/docs/source/easierscrape.rst
--rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.2.1/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.436680 easierscrape-0.2.1/easierscrape/
--rw-rw-rw-   0        0        0       64 2023-04-04 01:00:40.000000 easierscrape-0.2.1/easierscrape/__init__.py
--rw-rw-rw-   0        0        0      803 2023-05-06 16:10:24.000000 easierscrape-0.2.1/easierscrape/__main__.py
--rw-rw-rw-   0        0        0       23 2023-05-06 16:30:28.000000 easierscrape-0.2.1/easierscrape/_version.py
--rw-rw-rw-   0        0        0    10744 2023-05-06 16:10:24.000000 easierscrape-0.2.1/easierscrape/easierscrape.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.467815 easierscrape-0.2.1/easierscrape/tests/
--rw-rw-rw-   0        0        0    27216 2023-05-06 16:10:24.000000 easierscrape-0.2.1/easierscrape/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.457207 easierscrape-0.2.1/easierscrape.egg-info/
--rw-rw-rw-   0        0        0    18493 2023-05-06 16:34:49.000000 easierscrape-0.2.1/easierscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-06 16:34:50.000000 easierscrape-0.2.1/easierscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 16:34:49.000000 easierscrape-0.2.1/easierscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      246 2023-05-06 16:34:49.000000 easierscrape-0.2.1/easierscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 16:34:49.000000 easierscrape-0.2.1/easierscrape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2434 2023-05-06 16:30:29.000000 easierscrape-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 16:34:50.477454 easierscrape-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-04-04 01:00:40.000000 easierscrape-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:14:45.253967 easierscrape-0.2.2/
+-rw-rw-rw-   0        0        0      550 2023-05-09 14:10:27.000000 easierscrape-0.2.2/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      289 2023-04-04 16:46:22.000000 easierscrape-0.2.2/.readthedocs.yml
+-rw-rw-rw-   0        0        0     1105 2023-04-04 01:00:40.000000 easierscrape-0.2.2/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11543 2023-05-08 21:04:27.000000 easierscrape-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      640 2023-05-08 21:04:27.000000 easierscrape-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2745 2023-04-11 20:59:45.000000 easierscrape-0.2.2/Makefile
+-rw-rw-rw-   0        0        0    18478 2023-05-09 14:14:45.252172 easierscrape-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4461 2023-05-05 19:55:40.000000 easierscrape-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 14:14:45.138876 easierscrape-0.2.2/docs/
+-rw-rw-rw-   0        0        0      654 2023-04-04 17:30:23.000000 easierscrape-0.2.2/docs/Makefile
+-rw-rw-rw-   0        0        0     1098 2023-05-09 14:10:27.000000 easierscrape-0.2.2/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:14:45.157091 easierscrape-0.2.2/docs/images/
+-rw-rw-rw-   0        0        0   242191 2023-05-06 16:10:24.000000 easierscrape-0.2.2/docs/images/cli_recording.gif
+-rw-rw-rw-   0        0        0    92263 2023-05-06 16:10:24.000000 easierscrape-0.2.2/docs/images/demo_recording.gif
+-rw-rw-rw-   0        0        0    14927 2023-05-08 21:04:27.000000 easierscrape-0.2.2/docs/images/screenshot.png
+-rw-rw-rw-   0        0        0     3072 2023-05-08 21:04:27.000000 easierscrape-0.2.2/docs/index.md
+-rwxrwxrwx   0        0        0      800 2023-04-04 17:30:23.000000 easierscrape-0.2.2/docs/make.bat
+-rw-rw-rw-   0        0        0      109 2023-05-09 14:10:27.000000 easierscrape-0.2.2/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 14:14:45.166775 easierscrape-0.2.2/docs/source/
+-rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.2.2/docs/source/easierscrape.rst
+-rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.2.2/docs/source/modules.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 14:14:45.205397 easierscrape-0.2.2/easierscrape/
+-rw-rw-rw-   0        0        0       64 2023-04-04 01:00:40.000000 easierscrape-0.2.2/easierscrape/__init__.py
+-rw-rw-rw-   0        0        0      803 2023-05-06 16:10:24.000000 easierscrape-0.2.2/easierscrape/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-05-09 14:10:27.000000 easierscrape-0.2.2/easierscrape/_version.py
+-rw-rw-rw-   0        0        0    10744 2023-05-06 16:10:24.000000 easierscrape-0.2.2/easierscrape/easierscrape.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:14:45.244880 easierscrape-0.2.2/easierscrape/tests/
+-rw-rw-rw-   0        0        0    27216 2023-05-06 16:10:24.000000 easierscrape-0.2.2/easierscrape/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:14:45.232235 easierscrape-0.2.2/easierscrape.egg-info/
+-rw-rw-rw-   0        0        0    18478 2023-05-09 14:14:44.000000 easierscrape-0.2.2/easierscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-05-09 14:14:44.000000 easierscrape-0.2.2/easierscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:14:44.000000 easierscrape-0.2.2/easierscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      246 2023-05-09 14:14:44.000000 easierscrape-0.2.2/easierscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-09 14:14:44.000000 easierscrape-0.2.2/easierscrape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2434 2023-05-09 14:10:27.000000 easierscrape-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 14:14:45.254947 easierscrape-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-04-04 01:00:40.000000 easierscrape-0.2.2/setup.py
```

### Comparing `easierscrape-0.2.1/.bumpversion.cfg` & `easierscrape-0.2.2/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.1
+current_version = 0.2.2
 commit = True
 tag = True
 
 [bumpversion:file:easierscrape/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `easierscrape-0.2.1/CONTRIBUTING.md` & `easierscrape-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/LICENSE` & `easierscrape-0.2.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Daniel Greco
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `easierscrape-0.2.1/MANIFEST.in` & `easierscrape-0.2.2/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 include .readthedocs.yml
 include pyproject.toml
 include Makefile
 
 recursive-include docs *.bat
 recursive-include docs *.gif
 recursive-include docs *.md
+recursive-include docs *.png
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 
 prune .github
 exclude .gitignore
```

### Comparing `easierscrape-0.2.1/Makefile` & `easierscrape-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/PKG-INFO` & `easierscrape-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierscrape
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library which does some basic web scraping operations
 Author-email: Daniel Greco <dag2226@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,15 +187,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright 2023 Daniel Greco
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `easierscrape-0.2.1/README.md` & `easierscrape-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/docs/Makefile` & `easierscrape-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/docs/conf.py` & `easierscrape-0.2.2/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -- Path setup --------------------------------------------------------------
 sys.path.insert(0, os.path.abspath('../'))
 
 # -- Project information -----------------------------------------------------
 project = 'easierscrape'
 copyright = '2023, Daniel Greco'
 author = 'Daniel Greco'
-release = '0.2.1'
+release = '0.2.2'
 
 master_doc = 'index'
 
 # -- General configuration ---------------------------------------------------
 extensions = ['recommonmark', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages', 'sphinx.ext.napoleon']
 source_suffix = ['.rst', '.md']
```

### Comparing `easierscrape-0.2.1/docs/images/cli_recording.gif` & `easierscrape-0.2.2/docs/images/cli_recording.gif`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/docs/images/demo_recording.gif` & `easierscrape-0.2.2/docs/images/demo_recording.gif`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/docs/make.bat` & `easierscrape-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/easierscrape/__main__.py` & `easierscrape-0.2.2/easierscrape/__main__.py`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/easierscrape/easierscrape.py` & `easierscrape-0.2.2/easierscrape/easierscrape.py`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/easierscrape/tests/test_all.py` & `easierscrape-0.2.2/easierscrape/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.1/easierscrape.egg-info/PKG-INFO` & `easierscrape-0.2.2/easierscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierscrape
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library which does some basic web scraping operations
 Author-email: Daniel Greco <dag2226@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,15 +187,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright 2023 Daniel Greco
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `easierscrape-0.2.1/easierscrape.egg-info/SOURCES.txt` & `easierscrape-0.2.2/easierscrape.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docs/Makefile
 docs/conf.py
 docs/index.md
 docs/make.bat
 docs/requirements.txt
 docs/images/cli_recording.gif
 docs/images/demo_recording.gif
+docs/images/screenshot.png
 docs/source/easierscrape.rst
 docs/source/modules.rst
 easierscrape/__init__.py
 easierscrape/__main__.py
 easierscrape/_version.py
 easierscrape/easierscrape.py
 easierscrape.egg-info/PKG-INFO
```

### Comparing `easierscrape-0.2.1/pyproject.toml` & `easierscrape-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "easierscrape"
 authors = [{name = "Daniel Greco", email = "dag2226@columbia.edu"}]
 description="A library which does some basic web scraping operations"
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.2"
 requires-python = ">=3.7"
 
 dependencies = [
     "anytree",
     "beautifulsoup4",
     "lxml",
     "openpyxl",
```

