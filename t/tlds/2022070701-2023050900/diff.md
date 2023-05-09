# Comparing `tmp/tlds-2022070701.tar.gz` & `tmp/tlds-2023050900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tlds-2022070701.tar", last modified: Fri Jul  8 17:39:34 2022, max compression
+gzip compressed data, was "tlds-2023050900.tar", last modified: Tue May  9 21:19:57 2023, max compression
```

## Comparing `tlds-2022070701.tar` & `tlds-2023050900.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-08 17:39:34.000000 tlds-2022070701/
--rw-r--r--   0 runner    (1001) docker     (116)     1667 2022-07-08 17:39:34.000000 tlds-2022070701/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-07-08 17:39:34.000000 tlds-2022070701/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-08 17:39:34.000000 tlds-2022070701/tlds/
--rw-r--r--   0 runner    (1001) docker     (116)       21 2022-07-08 17:39:29.000000 tlds-2022070701/tlds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      928 2022-07-08 17:39:29.000000 tlds-2022070701/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1688 2022-07-08 17:39:29.000000 tlds-2022070701/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-08 17:39:34.000000 tlds-2022070701/tlds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1667 2022-07-08 17:39:34.000000 tlds-2022070701/tlds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      181 2022-07-08 17:39:34.000000 tlds-2022070701/tlds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-08 17:39:34.000000 tlds-2022070701/tlds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-08 17:39:34.000000 tlds-2022070701/tlds.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        5 2022-07-08 17:39:34.000000 tlds-2022070701/tlds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:57.414707 tlds-2023050900/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-09 21:19:51.000000 tlds-2023050900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-09 21:19:57.414707 tlds-2023050900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-09 21:19:51.000000 tlds-2023050900/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 21:19:57.414707 tlds-2023050900/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-09 21:19:51.000000 tlds-2023050900/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:57.410706 tlds-2023050900/tlds/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 21:19:51.000000 tlds-2023050900/tlds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-09 21:19:51.000000 tlds-2023050900/tlds/_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:57.414707 tlds-2023050900/tlds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:19:57.000000 tlds-2023050900/tlds.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tlds-2022070701/PKG-INFO` & `tlds-2023050900/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tlds
-Version: 2022070701
+Version: 2023050900
 Summary: Automatically updated list of valid TLDs taken directly from IANA
 Home-page: https://github.com/kichik/tlds
 Author: Amir Szekely
 Author-email: kichik@gmail.com
 License: MIT
