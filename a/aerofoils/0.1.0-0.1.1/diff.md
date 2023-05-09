# Comparing `tmp/aerofoils-0.1.0.tar.gz` & `tmp/aerofoils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerofoils-0.1.0.tar", last modified: Tue May  9 10:18:40 2023, max compression
+gzip compressed data, was "aerofoils-0.1.1.tar", last modified: Tue May  9 10:23:47 2023, max compression
```

## Comparing `aerofoils-0.1.0.tar` & `aerofoils-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:18:40.913085 aerofoils-0.1.0/
--rw-r--r--   0 tiao      (1000) tiao      (1000)      155 2023-05-09 10:08:57.000000 aerofoils-0.1.0/AUTHORS.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)     3501 2023-05-09 10:08:57.000000 aerofoils-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)       89 2023-05-09 10:08:57.000000 aerofoils-0.1.0/HISTORY.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)     1069 2023-05-09 10:08:57.000000 aerofoils-0.1.0/LICENSE
--rw-r--r--   0 tiao      (1000) tiao      (1000)      262 2023-05-09 10:08:57.000000 aerofoils-0.1.0/MANIFEST.in
--rw-r--r--   0 tiao      (1000) tiao      (1000)     1729 2023-05-09 10:18:40.913085 aerofoils-0.1.0/PKG-INFO
--rw-r--r--   0 tiao      (1000) tiao      (1000)      972 2023-05-09 10:08:57.000000 aerofoils-0.1.0/README.rst
-drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:18:40.913085 aerofoils-0.1.0/aerofoils.egg-info/
--rw-r--r--   0 tiao      (1000) tiao      (1000)     1729 2023-05-09 10:18:40.000000 aerofoils-0.1.0/aerofoils.egg-info/PKG-INFO
--rw-r--r--   0 tiao      (1000) tiao      (1000)      581 2023-05-09 10:18:40.000000 aerofoils-0.1.0/aerofoils.egg-info/SOURCES.txt
--rw-r--r--   0 tiao      (1000) tiao      (1000)        1 2023-05-09 10:18:40.000000 aerofoils-0.1.0/aerofoils.egg-info/dependency_links.txt
--rw-r--r--   0 tiao      (1000) tiao      (1000)       45 2023-05-09 10:18:40.000000 aerofoils-0.1.0/aerofoils.egg-info/entry_points.txt
--rw-r--r--   0 tiao      (1000) tiao      (1000)        1 2023-05-09 10:18:40.000000 aerofoils-0.1.0/aerofoils.egg-info/not-zip-safe
--rw-r--r--   0 tiao      (1000) tiao      (1000)       11 2023-05-09 10:18:40.000000 aerofoils-0.1.0/aerofoils.egg-info/requires.txt
--rw-r--r--   0 tiao      (1000) tiao      (1000)        8 2023-05-09 10:18:40.000000 aerofoils-0.1.0/aerofoils.egg-info/top_level.txt
-drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:18:40.913085 aerofoils-0.1.0/airfoil/
--rw-r--r--   0 tiao      (1000) tiao      (1000)      125 2023-05-09 10:08:57.000000 aerofoils-0.1.0/airfoil/__init__.py
--rw-r--r--   0 tiao      (1000) tiao      (1000)       19 2023-05-09 10:08:57.000000 aerofoils-0.1.0/airfoil/airfoil.py
--rw-r--r--   0 tiao      (1000) tiao      (1000)      399 2023-05-09 10:08:57.000000 aerofoils-0.1.0/airfoil/cli.py
-drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:18:40.913085 aerofoils-0.1.0/docs/
--rw-r--r--   0 tiao      (1000) tiao      (1000)      608 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/Makefile
--rw-r--r--   0 tiao      (1000) tiao      (1000)       28 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/authors.rst
--rwxr-xr-x   0 tiao      (1000) tiao      (1000)     4776 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/conf.py
--rw-r--r--   0 tiao      (1000) tiao      (1000)       33 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/contributing.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)       28 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/history.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)      305 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/index.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)     1105 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/installation.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)      805 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/make.bat
--rw-r--r--   0 tiao      (1000) tiao      (1000)       27 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/readme.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)       70 2023-05-09 10:08:57.000000 aerofoils-0.1.0/docs/usage.rst
--rw-r--r--   0 tiao      (1000) tiao      (1000)      424 2023-05-09 10:18:40.916419 aerofoils-0.1.0/setup.cfg
--rw-r--r--   0 tiao      (1000) tiao      (1000)     1349 2023-05-09 10:18:32.000000 aerofoils-0.1.0/setup.py
-drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:18:40.913085 aerofoils-0.1.0/tests/
--rw-r--r--   0 tiao      (1000) tiao      (1000)       37 2023-05-09 10:08:57.000000 aerofoils-0.1.0/tests/__init__.py
--rw-r--r--   0 tiao      (1000) tiao      (1000)      979 2023-05-09 10:08:57.000000 aerofoils-0.1.0/tests/test_airfoil.py
+drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:23:47.639982 aerofoils-0.1.1/
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      155 2023-05-09 10:22:44.000000 aerofoils-0.1.1/AUTHORS.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)     3523 2023-05-09 10:22:44.000000 aerofoils-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       89 2023-05-09 10:22:44.000000 aerofoils-0.1.1/HISTORY.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)     1069 2023-05-09 10:22:44.000000 aerofoils-0.1.1/LICENSE
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      262 2023-05-09 10:22:44.000000 aerofoils-0.1.1/MANIFEST.in
+-rw-r--r--   0 tiao      (1000) tiao      (1000)     1772 2023-05-09 10:23:47.639982 aerofoils-0.1.1/PKG-INFO
+-rw-r--r--   0 tiao      (1000) tiao      (1000)     1002 2023-05-09 10:22:44.000000 aerofoils-0.1.1/README.rst
+drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:23:47.636649 aerofoils-0.1.1/aerofoils/
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      126 2023-05-09 10:23:40.000000 aerofoils-0.1.1/aerofoils/__init__.py
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       19 2023-05-09 10:22:44.000000 aerofoils-0.1.1/aerofoils/aerofoils.py
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      405 2023-05-09 10:22:44.000000 aerofoils-0.1.1/aerofoils/cli.py
+drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:23:47.636649 aerofoils-0.1.1/aerofoils.egg-info/
+-rw-r--r--   0 tiao      (1000) tiao      (1000)     1772 2023-05-09 10:23:47.000000 aerofoils-0.1.1/aerofoils.egg-info/PKG-INFO
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      591 2023-05-09 10:23:47.000000 aerofoils-0.1.1/aerofoils.egg-info/SOURCES.txt
+-rw-r--r--   0 tiao      (1000) tiao      (1000)        1 2023-05-09 10:23:47.000000 aerofoils-0.1.1/aerofoils.egg-info/dependency_links.txt
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       49 2023-05-09 10:23:47.000000 aerofoils-0.1.1/aerofoils.egg-info/entry_points.txt
+-rw-r--r--   0 tiao      (1000) tiao      (1000)        1 2023-05-09 10:23:47.000000 aerofoils-0.1.1/aerofoils.egg-info/not-zip-safe
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       11 2023-05-09 10:23:47.000000 aerofoils-0.1.1/aerofoils.egg-info/requires.txt
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       10 2023-05-09 10:23:47.000000 aerofoils-0.1.1/aerofoils.egg-info/top_level.txt
+drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:23:47.639982 aerofoils-0.1.1/docs/
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      610 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/Makefile
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       28 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 tiao      (1000) tiao      (1000)     4798 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/conf.py
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       33 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/contributing.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       28 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/history.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      306 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/index.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)     1118 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/installation.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      807 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/make.bat
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       27 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/readme.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       73 2023-05-09 10:22:44.000000 aerofoils-0.1.1/docs/usage.rst
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      426 2023-05-09 10:23:47.639982 aerofoils-0.1.1/setup.cfg
+-rw-r--r--   0 tiao      (1000) tiao      (1000)     1370 2023-05-09 10:23:40.000000 aerofoils-0.1.1/setup.py
+drwxr-xr-x   0 tiao      (1000) tiao      (1000)        0 2023-05-09 10:23:47.639982 aerofoils-0.1.1/tests/
+-rw-r--r--   0 tiao      (1000) tiao      (1000)       39 2023-05-09 10:22:44.000000 aerofoils-0.1.1/tests/__init__.py
+-rw-r--r--   0 tiao      (1000) tiao      (1000)      989 2023-05-09 10:22:44.000000 aerofoils-0.1.1/tests/test_aerofoils.py
```

### Comparing `aerofoils-0.1.0/CONTRIBUTING.rst` & `aerofoils-0.1.1/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/ltiao/airfoil/issues.
+Report bugs at https://github.com/ltiao/aerofoils/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -34,56 +34,56 @@
 
 Look through the GitHub issues for features. Anything tagged with "enhancement"
 and "help wanted" is open to whoever wants to implement it.
 
 Write Documentation
 ~~~~~~~~~~~~~~~~~~~
 
