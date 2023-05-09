# Comparing `tmp/prettycopy-0.2.0.tar.gz` & `tmp/prettycopy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettycopy-0.2.0.tar", last modified: Sat May  6 02:30:39 2023, max compression
+gzip compressed data, was "prettycopy-0.2.1.tar", last modified: Tue May  9 03:02:16 2023, max compression
```

## Comparing `prettycopy-0.2.0.tar` & `prettycopy-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.972949 prettycopy-0.2.0/
--rw-rw-rw-   0        0        0      533 2023-05-04 21:01:54.000000 prettycopy-0.2.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0      772 2023-04-17 05:17:35.000000 prettycopy-0.2.0/.readthedocs.yaml
--rw-rw-rw-   0        0        0     2197 2023-04-17 05:17:35.000000 prettycopy-0.2.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-02-08 23:02:52.000000 prettycopy-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      584 2023-04-17 05:17:35.000000 prettycopy-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2254 2023-04-22 23:54:45.000000 prettycopy-0.2.0/Makefile
--rw-rw-rw-   0        0        0    18270 2023-05-06 02:30:39.970973 prettycopy-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4210 2023-05-06 02:29:22.000000 prettycopy-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.863949 prettycopy-0.2.0/docs/
--rw-rw-rw-   0        0        0      634 2023-03-31 21:48:57.000000 prettycopy-0.2.0/docs/Makefile
--rw-rw-rw-   0        0        0     1302 2023-05-04 21:01:54.000000 prettycopy-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0     2343 2023-05-03 21:49:41.000000 prettycopy-0.2.0/docs/dev_intro.md
-drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.923951 prettycopy-0.2.0/docs/images/
--rw-rw-rw-   0        0        0   563910 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/bullets_nopc.gif
--rw-rw-rw-   0        0        0   464377 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/bullettopar_pc.gif
--rw-rw-rw-   0        0        0   471068 2023-05-06 02:29:22.000000 prettycopy-0.2.0/docs/images/nobullets_pc.gif
--rw-rw-rw-   0        0        0    72027 2023-05-03 21:49:41.000000 prettycopy-0.2.0/docs/images/pchelp.gif
--rw-rw-rw-   0        0        0   161236 2023-05-03 21:49:41.000000 prettycopy-0.2.0/docs/images/pcnonewlines.gif
--rw-rw-rw-   0        0        0   324242 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/quote_pc.gif
--rw-rw-rw-   0        0        0   292299 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/quotes_nopc.gif
--rw-rw-rw-   0        0        0   297103 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/simplequote_pc.gif
--rw-rw-rw-   0        0        0   312971 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/smartcopy_pc.gif
--rw-rw-rw-   0        0        0   151015 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/trimspace_nopc.gif
--rw-rw-rw-   0        0        0   164560 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/trimspacing_pc.gif
--rw-rw-rw-   0        0        0     7654 2023-05-06 02:29:22.000000 prettycopy-0.2.0/docs/index.md
--rwxrwxrwx   0        0        0      765 2023-03-31 21:48:57.000000 prettycopy-0.2.0/docs/make.bat
--rw-rw-rw-   0        0        0       64 2023-04-23 00:24:41.000000 prettycopy-0.2.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.941949 prettycopy-0.2.0/prettycopy/
--rw-rw-rw-   0        0        0      103 2023-05-04 21:01:54.000000 prettycopy-0.2.0/prettycopy/__init__.py
--rw-rw-rw-   0        0        0       69 2023-05-03 21:49:41.000000 prettycopy-0.2.0/prettycopy/__main__.py
--rw-rw-rw-   0        0        0       22 2023-05-04 21:01:54.000000 prettycopy-0.2.0/prettycopy/_version.py
--rw-rw-rw-   0        0        0     3256 2023-05-06 02:29:22.000000 prettycopy-0.2.0/prettycopy/command_line.py
--rw-rw-rw-   0        0        0    11579 2023-05-06 02:29:22.000000 prettycopy-0.2.0/prettycopy/prettycopy.py
-drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.966951 prettycopy-0.2.0/prettycopy/tests/
--rw-rw-rw-   0        0        0    26120 2023-05-06 02:29:22.000000 prettycopy-0.2.0/prettycopy/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.962955 prettycopy-0.2.0/prettycopy.egg-info/
--rw-rw-rw-   0        0        0    18270 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      259 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2371 2023-05-06 02:29:22.000000 prettycopy-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 02:30:39.973959 prettycopy-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-27 19:31:32.000000 prettycopy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:02:16.693688 prettycopy-0.2.1/
+-rw-rw-rw-   0        0        0      533 2023-05-09 02:59:42.000000 prettycopy-0.2.1/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      772 2023-04-17 05:17:35.000000 prettycopy-0.2.1/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     2197 2023-04-17 05:17:35.000000 prettycopy-0.2.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-02-08 23:02:52.000000 prettycopy-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      584 2023-04-17 05:17:35.000000 prettycopy-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2254 2023-04-22 23:54:45.000000 prettycopy-0.2.1/Makefile
+-rw-rw-rw-   0        0        0    17468 2023-05-09 03:02:16.692692 prettycopy-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3422 2023-05-09 02:47:10.000000 prettycopy-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 03:02:16.583690 prettycopy-0.2.1/docs/
+-rw-rw-rw-   0        0        0      634 2023-03-31 21:48:57.000000 prettycopy-0.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0     1302 2023-05-09 02:59:42.000000 prettycopy-0.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0     2343 2023-05-03 21:49:41.000000 prettycopy-0.2.1/docs/dev_intro.md
+drwxrwxrwx   0        0        0        0 2023-05-09 03:02:16.647689 prettycopy-0.2.1/docs/images/
+-rw-rw-rw-   0        0        0   563910 2023-05-04 20:53:34.000000 prettycopy-0.2.1/docs/images/bullets_nopc.gif
+-rw-rw-rw-   0        0        0   464526 2023-05-06 03:09:17.000000 prettycopy-0.2.1/docs/images/bullettolist_pc.gif
+-rw-rw-rw-   0        0        0   464377 2023-05-04 20:53:34.000000 prettycopy-0.2.1/docs/images/bullettopar_pc.gif
+-rw-rw-rw-   0        0        0    72027 2023-05-03 21:49:41.000000 prettycopy-0.2.1/docs/images/pchelp.gif
+-rw-rw-rw-   0        0        0   161236 2023-05-03 21:49:41.000000 prettycopy-0.2.1/docs/images/pcnonewlines.gif
+-rw-rw-rw-   0        0        0   324242 2023-05-04 20:53:34.000000 prettycopy-0.2.1/docs/images/quote_pc.gif
+-rw-rw-rw-   0        0        0   292299 2023-05-04 20:53:34.000000 prettycopy-0.2.1/docs/images/quotes_nopc.gif
+-rw-rw-rw-   0        0        0   489167 2023-05-09 02:47:10.000000 prettycopy-0.2.1/docs/images/remove_pc.gif
+-rw-rw-rw-   0        0        0   297103 2023-05-04 20:53:34.000000 prettycopy-0.2.1/docs/images/simplequote_pc.gif
+-rw-rw-rw-   0        0        0   312971 2023-05-04 20:53:34.000000 prettycopy-0.2.1/docs/images/smartcopy_pc.gif
+-rw-rw-rw-   0        0        0   151015 2023-05-04 20:53:34.000000 prettycopy-0.2.1/docs/images/trimspace_nopc.gif
+-rw-rw-rw-   0        0        0   164560 2023-05-04 20:53:34.000000 prettycopy-0.2.1/docs/images/trimspacing_pc.gif
+-rw-rw-rw-   0        0        0     8077 2023-05-09 02:47:10.000000 prettycopy-0.2.1/docs/index.md
+-rwxrwxrwx   0        0        0      765 2023-03-31 21:48:57.000000 prettycopy-0.2.1/docs/make.bat
+-rw-rw-rw-   0        0        0       64 2023-05-09 02:47:10.000000 prettycopy-0.2.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 03:02:16.665691 prettycopy-0.2.1/prettycopy/
+-rw-rw-rw-   0        0        0      103 2023-05-09 02:59:42.000000 prettycopy-0.2.1/prettycopy/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-03 21:49:41.000000 prettycopy-0.2.1/prettycopy/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-05-09 02:59:42.000000 prettycopy-0.2.1/prettycopy/_version.py
+-rw-rw-rw-   0        0        0     3970 2023-05-09 02:47:10.000000 prettycopy-0.2.1/prettycopy/command_line.py
+-rw-rw-rw-   0        0        0    13251 2023-05-09 02:51:01.000000 prettycopy-0.2.1/prettycopy/prettycopy.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:02:16.687690 prettycopy-0.2.1/prettycopy/tests/
+-rw-rw-rw-   0        0        0    29416 2023-05-09 02:47:10.000000 prettycopy-0.2.1/prettycopy/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:02:16.683688 prettycopy-0.2.1/prettycopy.egg-info/
+-rw-rw-rw-   0        0        0    17468 2023-05-09 03:02:16.000000 prettycopy-0.2.1/prettycopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      909 2023-05-09 03:02:16.000000 prettycopy-0.2.1/prettycopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 03:02:16.000000 prettycopy-0.2.1/prettycopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-09 03:02:16.000000 prettycopy-0.2.1/prettycopy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      244 2023-05-09 03:02:16.000000 prettycopy-0.2.1/prettycopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 03:02:16.000000 prettycopy-0.2.1/prettycopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2349 2023-05-09 02:59:42.000000 prettycopy-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 03:02:16.694691 prettycopy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-27 19:31:32.000000 prettycopy-0.2.1/setup.py
```

### Comparing `prettycopy-0.2.0/.bumpversion.cfg` & `prettycopy-0.2.1/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 commit = True
 tag = True
 
 [bumpversion:file:prettycopy/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `prettycopy-0.2.0/.readthedocs.yaml` & `prettycopy-0.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/CONTRIBUTING.md` & `prettycopy-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/LICENSE` & `prettycopy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/MANIFEST.in` & `prettycopy-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/Makefile` & `prettycopy-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/PKG-INFO` & `prettycopy-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettycopy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A better copy-paster
 Author-email: Adi Gal <adigal03@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,20 +224,20 @@
 A beginner-friendly library for clean, format-friendly copy-pasting.
 
 [![License](https://img.shields.io/github/license/hippothebrave/prettycopy)](https://github.com/hippothebrave/prettycopy/blob/main/LICENSE)
 [![GitHub issues](https://img.shields.io/github/issues/hippothebrave/prettycopy)](https://github.com/hippothebrave/prettycopy/issues)
 [![Build Status](https://github.com/hippothebrave/prettycopy/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/hippothebrave/prettycopy/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/hippothebrave/prettycopy/branch/main/graph/badge.svg)](https://codecov.io/gh/hippothebrave/prettycopy)
 [![PyPI](https://img.shields.io/pypi/v/prettycopy)](https://pypi.org/project/prettycopy/)
-[![Documentation](https://img.shields.io/badge/Documentation-ReadTheDocs-informational)](https://prettycopy.readthedocs.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/prettycopy/badge/?version=latest)](https://prettycopy.readthedocs.io/en/latest/?badge=latest)
 
 ## Overview
 Copying and pasting text is one of the most commonly-used functionalities we have on our computers. But sometimes, there are formatting issues in the text you're copying that a simple 'paste without formatting' can't fix.
 
-Enter prettycopy.
+Enter PrettyCopy.
 
 PrettyCopy will help you clean up the text on your clipboard *before* you paste it. Just copy text, run a PrettyCopy function, and you'll be able to paste it with corrections already in place!
 
 See our documentation [here](https://prettycopy.readthedocs.io/en/latest/).
 
 ### Installation
 
@@ -245,15 +245,17 @@
 
 ```bash
 pip install prettycopy
 ```
 
 ## Usage
 
-So... how do you use PrettyCopy? It's very simple! You can use PrettyCopy at the command line, or through your own program.
+So... how do you use PrettyCopy? It's very simple! You can use PrettyCopy functions at the command line, or through your own program.
+
+Learn more about the functions using `prettycopy --help` at the command line, or by checking our [documentation](https://prettycopy.readthedocs.io/en/latest/).
 
 ### Command Line
 Copy a piece of text.
 In the command line, type `prettycopy [function_name] [any_args]`. 
 PrettyCopy will print the corrected text, just to show you what your clipboard current contains. 
 Now, as soon as you paste, the text will already be corrected.
 
@@ -261,30 +263,14 @@
 
 Confused? Type `prettycopy --help` to get a list of possible functions, and `prettycopy [function_name] --help` to get help for any particular function.
 
 ### In a Program
 PrettyCopy will take in some text, correct it, and copy the corrected text to your clipboard. It will also return the corrected text as a return value, in case you want to keep using it (for example, in a nested function).
 By default, PrettyCopy will run on the text in your clipboard. If you want to correct a different text, enter your preferred text as an argument.
 
-### Functions
-
-`prettycopy.nonewlines(optional_text)`: Removes all line breaks from the text.
-
-`prettycopy.nobullets(optional_text)`: Removes all bullet symbols (•) and replaces them with line breaks.
-
-`prettycopy.bullettopar(optional_text)`: Removes all line breaks and bullet symbols (•) and replaces them with spaces, returning a single paragraph.
-
-`prettycopy.simplequote(optional_text)`: Adds quotation marks around the text.
-
-`prettycopy.quote(optional_end_punctuation, optional_text)`: Adds quotation marks around the text, ending in a punctuation mark. The default is a comma.
-
-> Example: *this is a test* --> prettycopy.quote() --> *"this is a test,"*
-
-> Example: *this is a test* --> prettycopy.quote('!') --> *"this is a test!"*
-
-`prettycopy.trimspacing(optional_text)`: Removes empty lines.
+## Examples
+PrettyCopy can be used for fixing issues with line breaks; removing extraneous bullet point symbols; adding quotation marks (and optional punctuation) around a copied text; and more! 
 
-`prettycopy.smartcopy(optional_text)`: Removes line breaks in an intelligent manner: adding spaces between words, but not inside words that have been split.
+![](https://github.com/hippothebrave/prettycopy/blob/main/docs/images/smartcopy_pc.gif)
 
-> Example: *this\nis a te\nst* --> prettycopy.smartcopy() --> *this is a test*
+See the [documentation](https://prettycopy.readthedocs.io/en/latest/) for the complete list of functions.
 
-`prettycopy.betterbullets(docID)`: If you enter the document ID of an editable Google Doc (the long string of letters and numbers in the URL), this function will copy the text in your clipboard to the end of the document, replacing all bullet symbols (•) with correctly-formatted bullet points. Still under construction.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prettycopy-0.2.0/README.md` & `prettycopy-0.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 A beginner-friendly library for clean, format-friendly copy-pasting.
 
 [![License](https://img.shields.io/github/license/hippothebrave/prettycopy)](https://github.com/hippothebrave/prettycopy/blob/main/LICENSE)
 [![GitHub issues](https://img.shields.io/github/issues/hippothebrave/prettycopy)](https://github.com/hippothebrave/prettycopy/issues)
 [![Build Status](https://github.com/hippothebrave/prettycopy/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/hippothebrave/prettycopy/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/hippothebrave/prettycopy/branch/main/graph/badge.svg)](https://codecov.io/gh/hippothebrave/prettycopy)
 [![PyPI](https://img.shields.io/pypi/v/prettycopy)](https://pypi.org/project/prettycopy/)
-[![Documentation](https://img.shields.io/badge/Documentation-ReadTheDocs-informational)](https://prettycopy.readthedocs.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/prettycopy/badge/?version=latest)](https://prettycopy.readthedocs.io/en/latest/?badge=latest)
 
 ## Overview
 Copying and pasting text is one of the most commonly-used functionalities we have on our computers. But sometimes, there are formatting issues in the text you're copying that a simple 'paste without formatting' can't fix.
 
-Enter prettycopy.
+Enter PrettyCopy.
 
 PrettyCopy will help you clean up the text on your clipboard *before* you paste it. Just copy text, run a PrettyCopy function, and you'll be able to paste it with corrections already in place!
 
 See our documentation [here](https://prettycopy.readthedocs.io/en/latest/).
 
 ### Installation
 
@@ -23,15 +23,17 @@
 
 ```bash
 pip install prettycopy
 ```
 
 ## Usage
 
-So... how do you use PrettyCopy? It's very simple! You can use PrettyCopy at the command line, or through your own program.
+So... how do you use PrettyCopy? It's very simple! You can use PrettyCopy functions at the command line, or through your own program.
+
+Learn more about the functions using `prettycopy --help` at the command line, or by checking our [documentation](https://prettycopy.readthedocs.io/en/latest/).
 
 ### Command Line
 Copy a piece of text.
 In the command line, type `prettycopy [function_name] [any_args]`. 
 PrettyCopy will print the corrected text, just to show you what your clipboard current contains. 
 Now, as soon as you paste, the text will already be corrected.
 
@@ -39,30 +41,14 @@
 
 Confused? Type `prettycopy --help` to get a list of possible functions, and `prettycopy [function_name] --help` to get help for any particular function.
 
 ### In a Program
 PrettyCopy will take in some text, correct it, and copy the corrected text to your clipboard. It will also return the corrected text as a return value, in case you want to keep using it (for example, in a nested function).
 By default, PrettyCopy will run on the text in your clipboard. If you want to correct a different text, enter your preferred text as an argument.
 
-### Functions
-
-`prettycopy.nonewlines(optional_text)`: Removes all line breaks from the text.
-
-`prettycopy.nobullets(optional_text)`: Removes all bullet symbols (•) and replaces them with line breaks.
-
-`prettycopy.bullettopar(optional_text)`: Removes all line breaks and bullet symbols (•) and replaces them with spaces, returning a single paragraph.
-
-`prettycopy.simplequote(optional_text)`: Adds quotation marks around the text.
-
-`prettycopy.quote(optional_end_punctuation, optional_text)`: Adds quotation marks around the text, ending in a punctuation mark. The default is a comma.
-
-> Example: *this is a test* --> prettycopy.quote() --> *"this is a test,"*
-
-> Example: *this is a test* --> prettycopy.quote('!') --> *"this is a test!"*
-
-`prettycopy.trimspacing(optional_text)`: Removes empty lines.
+## Examples
+PrettyCopy can be used for fixing issues with line breaks; removing extraneous bullet point symbols; adding quotation marks (and optional punctuation) around a copied text; and more! 
 
-`prettycopy.smartcopy(optional_text)`: Removes line breaks in an intelligent manner: adding spaces between words, but not inside words that have been split.
+![](https://github.com/hippothebrave/prettycopy/blob/main/docs/images/smartcopy_pc.gif)
 
-> Example: *this\nis a te\nst* --> prettycopy.smartcopy() --> *this is a test*
+See the [documentation](https://prettycopy.readthedocs.io/en/latest/) for the complete list of functions.
 
-`prettycopy.betterbullets(docID)`: If you enter the document ID of an editable Google Doc (the long string of letters and numbers in the URL), this function will copy the text in your clipboard to the end of the document, replacing all bullet symbols (•) with correctly-formatted bullet points. Still under construction.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prettycopy-0.2.0/docs/Makefile` & `prettycopy-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/conf.py` & `prettycopy-0.2.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'prettycopy'
 copyright = '2023, Adi Gal'
 author = 'Adi Gal'
-release = "0.2.0"
+release = "0.2.1"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['myst_parser', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages'] #prev, recommonmark
 source_suffix = ['.rst', '.md']
```

### Comparing `prettycopy-0.2.0/docs/dev_intro.md` & `prettycopy-0.2.1/docs/dev_intro.md`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/bullets_nopc.gif` & `prettycopy-0.2.1/docs/images/bullets_nopc.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/bullettopar_pc.gif` & `prettycopy-0.2.1/docs/images/bullettopar_pc.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/pchelp.gif` & `prettycopy-0.2.1/docs/images/pchelp.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/pcnonewlines.gif` & `prettycopy-0.2.1/docs/images/pcnonewlines.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/quote_pc.gif` & `prettycopy-0.2.1/docs/images/quote_pc.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/quotes_nopc.gif` & `prettycopy-0.2.1/docs/images/quotes_nopc.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/simplequote_pc.gif` & `prettycopy-0.2.1/docs/images/simplequote_pc.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/smartcopy_pc.gif` & `prettycopy-0.2.1/docs/images/smartcopy_pc.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/trimspace_nopc.gif` & `prettycopy-0.2.1/docs/images/trimspace_nopc.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/images/trimspacing_pc.gif` & `prettycopy-0.2.1/docs/images/trimspacing_pc.gif`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/docs/index.md` & `prettycopy-0.2.1/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 6060 607b 746f 6374 7265 657d 0a3a 6869  ```{toctree}.:hi
 00000010: 6464 656e 3a0a 0a64 6576 5f69 6e74 726f  dden:..dev_intro
 00000020: 2e6d 640a 6060 600a 0a23 2057 656c 636f  .md.```..# Welco
-00000030: 6d65 2074 6f20 7072 6574 7479 636f 7079  me to prettycopy
+00000030: 6d65 2074 6f20 5072 6574 7479 436f 7079  me to PrettyCopy
 00000040: 2773 2064 6f63 756d 656e 7461 7469 6f6e  's documentation
 00000050: 210a 0a57 656c 636f 6d65 2074 6f20 5072  !..Welcome to Pr
 00000060: 6574 7479 436f 7079 3a20 6120 6265 6769  ettyCopy: a begi
 00000070: 6e6e 6572 2d66 7269 656e 646c 7920 6c69  nner-friendly li
 00000080: 6272 6172 7920 696e 7465 6e64 6564 2074  brary intended t
 00000090: 6f20 656e 7375 7265 2063 6c65 616e 2c20  o ensure clean, 
 000000a0: 666f 726d 6174 2d66 7269 656e 646c 7920  format-friendly 
@@ -49,431 +49,457 @@
 00000300: 2e69 6f2f 6768 2f68 6970 706f 7468 6562  .io/gh/hippotheb
 00000310: 7261 7665 2f70 7265 7474 7963 6f70 7929  rave/prettycopy)
 00000320: 0a5b 215b 5079 5049 5d28 6874 7470 733a  .[![PyPI](https:
 00000330: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
 00000340: 2f70 7970 692f 762f 7072 6574 7479 636f  /pypi/v/prettyco
 00000350: 7079 295d 2868 7474 7073 3a2f 2f70 7970  py)](https://pyp
 00000360: 692e 6f72 672f 7072 6f6a 6563 742f 7072  i.org/project/pr
-00000370: 6574 7479 636f 7079 2f29 0a0a 2323 204f  ettycopy/)..## O
-00000380: 7665 7276 6965 770a 4576 6572 796f 6e65  verview.Everyone
-00000390: 2063 6f70 6965 7320 616e 6420 7061 7374   copies and past
-000003a0: 6573 2074 6578 742e 2042 7574 2073 6f6d  es text. But som
-000003b0: 6574 696d 6573 2c20 7468 6572 6520 6172  etimes, there ar
-000003c0: 6520 666f 726d 6174 7469 6e67 2069 7373  e formatting iss
-000003d0: 7565 7320 696e 2074 6865 2074 6578 7420  ues in the text 
-000003e0: 796f 7527 7265 2063 6f70 7969 6e67 2d2d  you're copying--
-000003f0: 616e 6420 7768 6f20 7761 6e74 7320 746f  and who wants to
-00000400: 2073 7065 6e64 2074 6865 6972 2074 696d   spend their tim
-00000410: 6520 636f 7272 6563 7469 6e67 2066 6f72  e correcting for
-00000420: 6d61 743f 0a0a 456e 7465 7220 5072 6574  mat?..Enter Pret
-00000430: 7479 436f 7079 2e0a 0a50 7265 7474 7943  tyCopy...PrettyC
-00000440: 6f70 7920 7769 6c6c 2068 656c 7020 796f  opy will help yo
-00000450: 7520 636c 6561 6e20 7570 2074 6865 2074  u clean up the t
-00000460: 6578 7420 6f6e 2079 6f75 7220 636c 6970  ext on your clip
-00000470: 626f 6172 6420 2a62 6566 6f72 652a 2079  board *before* y
-00000480: 6f75 2070 6173 7465 2069 742e 204a 7573  ou paste it. Jus
-00000490: 7420 636f 7079 2074 6578 742c 2072 756e  t copy text, run
-000004a0: 2061 2050 7265 7474 7943 6f70 7920 6675   a PrettyCopy fu
-000004b0: 6e63 7469 6f6e 2c20 616e 6420 796f 7527  nction, and you'
-000004c0: 6c6c 2062 6520 6162 6c65 2074 6f20 7061  ll be able to pa
-000004d0: 7374 6520 6974 2077 6974 6820 636f 7272  ste it with corr
-000004e0: 6563 7469 6f6e 7320 2a61 6c72 6561 6479  ections *already
-000004f0: 2069 6e20 706c 6163 652a 210a 0a23 2320   in place*!..## 
-00000500: 496e 7374 616c 6c61 7469 6f6e 0a0a 4966  Installation..If
-00000510: 2079 6f75 2061 6c72 6561 6479 2068 6176   you already hav
-00000520: 6520 5079 7468 6f6e 2c20 6a75 7374 2072  e Python, just r
-00000530: 756e 3a0a 0a60 6060 7079 7468 6f6e 0a70  un:..```python.p
-00000540: 6970 2069 6e73 7461 6c6c 2070 7265 7474  ip install prett
-00000550: 7963 6f70 790a 6060 600a 0a23 2320 5573  ycopy.```..## Us
-00000560: 6167 650a 0a53 6f2e 2e2e 2068 6f77 2064  age..So... how d
-00000570: 6f20 796f 7520 7573 6520 5072 6574 7479  o you use Pretty
-00000580: 436f 7079 3f20 4974 2773 2076 6572 7920  Copy? It's very 
-00000590: 7369 6d70 6c65 2120 596f 7520 6361 6e20  simple! You can 
-000005a0: 7573 6520 5072 6574 7479 436f 7079 2061  use PrettyCopy a
-000005b0: 7420 7468 6520 636f 6d6d 616e 6420 6c69  t the command li
-000005c0: 6e65 2c20 6f72 2074 6872 6f75 6768 2079  ne, or through y
-000005d0: 6f75 7220 6f77 6e20 7072 6f67 7261 6d2e  our own program.
-000005e0: 0a0a 2323 2320 436f 6d6d 616e 6420 4c69  ..### Command Li
-000005f0: 6e65 0a43 6f70 7920 6120 7069 6563 6520  ne.Copy a piece 
-00000600: 6f66 2074 6578 742e 0a49 6e20 7468 6520  of text..In the 
-00000610: 636f 6d6d 616e 6420 6c69 6e65 2c20 7479  command line, ty
-00000620: 7065 2060 7072 6574 7479 636f 7079 205b  pe `prettycopy [
-00000630: 6675 6e63 7469 6f6e 5f6e 616d 655d 205b  function_name] [
-00000640: 616e 795f 6172 6773 5d60 2e20 0a50 7265  any_args]`. .Pre
-00000650: 7474 7943 6f70 7920 7769 6c6c 2070 7269  ttyCopy will pri
-00000660: 6e74 2074 6865 2028 636f 7272 6563 7465  nt the (correcte
-00000670: 6429 2063 6f6e 7465 6e74 7320 6f66 2079  d) contents of y
-00000680: 6f75 7220 636c 6970 626f 6172 642e 0a57  our clipboard..W
-00000690: 6865 6e20 796f 7520 7061 7374 652c 2074  hen you paste, t
-000006a0: 6865 2074 6578 7420 7769 6c6c 2061 6c72  he text will alr
-000006b0: 6561 6479 2062 6520 636f 7272 6563 7465  eady be correcte
-000006c0: 6421 0a0a 5468 6572 6520 6172 6520 616c  d!..There are al
-000006d0: 736f 206f 7074 696f 6e61 6c20 2a66 6c61  so optional *fla
-000006e0: 6773 2e2a 200a 602d 2d6e 6f2d 6f75 7470  gs.* .`--no-outp
-000006f0: 7574 6020 7769 6c6c 2070 7265 7665 6e74  ut` will prevent
-00000700: 2050 7265 7474 7943 6f70 7920 6672 6f6d   PrettyCopy from
-00000710: 2063 6f70 7969 6e67 2079 6f75 7220 636c   copying your cl
-00000720: 6970 626f 6172 6420 636f 6e74 656e 7473  ipboard contents
-00000730: 2074 6f20 7468 6520 7465 726d 696e 616c   to the terminal
-00000740: 2e20 2855 7365 6675 6c20 666f 7220 6c6f  . (Useful for lo
-00000750: 6e67 2069 6e70 7574 732e 290a 602d 2d74  ng inputs.).`--t
-00000760: 6578 7420 2279 6f75 725f 7465 7874 5f68  ext "your_text_h
-00000770: 6572 6522 6020 616c 6c6f 7773 2079 6f75  ere"` allows you
-00000780: 2074 6f20 7573 6520 6120 636f 6d6d 616e   to use a comman
-00000790: 642d 6c69 6e65 2073 7472 696e 6720 2874  d-line string (t
-000007a0: 6f20 7468 6520 6c65 6674 206f 6620 7468  o the left of th
-000007b0: 6520 666c 6167 2c20 656e 6361 7365 6420  e flag, encased 
-000007c0: 696e 2071 756f 7461 7469 6f6e 206d 6172  in quotation mar
-000007d0: 6b73 2920 696e 7374 6561 6420 6f66 2079  ks) instead of y
-000007e0: 6f75 7220 6375 7272 656e 7420 636c 6970  our current clip
-000007f0: 626f 6172 6420 636f 6e74 656e 7473 2e20  board contents. 
-00000800: 4e6f 7465 2074 6861 7420 2a79 6f75 7220  Note that *your 
-00000810: 636c 6970 626f 6172 6420 636f 6e74 656e  clipboard conten
-00000820: 7473 2077 696c 6c20 7374 696c 6c20 6265  ts will still be
-00000830: 2072 6570 6c61 6365 642a 2120 0a0a 436f   replaced*! ..Co
-00000840: 6e66 7573 6564 3f20 5479 7065 2060 7072  nfused? Type `pr
-00000850: 6574 7479 636f 7079 202d 2d68 656c 7060  ettycopy --help`
-00000860: 2074 6f20 6765 7420 6120 6c69 7374 206f   to get a list o
-00000870: 6620 706f 7373 6962 6c65 2066 756e 6374  f possible funct
-00000880: 696f 6e73 2c20 616e 6420 6070 7265 7474  ions, and `prett
-00000890: 7963 6f70 7920 5b66 756e 6374 696f 6e5f  ycopy [function_
-000008a0: 6e61 6d65 5d20 2d2d 6865 6c70 6020 746f  name] --help` to
-000008b0: 2067 6574 2068 656c 7020 666f 7220 616e   get help for an
-000008c0: 7920 7061 7274 6963 756c 6172 2066 756e  y particular fun
-000008d0: 6374 696f 6e2e 0a0a 6060 607b 6576 616c  ction...```{eval
-000008e0: 2d72 7374 7d0a 2e2e 2069 6d61 6765 3a3a  -rst}... image::
-000008f0: 2068 7474 7073 3a2f 2f72 6177 2e67 6974   https://raw.git
-00000900: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000910: 6f6d 2f68 6970 706f 7468 6562 7261 7665  om/hippothebrave
-00000920: 2f70 7265 7474 7963 6f70 792f 6d61 696e  /prettycopy/main
-00000930: 2f64 6f63 732f 696d 6167 6573 2f70 6368  /docs/images/pch
-00000940: 656c 702e 6769 660a 2020 2020 3a77 6964  elp.gif.    :wid
-00000950: 7468 3a20 3730 300a 2020 2020 3a61 6c69  th: 700.    :ali
-00000960: 676e 3a20 6365 6e74 6572 0a60 6060 0a0a  gn: center.```..
-00000970: 2323 2320 496e 2061 2050 726f 6772 616d  ### In a Program
-00000980: 0a45 6163 6820 5072 6574 7479 436f 7079  .Each PrettyCopy
-00000990: 2066 756e 6374 696f 6e20 7461 6b65 7320   function takes 
-000009a0: 696e 2061 2073 7472 696e 672c 2063 6f72  in a string, cor
-000009b0: 7265 6374 7320 6974 2c20 616e 6420 636f  rects it, and co
-000009c0: 7069 6573 2074 6865 2063 6f72 7265 6374  pies the correct
-000009d0: 6564 2074 6578 7420 746f 2079 6f75 7220  ed text to your 
-000009e0: 636c 6970 626f 6172 642e 2049 7420 7769  clipboard. It wi
-000009f0: 6c6c 2061 6c73 6f20 7265 7475 726e 2074  ll also return t
-00000a00: 6865 2063 6f72 7265 6374 6564 2074 6578  he corrected tex
-00000a10: 7420 6173 2061 2072 6574 7572 6e20 7661  t as a return va
-00000a20: 6c75 652c 2069 6e20 6361 7365 2079 6f75  lue, in case you
-00000a30: 2077 616e 7420 746f 206b 6565 7020 7573   want to keep us
-00000a40: 696e 6720 6974 2028 666f 7220 6578 616d  ing it (for exam
-00000a50: 706c 652c 2069 6e20 6120 6e65 7374 6564  ple, in a nested
-00000a60: 2066 756e 6374 696f 6e29 2e0a 4279 2064   function)..By d
-00000a70: 6566 6175 6c74 2c20 5072 6574 7479 436f  efault, PrettyCo
-00000a80: 7079 2077 696c 6c20 7275 6e20 6f6e 2074  py will run on t
-00000a90: 6865 2074 6578 7420 696e 2079 6f75 7220  he text in your 
-00000aa0: 636c 6970 626f 6172 642e 2049 6620 796f  clipboard. If yo
-00000ab0: 7520 7761 6e74 2074 6f20 636f 7272 6563  u want to correc
-00000ac0: 7420 6120 6469 6666 6572 656e 7420 7465  t a different te
-00000ad0: 7874 2c20 656e 7465 7220 796f 7572 2070  xt, enter your p
-00000ae0: 7265 6665 7272 6564 2074 6578 7420 6173  referred text as
-00000af0: 2061 6e20 6172 6775 6d65 6e74 2e0a 0a23   an argument...#
-00000b00: 2320 4675 6e63 7469 6f6e 730a 0a23 2323  # Functions..###
-00000b10: 2053 6d61 7274 2043 6f70 792d 616e 642d   Smart Copy-and-
-00000b20: 5061 7365 0a0a 5768 656e 2063 6f70 7969  Pase..When copyi
-00000b30: 6e67 2061 6e64 2070 6173 7469 6e67 2062  ng and pasting b
-00000b40: 6574 7765 656e 2066 6f72 6d61 7473 2c20  etween formats, 
-00000b50: 6c69 6e65 2062 7265 616b 7320 6361 6e20  line breaks can 
-00000b60: 6170 7065 6172 2062 6574 7765 656e 2c20  appear between, 
-00000b70: 6f72 2065 7665 6e20 7769 7468 696e 2c20  or even within, 
-00000b80: 6f72 6469 6e61 7279 2077 6f72 6473 2e0a  ordinary words..
-00000b90: 0a60 6060 7b65 7661 6c2d 7273 747d 0a2e  .```{eval-rst}..
-00000ba0: 2e20 696d 6167 653a 3a20 6874 7470 733a  . image:: https:
-00000bb0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000bc0: 636f 6e74 656e 742e 636f 6d2f 6869 7070  content.com/hipp
-00000bd0: 6f74 6865 6272 6176 652f 7072 6574 7479  othebrave/pretty
-00000be0: 636f 7079 2f6d 6169 6e2f 646f 6373 2f69  copy/main/docs/i
-00000bf0: 6d61 6765 732f 736d 6172 7463 6f70 795f  mages/smartcopy_
-00000c00: 7063 2e67 6966 0a20 2020 203a 7769 6474  pc.gif.    :widt
-00000c10: 683a 2037 3030 0a20 2020 203a 616c 6967  h: 700.    :alig
-00000c20: 6e3a 2063 656e 7465 720a 6060 600a 0a54  n: center.```..T
-00000c30: 6865 2060 736d 6172 7463 6f70 7960 2066  he `smartcopy` f
-00000c40: 756e 6374 696f 6e20 6361 6e20 666f 7220  unction can for 
-00000c50: 7468 6520 6d6f 7374 2070 6172 7420 6469  the most part di
-00000c60: 7374 696e 6775 6973 6820 6265 7477 6565  stinguish betwee
-00000c70: 6e20 7468 656d 2c20 616c 6c6f 7769 6e67  n them, allowing
-00000c80: 2079 6f75 7220 636f 7079 2d61 6e64 2d70   your copy-and-p
-00000c90: 6173 7465 2065 7870 6572 6965 6e63 6520  aste experience 
-00000ca0: 746f 2062 6520 6173 2073 6d6f 6f74 6820  to be as smooth 
-00000cb0: 6173 2070 6f73 7369 626c 652e 0a0a 6060  as possible...``
-00000cc0: 607b 6576 616c 2d72 7374 7d0a 2e2e 2061  `{eval-rst}... a
-00000cd0: 7574 6f66 756e 6374 696f 6e3a 3a20 7072  utofunction:: pr
-00000ce0: 6574 7479 636f 7079 2e70 7265 7474 7963  ettycopy.prettyc
+00000370: 6574 7479 636f 7079 2f29 0a5b 215b 446f  ettycopy/).[![Do
+00000380: 6375 6d65 6e74 6174 696f 6e20 5374 6174  cumentation Stat
+00000390: 7573 5d28 6874 7470 733a 2f2f 7265 6164  us](https://read
+000003a0: 7468 6564 6f63 732e 6f72 672f 7072 6f6a  thedocs.org/proj
+000003b0: 6563 7473 2f70 7265 7474 7963 6f70 792f  ects/prettycopy/
+000003c0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+000003d0: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
+000003e0: 7072 6574 7479 636f 7079 2e72 6561 6474  prettycopy.readt
+000003f0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000400: 6573 742f 3f62 6164 6765 3d6c 6174 6573  est/?badge=lates
+00000410: 7429 0a0a 2323 204f 7665 7276 6965 770a  t)..## Overview.
+00000420: 4576 6572 7962 6f64 7920 636f 7069 6573  Everybody copies
+00000430: 2061 6e64 2070 6173 7465 7320 7465 7874   and pastes text
+00000440: 2e20 4275 7420 736f 6d65 7469 6d65 732c  . But sometimes,
+00000450: 2074 6865 7265 2061 7265 2066 6f72 6d61   there are forma
+00000460: 7474 696e 6720 6973 7375 6573 2069 6e20  tting issues in 
+00000470: 7468 6520 7465 7874 2079 6f75 2772 6520  the text you're 
+00000480: 636f 7079 696e 672d 2d61 6e64 2077 686f  copying--and who
+00000490: 2077 616e 7473 2074 6f20 7370 656e 6420   wants to spend 
+000004a0: 616c 6c20 7468 6569 7220 7469 6d65 2063  all their time c
+000004b0: 6f72 7265 6374 696e 6720 666f 726d 6174  orrecting format
+000004c0: 7469 6e67 3f0a 0a45 6e74 6572 2050 7265  ting?..Enter Pre
+000004d0: 7474 7943 6f70 792e 0a0a 5072 6574 7479  ttyCopy...Pretty
+000004e0: 436f 7079 2077 696c 6c20 6865 6c70 2079  Copy will help y
+000004f0: 6f75 2063 6c65 616e 2075 7020 7468 6520  ou clean up the 
+00000500: 7465 7874 206f 6e20 796f 7572 2063 6c69  text on your cli
+00000510: 7062 6f61 7264 202a 6265 666f 7265 2a20  pboard *before* 
+00000520: 796f 7520 7061 7374 6520 6974 2e20 4a75  you paste it. Ju
+00000530: 7374 2063 6f70 7920 7465 7874 2c20 7275  st copy text, ru
+00000540: 6e20 6120 5072 6574 7479 436f 7079 2066  n a PrettyCopy f
+00000550: 756e 6374 696f 6e2c 2061 6e64 2079 6f75  unction, and you
+00000560: 276c 6c20 6265 2061 626c 6520 746f 2070  'll be able to p
+00000570: 6173 7465 2069 7420 7769 7468 2063 6f72  aste it with cor
+00000580: 7265 6374 696f 6e73 202a 616c 7265 6164  rections *alread
+00000590: 7920 696e 2070 6c61 6365 2a21 0a0a 2323  y in place*!..##
+000005a0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a49   Installation..I
+000005b0: 6620 796f 7520 616c 7265 6164 7920 6861  f you already ha
+000005c0: 7665 2050 7974 686f 6e2c 206a 7573 7420  ve Python, just 
+000005d0: 7275 6e3a 0a0a 6060 6070 7974 686f 6e0a  run:..```python.
+000005e0: 7069 7020 696e 7374 616c 6c20 7072 6574  pip install pret
+000005f0: 7479 636f 7079 0a60 6060 0a0a 2323 2055  tycopy.```..## U
+00000600: 7361 6765 0a0a 536f 2e2e 2e20 686f 7720  sage..So... how 
+00000610: 646f 2079 6f75 2075 7365 2050 7265 7474  do you use Prett
+00000620: 7943 6f70 793f 2049 7427 7320 7665 7279  yCopy? It's very
+00000630: 2073 696d 706c 6521 2059 6f75 2063 616e   simple! You can
+00000640: 2075 7365 2050 7265 7474 7943 6f70 7920   use PrettyCopy 
+00000650: 6174 2074 6865 2063 6f6d 6d61 6e64 206c  at the command l
+00000660: 696e 652c 206f 7220 7468 726f 7567 6820  ine, or through 
+00000670: 796f 7572 206f 776e 2070 726f 6772 616d  your own program
+00000680: 2e0a 0a23 2323 2043 6f6d 6d61 6e64 204c  ...### Command L
+00000690: 696e 650a 436f 7079 2061 2070 6965 6365  ine.Copy a piece
+000006a0: 206f 6620 7465 7874 2e0a 0a49 6e20 7468   of text...In th
+000006b0: 6520 636f 6d6d 616e 6420 6c69 6e65 2c20  e command line, 
+000006c0: 7479 7065 2060 7072 6574 7479 636f 7079  type `prettycopy
+000006d0: 205b 6675 6e63 7469 6f6e 5f6e 616d 655d   [function_name]
+000006e0: 205b 616e 795f 6172 6773 5d60 2e20 0a0a   [any_args]`. ..
+000006f0: 5072 6574 7479 436f 7079 2077 696c 6c20  PrettyCopy will 
+00000700: 7072 696e 7420 7468 6520 2863 6f72 7265  print the (corre
+00000710: 6374 6564 2920 636f 6e74 656e 7473 206f  cted) contents o
+00000720: 6620 796f 7572 2063 6c69 7062 6f61 7264  f your clipboard
+00000730: 2e0a 0a57 6865 6e20 796f 7520 7061 7374  ...When you past
+00000740: 652c 2074 6865 2074 6578 7420 7769 6c6c  e, the text will
+00000750: 2061 6c72 6561 6479 2062 6520 636f 7272   already be corr
+00000760: 6563 7465 6421 0a0a 0a54 6865 7265 2061  ected!...There a
+00000770: 7265 2061 6c73 6f20 6f70 7469 6f6e 616c  re also optional
+00000780: 202a 666c 6167 732e 2a20 0a0a 602d 2d6e   *flags.* ..`--n
+00000790: 6f2d 6f75 7470 7574 6020 7769 6c6c 2070  o-output` will p
+000007a0: 7265 7665 6e74 2050 7265 7474 7943 6f70  revent PrettyCop
+000007b0: 7920 6672 6f6d 2063 6f70 7969 6e67 2079  y from copying y
+000007c0: 6f75 7220 636c 6970 626f 6172 6420 636f  our clipboard co
+000007d0: 6e74 656e 7473 2074 6f20 7468 6520 7465  ntents to the te
+000007e0: 726d 696e 616c 2e20 2855 7365 6675 6c20  rminal. (Useful 
+000007f0: 666f 7220 6c6f 6e67 2069 6e70 7574 732e  for long inputs.
+00000800: 290a 0a60 2d2d 7465 7874 2022 796f 7572  )..`--text "your
+00000810: 5f74 6578 745f 6865 7265 2260 2061 6c6c  _text_here"` all
+00000820: 6f77 7320 796f 7520 746f 2075 7365 2061  ows you to use a
+00000830: 2063 6f6d 6d61 6e64 2d6c 696e 6520 7374   command-line st
+00000840: 7269 6e67 2028 746f 2074 6865 2072 6967  ring (to the rig
+00000850: 6874 206f 6620 7468 6520 666c 6167 2c20  ht of the flag, 
+00000860: 656e 6361 7365 6420 696e 2071 756f 7461  encased in quota
+00000870: 7469 6f6e 206d 6172 6b73 2920 696e 7374  tion marks) inst
+00000880: 6561 6420 6f66 2079 6f75 7220 6375 7272  ead of your curr
+00000890: 656e 7420 636c 6970 626f 6172 6420 636f  ent clipboard co
+000008a0: 6e74 656e 7473 2e20 4e6f 7465 2074 6861  ntents. Note tha
+000008b0: 7420 2a79 6f75 7220 636c 6970 626f 6172  t *your clipboar
+000008c0: 6420 636f 6e74 656e 7473 2077 696c 6c20  d contents will 
+000008d0: 7374 696c 6c20 6265 2072 6570 6c61 6365  still be replace
+000008e0: 642a 2120 0a0a 436f 6e66 7573 6564 3f20  d*! ..Confused? 
+000008f0: 5479 7065 2060 7072 6574 7479 636f 7079  Type `prettycopy
+00000900: 202d 2d68 656c 7060 2074 6f20 6765 7420   --help` to get 
+00000910: 6120 6c69 7374 206f 6620 706f 7373 6962  a list of possib
+00000920: 6c65 2066 756e 6374 696f 6e73 2c20 616e  le functions, an
+00000930: 6420 6070 7265 7474 7963 6f70 7920 5b66  d `prettycopy [f
+00000940: 756e 6374 696f 6e5f 6e61 6d65 5d20 2d2d  unction_name] --
+00000950: 6865 6c70 6020 746f 2067 6574 2068 656c  help` to get hel
+00000960: 7020 666f 7220 616e 7920 7061 7274 6963  p for any partic
+00000970: 756c 6172 2066 756e 6374 696f 6e2e 0a0a  ular function...
+00000980: 6060 607b 6576 616c 2d72 7374 7d0a 2e2e  ```{eval-rst}...
+00000990: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
+000009a0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+000009b0: 6f6e 7465 6e74 2e63 6f6d 2f68 6970 706f  ontent.com/hippo
+000009c0: 7468 6562 7261 7665 2f70 7265 7474 7963  thebrave/prettyc
+000009d0: 6f70 792f 6d61 696e 2f64 6f63 732f 696d  opy/main/docs/im
+000009e0: 6167 6573 2f70 6368 656c 702e 6769 660a  ages/pchelp.gif.
+000009f0: 2020 2020 3a77 6964 7468 3a20 3730 300a      :width: 700.
+00000a00: 2020 2020 3a61 6c69 676e 3a20 6365 6e74      :align: cent
+00000a10: 6572 0a60 6060 0a0a 2323 2320 496e 2061  er.```..### In a
+00000a20: 2050 726f 6772 616d 0a45 6163 6820 5072   Program.Each Pr
+00000a30: 6574 7479 436f 7079 2066 756e 6374 696f  ettyCopy functio
+00000a40: 6e20 7461 6b65 7320 696e 2061 2073 7472  n takes in a str
+00000a50: 696e 672c 2063 6f72 7265 6374 7320 6974  ing, corrects it
+00000a60: 2c20 616e 6420 636f 7069 6573 2074 6865  , and copies the
+00000a70: 2063 6f72 7265 6374 6564 2074 6578 7420   corrected text 
+00000a80: 746f 2079 6f75 7220 636c 6970 626f 6172  to your clipboar
+00000a90: 642e 2049 7420 7769 6c6c 2061 6c73 6f20  d. It will also 
+00000aa0: 7265 7475 726e 2074 6865 2063 6f72 7265  return the corre
+00000ab0: 6374 6564 2074 6578 7420 6173 2061 2072  cted text as a r
+00000ac0: 6574 7572 6e20 7661 6c75 652c 2069 6e20  eturn value, in 
+00000ad0: 6361 7365 2079 6f75 2077 616e 7420 746f  case you want to
+00000ae0: 206b 6565 7020 7573 696e 6720 6974 2028   keep using it (
+00000af0: 666f 7220 6578 616d 706c 652c 2069 6e20  for example, in 
+00000b00: 6120 6e65 7374 6564 2066 756e 6374 696f  a nested functio
+00000b10: 6e29 2e0a 0a42 7920 6465 6661 756c 742c  n)...By default,
+00000b20: 2050 7265 7474 7943 6f70 7920 7769 6c6c   PrettyCopy will
+00000b30: 2072 756e 206f 6e20 7468 6520 7465 7874   run on the text
+00000b40: 2069 6e20 796f 7572 2063 6c69 7062 6f61   in your clipboa
+00000b50: 7264 2e20 4966 2079 6f75 2077 616e 7420  rd. If you want 
+00000b60: 746f 2063 6f72 7265 6374 2061 2064 6966  to correct a dif
+00000b70: 6665 7265 6e74 2074 6578 742c 2065 6e74  ferent text, ent
+00000b80: 6572 2079 6f75 7220 7072 6566 6572 7265  er your preferre
+00000b90: 6420 7465 7874 2061 7320 616e 2061 7267  d text as an arg
+00000ba0: 756d 656e 742e 0a0a 2323 2046 756e 6374  ument...## Funct
+00000bb0: 696f 6e73 0a0a 2323 2320 536d 6172 7420  ions..### Smart 
+00000bc0: 436f 7079 2d61 6e64 2d50 6173 7465 0a0a  Copy-and-Paste..
+00000bd0: 5768 656e 2063 6f70 7969 6e67 2061 6e64  When copying and
+00000be0: 2070 6173 7469 6e67 2062 6574 7765 656e   pasting between
+00000bf0: 2066 6f72 6d61 7473 2c20 6c69 6e65 2062   formats, line b
+00000c00: 7265 616b 7320 6361 6e20 6170 7065 6172  reaks can appear
+00000c10: 2062 6574 7765 656e 2c20 6f72 2065 7665   between, or eve
+00000c20: 6e20 7769 7468 696e 2c20 6f72 6469 6e61  n within, ordina
+00000c30: 7279 2077 6f72 6473 2e20 5468 6520 6073  ry words. The `s
+00000c40: 6d61 7274 636f 7079 6020 6675 6e63 7469  martcopy` functi
+00000c50: 6f6e 2063 616e 2066 6f72 2074 6865 206d  on can for the m
+00000c60: 6f73 7420 7061 7274 2064 6973 7469 6e67  ost part disting
+00000c70: 7569 7368 2062 6574 7765 656e 2074 6865  uish between the
+00000c80: 6d2c 2061 6c6c 6f77 696e 6720 796f 7572  m, allowing your
+00000c90: 2063 6f70 792d 616e 642d 7061 7374 6520   copy-and-paste 
+00000ca0: 6578 7065 7269 656e 6365 2074 6f20 6265  experience to be
+00000cb0: 2061 7320 736d 6f6f 7468 2061 7320 706f   as smooth as po
+00000cc0: 7373 6962 6c65 2e0a 0a60 6060 7b65 7661  ssible...```{eva
+00000cd0: 6c2d 7273 747d 0a2e 2e20 6175 746f 6675  l-rst}... autofu
+00000ce0: 6e63 7469 6f6e 3a3a 2070 7265 7474 7963  nction:: prettyc
 00000cf0: 6f70 792e 736d 6172 7463 6f70 790a 6060  opy.smartcopy.``
 00000d00: 600a 0a45 5841 4d50 4c45 533a 0a0a 6060  `..EXAMPLES:..``
 00000d10: 607b 6576 616c 2d72 7374 7d0a 2e2e 2069  `{eval-rst}... i
 00000d20: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f72  mage:: https://r
 00000d30: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
 00000d40: 7465 6e74 2e63 6f6d 2f68 6970 706f 7468  tent.com/hippoth
 00000d50: 6562 7261 7665 2f70 7265 7474 7963 6f70  ebrave/prettycop
 00000d60: 792f 6d61 696e 2f64 6f63 732f 696d 6167  y/main/docs/imag
 00000d70: 6573 2f73 6d61 7274 636f 7079 5f70 632e  es/smartcopy_pc.
 00000d80: 6769 660a 2020 2020 3a77 6964 7468 3a20  gif.    :width: 
 00000d90: 3730 300a 2020 2020 3a61 6c69 676e 3a20  700.    :align: 
 00000da0: 6365 6e74 6572 0a60 6060 0a0a 6060 6070  center.```..```p
 00000db0: 7974 686f 6e0a 696d 706f 7274 2070 7265  ython.import pre
-00000dc0: 7474 7963 6f70 792e 7072 6574 7479 636f  ttycopy.prettyco
-00000dd0: 7079 2061 7320 7063 0a23 2049 6620 796f  py as pc.# If yo
-00000de0: 7520 6861 7665 2063 6f70 6965 6420 7468  u have copied th
-00000df0: 6520 7465 7874 3a0a 2020 2020 2320 4578  e text:.    # Ex
-00000e00: 616d 706c 6520 7365 6e0a 2020 2020 2320  ample sen.    # 
-00000e10: 7465 6e63 6520 676f 6573 0a20 2020 2023  tence goes.    #
-00000e20: 2068 6572 652e 0a70 632e 736d 6172 7463   here..pc.smartc
-00000e30: 6f70 7928 290a 2320 796f 7572 2063 6c69  opy().# your cli
-00000e40: 7062 6f61 7264 2063 6f6e 7465 6e74 2062  pboard content b
-00000e50: 6563 6f6d 6573 3a20 0a20 2020 2023 2045  ecomes: .    # E
-00000e60: 7861 6d70 6c65 2073 656e 7465 6e63 6520  xample sentence 
-00000e70: 676f 6573 2068 6572 652e 0a60 6060 0a0a  goes here..```..
-00000e80: 2323 2320 4275 6c6c 6574 2d50 6f69 6e74  ### Bullet-Point
-00000e90: 2043 6c65 616e 696e 670a 0a53 6f6d 6574   Cleaning..Somet
-00000ea0: 696d 6573 2079 6f75 2077 616e 7420 746f  imes you want to
-00000eb0: 2063 6f70 7920 6120 7069 6563 6520 6f66   copy a piece of
-00000ec0: 2074 6578 7420 7769 7468 2062 756c 6c65   text with bulle
-00000ed0: 7420 706f 696e 7473 2e20 5468 6973 2064  t points. This d
-00000ee0: 6f65 736e 2774 2061 6c77 6179 7320 776f  oesn't always wo
-00000ef0: 726b 2074 6865 2077 6179 2079 6f75 2764  rk the way you'd
-00000f00: 206c 696b 6520 6974 2074 6f2e 0a0a 6060   like it to...``
-00000f10: 607b 6576 616c 2d72 7374 7d0a 2e2e 2069  `{eval-rst}... i
-00000f20: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f72  mage:: https://r
-00000f30: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000f40: 7465 6e74 2e63 6f6d 2f68 6970 706f 7468  tent.com/hippoth
-00000f50: 6562 7261 7665 2f70 7265 7474 7963 6f70  ebrave/prettycop
-00000f60: 792f 6d61 696e 2f64 6f63 732f 696d 6167  y/main/docs/imag
-00000f70: 6573 2f62 756c 6c65 7473 5f6e 6f70 632e  es/bullets_nopc.
-00000f80: 6769 660a 2020 2020 3a77 6964 7468 3a20  gif.    :width: 
-00000f90: 3730 300a 2020 2020 3a61 6c69 676e 3a20  700.    :align: 
-00000fa0: 6365 6e74 6572 0a60 6060 0a0a 5573 696e  center.```..Usin
-00000fb0: 6720 5072 6574 7479 436f 7079 2c20 796f  g PrettyCopy, yo
-00000fc0: 7520 6361 6e20 7475 726e 2074 6865 2074  u can turn the t
-00000fd0: 6578 7420 696e 746f 2061 2063 6c65 616e  ext into a clean
-00000fe0: 206c 6973 742c 206f 7220 696e 746f 2061   list, or into a
-00000ff0: 2073 696e 676c 6520 7061 7261 6772 6170   single paragrap
-00001000: 682e 0a0a 6060 607b 6576 616c 2d72 7374  h...```{eval-rst
-00001010: 7d0a 2e2e 2061 7574 6f66 756e 6374 696f  }... autofunctio
-00001020: 6e3a 3a20 7072 6574 7479 636f 7079 2e70  n:: prettycopy.p
-00001030: 7265 7474 7963 6f70 792e 6e6f 6275 6c6c  rettycopy.nobull
-00001040: 6574 730a 6060 600a 0a45 5841 4d50 4c45  ets.```..EXAMPLE
-00001050: 533a 0a0a 6060 607b 6576 616c 2d72 7374  S:..```{eval-rst
-00001060: 7d0a 2e2e 2069 6d61 6765 3a3a 2068 7474  }... image:: htt
-00001070: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00001080: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f68  sercontent.com/h
-00001090: 6970 706f 7468 6562 7261 7665 2f70 7265  ippothebrave/pre
-000010a0: 7474 7963 6f70 792f 6d61 696e 2f64 6f63  ttycopy/main/doc
-000010b0: 732f 696d 6167 6573 2f6e 6f62 756c 6c65  s/images/nobulle
-000010c0: 7473 5f70 632e 6769 660a 2020 2020 3a77  ts_pc.gif.    :w
-000010d0: 6964 7468 3a20 3730 300a 2020 2020 3a61  idth: 700.    :a
-000010e0: 6c69 676e 3a20 6365 6e74 6572 0a60 6060  lign: center.```
-000010f0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-00001100: 7274 2070 7265 7474 7963 6f70 792e 7072  rt prettycopy.pr
-00001110: 6574 7479 636f 7079 2061 7320 7063 0a23  ettycopy as pc.#
-00001120: 2049 6620 796f 7520 6861 7665 2063 6f70   If you have cop
-00001130: 6965 6420 7468 6520 7465 7874 3a0a 2020  ied the text:.  
-00001140: 2020 2320 e280 a220 4578 616d 706c 650a    # ... Example.
-00001150: 2020 2020 2320 e280 a220 7465 7874 0a20      # ... text. 
-00001160: 2020 2023 20e2 80a2 2068 6572 650a 7063     # ... here.pc
-00001170: 2e6e 6f62 756c 6c65 7473 2829 0a23 2079  .nobullets().# y
-00001180: 6f75 7220 636c 6970 626f 6172 6420 636f  our clipboard co
-00001190: 6e74 656e 7420 6265 636f 6d65 733a 200a  ntent becomes: .
-000011a0: 2020 2020 2320 4578 616d 706c 6520 0a20      # Example . 
-000011b0: 2020 2023 2074 6578 7420 0a20 2020 2023     # text .    #
-000011c0: 2068 6572 650a 6060 600a 0a0a 0a60 6060   here.```....```
-000011d0: 7b65 7661 6c2d 7273 747d 0a2e 2e20 6175  {eval-rst}... au
-000011e0: 746f 6675 6e63 7469 6f6e 3a3a 2070 7265  tofunction:: pre
-000011f0: 7474 7963 6f70 792e 7072 6574 7479 636f  ttycopy.prettyco
-00001200: 7079 2e62 756c 6c65 7474 6f70 6172 0a60  py.bullettopar.`
-00001210: 6060 0a0a 4558 414d 504c 4553 3a0a 0a60  ``..EXAMPLES:..`
-00001220: 6060 7b65 7661 6c2d 7273 747d 0a2e 2e20  ``{eval-rst}... 
-00001230: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-00001240: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00001250: 6e74 656e 742e 636f 6d2f 6869 7070 6f74  ntent.com/hippot
-00001260: 6865 6272 6176 652f 7072 6574 7479 636f  hebrave/prettyco
-00001270: 7079 2f6d 6169 6e2f 646f 6373 2f69 6d61  py/main/docs/ima
-00001280: 6765 732f 6275 6c6c 6574 746f 7061 725f  ges/bullettopar_
-00001290: 7063 2e67 6966 0a20 2020 203a 7769 6474  pc.gif.    :widt
-000012a0: 683a 2037 3030 0a20 2020 203a 616c 6967  h: 700.    :alig
-000012b0: 6e3a 2063 656e 7465 720a 6060 600a 0a60  n: center.```..`
-000012c0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-000012d0: 7072 6574 7479 636f 7079 0a23 2049 6620  prettycopy.# If 
-000012e0: 796f 7520 6861 7665 2063 6f70 6965 6420  you have copied 
-000012f0: 7468 6520 7465 7874 3a0a 2020 2020 2320  the text:.    # 
-00001300: e280 a220 4578 616d 706c 650a 2020 2020  ... Example.    
-00001310: 2320 e280 a220 7465 7874 0a20 2020 2023  # ... text.    #
-00001320: 20e2 80a2 2068 6572 650a 7072 6574 7479   ... here.pretty
-00001330: 636f 7079 2e62 756c 6c65 7474 6f70 6172  copy.bullettopar
-00001340: 2829 0a23 2079 6f75 7220 636c 6970 626f  ().# your clipbo
-00001350: 6172 6420 636f 6e74 656e 7420 6265 636f  ard content beco
-00001360: 6d65 733a 200a 2020 2020 2320 4578 616d  mes: .    # Exam
-00001370: 706c 6520 7465 7874 2068 6572 650a 6060  ple text here.``
-00001380: 600a 0a0a 2323 2320 4c69 6e65 2042 7265  `...### Line Bre
-00001390: 616b 2043 6c65 616e 696e 670a 0a4c 696e  ak Cleaning..Lin
-000013a0: 6520 6272 6561 6b73 2061 6c73 6f20 646f  e breaks also do
-000013b0: 6e27 7420 616c 7761 7973 2063 6f70 7920  n't always copy 
-000013c0: 6f76 6572 2072 6967 6874 2e0a 0a60 6060  over right...```
-000013d0: 7b65 7661 6c2d 7273 747d 0a2e 2e20 696d  {eval-rst}... im
-000013e0: 6167 653a 3a20 6874 7470 733a 2f2f 7261  age:: https://ra
-000013f0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00001400: 656e 742e 636f 6d2f 6869 7070 6f74 6865  ent.com/hippothe
-00001410: 6272 6176 652f 7072 6574 7479 636f 7079  brave/prettycopy
-00001420: 2f6d 6169 6e2f 646f 6373 2f69 6d61 6765  /main/docs/image
-00001430: 732f 7472 696d 7370 6163 655f 6e6f 7063  s/trimspace_nopc
-00001440: 2e67 6966 0a20 2020 203a 7769 6474 683a  .gif.    :width:
-00001450: 2037 3030 0a20 2020 203a 616c 6967 6e3a   700.    :align:
-00001460: 2063 656e 7465 720a 6060 600a 0a50 7265   center.```..Pre
-00001470: 7474 7943 6f70 7920 6861 7320 6675 6e63  ttyCopy has func
-00001480: 7469 6f6e 7320 746f 2066 6978 2074 6861  tions to fix tha
-00001490: 7421 0a0a 0a60 6060 7b65 7661 6c2d 7273  t!...```{eval-rs
-000014a0: 747d 0a2e 2e20 6175 746f 6675 6e63 7469  t}... autofuncti
-000014b0: 6f6e 3a3a 2070 7265 7474 7963 6f70 792e  on:: prettycopy.
-000014c0: 7072 6574 7479 636f 7079 2e6e 6f6e 6577  prettycopy.nonew
-000014d0: 6c69 6e65 730a 6060 600a 0a45 5841 4d50  lines.```..EXAMP
-000014e0: 4c45 533a 0a0a 6060 607b 6576 616c 2d72  LES:..```{eval-r
-000014f0: 7374 7d0a 2e2e 2069 6d61 6765 3a3a 2068  st}... image:: h
-00001500: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00001510: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00001520: 2f68 6970 706f 7468 6562 7261 7665 2f70  /hippothebrave/p
-00001530: 7265 7474 7963 6f70 792f 6d61 696e 2f64  rettycopy/main/d
-00001540: 6f63 732f 696d 6167 6573 2f70 636e 6f6e  ocs/images/pcnon
-00001550: 6577 6c69 6e65 732e 6769 660a 2020 2020  ewlines.gif.    
-00001560: 3a77 6964 7468 3a20 3730 300a 2020 2020  :width: 700.    
-00001570: 3a61 6c69 676e 3a20 6365 6e74 6572 0a60  :align: center.`
-00001580: 6060 0a0a 6060 6070 7974 686f 6e0a 696d  ``..```python.im
-00001590: 706f 7274 2070 7265 7474 7963 6f70 792e  port prettycopy.
-000015a0: 7072 6574 7479 636f 7079 2061 7320 7063  prettycopy as pc
-000015b0: 0a23 2049 6620 796f 7520 6861 7665 2063  .# If you have c
-000015c0: 6f70 6965 6420 7468 6520 7465 7874 3a0a  opied the text:.
-000015d0: 2020 2020 2320 4578 616d 706c 650a 2020      # Example.  
-000015e0: 2020 2320 7465 7874 0a20 2020 2023 2068    # text.    # h
-000015f0: 6572 650a 7063 2e6e 6f6e 6577 6c69 6e65  ere.pc.nonewline
-00001600: 7328 290a 2320 796f 7572 2063 6c69 7062  s().# your clipb
-00001610: 6f61 7264 2063 6f6e 7465 6e74 2062 6563  oard content bec
-00001620: 6f6d 6573 3a20 0a20 2020 2023 2045 7861  omes: .    # Exa
-00001630: 6d70 6c65 2074 6578 7420 6865 7265 0a60  mple text here.`
-00001640: 6060 0a0a 0a60 6060 7b65 7661 6c2d 7273  ``...```{eval-rs
-00001650: 747d 0a2e 2e20 6175 746f 6675 6e63 7469  t}... autofuncti
-00001660: 6f6e 3a3a 2070 7265 7474 7963 6f70 792e  on:: prettycopy.
-00001670: 7072 6574 7479 636f 7079 2e74 7269 6d73  prettycopy.trims
-00001680: 7061 6369 6e67 0a60 6060 0a0a 4558 414d  pacing.```..EXAM
-00001690: 504c 4553 3a0a 0a60 6060 7b65 7661 6c2d  PLES:..```{eval-
-000016a0: 7273 747d 0a2e 2e20 696d 6167 653a 3a20  rst}... image:: 
-000016b0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-000016c0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000016d0: 6d2f 6869 7070 6f74 6865 6272 6176 652f  m/hippothebrave/
-000016e0: 7072 6574 7479 636f 7079 2f6d 6169 6e2f  prettycopy/main/
-000016f0: 646f 6373 2f69 6d61 6765 732f 7472 696d  docs/images/trim
-00001700: 7370 6163 696e 675f 7063 2e67 6966 0a20  spacing_pc.gif. 
-00001710: 2020 203a 7769 6474 683a 2037 3030 0a20     :width: 700. 
-00001720: 2020 203a 616c 6967 6e3a 2063 656e 7465     :align: cente
-00001730: 720a 6060 600a 0a60 6060 7079 7468 6f6e  r.```..```python
-00001740: 0a69 6d70 6f72 7420 7072 6574 7479 636f  .import prettyco
-00001750: 7079 2e70 7265 7474 7963 6f70 7920 6173  py.prettycopy as
-00001760: 2070 630a 2320 4966 2079 6f75 2068 6176   pc.# If you hav
-00001770: 6520 636f 7069 6564 2074 6865 2074 6578  e copied the tex
-00001780: 743a 0a20 2020 2023 2045 7861 6d70 6c65  t:.    # Example
-00001790: 200a 2020 2020 2320 0a20 2020 2023 2074   .    # .    # t
-000017a0: 6578 7420 0a20 2020 2023 200a 2020 2020  ext .    # .    
-000017b0: 2320 6865 7265 0a70 632e 7472 696d 7370  # here.pc.trimsp
-000017c0: 6163 696e 6728 290a 2320 796f 7572 2063  acing().# your c
-000017d0: 6c69 7062 6f61 7264 2063 6f6e 7465 6e74  lipboard content
-000017e0: 2062 6563 6f6d 6573 3a20 0a20 2020 2023   becomes: .    #
-000017f0: 2045 7861 6d70 6c65 0a20 2020 2023 2074   Example.    # t
-00001800: 6578 7420 0a20 2020 2023 2068 6572 650a  ext .    # here.
-00001810: 6060 600a 0a0a 2323 2320 436f 7079 696e  ```...### Copyin
-00001820: 6720 5175 6f74 6573 0a0a 4576 6572 2077  g Quotes..Ever w
-00001830: 616e 7465 6420 746f 2063 6f70 7920 6120  anted to copy a 
-00001840: 7175 6f74 6520 6672 6f6d 2061 2064 6f63  quote from a doc
-00001850: 756d 656e 743f 0a0a 6060 607b 6576 616c  ument?..```{eval
-00001860: 2d72 7374 7d0a 2e2e 2069 6d61 6765 3a3a  -rst}... image::
-00001870: 2068 7474 7073 3a2f 2f72 6177 2e67 6974   https://raw.git
-00001880: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001890: 6f6d 2f68 6970 706f 7468 6562 7261 7665  om/hippothebrave
-000018a0: 2f70 7265 7474 7963 6f70 792f 6d61 696e  /prettycopy/main
-000018b0: 2f64 6f63 732f 696d 6167 6573 2f71 756f  /docs/images/quo
-000018c0: 7465 735f 6e6f 7063 2e67 6966 0a20 2020  tes_nopc.gif.   
-000018d0: 203a 7769 6474 683a 2037 3030 0a20 2020   :width: 700.   
-000018e0: 203a 616c 6967 6e3a 2063 656e 7465 720a   :align: center.
-000018f0: 6060 600a 0a50 7265 7474 7943 6f70 7920  ```..PrettyCopy 
-00001900: 6361 6e20 6865 6c70 210a 0a0a 6060 607b  can help!...```{
-00001910: 6576 616c 2d72 7374 7d0a 2e2e 2061 7574  eval-rst}... aut
-00001920: 6f66 756e 6374 696f 6e3a 3a20 7072 6574  ofunction:: pret
-00001930: 7479 636f 7079 2e70 7265 7474 7963 6f70  tycopy.prettycop
-00001940: 792e 7369 6d70 6c65 7175 6f74 650a 6060  y.simplequote.``
-00001950: 600a 0a45 5841 4d50 4c45 533a 0a0a 6060  `..EXAMPLES:..``
-00001960: 607b 6576 616c 2d72 7374 7d0a 2e2e 2069  `{eval-rst}... i
-00001970: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f72  mage:: https://r
-00001980: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00001990: 7465 6e74 2e63 6f6d 2f68 6970 706f 7468  tent.com/hippoth
-000019a0: 6562 7261 7665 2f70 7265 7474 7963 6f70  ebrave/prettycop
-000019b0: 792f 6d61 696e 2f64 6f63 732f 696d 6167  y/main/docs/imag
-000019c0: 6573 2f73 696d 706c 6571 756f 7465 5f70  es/simplequote_p
-000019d0: 632e 6769 660a 2020 2020 3a77 6964 7468  c.gif.    :width
-000019e0: 3a20 3730 300a 2020 2020 3a61 6c69 676e  : 700.    :align
-000019f0: 3a20 6365 6e74 6572 0a60 6060 0a0a 6060  : center.```..``
-00001a00: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
-00001a10: 7265 7474 7963 6f70 792e 7072 6574 7479  rettycopy.pretty
-00001a20: 636f 7079 2061 7320 7063 0a23 2049 6620  copy as pc.# If 
-00001a30: 796f 7520 6861 7665 2063 6f70 6965 6420  you have copied 
-00001a40: 7468 6520 7465 7874 3a0a 2020 2020 2320  the text:.    # 
-00001a50: 4578 616d 706c 6520 7465 7874 2068 6572  Example text her
-00001a60: 650a 7063 2e73 696d 706c 6571 756f 7465  e.pc.simplequote
-00001a70: 2829 0a23 2079 6f75 7220 636c 6970 626f  ().# your clipbo
-00001a80: 6172 6420 636f 6e74 656e 7420 6265 636f  ard content beco
-00001a90: 6d65 733a 200a 2020 2020 2320 2245 7861  mes: .    # "Exa
-00001aa0: 6d70 6c65 2074 6578 7420 6865 7265 220a  mple text here".
-00001ab0: 6060 600a 0a0a 0a60 6060 7b65 7661 6c2d  ```....```{eval-
-00001ac0: 7273 747d 0a2e 2e20 6175 746f 6675 6e63  rst}... autofunc
-00001ad0: 7469 6f6e 3a3a 2070 7265 7474 7963 6f70  tion:: prettycop
-00001ae0: 792e 7072 6574 7479 636f 7079 2e71 756f  y.prettycopy.quo
-00001af0: 7465 0a60 6060 0a0a 4558 414d 504c 4553  te.```..EXAMPLES
-00001b00: 3a0a 0a60 6060 7b65 7661 6c2d 7273 747d  :..```{eval-rst}
-00001b10: 0a2e 2e20 696d 6167 653a 3a20 6874 7470  ... image:: http
-00001b20: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00001b30: 6572 636f 6e74 656e 742e 636f 6d2f 6869  ercontent.com/hi
-00001b40: 7070 6f74 6865 6272 6176 652f 7072 6574  ppothebrave/pret
-00001b50: 7479 636f 7079 2f6d 6169 6e2f 646f 6373  tycopy/main/docs
-00001b60: 2f69 6d61 6765 732f 7175 6f74 655f 7063  /images/quote_pc
-00001b70: 2e67 6966 0a20 2020 203a 7769 6474 683a  .gif.    :width:
-00001b80: 2037 3030 0a20 2020 203a 616c 6967 6e3a   700.    :align:
-00001b90: 2063 656e 7465 720a 6060 600a 0a60 6060   center.```..```
-00001ba0: 7079 7468 6f6e 0a69 6d70 6f72 7420 7072  python.import pr
-00001bb0: 6574 7479 636f 7079 2e70 7265 7474 7963  ettycopy.prettyc
-00001bc0: 6f70 7920 6173 2070 630a 2320 4966 2079  opy as pc.# If y
-00001bd0: 6f75 2068 6176 6520 636f 7069 6564 2074  ou have copied t
-00001be0: 6865 2074 6578 743a 0a20 2020 2023 2045  he text:.    # E
-00001bf0: 7861 6d70 6c65 2074 6578 7420 6865 7265  xample text here
-00001c00: 0a70 632e 7175 6f74 6528 290a 2320 796f  .pc.quote().# yo
-00001c10: 7572 2063 6c69 7062 6f61 7264 2063 6f6e  ur clipboard con
-00001c20: 7465 6e74 2062 6563 6f6d 6573 3a20 0a20  tent becomes: . 
-00001c30: 2020 2023 2022 4578 616d 706c 6520 7465     # "Example te
-00001c40: 7874 2068 6572 652c 220a 0a23 2049 6620  xt here,"..# If 
-00001c50: 796f 7520 636f 7079 2074 6865 2073 616d  you copy the sam
-00001c60: 6520 7465 7874 3a0a 2020 2020 2320 4578  e text:.    # Ex
-00001c70: 616d 706c 6520 7465 7874 2068 6572 650a  ample text here.
-00001c80: 7063 2e71 756f 7465 2827 2127 290a 2320  pc.quote('!').# 
-00001c90: 796f 7572 2063 6c69 7062 6f61 7264 2063  your clipboard c
-00001ca0: 6f6e 7465 6e74 2062 6563 6f6d 6573 3a20  ontent becomes: 
-00001cb0: 0a20 2020 2023 2022 4578 616d 706c 6520  .    # "Example 
-00001cc0: 7465 7874 2068 6572 6521 220a 6060 600a  text here!".```.
-00001cd0: 0a23 2323 2049 6e74 6567 7261 7469 6f6e  .### Integration
-00001ce0: 730a 0a0a 6060 607b 6576 616c 2d72 7374  s...```{eval-rst
-00001cf0: 7d0a 2e2e 2061 7574 6f66 756e 6374 696f  }... autofunctio
-00001d00: 6e3a 3a20 7072 6574 7479 636f 7079 2e70  n:: prettycopy.p
-00001d10: 7265 7474 7963 6f70 792e 6265 7474 6572  rettycopy.better
-00001d20: 6275 6c6c 6574 730a 6060 600a 0a28 4e6f  bullets.```..(No
-00001d30: 7465 3a20 7468 6973 2066 756e 6374 696f  te: this functio
-00001d40: 6e20 6973 2073 7469 6c6c 2075 6e64 6572  n is still under
-00001d50: 2064 6576 656c 6f70 6d65 6e74 2120 2a44   development! *D
-00001d60: 6f20 6e6f 7420 7573 6520 6974 2e20 4974  o not use it. It
-00001d70: 2077 696c 6c20 6e6f 7420 776f 726b 2e2a   will not work.*
-00001d80: 290a 0a23 2320 466f 7220 6465 7665 6c6f  )..## For develo
-00001d90: 7065 7273 0a0a 416e 7920 696e 7465 7265  pers..Any intere
-00001da0: 7374 6564 2064 6576 656c 6f70 6572 732c  sted developers,
-00001db0: 2070 6c65 6173 6520 6865 6164 2074 6f20   please head to 
-00001dc0: 5b49 6e74 726f 2066 6f72 2044 6576 656c  [Intro for Devel
-00001dd0: 6f70 6572 735d 2864 6576 5f69 6e74 726f  opers](dev_intro
-00001de0: 2e6d 6429 2e0a                           .md)..
+00000dc0: 7474 7963 6f70 790a 2320 4966 2079 6f75  ttycopy.# If you
+00000dd0: 2068 6176 6520 636f 7069 6564 2074 6865   have copied the
+00000de0: 2074 6578 743a 0a20 2020 2023 2045 7861   text:.    # Exa
+00000df0: 6d70 6c65 2073 656e 0a20 2020 2023 2074  mple sen.    # t
+00000e00: 656e 6365 2067 6f65 730a 2020 2020 2320  ence goes.    # 
+00000e10: 6865 7265 2e0a 7072 6574 7479 636f 7079  here..prettycopy
+00000e20: 2e73 6d61 7274 636f 7079 2829 0a23 2079  .smartcopy().# y
+00000e30: 6f75 7220 636c 6970 626f 6172 6420 636f  our clipboard co
+00000e40: 6e74 656e 7420 6265 636f 6d65 733a 200a  ntent becomes: .
+00000e50: 2020 2020 2320 4578 616d 706c 6520 7365      # Example se
+00000e60: 6e74 656e 6365 2067 6f65 7320 6865 7265  ntence goes here
+00000e70: 2e0a 6060 600a 0a23 2323 2042 756c 6c65  ..```..### Bulle
+00000e80: 742d 506f 696e 7420 436c 6561 6e69 6e67  t-Point Cleaning
+00000e90: 0a0a 536f 6d65 7469 6d65 7320 796f 7520  ..Sometimes you 
+00000ea0: 7761 6e74 2074 6f20 636f 7079 2061 2070  want to copy a p
+00000eb0: 6965 6365 206f 6620 7465 7874 2077 6974  iece of text wit
+00000ec0: 6820 6275 6c6c 6574 2070 6f69 6e74 732e  h bullet points.
+00000ed0: 2054 6869 7320 646f 6573 6e27 7420 616c   This doesn't al
+00000ee0: 7761 7973 2077 6f72 6b20 7468 6520 7761  ways work the wa
+00000ef0: 7920 796f 7527 6420 6c69 6b65 2069 7420  y you'd like it 
+00000f00: 746f 2e0a 0a60 6060 7b65 7661 6c2d 7273  to...```{eval-rs
+00000f10: 747d 0a2e 2e20 696d 6167 653a 3a20 6874  t}... image:: ht
+00000f20: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000f30: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000f40: 6869 7070 6f74 6865 6272 6176 652f 7072  hippothebrave/pr
+00000f50: 6574 7479 636f 7079 2f6d 6169 6e2f 646f  ettycopy/main/do
+00000f60: 6373 2f69 6d61 6765 732f 6275 6c6c 6574  cs/images/bullet
+00000f70: 735f 6e6f 7063 2e67 6966 0a20 2020 203a  s_nopc.gif.    :
+00000f80: 7769 6474 683a 2037 3030 0a20 2020 203a  width: 700.    :
+00000f90: 616c 6967 6e3a 2063 656e 7465 720a 6060  align: center.``
+00000fa0: 600a 0a55 7369 6e67 2050 7265 7474 7943  `..Using PrettyC
+00000fb0: 6f70 792c 2079 6f75 2063 616e 2074 7572  opy, you can tur
+00000fc0: 6e20 7468 6520 7465 7874 2069 6e74 6f20  n the text into 
+00000fd0: 6120 636c 6561 6e20 6c69 7374 2c20 6f72  a clean list, or
+00000fe0: 2069 6e74 6f20 6120 7369 6e67 6c65 2070   into a single p
+00000ff0: 6172 6167 7261 7068 2e0a 0a60 6060 7b65  aragraph...```{e
+00001000: 7661 6c2d 7273 747d 0a2e 2e20 6175 746f  val-rst}... auto
+00001010: 6675 6e63 7469 6f6e 3a3a 2070 7265 7474  function:: prett
+00001020: 7963 6f70 792e 6275 6c6c 6574 746f 6c69  ycopy.bullettoli
+00001030: 7374 0a60 6060 0a0a 4558 414d 504c 4553  st.```..EXAMPLES
+00001040: 3a0a 0a60 6060 7b65 7661 6c2d 7273 747d  :..```{eval-rst}
+00001050: 0a2e 2e20 696d 6167 653a 3a20 6874 7470  ... image:: http
+00001060: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001070: 6572 636f 6e74 656e 742e 636f 6d2f 6869  ercontent.com/hi
+00001080: 7070 6f74 6865 6272 6176 652f 7072 6574  ppothebrave/pret
+00001090: 7479 636f 7079 2f6d 6169 6e2f 646f 6373  tycopy/main/docs
+000010a0: 2f69 6d61 6765 732f 6275 6c6c 6574 746f  /images/bulletto
+000010b0: 6c69 7374 5f70 632e 6769 660a 2020 2020  list_pc.gif.    
+000010c0: 3a77 6964 7468 3a20 3730 300a 2020 2020  :width: 700.    
+000010d0: 3a61 6c69 676e 3a20 6365 6e74 6572 0a60  :align: center.`
+000010e0: 6060 0a0a 6060 6070 7974 686f 6e0a 696d  ``..```python.im
+000010f0: 706f 7274 2070 7265 7474 7963 6f70 790a  port prettycopy.
+00001100: 2320 4966 2079 6f75 2068 6176 6520 636f  # If you have co
+00001110: 7069 6564 2074 6865 2074 6578 743a 0a20  pied the text:. 
+00001120: 2020 2023 20e2 80a2 2045 7861 6d70 6c65     # ... Example
+00001130: 0a20 2020 2023 20e2 80a2 2074 6578 740a  .    # ... text.
+00001140: 2020 2020 2320 e280 a220 6865 7265 0a70      # ... here.p
+00001150: 7265 7474 7963 6f70 792e 6275 6c6c 6574  rettycopy.bullet
+00001160: 746f 6c69 7374 2829 0a23 2079 6f75 7220  tolist().# your 
+00001170: 636c 6970 626f 6172 6420 636f 6e74 656e  clipboard conten
+00001180: 7420 6265 636f 6d65 733a 200a 2020 2020  t becomes: .    
+00001190: 2320 4578 616d 706c 6520 0a20 2020 2023  # Example .    #
+000011a0: 2074 6578 7420 0a20 2020 2023 2068 6572   text .    # her
+000011b0: 650a 6060 600a 0a0a 0a60 6060 7b65 7661  e.```....```{eva
+000011c0: 6c2d 7273 747d 0a2e 2e20 6175 746f 6675  l-rst}... autofu
+000011d0: 6e63 7469 6f6e 3a3a 2070 7265 7474 7963  nction:: prettyc
+000011e0: 6f70 792e 6275 6c6c 6574 746f 7061 720a  opy.bullettopar.
+000011f0: 6060 600a 0a45 5841 4d50 4c45 533a 0a0a  ```..EXAMPLES:..
+00001200: 6060 607b 6576 616c 2d72 7374 7d0a 2e2e  ```{eval-rst}...
+00001210: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
+00001220: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001230: 6f6e 7465 6e74 2e63 6f6d 2f68 6970 706f  ontent.com/hippo
+00001240: 7468 6562 7261 7665 2f70 7265 7474 7963  thebrave/prettyc
+00001250: 6f70 792f 6d61 696e 2f64 6f63 732f 696d  opy/main/docs/im
+00001260: 6167 6573 2f62 756c 6c65 7474 6f70 6172  ages/bullettopar
+00001270: 5f70 632e 6769 660a 2020 2020 3a77 6964  _pc.gif.    :wid
+00001280: 7468 3a20 3730 300a 2020 2020 3a61 6c69  th: 700.    :ali
+00001290: 676e 3a20 6365 6e74 6572 0a60 6060 0a0a  gn: center.```..
+000012a0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+000012b0: 2070 7265 7474 7963 6f70 790a 2320 4966   prettycopy.# If
+000012c0: 2079 6f75 2068 6176 6520 636f 7069 6564   you have copied
+000012d0: 2074 6865 2074 6578 743a 0a20 2020 2023   the text:.    #
+000012e0: 20e2 80a2 2045 7861 6d70 6c65 0a20 2020   ... Example.   
+000012f0: 2023 20e2 80a2 2074 6578 740a 2020 2020   # ... text.    
+00001300: 2320 e280 a220 6865 7265 0a70 7265 7474  # ... here.prett
+00001310: 7963 6f70 792e 6275 6c6c 6574 746f 7061  ycopy.bullettopa
+00001320: 7228 290a 2320 796f 7572 2063 6c69 7062  r().# your clipb
+00001330: 6f61 7264 2063 6f6e 7465 6e74 2062 6563  oard content bec
+00001340: 6f6d 6573 3a20 0a20 2020 2023 2045 7861  omes: .    # Exa
+00001350: 6d70 6c65 2074 6578 7420 6865 7265 0a60  mple text here.`
+00001360: 6060 0a0a 0a23 2323 204c 696e 6520 4272  ``...### Line Br
+00001370: 6561 6b20 436c 6561 6e69 6e67 0a0a 4c69  eak Cleaning..Li
+00001380: 6e65 2062 7265 616b 7320 616c 736f 2064  ne breaks also d
+00001390: 6f6e 2774 2061 6c77 6179 7320 636f 7079  on't always copy
+000013a0: 206f 7665 7220 7269 6768 742e 0a0a 6060   over right...``
+000013b0: 607b 6576 616c 2d72 7374 7d0a 2e2e 2069  `{eval-rst}... i
+000013c0: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f72  mage:: https://r
+000013d0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000013e0: 7465 6e74 2e63 6f6d 2f68 6970 706f 7468  tent.com/hippoth
+000013f0: 6562 7261 7665 2f70 7265 7474 7963 6f70  ebrave/prettycop
+00001400: 792f 6d61 696e 2f64 6f63 732f 696d 6167  y/main/docs/imag
+00001410: 6573 2f74 7269 6d73 7061 6365 5f6e 6f70  es/trimspace_nop
+00001420: 632e 6769 660a 2020 2020 3a77 6964 7468  c.gif.    :width
+00001430: 3a20 3730 300a 2020 2020 3a61 6c69 676e  : 700.    :align
+00001440: 3a20 6365 6e74 6572 0a60 6060 0a0a 5072  : center.```..Pr
+00001450: 6574 7479 436f 7079 2068 6173 2066 756e  ettyCopy has fun
+00001460: 6374 696f 6e73 2074 6f20 6669 7820 7468  ctions to fix th
+00001470: 6174 210a 0a0a 6060 607b 6576 616c 2d72  at!...```{eval-r
+00001480: 7374 7d0a 2e2e 2061 7574 6f66 756e 6374  st}... autofunct
+00001490: 696f 6e3a 3a20 7072 6574 7479 636f 7079  ion:: prettycopy
+000014a0: 2e6e 6f6e 6577 6c69 6e65 730a 6060 600a  .nonewlines.```.
+000014b0: 0a45 5841 4d50 4c45 533a 0a0a 6060 607b  .EXAMPLES:..```{
+000014c0: 6576 616c 2d72 7374 7d0a 2e2e 2069 6d61  eval-rst}... ima
+000014d0: 6765 3a3a 2068 7474 7073 3a2f 2f72 6177  ge:: https://raw
+000014e0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000014f0: 6e74 2e63 6f6d 2f68 6970 706f 7468 6562  nt.com/hippotheb
+00001500: 7261 7665 2f70 7265 7474 7963 6f70 792f  rave/prettycopy/
+00001510: 6d61 696e 2f64 6f63 732f 696d 6167 6573  main/docs/images
+00001520: 2f70 636e 6f6e 6577 6c69 6e65 732e 6769  /pcnonewlines.gi
+00001530: 660a 2020 2020 3a77 6964 7468 3a20 3730  f.    :width: 70
+00001540: 300a 2020 2020 3a61 6c69 676e 3a20 6365  0.    :align: ce
+00001550: 6e74 6572 0a60 6060 0a0a 6060 6070 7974  nter.```..```pyt
+00001560: 686f 6e0a 696d 706f 7274 2070 7265 7474  hon.import prett
+00001570: 7963 6f70 790a 2320 4966 2079 6f75 2068  ycopy.# If you h
+00001580: 6176 6520 636f 7069 6564 2074 6865 2074  ave copied the t
+00001590: 6578 743a 0a20 2020 2023 2045 7861 6d70  ext:.    # Examp
+000015a0: 6c65 0a20 2020 2023 2074 6578 740a 2020  le.    # text.  
+000015b0: 2020 2320 6865 7265 0a70 7265 7474 7963    # here.prettyc
+000015c0: 6f70 792e 6e6f 6e65 776c 696e 6573 2829  opy.nonewlines()
+000015d0: 0a23 2079 6f75 7220 636c 6970 626f 6172  .# your clipboar
+000015e0: 6420 636f 6e74 656e 7420 6265 636f 6d65  d content become
+000015f0: 733a 200a 2020 2020 2320 4578 616d 706c  s: .    # Exampl
+00001600: 6520 7465 7874 2068 6572 650a 6060 600a  e text here.```.
+00001610: 0a0a 6060 607b 6576 616c 2d72 7374 7d0a  ..```{eval-rst}.
+00001620: 2e2e 2061 7574 6f66 756e 6374 696f 6e3a  .. autofunction:
+00001630: 3a20 7072 6574 7479 636f 7079 2e74 7269  : prettycopy.tri
+00001640: 6d73 7061 6369 6e67 0a60 6060 0a0a 4558  mspacing.```..EX
+00001650: 414d 504c 4553 3a0a 0a60 6060 7b65 7661  AMPLES:..```{eva
+00001660: 6c2d 7273 747d 0a2e 2e20 696d 6167 653a  l-rst}... image:
+00001670: 3a20 6874 7470 733a 2f2f 7261 772e 6769  : https://raw.gi
+00001680: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00001690: 636f 6d2f 6869 7070 6f74 6865 6272 6176  com/hippothebrav
+000016a0: 652f 7072 6574 7479 636f 7079 2f6d 6169  e/prettycopy/mai
+000016b0: 6e2f 646f 6373 2f69 6d61 6765 732f 7472  n/docs/images/tr
+000016c0: 696d 7370 6163 696e 675f 7063 2e67 6966  imspacing_pc.gif
+000016d0: 0a20 2020 203a 7769 6474 683a 2037 3030  .    :width: 700
+000016e0: 0a20 2020 203a 616c 6967 6e3a 2063 656e  .    :align: cen
+000016f0: 7465 720a 6060 600a 0a60 6060 7079 7468  ter.```..```pyth
+00001700: 6f6e 0a69 6d70 6f72 7420 7072 6574 7479  on.import pretty
+00001710: 636f 7079 0a23 2049 6620 796f 7520 6861  copy.# If you ha
+00001720: 7665 2063 6f70 6965 6420 7468 6520 7465  ve copied the te
+00001730: 7874 3a0a 2020 2020 2320 4578 616d 706c  xt:.    # Exampl
+00001740: 6520 0a20 2020 2023 200a 2020 2020 2320  e .    # .    # 
+00001750: 7465 7874 200a 2020 2020 2320 0a20 2020  text .    # .   
+00001760: 2023 2068 6572 650a 7072 6574 7479 636f   # here.prettyco
+00001770: 7079 2e74 7269 6d73 7061 6369 6e67 2829  py.trimspacing()
+00001780: 0a23 2079 6f75 7220 636c 6970 626f 6172  .# your clipboar
+00001790: 6420 636f 6e74 656e 7420 6265 636f 6d65  d content become
+000017a0: 733a 200a 2020 2020 2320 4578 616d 706c  s: .    # Exampl
+000017b0: 650a 2020 2020 2320 7465 7874 200a 2020  e.    # text .  
+000017c0: 2020 2320 6865 7265 0a60 6060 0a0a 0a23    # here.```...#
+000017d0: 2323 2043 6f70 7969 6e67 2051 756f 7465  ## Copying Quote
+000017e0: 730a 0a45 7665 7220 7761 6e74 6564 2074  s..Ever wanted t
+000017f0: 6f20 636f 7079 2061 2071 756f 7465 2066  o copy a quote f
+00001800: 726f 6d20 6120 646f 6375 6d65 6e74 3f0a  rom a document?.
+00001810: 0a60 6060 7b65 7661 6c2d 7273 747d 0a2e  .```{eval-rst}..
+00001820: 2e20 696d 6167 653a 3a20 6874 7470 733a  . image:: https:
+00001830: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00001840: 636f 6e74 656e 742e 636f 6d2f 6869 7070  content.com/hipp
+00001850: 6f74 6865 6272 6176 652f 7072 6574 7479  othebrave/pretty
+00001860: 636f 7079 2f6d 6169 6e2f 646f 6373 2f69  copy/main/docs/i
+00001870: 6d61 6765 732f 7175 6f74 6573 5f6e 6f70  mages/quotes_nop
+00001880: 632e 6769 660a 2020 2020 3a77 6964 7468  c.gif.    :width
+00001890: 3a20 3730 300a 2020 2020 3a61 6c69 676e  : 700.    :align
+000018a0: 3a20 6365 6e74 6572 0a60 6060 0a0a 5072  : center.```..Pr
+000018b0: 6574 7479 436f 7079 2063 616e 2068 656c  ettyCopy can hel
+000018c0: 7021 0a0a 0a60 6060 7b65 7661 6c2d 7273  p!...```{eval-rs
+000018d0: 747d 0a2e 2e20 6175 746f 6675 6e63 7469  t}... autofuncti
+000018e0: 6f6e 3a3a 2070 7265 7474 7963 6f70 792e  on:: prettycopy.
+000018f0: 7369 6d70 6c65 7175 6f74 650a 6060 600a  simplequote.```.
+00001900: 0a45 5841 4d50 4c45 533a 0a0a 6060 607b  .EXAMPLES:..```{
+00001910: 6576 616c 2d72 7374 7d0a 2e2e 2069 6d61  eval-rst}... ima
+00001920: 6765 3a3a 2068 7474 7073 3a2f 2f72 6177  ge:: https://raw
+00001930: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00001940: 6e74 2e63 6f6d 2f68 6970 706f 7468 6562  nt.com/hippotheb
+00001950: 7261 7665 2f70 7265 7474 7963 6f70 792f  rave/prettycopy/
+00001960: 6d61 696e 2f64 6f63 732f 696d 6167 6573  main/docs/images
+00001970: 2f73 696d 706c 6571 756f 7465 5f70 632e  /simplequote_pc.
+00001980: 6769 660a 2020 2020 3a77 6964 7468 3a20  gif.    :width: 
+00001990: 3730 300a 2020 2020 3a61 6c69 676e 3a20  700.    :align: 
+000019a0: 6365 6e74 6572 0a60 6060 0a0a 6060 6070  center.```..```p
+000019b0: 7974 686f 6e0a 696d 706f 7274 2070 7265  ython.import pre
+000019c0: 7474 7963 6f70 790a 2320 4966 2079 6f75  ttycopy.# If you
+000019d0: 2068 6176 6520 636f 7069 6564 2074 6865   have copied the
+000019e0: 2074 6578 743a 0a20 2020 2023 2045 7861   text:.    # Exa
+000019f0: 6d70 6c65 2074 6578 7420 6865 7265 0a70  mple text here.p
+00001a00: 7265 7474 7963 6f70 792e 7369 6d70 6c65  rettycopy.simple
+00001a10: 7175 6f74 6528 290a 2320 796f 7572 2063  quote().# your c
+00001a20: 6c69 7062 6f61 7264 2063 6f6e 7465 6e74  lipboard content
+00001a30: 2062 6563 6f6d 6573 3a20 0a20 2020 2023   becomes: .    #
+00001a40: 2022 4578 616d 706c 6520 7465 7874 2068   "Example text h
+00001a50: 6572 6522 0a60 6060 0a0a 0a0a 6060 607b  ere".```....```{
+00001a60: 6576 616c 2d72 7374 7d0a 2e2e 2061 7574  eval-rst}... aut
+00001a70: 6f66 756e 6374 696f 6e3a 3a20 7072 6574  ofunction:: pret
+00001a80: 7479 636f 7079 2e71 756f 7465 0a60 6060  tycopy.quote.```
+00001a90: 0a0a 4558 414d 504c 4553 3a0a 0a60 6060  ..EXAMPLES:..```
+00001aa0: 7b65 7661 6c2d 7273 747d 0a2e 2e20 696d  {eval-rst}... im
+00001ab0: 6167 653a 3a20 6874 7470 733a 2f2f 7261  age:: https://ra
+00001ac0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00001ad0: 656e 742e 636f 6d2f 6869 7070 6f74 6865  ent.com/hippothe
+00001ae0: 6272 6176 652f 7072 6574 7479 636f 7079  brave/prettycopy
+00001af0: 2f6d 6169 6e2f 646f 6373 2f69 6d61 6765  /main/docs/image
+00001b00: 732f 7175 6f74 655f 7063 2e67 6966 0a20  s/quote_pc.gif. 
+00001b10: 2020 203a 7769 6474 683a 2037 3030 0a20     :width: 700. 
+00001b20: 2020 203a 616c 6967 6e3a 2063 656e 7465     :align: cente
+00001b30: 720a 6060 600a 0a60 6060 7079 7468 6f6e  r.```..```python
+00001b40: 0a69 6d70 6f72 7420 7072 6574 7479 636f  .import prettyco
+00001b50: 7079 0a23 2049 6620 796f 7520 6861 7665  py.# If you have
+00001b60: 2063 6f70 6965 6420 7468 6520 7465 7874   copied the text
+00001b70: 3a0a 2020 2020 2320 4578 616d 706c 6520  :.    # Example 
+00001b80: 7465 7874 2068 6572 650a 7072 6574 7479  text here.pretty
+00001b90: 636f 7079 2e71 756f 7465 2829 0a23 2079  copy.quote().# y
+00001ba0: 6f75 7220 636c 6970 626f 6172 6420 636f  our clipboard co
+00001bb0: 6e74 656e 7420 6265 636f 6d65 733a 200a  ntent becomes: .
+00001bc0: 2020 2020 2320 2245 7861 6d70 6c65 2074      # "Example t
+00001bd0: 6578 7420 6865 7265 2c22 0a0a 2320 4966  ext here,"..# If
+00001be0: 2079 6f75 2063 6f70 7920 7468 6520 7361   you copy the sa
+00001bf0: 6d65 2074 6578 743a 0a20 2020 2023 2045  me text:.    # E
+00001c00: 7861 6d70 6c65 2074 6578 7420 6865 7265  xample text here
+00001c10: 0a70 7265 7474 7963 6f70 792e 7175 6f74  .prettycopy.quot
+00001c20: 6528 2721 2729 0a23 2079 6f75 7220 636c  e('!').# your cl
+00001c30: 6970 626f 6172 6420 636f 6e74 656e 7420  ipboard content 
+00001c40: 6265 636f 6d65 733a 200a 2020 2020 2320  becomes: .    # 
+00001c50: 2245 7861 6d70 6c65 2074 6578 7420 6865  "Example text he
+00001c60: 7265 2122 0a60 6060 0a23 2323 204d 6973  re!".```.### Mis
+00001c70: 6365 6c6c 616e 656f 7573 200a 0a54 6865  cellaneous ..The
+00001c80: 7265 2061 7265 206f 7468 6572 2077 6179  re are other way
+00001c90: 7320 7468 6174 2079 6f75 206d 6967 6874  s that you might
+00001ca0: 2077 616e 7420 746f 2065 6469 7420 7468   want to edit th
+00001cb0: 6520 7465 7874 2074 6861 7420 796f 7520  e text that you 
+00001cc0: 636f 7069 6564 2062 6566 6f72 6520 7061  copied before pa
+00001cd0: 7374 696e 6720 6974 2e20 5072 6574 7479  sting it. Pretty
+00001ce0: 436f 7079 2063 616e 2068 656c 7020 796f  Copy can help yo
+00001cf0: 7520 6865 7265 2c20 746f 6f21 0a0a 6060  u here, too!..``
+00001d00: 607b 6576 616c 2d72 7374 7d0a 2e2e 2061  `{eval-rst}... a
+00001d10: 7574 6f66 756e 6374 696f 6e3a 3a20 7072  utofunction:: pr
+00001d20: 6574 7479 636f 7079 2e72 656d 6f76 650a  ettycopy.remove.
+00001d30: 6060 600a 0a45 5841 4d50 4c45 533a 0a0a  ```..EXAMPLES:..
+00001d40: 6060 607b 6576 616c 2d72 7374 7d0a 2e2e  ```{eval-rst}...
+00001d50: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
+00001d60: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001d70: 6f6e 7465 6e74 2e63 6f6d 2f68 6970 706f  ontent.com/hippo
+00001d80: 7468 6562 7261 7665 2f70 7265 7474 7963  thebrave/prettyc
+00001d90: 6f70 792f 6d61 696e 2f64 6f63 732f 696d  opy/main/docs/im
+00001da0: 6167 6573 2f72 656d 6f76 655f 7063 2e67  ages/remove_pc.g
+00001db0: 6966 0a20 2020 203a 7769 6474 683a 2037  if.    :width: 7
+00001dc0: 3030 0a20 2020 203a 616c 6967 6e3a 2063  00.    :align: c
+00001dd0: 656e 7465 720a 6060 600a 0a60 6060 7079  enter.```..```py
+00001de0: 7468 6f6e 0a69 6d70 6f72 7420 7072 6574  thon.import pret
+00001df0: 7479 636f 7079 0a23 2049 6620 796f 7520  tycopy.# If you 
+00001e00: 6861 7665 2063 6f70 6965 6420 7468 6520  have copied the 
+00001e10: 7465 7874 3a0a 2020 2020 2320 4578 616d  text:.    # Exam
+00001e20: 706c 6520 7465 7874 2068 6572 650a 7072  ple text here.pr
+00001e30: 6574 7479 636f 7079 2e72 656d 6f76 6528  ettycopy.remove(
+00001e40: 2765 7827 290a 2320 796f 7572 2063 6c69  'ex').# your cli
+00001e50: 7062 6f61 7264 2063 6f6e 7465 6e74 2062  pboard content b
+00001e60: 6563 6f6d 6573 3a20 0a20 2020 2023 2045  ecomes: .    # E
+00001e70: 7861 6d70 6c65 2074 7420 6865 7265 0a60  xample tt here.`
+00001e80: 6060 0a0a 2323 2320 496e 7465 6772 6174  ``..### Integrat
+00001e90: 696f 6e73 0a0a 284e 6f74 653a 2074 6869  ions..(Note: thi
+00001ea0: 7320 6675 6e63 7469 6f6e 2069 7320 7374  s function is st
+00001eb0: 696c 6c20 756e 6465 7220 6465 7665 6c6f  ill under develo
+00001ec0: 706d 656e 7421 202a 446f 206e 6f74 2075  pment! *Do not u
+00001ed0: 7365 2069 742e 2049 7420 7769 6c6c 206e  se it. It will n
+00001ee0: 6f74 2077 6f72 6b2e 2a29 0a0a 6060 607b  ot work.*)..```{
+00001ef0: 6576 616c 2d72 7374 7d0a 2e2e 2061 7574  eval-rst}... aut
+00001f00: 6f66 756e 6374 696f 6e3a 3a20 7072 6574  ofunction:: pret
+00001f10: 7479 636f 7079 2e62 6574 7465 7262 756c  tycopy.betterbul
+00001f20: 6c65 7473 0a60 6060 0a0a 2323 2046 6f72  lets.```..## For
+00001f30: 2064 6576 656c 6f70 6572 730a 0a41 6e79   developers..Any
+00001f40: 2069 6e74 6572 6573 7465 6420 6465 7665   interested deve
+00001f50: 6c6f 7065 7273 2c20 706c 6561 7365 2068  lopers, please h
+00001f60: 6561 6420 746f 205b 496e 7472 6f20 666f  ead to [Intro fo
+00001f70: 7220 4465 7665 6c6f 7065 7273 5d28 6465  r Developers](de
+00001f80: 765f 696e 7472 6f2e 6d64 292e 0a         v_intro.md)..
```

### Comparing `prettycopy-0.2.0/docs/make.bat` & `prettycopy-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `prettycopy-0.2.0/prettycopy/command_line.py` & `prettycopy-0.2.1/prettycopy/command_line.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,24 +19,24 @@
         if output:
             print(ret)
     except ValueError:
         print(typer.style("Input should have been a string!", fg="white", bg="red"))
 
 
 @app.command()
-def nobullets(text: str = "", output: bool = True):
+def bullettolist(text: str = "", output: bool = True):
     """
     Remove all line breaks and bullet points.
     From clipboard, or, optionally, --text.
     """
     try:
         if text:
-            ret = pc.nobullets(text)
+            ret = pc.bullettolist(text)
         else:
-            ret = pc.nobullets()
+            ret = pc.bullettolist()
         if output:
             print(ret)
     except ValueError:
         print(typer.style("Input should have been a string!", fg="white", bg="red"))
 
 
 @app.command()
@@ -118,7 +118,28 @@
             ret = pc.smartcopy(text)
         else:
             ret = pc.smartcopy()
         if output:
             print(ret)
     except ValueError:
         print(typer.style("Input should have been a string!", fg="white", bg="red"))
+
+
+@app.command()
+def remove(substring: str, replacement: str = "", text: str = "", output: bool = True):
+    """
+    Remove all instances of a substring.
+    From the clipboard, or, optionally, --text.
+    """
+    try:
+        if text and replacement:
+            ret = pc.remove(substring, replacement, text)
+        elif text and not replacement:
+            ret = pc.remove(substring, text=text)
+        elif replacement and not text:
+            ret = pc.remove(substring, replacement=replacement)
+        else:
+            ret = pc.remove(substring)
+        if output:
+            print(ret)
+    except ValueError:
+        print(typer.style("Input should have been a string!", fg="white", bg="red"))
```

### Comparing `prettycopy-0.2.0/prettycopy/prettycopy.py` & `prettycopy-0.2.1/prettycopy/prettycopy.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 import googleapiclient.discovery
 
 import nltk
 from nltk import tokenize
 from nltk.corpus import words
 from textblob import TextBlob
-from spellchecker import SpellChecker
 
 try:
     nltk.data.find('tokenizers/words')
 except LookupError:
     nltk.download("words", quiet=True)
 
 try:
@@ -27,18 +26,18 @@
     nltk.download("punkt", quiet=True)
 
 
 # PUBLIC FUNCTIONS
 
 
 def nonewlines(text=None):
-    """Remove all newlines.
+    """Remove all line breaks.
 
-    Takes in a text input from the argument or (by default) the clipboard, removes all newlines,
-    and recopies it to the clipboard.
+    Removes line breaks from a text and recopies to the clipboard.
+    Input comes from either an argument or (by default) the clipboard.
 
     Args:
         text (str): Any text; optional, default None.
 
     Returns:
         str: Corrected text.
 
@@ -52,19 +51,20 @@
         raise ValueError("PrettyCopy can only take in strings!")
 
     text = ' '.join([line.strip() for line in text.split()])
     pyperclip.copy(text)
     return text
 
 
-def nobullets(text=None):
-    """Take out old newlines, replace bullets with newlines.
+def bullettolist(text=None):
+    """Take out old line breaks. Replace bullets with line breaks.
 
-    Takes in a text input from the argument or (by default) the clipboard. Removes all newlines,
-    and replaces any bullet symbols with newlines.
+    Removes newline symbols from a text, replacing bullet symbols with line breaks.
+    Recopies to the clipboard.
+    Input comes from either an argument or (by default) the clipboard.
 
     Args:
         text (str): Any text; optional, default None.
 
     Returns:
         str: Corrected text.
 
@@ -82,16 +82,17 @@
     pyperclip.copy(text)
     return text
 
 
 def bullettopar(text=None):
     """Remove newlines, replace bullets with spaces
 
-    Takes in a text input from the argument or (by default) the clipboard. Removes all newlines,
-    and replaces any bullet symbols with a space.
+    Removes all newlines from a text, replacing any bullet symbols with a space.
+    Recopies to the clipboard.
+    Input comes from either an argument or (by default) the clipboard.
 
     Args:
         text (str): Any text; optional, default None.
 
     Returns:
         str: Corrected text.
 
@@ -109,15 +110,17 @@
     pyperclip.copy(text)
     return text
 
 
 def simplequote(text=None):
     """Add quotes around clipboard contents.
 
-    Adds quotation marks around a text input from the argument or (by default) the clipboard.
+    Adds quotation marks around a cleaned (via smartcopy()) text input.
+    Recopies to the clipboard.
+    Input comes from either an argument or (by default) the clipboard.
 
     Args:
         text (str): Any text; optional, default None.
 
     Returns:
         str: Corrected text.
 
@@ -138,15 +141,17 @@
     pyperclip.copy(text)
     return text
 
 
 def quote(end_punctuation=None, text=None):
     """Add quotes (and optional punctuation) around clipboard contents.
 
-    Adds quotation marks and end punctuation to a text input from the argument or (by default) the clipboard.
+    Adds quotation marks and end punctuation to a cleaned (via smartcopy()) text.
+    Recopies to the clipboard.
+    Input comes from either an argument or (by default) the clipboard.
 
     Args:
         end_punctuation (str): A single-character string containing one of: [.,!?]
         text (str): Any text; optional, default None.
 
     Returns:
         str: Corrected text.
@@ -175,15 +180,16 @@
     pyperclip.copy(text)
     return text
 
 
 def trimspacing(text=None):
     """Removes empty lines clipboard contents.
 
-    Removes empty lines from a text input from the argument or (by default) the clipboard.
+    Removes empty lines from a text. Recopies to the clipboard.
+    Input comes from either an argument or (by default) the clipboard.
 
     Args:
         text (str): Any text; optional, default None.
 
     Returns:
         str: Corrected text.
 
@@ -213,15 +219,15 @@
         docID (str): The ID of a Google Doc.
 
     Returns:
         str: Corrected text.
 
     """
     # get content
-    text = nobullets()
+    text = bullettolist()
 
     # authenticate so that you can access the google doc
     service = _getservice(docID)
 
     # find end of current google doc content
     document = service.documents().get(documentId=docID).execute()
     doclines = document.get('body')['content']
@@ -272,16 +278,20 @@
     # return
     return text
 
 
 def smartcopy(text=None):
     """Removes line breaks from clipboard contents in a smart way.
 
-    Removes line breaks--adding a space if a line break splits a word in two, but not
-    if the line break is between words--from a text input from the argument or (by default) the clipboard.
+    Removes line breaks from a text.
+    Adds a space if a line break is between words or after punctuation,
+    but not if the line break splits a word in two (with or without an
+    intemediary dash.)
+    Recopies to the clipboard.
+    Input comes from either an argument or (by default) the clipboard.
 
     Args:
         text (str): Any text; optional, default None.
 
     Returns:
         str: Corrected text.
 
@@ -309,14 +319,47 @@
 
     text = ''.join(lines)
 
     pyperclip.copy(text)
     return text
 
 
+def remove(substring, replacement=None, text=None):
+    """Remove a substring (and optionally replace it) from clipboard contents.
+
+    Removes a substring from a text, optionally replacing it with another substring.
+    Recopies to the clipboard.
+    Input comes from either an argument or (by default) the clipboard.
+
+    Args:
+        substring (str): A string to be removed or replaced.
+        text (str): Any text; optional, default None.
+
+    Returns:
+        str: Corrected text.
+
+    Warning:
+        Changes contents of the clipboard.
+
+    """
+
+    if text is None:
+        text = pyperclip.paste()
+    if not isinstance(text, str):
+        raise ValueError("PrettyCopy can only take in strings!")
+
+    if replacement:
+        text = text.replace(substring, replacement)
+    else:
+        text = text.replace(substring, '')
+
+    pyperclip.copy(text)
+    return text
+
+
 # HIDDEN FUNCTIONS
 
 
 # Authorizes the user to access Google Docs
 # CITATION: Google Docs API quickstart
 def _getservice(DOCUMENT_ID, SCOPES=None):
     """Credentials testing
@@ -364,38 +407,49 @@
         return
 
     return service
 
 
 def _cleanlines(line):
     """
-    Removes newlines from a given line, adding a space if it's surrounded by
+    Removes newline symbols from a given line, adding a space if it's surrounded by
     recognizable English words, and no space if it isn't.
     """
-    spell = SpellChecker()
     # remove newlines "within words"
     for match in re.finditer(r"([A-Za-z0-9]+)(\r?\n)+([A-Za-z0-9]+)", line):
         b1 = TextBlob(match.group(1))
         b2 = TextBlob(match.group(3))
 
         loc = line.find(str(match.group(1) + match.group(2) + match.group(3))) + len(match.group(1))
 
-        if (
-            match.group(1) == spell.correction(match.group(1))
-            or match.group(1) == b1.correct()
-            or match.group(1) in words.words()
-        ) and (
-            match.group(3) == spell.correction(match.group(3))
-            or match.group(3) == b2.correct()
-            or match.group(3) in words.words()
+        if (match.group(1) == b1.correct() or match.group(1) in words.words()) and (
+            match.group(3) == b2.correct() or match.group(3) in words.words()
         ):
             line = list(line)
             line[loc] = " "
             line = ''.join(line)
         else:
             line = list(line)
             line[loc] = ""
             line = ''.join(line)
 
+    # remove dashes "within words"
+    for match in re.finditer(r"([A-Za-z0-9]+)-(\r?\n)+([A-Za-z0-9]+)", line):
+        b1 = TextBlob(match.group(1))
+        b2 = TextBlob(match.group(3))
+
+        loc = match.start() + len(match.group(1))
+
+        if (match.group(1) == b1.correct() or match.group(1) in words.words()) and (
+            match.group(3) == b2.correct() or match.group(3) in words.words()
+        ):
+            continue
+        else:
+            line = list(line)
+            print(line[loc])
+            line[loc] = ""
+            line = ''.join(line)
+
     # remove any remaining newlines
+    line = re.sub(r"([.,;!?%\"])+(\r?\n)+", r"\1 ", line)
     line = re.sub(r"(\r?\n)+", "", line)
     return line
```

### Comparing `prettycopy-0.2.0/prettycopy/tests/test_all.py` & `prettycopy-0.2.1/prettycopy/tests/test_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,58 +42,58 @@
 
         # Text from argument
         ret = pc.nonewlines("Another\n line \nof text\n here.")
         assert ret == "Another line of text here."
         assert copy_mock.call_args.args == (ret,)
 
 
-def test_nobullets():
+def test_bullettolist():
     with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock, patch(
         "prettycopy.prettycopy.nonewlines"
     ) as newline_mock:
         # Bad type
         paste_mock.return_value = 42
         with pytest.raises(ValueError):
-            ret = pc.nobullets()
+            ret = pc.bullettolist()
 
         # No spaces
         paste_mock.return_value = "•Test\n•Test"
         newline_mock.return_value = '•Test •Test'
-        ret = pc.nobullets()
+        ret = pc.bullettolist()
         assert newline_mock.call_args.args == ("•Test\n•Test",)
         assert ret == "Test\nTest"
         assert copy_mock.call_args.args == (ret,)
 
         # Spaces between bullet and text
         paste_mock.return_value = "• Test\n• Test"
         newline_mock.return_value = '• Test • Test'
-        ret = pc.nobullets()
+        ret = pc.bullettolist()
         assert newline_mock.call_args.args == ("• Test\n• Test",)
         assert ret == "Test\nTest"
         assert copy_mock.call_args.args == (ret,)
 
         # Spaces around bullet and text
         paste_mock.return_value = "   • Test\n  •\tTest   •"
         newline_mock.return_value = '• Test • Test •'
-        ret = pc.nobullets()
+        ret = pc.bullettolist()
         assert newline_mock.call_args.args == ("   • Test\n  •\tTest   •",)
         assert ret == "Test\nTest"
         assert copy_mock.call_args.args == (ret,)
 
         # Bullets within words
         paste_mock.return_value = "•   Te•st• Test"
         newline_mock.return_value = '• Te•st• Test'
-        ret = pc.nobullets()
+        ret = pc.bullettolist()
         assert newline_mock.call_args.args == ("•   Te•st• Test",)
         assert ret == "Te\nst\nTest"
         assert copy_mock.call_args.args == (ret,)
 
         # Text from argument
         newline_mock.return_value = '•Another •Test'
-        ret = pc.nobullets("•Another\n•Test")
+        ret = pc.bullettolist("•Another\n•Test")
         assert newline_mock.call_args.args == ("•Another\n•Test",)
         assert ret == "Another\nTest"
         assert copy_mock.call_args.args == (ret,)
 
 
 def test_bullettopar():
     with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock:
@@ -246,15 +246,14 @@
 
         # text from argument
         ret = pc.trimspacing("Another\r\n\r\n\r\ntest")
         assert ret == "Another\ntest"
         assert copy_mock.call_args.args == (ret,)
 
 
-# TODO: check that HTTPError is printed in Test 4
 def test_getservice():
     with patch("os.path.exists") as os_mock, patch(
         "google.oauth2.credentials.Credentials.from_authorized_user_file"
     ) as creds_file_mock, patch(
         "google_auth_oauthlib.flow.InstalledAppFlow.from_client_secrets_file"
     ) as get_secrets_mock, patch(
         "builtins.open"
@@ -272,15 +271,15 @@
         os_mock.return_value = True
         os_mock.call_count = 0
         fakecreds1 = MagicMock()
         fakecreds1.valid = True
         creds_file_mock.return_value = fakecreds1
         # build service
         fakeservice1 = MagicMock()
-        build_mock.return_value = fakeservice1  # FIXME there was an issue here
+        build_mock.return_value = fakeservice1
 
         ret = pc._getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0')
 
         assert os_mock.call_count == 1
         assert creds_file_mock.call_count == 1
         assert build_mock.call_args.args == (
             'docs',
@@ -432,59 +431,101 @@
         assert ret == "Sentence one.\nSentence two."
         assert copy_mock.call_args.args == (ret,)
 
         assert True
 
 
 def test_cleanlines():
-    with patch("spellchecker.SpellChecker") as spellchecker_mock, patch("textblob.TextBlob") as textblob_mock, patch(
-        "nltk.corpus.words"
-    ) as words_mock:
+    with patch("textblob.TextBlob") as textblob_mock, patch("nltk.corpus.words") as words_mock:
         # no space needed
-        spell = MagicMock()
-        spellchecker_mock.return_value = spell
-        spell.correction = MagicMock()
-        spell.correction.side_effect = ["sent", "nice", "go", "is"]
         b1 = MagicMock()
         b1.correct = MagicMock()
         b2 = MagicMock()
         b2.correct = MagicMock()
         textblob_mock.side_effect = [b1, b2]
         b1.correct.side_effect = ["sent", "go"]
         b2.correct.side_effect = ["nice", "is"]
         words_mock.return_value = False
         line = "Sente\nnce 1 goe\ns here."
         ret = pc._cleanlines(line)
         assert ret == "Sentence 1 goes here."
 
         # space needed
-        spell = MagicMock()
-        spellchecker_mock.return_value = spell
-        spell.correction = MagicMock()
-        spell.correction.side_effect = ["goes", "here"]
         b1 = MagicMock()
         b1.correct = MagicMock()
         b2 = MagicMock()
         b2.correct = MagicMock()
         textblob_mock.side_effect = [b1, b2]
         b1.correct.side_effect = ["goes"]
         b2.correct.side_effect = ["here"]
         words_mock.return_value = False
         line = "Sentence 2 goes\nhere."
         ret = pc._cleanlines(line)
         assert ret == "Sentence 2 goes here."
 
-        # newline not within a word
-        line = "Sentence 3 goes \nhere."
+        # space needed 2
+        b1 = MagicMock()
+        b1.correct = MagicMock()
+        b2 = MagicMock()
+        b2.correct = MagicMock()
+        textblob_mock.side_effect = [b1, b2]
+        b1.correct.side_effect = ["so"]
+        b2.correct.side_effect = ["tense"]
+        words_mock.return_value = False
+        line = "Se-\r\nntence 3 goes here."
         ret = pc._cleanlines(line)
         assert ret == "Sentence 3 goes here."
 
+        # space not needed 2
+        b1 = MagicMock()
+        b1.correct = MagicMock()
+        b2 = MagicMock()
+        b2.correct = MagicMock()
+        textblob_mock.side_effect = [b1, b2]
+        b1.correct.side_effect = ["Example"]
+        b2.correct.side_effect = ["sentence"]
+        words_mock.return_value = False
+        line = "Example-\r\nsentence 4 goes here."
+        ret = pc._cleanlines(line)
+        assert ret == "Example-sentence 4 goes here."
+
+        # newline not within a word
+        line = "Sentence 5 goes \nhere."
+        ret = pc._cleanlines(line)
+        assert ret == "Sentence 5 goes here."
+
         assert True
 
 
+def test_remove():
+    with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock:
+        # Bad type
+        paste_mock.return_value = 77
+        with pytest.raises(ValueError):
+            ret = pc.remove('x')
+
+        # Remove from clipboard
+        paste_mock.return_value = "Example text here."
+        ret = pc.remove('x')
+        assert ret == "Eample tet here."
+        assert copy_mock.call_args.args == (ret,)
+
+        # Remove from argument
+        paste_mock.return_value = None
+        ret = pc.remove('e', text="Example text here.")
+        assert ret == "Exampl txt hr."
+        assert copy_mock.call_args.args == (ret,)
+
+        # Replace
+        paste_mock.return_value = "Example text here."
+        ret = pc.remove('x', replacement='s')
+        assert ret == "Esample test here."
+        assert copy_mock.call_args.args == (ret,)
+
+
 # TODO: test for prettycopy.betterbullets
 
 
 # CLI testing
 def test_app():
     with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock:
         # no new lines
@@ -511,32 +552,32 @@
         assert result.exit_code == 0
         assert result.stdout == ''
         assert copy_mock.call_args.args == ("Testing sentence three here.",)
 
         # no bullets
         # clipboard input
         paste_mock.return_value = "•   Te•st• Test"
-        result = runner.invoke(app, ["nobullets"])
+        result = runner.invoke(app, ["bullettolist"])
         assert result.exit_code == 0
         assert result.stdout == "Te\nst\nTest" + '\n'
         assert copy_mock.call_args.args == ("Te\nst\nTest",)
         # text input
         paste_mock.return_value = None
-        result = runner.invoke(app, ["nobullets", "--text", "•test"])
+        result = runner.invoke(app, ["bullettolist", "--text", "•test"])
         assert result.exit_code == 0
         assert result.stdout == "test" + '\n'
         assert copy_mock.call_args.args == ("test",)
         # error
         paste_mock.return_value = 42
-        result = runner.invoke(app, ["nobullets"])
+        result = runner.invoke(app, ["bullettolist"])
         assert result.exit_code == 0
         assert result.stdout == typer.style("Input should have been a string!", fg="white", bg="red") + '\n'
         # no-output
         paste_mock.return_value = "•   Te•st• Test"
-        result = runner.invoke(app, ["nobullets", "--no-output"])
+        result = runner.invoke(app, ["bullettolist", "--no-output"])
         assert result.exit_code == 0
         assert result.stdout == ''
         assert copy_mock.call_args.args == ("Te\nst\nTest",)
 
         # bullet to par
         # clipboard input
         paste_mock.return_value = "Testing\n•sentence\n• one •here."
@@ -664,7 +705,46 @@
         assert result.stdout == typer.style("Input should have been a string!", fg="white", bg="red") + '\n'
         # no-output
         paste_mock.return_value = "Testing se\nntence three\nhere."
         result = runner.invoke(app, ["smartcopy", "--no-output"])
         assert result.exit_code == 0
         assert result.stdout == ''
         assert copy_mock.call_args.args == ("Testing sentence three here.",)
+
+        # remove
+        # clipboard input - remove
+        paste_mock.return_value = "Testing sentence one here."
+        result = runner.invoke(app, ["remove", "one"])
+        assert result.exit_code == 0
+        assert result.stdout == "Testing sentence  here." + '\n'
+        assert copy_mock.call_args.args == ("Testing sentence  here.",)
+        # text input - remove
+        paste_mock.return_value = None
+        result = runner.invoke(app, ["remove", "sen", "--text", "Testing sentence two here."])
+        assert result.exit_code == 0
+        assert result.stdout == "Testing tence two here." + '\n'
+        assert copy_mock.call_args.args == ("Testing tence two here.",)
+        # clipboard input - replace
+        paste_mock.return_value = "Testing sentence three here."
+        result = runner.invoke(app, ["remove", "en", "--replacement", "EN"])
+        assert result.exit_code == 0
+        assert result.stdout == "Testing sENtENce three here." + '\n'
+        assert copy_mock.call_args.args == ("Testing sENtENce three here.",)
+        # text input - replace
+        paste_mock.return_value = None
+        result = runner.invoke(
+            app, ["remove", "four", "--replacement", "twenty", "--text", "Testing sentence four here."]
+        )
+        assert result.exit_code == 0
+        assert result.stdout == "Testing sentence twenty here." + '\n'
+        assert copy_mock.call_args.args == ("Testing sentence twenty here.",)
+        # error
+        paste_mock.return_value = 42
+        result = runner.invoke(app, ["remove", "x"])
+        assert result.exit_code == 0
+        assert result.stdout == typer.style("Input should have been a string!", fg="white", bg="red") + '\n'
+        # no-output
+        paste_mock.return_value = "Testing sentence five here."
+        result = runner.invoke(app, ["remove", "here", "--no-output"])
+        assert result.exit_code == 0
+        assert result.stdout == ''
+        assert copy_mock.call_args.args == ("Testing sentence five .",)
```

### Comparing `prettycopy-0.2.0/prettycopy.egg-info/PKG-INFO` & `prettycopy-0.2.1/prettycopy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettycopy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A better copy-paster
 Author-email: Adi Gal <adigal03@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,20 +224,20 @@
 A beginner-friendly library for clean, format-friendly copy-pasting.
 
 [![License](https://img.shields.io/github/license/hippothebrave/prettycopy)](https://github.com/hippothebrave/prettycopy/blob/main/LICENSE)
 [![GitHub issues](https://img.shields.io/github/issues/hippothebrave/prettycopy)](https://github.com/hippothebrave/prettycopy/issues)
 [![Build Status](https://github.com/hippothebrave/prettycopy/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/hippothebrave/prettycopy/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/hippothebrave/prettycopy/branch/main/graph/badge.svg)](https://codecov.io/gh/hippothebrave/prettycopy)
 [![PyPI](https://img.shields.io/pypi/v/prettycopy)](https://pypi.org/project/prettycopy/)
-[![Documentation](https://img.shields.io/badge/Documentation-ReadTheDocs-informational)](https://prettycopy.readthedocs.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/prettycopy/badge/?version=latest)](https://prettycopy.readthedocs.io/en/latest/?badge=latest)
 
 ## Overview
 Copying and pasting text is one of the most commonly-used functionalities we have on our computers. But sometimes, there are formatting issues in the text you're copying that a simple 'paste without formatting' can't fix.
 
-Enter prettycopy.
+Enter PrettyCopy.
 
 PrettyCopy will help you clean up the text on your clipboard *before* you paste it. Just copy text, run a PrettyCopy function, and you'll be able to paste it with corrections already in place!
 
 See our documentation [here](https://prettycopy.readthedocs.io/en/latest/).
 
 ### Installation
 
@@ -245,15 +245,17 @@
 
 ```bash
 pip install prettycopy
 ```
 
 ## Usage
 
-So... how do you use PrettyCopy? It's very simple! You can use PrettyCopy at the command line, or through your own program.
+So... how do you use PrettyCopy? It's very simple! You can use PrettyCopy functions at the command line, or through your own program.
+
+Learn more about the functions using `prettycopy --help` at the command line, or by checking our [documentation](https://prettycopy.readthedocs.io/en/latest/).
 
 ### Command Line
 Copy a piece of text.
 In the command line, type `prettycopy [function_name] [any_args]`. 
 PrettyCopy will print the corrected text, just to show you what your clipboard current contains. 
 Now, as soon as you paste, the text will already be corrected.
 
@@ -261,30 +263,14 @@
 
 Confused? Type `prettycopy --help` to get a list of possible functions, and `prettycopy [function_name] --help` to get help for any particular function.
 
 ### In a Program
 PrettyCopy will take in some text, correct it, and copy the corrected text to your clipboard. It will also return the corrected text as a return value, in case you want to keep using it (for example, in a nested function).
 By default, PrettyCopy will run on the text in your clipboard. If you want to correct a different text, enter your preferred text as an argument.
 
-### Functions
-
-`prettycopy.nonewlines(optional_text)`: Removes all line breaks from the text.
-
-`prettycopy.nobullets(optional_text)`: Removes all bullet symbols (•) and replaces them with line breaks.
-
-`prettycopy.bullettopar(optional_text)`: Removes all line breaks and bullet symbols (•) and replaces them with spaces, returning a single paragraph.
-
-`prettycopy.simplequote(optional_text)`: Adds quotation marks around the text.
-
-`prettycopy.quote(optional_end_punctuation, optional_text)`: Adds quotation marks around the text, ending in a punctuation mark. The default is a comma.
-
-> Example: *this is a test* --> prettycopy.quote() --> *"this is a test,"*
-
-> Example: *this is a test* --> prettycopy.quote('!') --> *"this is a test!"*
-
-`prettycopy.trimspacing(optional_text)`: Removes empty lines.
+## Examples
+PrettyCopy can be used for fixing issues with line breaks; removing extraneous bullet point symbols; adding quotation marks (and optional punctuation) around a copied text; and more! 
 
-`prettycopy.smartcopy(optional_text)`: Removes line breaks in an intelligent manner: adding spaces between words, but not inside words that have been split.
+![](https://github.com/hippothebrave/prettycopy/blob/main/docs/images/smartcopy_pc.gif)
 
-> Example: *this\nis a te\nst* --> prettycopy.smartcopy() --> *this is a test*
+See the [documentation](https://prettycopy.readthedocs.io/en/latest/) for the complete list of functions.
 
-`prettycopy.betterbullets(docID)`: If you enter the document ID of an editable Google Doc (the long string of letters and numbers in the URL), this function will copy the text in your clipboard to the end of the document, replacing all bullet symbols (•) with correctly-formatted bullet points. Still under construction.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prettycopy-0.2.0/prettycopy.egg-info/SOURCES.txt` & `prettycopy-0.2.1/prettycopy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 docs/Makefile
 docs/conf.py
 docs/dev_intro.md
 docs/index.md
 docs/make.bat
 docs/requirements.txt
 docs/images/bullets_nopc.gif
+docs/images/bullettolist_pc.gif
 docs/images/bullettopar_pc.gif
-docs/images/nobullets_pc.gif
 docs/images/pchelp.gif
 docs/images/pcnonewlines.gif
 docs/images/quote_pc.gif
 docs/images/quotes_nopc.gif
+docs/images/remove_pc.gif
 docs/images/simplequote_pc.gif
 docs/images/smartcopy_pc.gif
 docs/images/trimspace_nopc.gif
 docs/images/trimspacing_pc.gif
 prettycopy/__init__.py
 prettycopy/__main__.py
 prettycopy/_version.py
```

### Comparing `prettycopy-0.2.0/pyproject.toml` & `prettycopy-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,25 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "prettycopy"
 authors = [{name = "Adi Gal", email = "adigal03@gmail.com"}]
 description="A better copy-paster"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.7"
 
 dependencies = [
     "pyperclip",
     "google-auth-oauthlib",
     "google-auth",
     "google-api-python-client",
     "nltk",
     "textblob",
     "typer",
-    "pyspellchecker",
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
```