-Description: ###################################################
-        Automatically updated list of valid TLDs for Python
-        ###################################################
-        
-        The `tlds` module provides a a set of valid TLDs directly taken from IANA_. The package is automatically updated daily.
-        
-        Available on PyPI_.
-        
-        .. _IANA: http://data.iana.org/TLD/tlds-alpha-by-domain.txt
-        .. _PyPI: https://pypi.org/pypi/tlds/
-        
-        .. image:: https://github.com/kichik/tlds/workflows/tlds%20build/badge.svg
-           :alt: Build status
-           :target: https://github.com/kichik/tlds/actions
-        
-        .. image:: https://img.shields.io/pypi/v/tlds?logo=pypi
-           :alt: PyPI
-           :target: https://pypi.org/pypi/tlds/
-        
-        .. image:: https://img.shields.io/pypi/dm/tlds?color=red
-           :alt: PyPI - Downloads
-           :target: https://pypi.org/pypi/tlds/
-        
-        Usage
-        -----
-        
-          >>> from tlds import tld_set
-          >>> 'com' in tld_set
-          True
-          >>> 'foobar' in tld_set
-          False
-          >>> 'pizza' in tld_set
-          True
-          >>>
-        
 Keywords: tld
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications
+License-File: LICENSE
+
+###################################################
+Automatically updated list of valid TLDs for Python
+###################################################
+
+The `tlds` module provides a a set of valid TLDs directly taken from IANA_. The package is automatically updated daily.
+
+Available on PyPI_.
+
+.. _IANA: http://data.iana.org/TLD/tlds-alpha-by-domain.txt
+.. _PyPI: https://pypi.org/pypi/tlds/
+
+.. image:: https://github.com/kichik/tlds/workflows/tlds%20build/badge.svg
+   :alt: Build status
+   :target: https://github.com/kichik/tlds/actions
+
+.. image:: https://img.shields.io/pypi/v/tlds?logo=pypi
+   :alt: PyPI
+   :target: https://pypi.org/pypi/tlds/
+
+.. image:: https://img.shields.io/pypi/dm/tlds?color=red
+   :alt: PyPI - Downloads
+   :target: https://pypi.org/pypi/tlds/
+
+Usage
+-----
+
+  >>> from tlds import tld_set
+  >>> 'com' in tld_set
+  True
+  >>> 'foobar' in tld_set
+  False
+  >>> 'pizza' in tld_set
+  True
+  >>>
```

### Comparing `tlds-2022070701/README.rst` & `tlds-2023050900/README.rst`

 * *Files identical despite different names*

### Comparing `tlds-2022070701/tlds.egg-info/PKG-INFO` & `tlds-2023050900/tlds.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tlds
-Version: 2022070701
+Version: 2023050900
 Summary: Automatically updated list of valid TLDs taken directly from IANA
 Home-page: https://github.com/kichik/tlds
 Author: Amir Szekely
 Author-email: kichik@gmail.com
 License: MIT
-Description: ###################################################
-        Automatically updated list of valid TLDs for Python
-        ###################################################
-        
-        The `tlds` module provides a a set of valid TLDs directly taken from IANA_. The package is automatically updated daily.
-        
-        Available on PyPI_.
-        
-        .. _IANA: http://data.iana.org/TLD/tlds-alpha-by-domain.txt
-        .. _PyPI: https://pypi.org/pypi/tlds/
-        
-        .. image:: https://github.com/kichik/tlds/workflows/tlds%20build/badge.svg
-           :alt: Build status
-           :target: https://github.com/kichik/tlds/actions
-        
-        .. image:: https://img.shields.io/pypi/v/tlds?logo=pypi
-           :alt: PyPI
-           :target: https://pypi.org/pypi/tlds/
-        
-        .. image:: https://img.shields.io/pypi/dm/tlds?color=red
-           :alt: PyPI - Downloads
-           :target: https://pypi.org/pypi/tlds/
-        
-        Usage
-        -----
-        
-          >>> from tlds import tld_set
-          >>> 'com' in tld_set
-          True
-          >>> 'foobar' in tld_set
-          False
-          >>> 'pizza' in tld_set
-          True
-          >>>
-        
 Keywords: tld
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications
+License-File: LICENSE
+
+###################################################
+Automatically updated list of valid TLDs for Python
+###################################################
+
+The `tlds` module provides a a set of valid TLDs directly taken from IANA_. The package is automatically updated daily.
+
+Available on PyPI_.
+
+.. _IANA: http://data.iana.org/TLD/tlds-alpha-by-domain.txt
+.. _PyPI: https://pypi.org/pypi/tlds/
+
+.. image:: https://github.com/kichik/tlds/workflows/tlds%20build/badge.svg
+   :alt: Build status
+   :target: https://github.com/kichik/tlds/actions
+
+.. image:: https://img.shields.io/pypi/v/tlds?logo=pypi
+   :alt: PyPI
+   :target: https://pypi.org/pypi/tlds/
+
+.. image:: https://img.shields.io/pypi/dm/tlds?color=red
+   :alt: PyPI - Downloads
+   :target: https://pypi.org/pypi/tlds/
+
+Usage
+-----
+
+  >>> from tlds import tld_set
+  >>> 'com' in tld_set
+  True
+  >>> 'foobar' in tld_set
+  False
+  >>> 'pizza' in tld_set
+  True
+  >>>
```