-Airfoils could always use more documentation, whether as part of the
-official Airfoils docs, in docstrings, or even on the web in blog posts,
+Aerofoils could always use more documentation, whether as part of the
+official Aerofoils docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/ltiao/airfoil/issues.
+The best way to send feedback is to file an issue at https://github.com/ltiao/aerofoils/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
 
 Get Started!
 ------------
 
-Ready to contribute? Here's how to set up `airfoil` for local development.
+Ready to contribute? Here's how to set up `aerofoils` for local development.
 
-1. Fork the `airfoil` repo on GitHub.
+1. Fork the `aerofoils` repo on GitHub.
 2. Clone your fork locally::
 
-    $ git clone git@github.com:your_name_here/airfoil.git
+    $ git clone git@github.com:your_name_here/aerofoils.git
 
 3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
 
-    $ mkvirtualenv airfoil
-    $ cd airfoil/
+    $ mkvirtualenv aerofoils
+    $ cd aerofoils/
     $ python setup.py develop
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
 5. When you're done making changes, check that your changes pass flake8 and the
    tests, including testing other Python versions with tox::
 
-    $ flake8 airfoil tests
+    $ flake8 aerofoils tests
     $ python setup.py test or pytest
     $ tox
 
    To get flake8 and tox, just pip install them into your virtualenv.
 
 6. Commit your changes and push your branch to GitHub::
 
