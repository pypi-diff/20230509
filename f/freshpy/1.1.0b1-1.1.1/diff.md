# Comparing `tmp/freshpy-1.1.0b1.tar.gz` & `tmp/freshpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freshpy-1.1.0b1.tar", last modified: Tue Jan  4 20:16:11 2022, max compression
+gzip compressed data, was "freshpy-1.1.1.tar", last modified: Mon May  8 22:00:38 2023, max compression
```

## Comparing `freshpy-1.1.0b1.tar` & `freshpy-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-01-04 20:16:11.070960 freshpy-1.1.0b1/
--rw-rw-rw-   0        0        0     1071 2021-12-28 15:29:54.000000 freshpy-1.1.0b1/LICENSE
--rw-rw-rw-   0        0        0       67 2021-12-30 20:05:30.000000 freshpy-1.1.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0     8818 2022-01-04 20:16:11.067960 freshpy-1.1.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     7128 2022-01-04 19:59:26.000000 freshpy-1.1.0b1/README.md
--rw-rw-rw-   0        0        0      110 2021-12-30 16:12:02.000000 freshpy-1.1.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-01-04 20:16:11.072960 freshpy-1.1.0b1/setup.cfg
--rw-rw-rw-   0        0        0     3341 2022-01-04 20:04:14.000000 freshpy-1.1.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-04 20:16:10.736966 freshpy-1.1.0b1/src/
-drwxrwxrwx   0        0        0        0 2022-01-04 20:16:10.853967 freshpy-1.1.0b1/src/freshpy/
--rw-rw-rw-   0        0        0      462 2021-12-30 19:47:02.000000 freshpy-1.1.0b1/src/freshpy/__init__.py
--rw-rw-rw-   0        0        0     3947 2022-01-04 17:01:45.000000 freshpy-1.1.0b1/src/freshpy/api.py
--rw-rw-rw-   0        0        0     7705 2022-01-04 19:50:19.000000 freshpy-1.1.0b1/src/freshpy/core.py
-drwxrwxrwx   0        0        0        0 2022-01-04 20:16:10.956965 freshpy-1.1.0b1/src/freshpy/errors/
--rw-rw-rw-   0        0        0      287 2021-12-28 16:30:03.000000 freshpy-1.1.0b1/src/freshpy/errors/__init__.py
--rw-rw-rw-   0        0        0    14482 2022-01-04 16:45:50.000000 freshpy-1.1.0b1/src/freshpy/errors/exceptions.py
--rw-rw-rw-   0        0        0      485 2021-12-28 16:30:03.000000 freshpy-1.1.0b1/src/freshpy/errors/handlers.py
--rw-rw-rw-   0        0        0     9032 2022-01-04 18:34:16.000000 freshpy-1.1.0b1/src/freshpy/tickets.py
-drwxrwxrwx   0        0        0        0 2022-01-04 20:16:11.057967 freshpy-1.1.0b1/src/freshpy/utils/
--rw-rw-rw-   0        0        0      271 2021-12-28 15:29:54.000000 freshpy-1.1.0b1/src/freshpy/utils/__init__.py
--rw-rw-rw-   0        0        0     1827 2021-12-30 21:10:08.000000 freshpy-1.1.0b1/src/freshpy/utils/core_utils.py
--rw-rw-rw-   0        0        0    11960 2021-12-28 15:29:54.000000 freshpy-1.1.0b1/src/freshpy/utils/log_utils.py
--rw-rw-rw-   0        0        0      754 2022-01-04 19:23:01.000000 freshpy-1.1.0b1/src/freshpy/utils/version.py
-drwxrwxrwx   0        0        0        0 2022-01-04 20:16:10.892979 freshpy-1.1.0b1/src/freshpy.egg-info/
--rw-rw-rw-   0        0        0     8818 2022-01-04 20:16:10.000000 freshpy-1.1.0b1/src/freshpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2022-01-04 20:16:10.000000 freshpy-1.1.0b1/src/freshpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-04 20:16:10.000000 freshpy-1.1.0b1/src/freshpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      259 2022-01-04 20:16:10.000000 freshpy-1.1.0b1/src/freshpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-01-04 20:16:10.000000 freshpy-1.1.0b1/src/freshpy.egg-info/top_level.txt
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 22:00:38.501896 freshpy-1.1.1/
+-rw-r--r--   0 shurtj     (501) staff       (20)     1071 2021-12-27 21:26:29.000000 freshpy-1.1.1/LICENSE
+-rw-r--r--   0 shurtj     (501) staff       (20)     8588 2023-05-08 22:00:38.501510 freshpy-1.1.1/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)     7130 2022-07-26 14:50:28.000000 freshpy-1.1.1/README.md
+-rw-r--r--   0 shurtj     (501) staff       (20)      104 2021-12-30 18:17:50.000000 freshpy-1.1.1/pyproject.toml
+-rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-05-08 22:00:38.501996 freshpy-1.1.1/setup.cfg
+-rw-r--r--   0 shurtj     (501) staff       (20)     3246 2023-05-08 21:57:41.000000 freshpy-1.1.1/setup.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 22:00:38.483351 freshpy-1.1.1/src/
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 22:00:38.490744 freshpy-1.1.1/src/freshpy/
+-rw-r--r--   0 shurtj     (501) staff       (20)      462 2021-12-30 18:33:24.000000 freshpy-1.1.1/src/freshpy/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3947 2022-07-26 14:50:28.000000 freshpy-1.1.1/src/freshpy/api.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     7705 2022-07-26 14:50:28.000000 freshpy-1.1.1/src/freshpy/core.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 22:00:38.496565 freshpy-1.1.1/src/freshpy/errors/
+-rw-r--r--   0 shurtj     (501) staff       (20)      287 2021-12-30 18:17:50.000000 freshpy-1.1.1/src/freshpy/errors/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    14482 2022-01-01 05:24:12.000000 freshpy-1.1.1/src/freshpy/errors/exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      485 2021-12-30 18:17:50.000000 freshpy-1.1.1/src/freshpy/errors/handlers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     9032 2022-07-26 14:50:28.000000 freshpy-1.1.1/src/freshpy/tickets.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 22:00:38.500984 freshpy-1.1.1/src/freshpy/utils/
+-rw-r--r--   0 shurtj     (501) staff       (20)      271 2021-12-30 18:17:50.000000 freshpy-1.1.1/src/freshpy/utils/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1770 2021-12-31 17:16:31.000000 freshpy-1.1.1/src/freshpy/utils/core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11960 2021-12-30 18:17:50.000000 freshpy-1.1.1/src/freshpy/utils/log_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      718 2023-05-08 21:59:16.000000 freshpy-1.1.1/src/freshpy/utils/version.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 22:00:38.493567 freshpy-1.1.1/src/freshpy.egg-info/
+-rw-r--r--   0 shurtj     (501) staff       (20)     8588 2023-05-08 22:00:38.000000 freshpy-1.1.1/src/freshpy.egg-info/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)      518 2023-05-08 22:00:38.000000 freshpy-1.1.1/src/freshpy.egg-info/SOURCES.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-05-08 22:00:38.000000 freshpy-1.1.1/src/freshpy.egg-info/dependency_links.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      259 2023-05-08 22:00:38.000000 freshpy-1.1.1/src/freshpy.egg-info/requires.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        8 2023-05-08 22:00:38.000000 freshpy-1.1.1/src/freshpy.egg-info/top_level.txt
```

### Comparing `freshpy-1.1.0b1/LICENSE` & `freshpy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freshpy-1.1.0b1/PKG-INFO` & `freshpy-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-Metadata-Version: 2.1
-Name: freshpy
-Version: 1.1.0b1
-Summary: A Python toolset for utilizing the Freshservice API
-Home-page: https://github.com/jeffshurtliff/freshpy
-Author: Jeff Shurtliff
-Author-email: jeff.shurtliff@rsa.com
-License: UNKNOWN
-Project-URL: Change Log, https://freshpy.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/jeffshurtliff/freshpy/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Communications
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Office/Business
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: sphinx
-License-File: LICENSE
-
-<a href='https://pypi.org/project/freshpy/'>
-    <img src="https://github.com/jeffshurtliff/freshpy/blob/main/docs/_static/freshpy-logo.png" width="100" />
-</a>
-
-# FreshPy
-A Python toolset for utilizing the Freshservice API
-
-<table>
-    <tr>
-        <td>Latest Stable Release</td>
-        <td>
-            <a href='https://pypi.org/project/freshpy/'>
-                <img alt="PyPI" src="https://img.shields.io/pypi/v/freshpy">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td>Latest Dev/Beta/RC Release</td>
-        <td>
-            <a href='https://pypi.org/project/freshpy/#history'>
-                <img alt="PyPI" src="https://img.shields.io/badge/pypi-1.1.0b1-blue">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td>Build Status</td>
-        <td>
-            N/A
-            <!--
-            <a href="https://github.com/jeffshurtliff/freshpy/blob/master/.github/workflows/pythonpackage.yml">
-                <img alt="GitHub Workflow Status" 
-                src="https://img.shields.io/github/workflow/status/jeffshurtliff/khoros/Python package">
-            </a>
-            -->
-        </td>
-    </tr>
-    <tr>
-        <td>Supported Versions</td>
-        <td>
-            <a href='https://pypi.org/project/freshpy/'>
-                <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/freshpy">
-            </a>
-        </td>
-    </tr>
-    <!--
-    <tr>
-        <td>Code Coverage</td>
-        <td>
-            <a href="https://codecov.io/gh/jeffshurtliff/freshpy">
-                <img src="https://codecov.io/gh/jeffshurtliff/freshpy/branch/master/graph/badge.svg" />
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td>Code Quality (LGTM)</td>
-        <td>
-            <a href="https://lgtm.com/projects/g/jeffshurtliff/freshpy">
-            <img alt="LGTM Grade" src="https://img.shields.io/lgtm/grade/python/github/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td>CodeFactor Grade</td>
-        <td>
-            <a href="https://lgtm.com/projects/g/jeffshurtliff/freshpy">
-            <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-    -->
-    <tr>
-        <td>Documentation</td>
-        <td>
-            <a href='https://freshpy.readthedocs.io/en/latest/?badge=latest'>
-                <img src='https://readthedocs.org/projects/freshpy/badge/?version=latest' alt='Documentation Status' /><br />
-            </a>
-        </td>
-    </tr>
-    <!--
-    <tr>
-        <td>Security Audits</td>
-        <td>
-            <a href="https://github.com/marketplace/actions/python-security-check-using-bandit">
-                <img alt="Bandit" src="https://img.shields.io/badge/security-bandit-yellow.svg">
-            </a><br />
-            <a href="https://github.com/marketplace/actions/pycharm-python-security-scanner">
-                <img alt="PyCharm Security Scanner" src="https://img.shields.io/badge/security-pycharm%20security%20scanner-green">
-            </a>
-        </td>
-    </tr>
-    -->
-    <tr>
-        <td>License</td>
-        <td>
-            <a href="https://github.com/jeffshurtliff/freshpy/blob/master/LICENSE">
-                <img alt="License (GitHub)" src="https://img.shields.io/github/license/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td style="vertical-align: top;">Issues</td>
-        <td>
-            <a href="https://github.com/jeffshurtliff/freshpy/issues">
-                <img style="margin-bottom:5px;" alt="GitHub open issues" src="https://img.shields.io/github/issues-raw/jeffshurtliff/freshpy"><br />
-            </a>
-            <a href="https://github.com/jeffshurtliff/freshpy/issues">
-                <img alt="GitHub closed issues" src="https://img.shields.io/github/issues-closed-raw/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td style="vertical-align: top;">Pull Requests</td>
-        <td>
-            <a href="https://github.com/jeffshurtliff/freshpy/pulls">
-                <img style="margin-bottom:5px;" alt="GitHub pull open requests" src="https://img.shields.io/github/issues-pr-raw/jeffshurtliff/freshpy"><br />
-            </a>
-            <a href="https://github.com/jeffshurtliff/freshpy/pulls">
-                <img alt="GitHub closed pull requests" src="https://img.shields.io/github/issues-pr-closed-raw/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-</table>
-
-## Installation
-The package can be installed via pip using the syntax below.
-
-```sh
-pip install freshpy --upgrade
-```
-
-You may also clone the repository and install from source using below.
-
-```sh
-git clone git://github.com/jeffshurtliff/freshpy.git
-cd freshpy/
-python setup.py install
-```
-
-## Usage
-This section provides basic usage instructions for the package.
-
-### Importing the package
-Rather than importing the base package, it is recommended that you import the primary `FreshPy` class using the syntax
-below.
-
-```python
-from freshpy import FreshPy
-```
-
-### Initializing a Khoros object instance
-The primary `FreshPy` object serves many purposes, the most important being to establish a connection to the 
-Freshservice environment with which you intend to interact. As such, when initializing an instance of the `FreshPy` 
-object, you will need to pass it the Freshservice URL (e.g. `example.freshservice.com`) and the API key it will use 
-to authenticate so that the connection can be established.
-
-#### Passing the information directly into the object
-The domain and API key can be passed directly into the `FreshPy` object when initializing it, as
-demonstrated in the example below.
-
-```python
-fresh = FreshPy(domain='example.freshservice.com', api_key='abc123DEF456')
-```
-
-### Interacting with the Freshservice API
-Once the `FreshPy` object instance has been initialized, it can be leveraged to interact with a Freshservice
-environment in many ways, which is fully documented in the official
-[documentation](https://api.freshservice.com/). The example below demonstrates how information for a specific incident 
-ticket can be retrieved in JSON format.
-
-```python
-ticket_data = fresh.tickets.get_ticket(1299)
-```
-
-## License
-[MIT License](https://github.com/jeffshurtliff/freshpy/blob/master/LICENSE)
-
-## Changelog
-Refer to the [changelog](https://freshpy.readthedocs.io/en/latest/changelog.html) for version change information.
-
-## Reporting Issues
-Issues can be reported within the [GitHub repository](https://github.com/jeffshurtliff/freshpy/issues).
-
-## Additional Resources
-Additional resources for leveraging the Freshservice API can be found in the official
-[Freshservice API Reference Documentation](https://api.freshservice.com/).
-
-## Donations
-If you would like to donate to this project then you can do so using 
-[this PayPal link](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=XDZ8M6UV6EFK6&item_name=FreshPy&currency_code=USD).
-
-## Disclaimer
-This package is considered unofficial and is in no way endorsed or supported by 
-[Freshservice](https://www.freshservice.com).
-
-
-
+Metadata-Version: 2.1
+Name: freshpy
+Version: 1.1.1
+Summary: A Python toolset for utilizing the Freshservice API
+Home-page: https://github.com/jeffshurtliff/freshpy
+Author: Jeff Shurtliff
+Author-email: jeff.shurtliff@rsa.com
+License: UNKNOWN
+Project-URL: Change Log, https://freshpy.readthedocs.io/en/latest/changelog.html
+Project-URL: Issue Tracker, https://github.com/jeffshurtliff/freshpy/issues
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Communications
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Office/Business
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: sphinx
+License-File: LICENSE
+
+<a href='https://pypi.org/project/freshpy/'>
+    <img src="https://github.com/jeffshurtliff/freshpy/blob/main/docs/_static/freshpy-logo.png" width="100" />
+</a>
+
+# FreshPy
+A Python toolset for utilizing the Freshservice API
+
+<table>
+    <tr>
+        <td>Latest Stable Release</td>
+        <td>
+            <a href='https://pypi.org/project/freshpy/'>
+                <img alt="PyPI" src="https://img.shields.io/pypi/v/freshpy">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td>Latest Dev/Beta/RC Release</td>
+        <td>
+            <a href='https://pypi.org/project/freshpy/#history'>
+                <img alt="PyPI" src="https://img.shields.io/badge/pypi-1.1.0b1-blue">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td>Build Status</td>
+        <td>
+            N/A
+            <!--
+            <a href="https://github.com/jeffshurtliff/freshpy/blob/master/.github/workflows/pythonpackage.yml">
+                <img alt="GitHub Workflow Status" 
+                src="https://img.shields.io/github/workflow/status/jeffshurtliff/freshpy/Python package">
+            </a>
+            -->
+        </td>
+    </tr>
+    <tr>
+        <td>Supported Versions</td>
+        <td>
+            <a href='https://pypi.org/project/freshpy/'>
+                <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/freshpy">
+            </a>
+        </td>
+    </tr>
+    <!--
+    <tr>
+        <td>Code Coverage</td>
+        <td>
+            <a href="https://codecov.io/gh/jeffshurtliff/freshpy">
+                <img src="https://codecov.io/gh/jeffshurtliff/freshpy/branch/master/graph/badge.svg" />
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td>Code Quality (LGTM)</td>
+        <td>
+            <a href="https://lgtm.com/projects/g/jeffshurtliff/freshpy">
+            <img alt="LGTM Grade" src="https://img.shields.io/lgtm/grade/python/github/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td>CodeFactor Grade</td>
+        <td>
+            <a href="https://lgtm.com/projects/g/jeffshurtliff/freshpy">
+            <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+    -->
+    <tr>
+        <td>Documentation</td>
+        <td>
+            <a href='https://freshpy.readthedocs.io/en/latest/?badge=latest'>
+                <img src='https://readthedocs.org/projects/freshpy/badge/?version=latest' alt='Documentation Status' /><br />
+            </a>
+        </td>
+    </tr>
+    <!--
+    <tr>
+        <td>Security Audits</td>
+        <td>
+            <a href="https://github.com/marketplace/actions/python-security-check-using-bandit">
+                <img alt="Bandit" src="https://img.shields.io/badge/security-bandit-yellow.svg">
+            </a><br />
+            <a href="https://github.com/marketplace/actions/pycharm-python-security-scanner">
+                <img alt="PyCharm Security Scanner" src="https://img.shields.io/badge/security-pycharm%20security%20scanner-green">
+            </a>
+        </td>
+    </tr>
+    -->
+    <tr>
+        <td>License</td>
+        <td>
+            <a href="https://github.com/jeffshurtliff/freshpy/blob/master/LICENSE">
+                <img alt="License (GitHub)" src="https://img.shields.io/github/license/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td style="vertical-align: top;">Issues</td>
+        <td>
+            <a href="https://github.com/jeffshurtliff/freshpy/issues">
+                <img style="margin-bottom:5px;" alt="GitHub open issues" src="https://img.shields.io/github/issues-raw/jeffshurtliff/freshpy"><br />
+            </a>
+            <a href="https://github.com/jeffshurtliff/freshpy/issues">
+                <img alt="GitHub closed issues" src="https://img.shields.io/github/issues-closed-raw/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td style="vertical-align: top;">Pull Requests</td>
+        <td>
+            <a href="https://github.com/jeffshurtliff/freshpy/pulls">
+                <img style="margin-bottom:5px;" alt="GitHub pull open requests" src="https://img.shields.io/github/issues-pr-raw/jeffshurtliff/freshpy"><br />
+            </a>
+            <a href="https://github.com/jeffshurtliff/freshpy/pulls">
+                <img alt="GitHub closed pull requests" src="https://img.shields.io/github/issues-pr-closed-raw/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+</table>
+
+## Installation
+The package can be installed via pip using the syntax below.
+
+```sh
+pip install freshpy --upgrade
+```
+
+You may also clone the repository and install from source using below.
+
+```sh
+git clone git://github.com/jeffshurtliff/freshpy.git
+cd freshpy/
+python setup.py install
+```
+
+## Usage
+This section provides basic usage instructions for the package.
+
+### Importing the package
+Rather than importing the base package, it is recommended that you import the primary `FreshPy` class using the syntax
+below.
+
+```python
+from freshpy import FreshPy
+```
+
+### Initializing a FreshPy object instance
+The primary `FreshPy` object serves many purposes, the most important being to establish a connection to the 
+Freshservice environment with which you intend to interact. As such, when initializing an instance of the `FreshPy` 
+object, you will need to pass it the Freshservice URL (e.g. `example.freshservice.com`) and the API key it will use 
+to authenticate so that the connection can be established.
+
+#### Passing the information directly into the object
+The domain and API key can be passed directly into the `FreshPy` object when initializing it, as
+demonstrated in the example below.
+
+```python
+fresh = FreshPy(domain='example.freshservice.com', api_key='abc123DEF456')
+```
+
+### Interacting with the Freshservice API
+Once the `FreshPy` object instance has been initialized, it can be leveraged to interact with a Freshservice
+environment in many ways, which is fully documented in the official
+[documentation](https://api.freshservice.com/). The example below demonstrates how information for a specific incident 
+ticket can be retrieved in JSON format.
+
+```python
+ticket_data = fresh.tickets.get_ticket(1299)
+```
+
+## License
+[MIT License](https://github.com/jeffshurtliff/freshpy/blob/master/LICENSE)
+
+## Changelog
+Refer to the [changelog](https://freshpy.readthedocs.io/en/latest/changelog.html) for version change information.
+
+## Reporting Issues
+Issues can be reported within the [GitHub repository](https://github.com/jeffshurtliff/freshpy/issues).
+
+## Additional Resources
+Additional resources for leveraging the Freshservice API can be found in the official
+[Freshservice API Reference Documentation](https://api.freshservice.com/).
+
+## Donations
+If you would like to donate to this project then you can do so using 
+[this PayPal link](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=XDZ8M6UV6EFK6&item_name=FreshPy&currency_code=USD).
+
+## Disclaimer
+This package is considered unofficial and is in no way endorsed or supported by 
+[Freshservice](https://www.freshservice.com).
+
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: freshpy Version: 1.1.0b1 Summary: A Python toolset
+Metadata-Version: 2.1 Name: freshpy Version: 1.1.1 Summary: A Python toolset
 for utilizing the Freshservice API Home-page: https://github.com/jeffshurtliff/
 freshpy Author: Jeff Shurtliff Author-email: jeff.shurtliff@rsa.com License:
 UNKNOWN Project-URL: Change Log, https://freshpy.readthedocs.io/en/latest/
 changelog.html Project-URL: Issue Tracker, https://github.com/jeffshurtliff/
 freshpy/issues Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
@@ -32,15 +32,15 @@
 ## Installation The package can be installed via pip using the syntax below.
 ```sh pip install freshpy --upgrade ``` You may also clone the repository and
 install from source using below. ```sh git clone git://github.com/
 jeffshurtliff/freshpy.git cd freshpy/ python setup.py install ``` ## Usage This
 section provides basic usage instructions for the package. ### Importing the
 package Rather than importing the base package, it is recommended that you
 import the primary `FreshPy` class using the syntax below. ```python from
-freshpy import FreshPy ``` ### Initializing a Khoros object instance The
+freshpy import FreshPy ``` ### Initializing a FreshPy object instance The
 primary `FreshPy` object serves many purposes, the most important being to
 establish a connection to the Freshservice environment with which you intend to
 interact. As such, when initializing an instance of the `FreshPy` object, you
 will need to pass it the Freshservice URL (e.g. `example.freshservice.com`) and
 the API key it will use to authenticate so that the connection can be
 established. #### Passing the information directly into the object The domain
 and API key can be passed directly into the `FreshPy` object when initializing
```

### Comparing `freshpy-1.1.0b1/README.md` & `freshpy-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     <tr>
         <td>Build Status</td>
         <td>
             N/A
             <!--
             <a href="https://github.com/jeffshurtliff/freshpy/blob/master/.github/workflows/pythonpackage.yml">
                 <img alt="GitHub Workflow Status" 
-                src="https://img.shields.io/github/workflow/status/jeffshurtliff/khoros/Python package">
+                src="https://img.shields.io/github/workflow/status/jeffshurtliff/freshpy/Python package">
             </a>
             -->
         </td>
     </tr>
     <tr>
         <td>Supported Versions</td>
         <td>
@@ -143,15 +143,15 @@
 Rather than importing the base package, it is recommended that you import the primary `FreshPy` class using the syntax
 below.
 
 ```python
 from freshpy import FreshPy
 ```
 
-### Initializing a Khoros object instance
+### Initializing a FreshPy object instance
 The primary `FreshPy` object serves many purposes, the most important being to establish a connection to the 
 Freshservice environment with which you intend to interact. As such, when initializing an instance of the `FreshPy` 
 object, you will need to pass it the Freshservice URL (e.g. `example.freshservice.com`) and the API key it will use 
 to authenticate so that the connection can be established.
 
 #### Passing the information directly into the object
 The domain and API key can be passed directly into the `FreshPy` object when initializing it, as
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 ## Installation The package can be installed via pip using the syntax below.
 ```sh pip install freshpy --upgrade ``` You may also clone the repository and
 install from source using below. ```sh git clone git://github.com/
 jeffshurtliff/freshpy.git cd freshpy/ python setup.py install ``` ## Usage This
 section provides basic usage instructions for the package. ### Importing the
 package Rather than importing the base package, it is recommended that you
 import the primary `FreshPy` class using the syntax below. ```python from
-freshpy import FreshPy ``` ### Initializing a Khoros object instance The
+freshpy import FreshPy ``` ### Initializing a FreshPy object instance The
 primary `FreshPy` object serves many purposes, the most important being to
 establish a connection to the Freshservice environment with which you intend to
 interact. As such, when initializing an instance of the `FreshPy` object, you
 will need to pass it the Freshservice URL (e.g. `example.freshservice.com`) and
 the API key it will use to authenticate so that the connection can be
 established. #### Passing the information directly into the object The domain
 and API key can be passed directly into the `FreshPy` object when initializing
```

### Comparing `freshpy-1.1.0b1/setup.py` & `freshpy-1.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-:Synopsis:          This script is the primary configuration file for the freshpy project
-:Created By:        Jeff Shurtliff
-:Last Modified:     Jeff Shurtliff
-:Modified Date:     04 Jan 2022
-"""
-
-import setuptools
-import codecs
-import os.path
-
-
-def read(rel_path):
-    """This function reads the ``version.py`` script in order to retrieve the version.
-
-    .. versionadded:: 1.0.0
-    """
-    here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
-        return fp.read()
-
-
-def get_version(rel_path):
-    """This function retrieves the current version of the package without needing to import the
-       :py:mod:`freshpy.utils.version` module in order to avoid dependency issues.
-
-    .. versionadded:: 1.0.0
-    """
-    for line in read(rel_path).splitlines():
-        if line.startswith('__version__'):
-            delimiter = '"' if '"' in line else "'"
-            return line.split(delimiter)[1]
-    raise RuntimeError("Unable to find the version string")
-
-
-with open('README.md', 'r') as fh:
-    long_description = fh.read()
-
-version = get_version('src/freshpy/utils/version.py')
-
-setuptools.setup(
-    name='freshpy',
-    version=version,
-    author='Jeff Shurtliff',
-    author_email='jeff.shurtliff@rsa.com',
-    description='A Python toolset for utilizing the Freshservice API',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/jeffshurtliff/freshpy",
-    project_urls={
-        'Change Log': 'https://freshpy.readthedocs.io/en/latest/changelog.html',
-        'Issue Tracker': 'https://github.com/jeffshurtliff/freshpy/issues',
-    },
-    package_dir={'': 'src'},
-    packages=setuptools.find_packages(where='src'),
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Environment :: Web Environment",
-        "Intended Audience :: Information Technology",
-        "Intended Audience :: System Administrators",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Topic :: Communications",
-        "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System",
-        "Topic :: Internet :: WWW/HTTP :: Site Management",
-        "Topic :: Office/Business",
-        "Topic :: Software Development :: Libraries :: Python Modules"
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-        "urllib3>=1.26.7",
-        "requests>=2.26.0",
-        "setuptools~=52.0.0"
-    ],
-    extras_require={
-        'sphinx': [
-            'Sphinx>=3.4.0',
-            'sphinxcontrib-applehelp>=1.0.2',
-            'sphinxcontrib-devhelp>=1.0.2',
-            'sphinxcontrib-htmlhelp>=1.0.3',
-            'sphinxcontrib-jsmath>=1.0.1',
-            'sphinxcontrib-qthelp>=1.0.3',
-            'sphinxcontrib-serializinghtml>=1.1.4'
-        ],
-    }
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""
+:Synopsis:          This script is the primary configuration file for the freshpy project
+:Created By:        Jeff Shurtliff
+:Last Modified:     Jeff Shurtliff
+:Modified Date:     08 May 2023
+"""
+
+import setuptools
+import codecs
+import os.path
+
+
+def read(rel_path):
+    """This function reads the ``version.py`` script in order to retrieve the version.
+
+    .. versionadded:: 1.0.0
+    """
+    here = os.path.abspath(os.path.dirname(__file__))
+    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+        return fp.read()
+
+
+def get_version(rel_path):
+    """This function retrieves the current version of the package without needing to import the
+       :py:mod:`freshpy.utils.version` module in order to avoid dependency issues.
+
+    .. versionadded:: 1.0.0
+    """
+    for line in read(rel_path).splitlines():
+        if line.startswith('__version__'):
+            delimiter = '"' if '"' in line else "'"
+            return line.split(delimiter)[1]
+    raise RuntimeError("Unable to find the version string")
+
+
+with open('README.md', 'r') as fh:
+    long_description = fh.read()
+
+version = get_version('src/freshpy/utils/version.py')
+
+setuptools.setup(
+    name='freshpy',
+    version=version,
+    author='Jeff Shurtliff',
+    author_email='jeff.shurtliff@rsa.com',
+    description='A Python toolset for utilizing the Freshservice API',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/jeffshurtliff/freshpy",
+    project_urls={
+        'Change Log': 'https://freshpy.readthedocs.io/en/latest/changelog.html',
+        'Issue Tracker': 'https://github.com/jeffshurtliff/freshpy/issues',
+    },
+    package_dir={'': 'src'},
+    packages=setuptools.find_packages(where='src'),
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Environment :: Web Environment",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: System Administrators",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Communications",
+        "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System",
+        "Topic :: Internet :: WWW/HTTP :: Site Management",
+        "Topic :: Office/Business",
+        "Topic :: Software Development :: Libraries :: Python Modules"
+    ],
+    python_requires='>=3.6',
+    install_requires=[
+        "urllib3>=1.26.7",
+        "requests>=2.23.0",
+        "setuptools>=52.0.0"
+    ],
+    extras_require={
+        'sphinx': [
+            'Sphinx>=3.4.0',
+            'sphinxcontrib-applehelp>=1.0.2',
+            'sphinxcontrib-devhelp>=1.0.2',
+            'sphinxcontrib-htmlhelp>=1.0.3',
+            'sphinxcontrib-jsmath>=1.0.1',
+            'sphinxcontrib-qthelp>=1.0.3',
+            'sphinxcontrib-serializinghtml>=1.1.4'
+        ],
+    }
+)
```

### Comparing `freshpy-1.1.0b1/src/freshpy/api.py` & `freshpy-1.1.1/src/freshpy/api.py`

 * *Files identical despite different names*

### Comparing `freshpy-1.1.0b1/src/freshpy/core.py` & `freshpy-1.1.1/src/freshpy/core.py`

 * *Files identical despite different names*

### Comparing `freshpy-1.1.0b1/src/freshpy/errors/exceptions.py` & `freshpy-1.1.1/src/freshpy/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `freshpy-1.1.0b1/src/freshpy/tickets.py` & `freshpy-1.1.1/src/freshpy/tickets.py`

 * *Files identical despite different names*

### Comparing `freshpy-1.1.0b1/src/freshpy/utils/core_utils.py` & `freshpy-1.1.1/src/freshpy/utils/core_utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# -*- coding: utf-8 -*-
-"""
-:Module:            freshpy.utils.core_utils
-:Synopsis:          Collection of supporting utilities and functions to complement the primary modules
-:Created By:        Jeff Shurtliff
-:Last Modified:     Jeff Shurtliff
-:Modified Date:     30 Dec 2021
-"""
-
-import urllib.parse
-
-
-def construct_query_string(existing_query=None, appendage=None):
-    """This function assists in constructing query strings for URIs to ensure they follow the appropriate format.
-
-    .. versionadded:: 1.0.0
-
-    :param existing_query: The existing query string (if any)
-    :type existing_query: str, None
-    :param appendage: The new addition to the query string to be appended (if any)
-    :type appendage: str, None
-    :returns: The constructed query string
-    """
-    combined_query = '' if existing_query is None else existing_query
-    if appendage:
-        if existing_query == '?':
-            combined_query = f'?{appendage}'
-        elif existing_query:
-            combined_query = existing_query + f'&{appendage}'
-        elif appendage.startswith('?'):
-            combined_query = appendage
-        else:
-            combined_query = f'?{appendage}'
-    return combined_query
-
-
-def url_encode(raw_string):
-    """This function encodes a string for use in URLs.
-
-    .. versionadded:: 1.0.0
-
-    :param raw_string: The raw string to be encoded
-    :type raw_string: str
-    :returns: The encoded string
-    """
-    return urllib.parse.quote_plus(raw_string)
-
-
-def url_decode(encoded_string):
-    """This function decodes a url-encoded string.
-
-    .. versionadded:: 1.0.0
-
-    :param encoded_string: The url-encoded string
-    :type encoded_string: str
-    :returns: The unencoded string
-    """
+# -*- coding: utf-8 -*-
+"""
+:Module:            freshpy.utils.core_utils
+:Synopsis:          Collection of supporting utilities and functions to complement the primary modules
+:Created By:        Jeff Shurtliff
+:Last Modified:     Jeff Shurtliff
+:Modified Date:     30 Dec 2021
+"""
+
+import urllib.parse
+
+
+def construct_query_string(existing_query=None, appendage=None):
+    """This function assists in constructing query strings for URIs to ensure they follow the appropriate format.
+
+    .. versionadded:: 1.0.0
+
+    :param existing_query: The existing query string (if any)
+    :type existing_query: str, None
+    :param appendage: The new addition to the query string to be appended (if any)
+    :type appendage: str, None
+    :returns: The constructed query string
+    """
+    combined_query = '' if existing_query is None else existing_query
+    if appendage:
+        if existing_query == '?':
+            combined_query = f'?{appendage}'
+        elif existing_query:
+            combined_query = existing_query + f'&{appendage}'
+        elif appendage.startswith('?'):
+            combined_query = appendage
+        else:
+            combined_query = f'?{appendage}'
+    return combined_query
+
+
+def url_encode(raw_string):
+    """This function encodes a string for use in URLs.
+
+    .. versionadded:: 1.0.0
+
+    :param raw_string: The raw string to be encoded
+    :type raw_string: str
+    :returns: The encoded string
+    """
+    return urllib.parse.quote_plus(raw_string)
+
+
+def url_decode(encoded_string):
+    """This function decodes a url-encoded string.
+
+    .. versionadded:: 1.0.0
+
+    :param encoded_string: The url-encoded string
+    :type encoded_string: str
+    :returns: The unencoded string
+    """
     return urllib.parse.unquote_plus(encoded_string)
```

### Comparing `freshpy-1.1.0b1/src/freshpy/utils/log_utils.py` & `freshpy-1.1.1/src/freshpy/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `freshpy-1.1.0b1/src/freshpy/utils/version.py` & `freshpy-1.1.1/src/freshpy/utils/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # -*- coding: utf-8 -*-
 """
 :Module:            freshpy.utils.version
 :Synopsis:          This simple script contains the package version
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     04 Jan 2022
+:Modified Date:     08 May 2023
 """
 
 from . import log_utils
 
 # Initialize logging
 logger = log_utils.initialize_logging(__name__)
 
 # Define special and global variables
-__version__ = "1.1.0b1"
+__version__ = "1.1.1"
 
 
 def get_full_version():
-    """This function returns the current full version of the ``freshpy`` package.
-
-    .. versionadded:: 1.0.0
-    """
+    """This function returns the current full version of the ``freshpy`` package."""
     return __version__
 
 
 def get_major_minor_version():
     """This function returns the current major.minor (i.e. X.Y) version of the ``freshpy`` package."""
     return ".".join(__version__.split(".")[:2])
```

### Comparing `freshpy-1.1.0b1/src/freshpy.egg-info/PKG-INFO` & `freshpy-1.1.1/src/freshpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-Metadata-Version: 2.1
-Name: freshpy
-Version: 1.1.0b1
-Summary: A Python toolset for utilizing the Freshservice API
-Home-page: https://github.com/jeffshurtliff/freshpy
-Author: Jeff Shurtliff
-Author-email: jeff.shurtliff@rsa.com
-License: UNKNOWN
-Project-URL: Change Log, https://freshpy.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/jeffshurtliff/freshpy/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Communications
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Office/Business
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: sphinx
-License-File: LICENSE
-
-<a href='https://pypi.org/project/freshpy/'>
-    <img src="https://github.com/jeffshurtliff/freshpy/blob/main/docs/_static/freshpy-logo.png" width="100" />
-</a>
-
-# FreshPy
-A Python toolset for utilizing the Freshservice API
-
-<table>
-    <tr>
-        <td>Latest Stable Release</td>
-        <td>
-            <a href='https://pypi.org/project/freshpy/'>
-                <img alt="PyPI" src="https://img.shields.io/pypi/v/freshpy">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td>Latest Dev/Beta/RC Release</td>
-        <td>
-            <a href='https://pypi.org/project/freshpy/#history'>
-                <img alt="PyPI" src="https://img.shields.io/badge/pypi-1.1.0b1-blue">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td>Build Status</td>
-        <td>
-            N/A
-            <!--
-            <a href="https://github.com/jeffshurtliff/freshpy/blob/master/.github/workflows/pythonpackage.yml">
-                <img alt="GitHub Workflow Status" 
-                src="https://img.shields.io/github/workflow/status/jeffshurtliff/khoros/Python package">
-            </a>
-            -->
-        </td>
-    </tr>
-    <tr>
-        <td>Supported Versions</td>
-        <td>
-            <a href='https://pypi.org/project/freshpy/'>
-                <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/freshpy">
-            </a>
-        </td>
-    </tr>
-    <!--
-    <tr>
-        <td>Code Coverage</td>
-        <td>
-            <a href="https://codecov.io/gh/jeffshurtliff/freshpy">
-                <img src="https://codecov.io/gh/jeffshurtliff/freshpy/branch/master/graph/badge.svg" />
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td>Code Quality (LGTM)</td>
-        <td>
-            <a href="https://lgtm.com/projects/g/jeffshurtliff/freshpy">
-            <img alt="LGTM Grade" src="https://img.shields.io/lgtm/grade/python/github/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td>CodeFactor Grade</td>
-        <td>
-            <a href="https://lgtm.com/projects/g/jeffshurtliff/freshpy">
-            <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-    -->
-    <tr>
-        <td>Documentation</td>
-        <td>
-            <a href='https://freshpy.readthedocs.io/en/latest/?badge=latest'>
-                <img src='https://readthedocs.org/projects/freshpy/badge/?version=latest' alt='Documentation Status' /><br />
-            </a>
-        </td>
-    </tr>
-    <!--
-    <tr>
-        <td>Security Audits</td>
-        <td>
-            <a href="https://github.com/marketplace/actions/python-security-check-using-bandit">
-                <img alt="Bandit" src="https://img.shields.io/badge/security-bandit-yellow.svg">
-            </a><br />
-            <a href="https://github.com/marketplace/actions/pycharm-python-security-scanner">
-                <img alt="PyCharm Security Scanner" src="https://img.shields.io/badge/security-pycharm%20security%20scanner-green">
-            </a>
-        </td>
-    </tr>
-    -->
-    <tr>
-        <td>License</td>
-        <td>
-            <a href="https://github.com/jeffshurtliff/freshpy/blob/master/LICENSE">
-                <img alt="License (GitHub)" src="https://img.shields.io/github/license/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td style="vertical-align: top;">Issues</td>
-        <td>
-            <a href="https://github.com/jeffshurtliff/freshpy/issues">
-                <img style="margin-bottom:5px;" alt="GitHub open issues" src="https://img.shields.io/github/issues-raw/jeffshurtliff/freshpy"><br />
-            </a>
-            <a href="https://github.com/jeffshurtliff/freshpy/issues">
-                <img alt="GitHub closed issues" src="https://img.shields.io/github/issues-closed-raw/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-    <tr>
-        <td style="vertical-align: top;">Pull Requests</td>
-        <td>
-            <a href="https://github.com/jeffshurtliff/freshpy/pulls">
-                <img style="margin-bottom:5px;" alt="GitHub pull open requests" src="https://img.shields.io/github/issues-pr-raw/jeffshurtliff/freshpy"><br />
-            </a>
-            <a href="https://github.com/jeffshurtliff/freshpy/pulls">
-                <img alt="GitHub closed pull requests" src="https://img.shields.io/github/issues-pr-closed-raw/jeffshurtliff/freshpy">
-            </a>
-        </td>
-    </tr>
-</table>
-
-## Installation
-The package can be installed via pip using the syntax below.
-
-```sh
-pip install freshpy --upgrade
-```
-
-You may also clone the repository and install from source using below.
-
-```sh
-git clone git://github.com/jeffshurtliff/freshpy.git
-cd freshpy/
-python setup.py install
-```
-
-## Usage
-This section provides basic usage instructions for the package.
-
-### Importing the package
-Rather than importing the base package, it is recommended that you import the primary `FreshPy` class using the syntax
-below.
-
-```python
-from freshpy import FreshPy
-```
-
-### Initializing a Khoros object instance
-The primary `FreshPy` object serves many purposes, the most important being to establish a connection to the 
-Freshservice environment with which you intend to interact. As such, when initializing an instance of the `FreshPy` 
-object, you will need to pass it the Freshservice URL (e.g. `example.freshservice.com`) and the API key it will use 
-to authenticate so that the connection can be established.
-
-#### Passing the information directly into the object
-The domain and API key can be passed directly into the `FreshPy` object when initializing it, as
-demonstrated in the example below.
-
-```python
-fresh = FreshPy(domain='example.freshservice.com', api_key='abc123DEF456')
-```
-
-### Interacting with the Freshservice API
-Once the `FreshPy` object instance has been initialized, it can be leveraged to interact with a Freshservice
-environment in many ways, which is fully documented in the official
-[documentation](https://api.freshservice.com/). The example below demonstrates how information for a specific incident 
-ticket can be retrieved in JSON format.
-
-```python
-ticket_data = fresh.tickets.get_ticket(1299)
-```
-
-## License
-[MIT License](https://github.com/jeffshurtliff/freshpy/blob/master/LICENSE)
-
-## Changelog
-Refer to the [changelog](https://freshpy.readthedocs.io/en/latest/changelog.html) for version change information.
-
-## Reporting Issues
-Issues can be reported within the [GitHub repository](https://github.com/jeffshurtliff/freshpy/issues).
-
-## Additional Resources
-Additional resources for leveraging the Freshservice API can be found in the official
-[Freshservice API Reference Documentation](https://api.freshservice.com/).
-
-## Donations
-If you would like to donate to this project then you can do so using 
-[this PayPal link](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=XDZ8M6UV6EFK6&item_name=FreshPy&currency_code=USD).
-
-## Disclaimer
-This package is considered unofficial and is in no way endorsed or supported by 
-[Freshservice](https://www.freshservice.com).
-
-
-
+Metadata-Version: 2.1
+Name: freshpy
+Version: 1.1.1
+Summary: A Python toolset for utilizing the Freshservice API
+Home-page: https://github.com/jeffshurtliff/freshpy
+Author: Jeff Shurtliff
+Author-email: jeff.shurtliff@rsa.com
+License: UNKNOWN
+Project-URL: Change Log, https://freshpy.readthedocs.io/en/latest/changelog.html
+Project-URL: Issue Tracker, https://github.com/jeffshurtliff/freshpy/issues
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Communications
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Office/Business
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: sphinx
+License-File: LICENSE
+
+<a href='https://pypi.org/project/freshpy/'>
+    <img src="https://github.com/jeffshurtliff/freshpy/blob/main/docs/_static/freshpy-logo.png" width="100" />
+</a>
+
+# FreshPy
+A Python toolset for utilizing the Freshservice API
+
+<table>
+    <tr>
+        <td>Latest Stable Release</td>
+        <td>
+            <a href='https://pypi.org/project/freshpy/'>
+                <img alt="PyPI" src="https://img.shields.io/pypi/v/freshpy">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td>Latest Dev/Beta/RC Release</td>
+        <td>
+            <a href='https://pypi.org/project/freshpy/#history'>
+                <img alt="PyPI" src="https://img.shields.io/badge/pypi-1.1.0b1-blue">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td>Build Status</td>
+        <td>
+            N/A
+            <!--
+            <a href="https://github.com/jeffshurtliff/freshpy/blob/master/.github/workflows/pythonpackage.yml">
+                <img alt="GitHub Workflow Status" 
+                src="https://img.shields.io/github/workflow/status/jeffshurtliff/freshpy/Python package">
+            </a>
+            -->
+        </td>
+    </tr>
+    <tr>
+        <td>Supported Versions</td>
+        <td>
+            <a href='https://pypi.org/project/freshpy/'>
+                <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/freshpy">
+            </a>
+        </td>
+    </tr>
+    <!--
+    <tr>
+        <td>Code Coverage</td>
+        <td>
+            <a href="https://codecov.io/gh/jeffshurtliff/freshpy">
+                <img src="https://codecov.io/gh/jeffshurtliff/freshpy/branch/master/graph/badge.svg" />
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td>Code Quality (LGTM)</td>
+        <td>
+            <a href="https://lgtm.com/projects/g/jeffshurtliff/freshpy">
+            <img alt="LGTM Grade" src="https://img.shields.io/lgtm/grade/python/github/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td>CodeFactor Grade</td>
+        <td>
+            <a href="https://lgtm.com/projects/g/jeffshurtliff/freshpy">
+            <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+    -->
+    <tr>
+        <td>Documentation</td>
+        <td>
+            <a href='https://freshpy.readthedocs.io/en/latest/?badge=latest'>
+                <img src='https://readthedocs.org/projects/freshpy/badge/?version=latest' alt='Documentation Status' /><br />
+            </a>
+        </td>
+    </tr>
+    <!--
+    <tr>
+        <td>Security Audits</td>
+        <td>
+            <a href="https://github.com/marketplace/actions/python-security-check-using-bandit">
+                <img alt="Bandit" src="https://img.shields.io/badge/security-bandit-yellow.svg">
+            </a><br />
+            <a href="https://github.com/marketplace/actions/pycharm-python-security-scanner">
+                <img alt="PyCharm Security Scanner" src="https://img.shields.io/badge/security-pycharm%20security%20scanner-green">
+            </a>
+        </td>
+    </tr>
+    -->
+    <tr>
+        <td>License</td>
+        <td>
+            <a href="https://github.com/jeffshurtliff/freshpy/blob/master/LICENSE">
+                <img alt="License (GitHub)" src="https://img.shields.io/github/license/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td style="vertical-align: top;">Issues</td>
+        <td>
+            <a href="https://github.com/jeffshurtliff/freshpy/issues">
+                <img style="margin-bottom:5px;" alt="GitHub open issues" src="https://img.shields.io/github/issues-raw/jeffshurtliff/freshpy"><br />
+            </a>
+            <a href="https://github.com/jeffshurtliff/freshpy/issues">
+                <img alt="GitHub closed issues" src="https://img.shields.io/github/issues-closed-raw/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+    <tr>
+        <td style="vertical-align: top;">Pull Requests</td>
+        <td>
+            <a href="https://github.com/jeffshurtliff/freshpy/pulls">
+                <img style="margin-bottom:5px;" alt="GitHub pull open requests" src="https://img.shields.io/github/issues-pr-raw/jeffshurtliff/freshpy"><br />
+            </a>
+            <a href="https://github.com/jeffshurtliff/freshpy/pulls">
+                <img alt="GitHub closed pull requests" src="https://img.shields.io/github/issues-pr-closed-raw/jeffshurtliff/freshpy">
+            </a>
+        </td>
+    </tr>
+</table>
+
+## Installation
+The package can be installed via pip using the syntax below.
+
+```sh
+pip install freshpy --upgrade
+```
+
+You may also clone the repository and install from source using below.
+
+```sh
+git clone git://github.com/jeffshurtliff/freshpy.git
+cd freshpy/
+python setup.py install
+```
+
+## Usage
+This section provides basic usage instructions for the package.
+
+### Importing the package
+Rather than importing the base package, it is recommended that you import the primary `FreshPy` class using the syntax
+below.
+
+```python
+from freshpy import FreshPy
+```
+
+### Initializing a FreshPy object instance
+The primary `FreshPy` object serves many purposes, the most important being to establish a connection to the 
+Freshservice environment with which you intend to interact. As such, when initializing an instance of the `FreshPy` 
+object, you will need to pass it the Freshservice URL (e.g. `example.freshservice.com`) and the API key it will use 
+to authenticate so that the connection can be established.
+
+#### Passing the information directly into the object
+The domain and API key can be passed directly into the `FreshPy` object when initializing it, as
+demonstrated in the example below.
+
+```python
+fresh = FreshPy(domain='example.freshservice.com', api_key='abc123DEF456')
+```
+
+### Interacting with the Freshservice API
+Once the `FreshPy` object instance has been initialized, it can be leveraged to interact with a Freshservice
+environment in many ways, which is fully documented in the official
+[documentation](https://api.freshservice.com/). The example below demonstrates how information for a specific incident 
+ticket can be retrieved in JSON format.
+
+```python
+ticket_data = fresh.tickets.get_ticket(1299)
+```
+
+## License
+[MIT License](https://github.com/jeffshurtliff/freshpy/blob/master/LICENSE)
+
+## Changelog
+Refer to the [changelog](https://freshpy.readthedocs.io/en/latest/changelog.html) for version change information.
+
+## Reporting Issues
+Issues can be reported within the [GitHub repository](https://github.com/jeffshurtliff/freshpy/issues).
+
+## Additional Resources
+Additional resources for leveraging the Freshservice API can be found in the official
+[Freshservice API Reference Documentation](https://api.freshservice.com/).
+
+## Donations
+If you would like to donate to this project then you can do so using 
+[this PayPal link](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=XDZ8M6UV6EFK6&item_name=FreshPy&currency_code=USD).
+
+## Disclaimer
+This package is considered unofficial and is in no way endorsed or supported by 
+[Freshservice](https://www.freshservice.com).
+
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: freshpy Version: 1.1.0b1 Summary: A Python toolset
+Metadata-Version: 2.1 Name: freshpy Version: 1.1.1 Summary: A Python toolset
 for utilizing the Freshservice API Home-page: https://github.com/jeffshurtliff/
 freshpy Author: Jeff Shurtliff Author-email: jeff.shurtliff@rsa.com License:
 UNKNOWN Project-URL: Change Log, https://freshpy.readthedocs.io/en/latest/
 changelog.html Project-URL: Issue Tracker, https://github.com/jeffshurtliff/
 freshpy/issues Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
@@ -32,15 +32,15 @@
 ## Installation The package can be installed via pip using the syntax below.
 ```sh pip install freshpy --upgrade ``` You may also clone the repository and
 install from source using below. ```sh git clone git://github.com/
 jeffshurtliff/freshpy.git cd freshpy/ python setup.py install ``` ## Usage This
 section provides basic usage instructions for the package. ### Importing the
 package Rather than importing the base package, it is recommended that you
 import the primary `FreshPy` class using the syntax below. ```python from
-freshpy import FreshPy ``` ### Initializing a Khoros object instance The
+freshpy import FreshPy ``` ### Initializing a FreshPy object instance The
 primary `FreshPy` object serves many purposes, the most important being to
 establish a connection to the Freshservice environment with which you intend to
 interact. As such, when initializing an instance of the `FreshPy` object, you
 will need to pass it the Freshservice URL (e.g. `example.freshservice.com`) and
 the API key it will use to authenticate so that the connection can be
 established. #### Passing the information directly into the object The domain
 and API key can be passed directly into the `FreshPy` object when initializing
```

### Comparing `freshpy-1.1.0b1/src/freshpy.egg-info/SOURCES.txt` & `freshpy-1.1.1/src/freshpy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/freshpy/__init__.py
 src/freshpy/api.py
 src/freshpy/core.py
 src/freshpy/tickets.py
```