@@ -99,23 +99,23 @@
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
 3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
-   https://travis-ci.com/ltiao/airfoil/pull_requests
+   https://travis-ci.com/ltiao/aerofoils/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
 
-$ pytest tests.test_airfoil
+$ pytest tests.test_aerofoils
 
 
 Deploying
 ---------
 
 A reminder for the maintainers on how to deploy.
 Make sure all your changes are committed (including an entry in HISTORY.rst).
```

### Comparing `aerofoils-0.1.0/LICENSE` & `aerofoils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aerofoils-0.1.0/PKG-INFO` & `aerofoils-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 Metadata-Version: 2.1
 Name: aerofoils
-Version: 0.1.0
-Summary: Airfoil Design
-Home-page: https://github.com/ltiao/airfoil
+Version: 0.1.1
+Summary: Aerofoil Design Toolkit
+Home-page: https://github.com/ltiao/aerofoils
 Author: Louis Tiao
 Author-email: louistiao@gmail.com
 License: MIT license
-Keywords: airfoil
+Keywords: aerofoils
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-========
-Airfoils
-========
+=========
+Aerofoils
+=========
 
 
-.. image:: https://img.shields.io/pypi/v/airfoil.svg
-        :target: https://pypi.python.org/pypi/airfoil
+.. image:: https://img.shields.io/pypi/v/aerofoils.svg
+        :target: https://pypi.python.org/pypi/aerofoils
 
-.. image:: https://img.shields.io/travis/ltiao/airfoil.svg
-        :target: https://travis-ci.com/ltiao/airfoil
+.. image:: https://img.shields.io/travis/ltiao/aerofoils.svg
+        :target: https://travis-ci.com/ltiao/aerofoils
 
-.. image:: https://readthedocs.org/projects/airfoil/badge/?version=latest
-        :target: https://airfoil.readthedocs.io/en/latest/?version=latest
+.. image:: https://readthedocs.org/projects/aerofoils/badge/?version=latest
+        :target: https://aerofoils.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
-.. image:: https://pyup.io/repos/github/ltiao/airfoil/shield.svg
-     :target: https://pyup.io/repos/github/ltiao/airfoil/
+.. image:: https://pyup.io/repos/github/ltiao/aerofoils/shield.svg
+     :target: https://pyup.io/repos/github/ltiao/aerofoils/
      :alt: Updates
 
 
 
-Airfoil Design
+Aerofoil Design Toolkit
 
 
 * Free software: MIT license
-* Documentation: https://airfoil.readthedocs.io.
+* Documentation: https://aerofoils.readthedocs.io.
 
 
 Features
 --------
 
 * TODO
```

### Comparing `aerofoils-0.1.0/aerofoils.egg-info/PKG-INFO` & `aerofoils-0.1.1/aerofoils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 Metadata-Version: 2.1
 Name: aerofoils
-Version: 0.1.0
-Summary: Airfoil Design
-Home-page: https://github.com/ltiao/airfoil
+Version: 0.1.1
+Summary: Aerofoil Design Toolkit
+Home-page: https://github.com/ltiao/aerofoils
 Author: Louis Tiao
 Author-email: louistiao@gmail.com
 License: MIT license
-Keywords: airfoil
+Keywords: aerofoils
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-========
-Airfoils
-========
+=========
+Aerofoils
+=========
 
 
-.. image:: https://img.shields.io/pypi/v/airfoil.svg
-        :target: https://pypi.python.org/pypi/airfoil
+.. image:: https://img.shields.io/pypi/v/aerofoils.svg
+        :target: https://pypi.python.org/pypi/aerofoils
 
-.. image:: https://img.shields.io/travis/ltiao/airfoil.svg
-        :target: https://travis-ci.com/ltiao/airfoil
+.. image:: https://img.shields.io/travis/ltiao/aerofoils.svg
+        :target: https://travis-ci.com/ltiao/aerofoils
 
-.. image:: https://readthedocs.org/projects/airfoil/badge/?version=latest
-        :target: https://airfoil.readthedocs.io/en/latest/?version=latest
+.. image:: https://readthedocs.org/projects/aerofoils/badge/?version=latest
+        :target: https://aerofoils.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
-.. image:: https://pyup.io/repos/github/ltiao/airfoil/shield.svg
-     :target: https://pyup.io/repos/github/ltiao/airfoil/
+.. image:: https://pyup.io/repos/github/ltiao/aerofoils/shield.svg
+     :target: https://pyup.io/repos/github/ltiao/aerofoils/
      :alt: Updates
 
 
 
-Airfoil Design
+Aerofoil Design Toolkit
 
 
 * Free software: MIT license
-* Documentation: https://airfoil.readthedocs.io.
+* Documentation: https://aerofoils.readthedocs.io.
 
 
 Features
 --------
 
 * TODO
```

### Comparing `aerofoils-0.1.0/aerofoils.egg-info/SOURCES.txt` & `aerofoils-0.1.1/aerofoils.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
+aerofoils/__init__.py
+aerofoils/aerofoils.py
+aerofoils/cli.py
 aerofoils.egg-info/PKG-INFO
 aerofoils.egg-info/SOURCES.txt
 aerofoils.egg-info/dependency_links.txt
 aerofoils.egg-info/entry_points.txt
 aerofoils.egg-info/not-zip-safe
 aerofoils.egg-info/requires.txt
 aerofoils.egg-info/top_level.txt
-airfoil/__init__.py
-airfoil/airfoil.py
-airfoil/cli.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
-tests/test_airfoil.py
+tests/test_aerofoils.py
```

### Comparing `aerofoils-0.1.0/docs/Makefile` & `aerofoils-0.1.1/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
 SPHINXOPTS    =
 SPHINXBUILD   = python -msphinx
-SPHINXPROJ    = airfoil
+SPHINXPROJ    = aerofoils
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `aerofoils-0.1.0/docs/conf.py` & `aerofoils-0.1.1/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# airfoil documentation build configuration file, created by
+# aerofoils documentation build configuration file, created by
 # sphinx-quickstart on Fri Jun  9 13:47:02 2017.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
@@ -17,15 +17,15 @@
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
 sys.path.insert(0, os.path.abspath('..'))
 
-import airfoil
+import aerofoils
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
@@ -42,26 +42,26 @@
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = 'Airfoils'
+project = 'Aerofoils'
 copyright = "2023, Louis Tiao"
 author = "Louis Tiao"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = airfoil.__version__
+version = aerofoils.__version__
 # The full version, including alpha/beta/rc tags.
-release = airfoil.__version__
+release = aerofoils.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
@@ -96,15 +96,15 @@
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'airfoildoc'
+htmlhelp_basename = 'aerofoilsdoc'
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
@@ -123,40 +123,40 @@
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'airfoil.tex',
-     'Airfoils Documentation',
+    (master_doc, 'aerofoils.tex',
+     'Aerofoils Documentation',
      'Louis Tiao', 'manual'),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'airfoil',
-     'Airfoils Documentation',
+    (master_doc, 'aerofoils',
+     'Aerofoils Documentation',
      [author], 1)
 ]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'airfoil',
-     'Airfoils Documentation',
+    (master_doc, 'aerofoils',
+     'Aerofoils Documentation',
      author,
-     'airfoil',
+     'aerofoils',
      'One line description of project.',
      'Miscellaneous'),
 ]
```

### Comparing `aerofoils-0.1.0/docs/make.bat` & `aerofoils-0.1.1/docs/make.bat`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=python -msphinx
 )
 set SOURCEDIR=.
 set BUILDDIR=_build
-set SPHINXPROJ=airfoil
+set SPHINXPROJ=aerofoils
 
 if "%1" == "" goto help
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The Sphinx module was not found. Make sure you have Sphinx installed,
```

### Comparing `aerofoils-0.1.0/setup.py` & `aerofoils-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,26 +24,26 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="Airfoil Design",
+    description="Aerofoil Design Toolkit",
     entry_points={
         'console_scripts': [
-            'airfoil=airfoil.cli:main',
+            'aerofoils=aerofoils.cli:main',
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
-    keywords='airfoil',
+    keywords='aerofoils',
     name='aerofoils',
-    packages=find_packages(include=['airfoil', 'airfoil.*']),
+    packages=find_packages(include=['aerofoils', 'aerofoils.*']),
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/ltiao/airfoil',
-    version='0.1.0',
+    url='https://github.com/ltiao/aerofoils',
+    version='0.1.1',
     zip_safe=False,
 )
```

