# Comparing `tmp/dinosaurs-1.0.0.tar.gz` & `tmp/dinosaurs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinosaurs-1.0.0.tar", last modified: Tue May  9 10:27:55 2023, max compression
+gzip compressed data, was "dinosaurs-2.0.0.tar", last modified: Tue May  9 10:57:25 2023, max compression
```

## Comparing `dinosaurs-1.0.0.tar` & `dinosaurs-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 hargy     (1000) hargy     (1000)        0 2023-05-09 10:27:55.855046 dinosaurs-1.0.0/
--rw-rw-r--   0 hargy     (1000) hargy     (1000)     1080 2023-05-09 10:19:39.000000 dinosaurs-1.0.0/LICENSE.txt
--rw-rw-r--   0 hargy     (1000) hargy     (1000)     1161 2023-05-09 10:27:55.855046 dinosaurs-1.0.0/PKG-INFO
--rw-rw-r--   0 hargy     (1000) hargy     (1000)       52 2023-05-09 10:18:11.000000 dinosaurs-1.0.0/README.md
--rw-rw-r--   0 hargy     (1000) hargy     (1000)       38 2023-05-09 10:27:55.855046 dinosaurs-1.0.0/setup.cfg
--rw-rw-r--   0 hargy     (1000) hargy     (1000)     7934 2023-05-09 10:27:19.000000 dinosaurs-1.0.0/setup.py
-drwxrwxr-x   0 hargy     (1000) hargy     (1000)        0 2023-05-09 10:27:55.855046 dinosaurs-1.0.0/src/
-drwxrwxr-x   0 hargy     (1000) hargy     (1000)        0 2023-05-09 10:27:55.855046 dinosaurs-1.0.0/src/dinosaurs.egg-info/
--rw-rw-r--   0 hargy     (1000) hargy     (1000)     1161 2023-05-09 10:27:55.000000 dinosaurs-1.0.0/src/dinosaurs.egg-info/PKG-INFO
--rw-rw-r--   0 hargy     (1000) hargy     (1000)      254 2023-05-09 10:27:55.000000 dinosaurs-1.0.0/src/dinosaurs.egg-info/SOURCES.txt
--rw-rw-r--   0 hargy     (1000) hargy     (1000)        1 2023-05-09 10:27:55.000000 dinosaurs-1.0.0/src/dinosaurs.egg-info/dependency_links.txt
--rw-rw-r--   0 hargy     (1000) hargy     (1000)       39 2023-05-09 10:27:55.000000 dinosaurs-1.0.0/src/dinosaurs.egg-info/entry_points.txt
--rw-rw-r--   0 hargy     (1000) hargy     (1000)       50 2023-05-09 10:27:55.000000 dinosaurs-1.0.0/src/dinosaurs.egg-info/requires.txt
--rw-rw-r--   0 hargy     (1000) hargy     (1000)        1 2023-05-09 10:27:55.000000 dinosaurs-1.0.0/src/dinosaurs.egg-info/top_level.txt
+drwxrwxr-x   0 hargy     (1000) hargy     (1000)        0 2023-05-09 10:57:25.606234 dinosaurs-2.0.0/
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)     1080 2023-05-09 10:19:39.000000 dinosaurs-2.0.0/LICENSE.txt
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)     1161 2023-05-09 10:57:25.606234 dinosaurs-2.0.0/PKG-INFO
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)       52 2023-05-09 10:18:11.000000 dinosaurs-2.0.0/README.md
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)       38 2023-05-09 10:57:25.606234 dinosaurs-2.0.0/setup.cfg
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)     7934 2023-05-09 10:54:05.000000 dinosaurs-2.0.0/setup.py
+drwxrwxr-x   0 hargy     (1000) hargy     (1000)        0 2023-05-09 10:57:25.602234 dinosaurs-2.0.0/src/
+drwxrwxr-x   0 hargy     (1000) hargy     (1000)        0 2023-05-09 10:57:25.606234 dinosaurs-2.0.0/src/dinosaurs.egg-info/
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)     1161 2023-05-09 10:57:25.000000 dinosaurs-2.0.0/src/dinosaurs.egg-info/PKG-INFO
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)      254 2023-05-09 10:57:25.000000 dinosaurs-2.0.0/src/dinosaurs.egg-info/SOURCES.txt
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)        1 2023-05-09 10:57:25.000000 dinosaurs-2.0.0/src/dinosaurs.egg-info/dependency_links.txt
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)       39 2023-05-09 10:57:25.000000 dinosaurs-2.0.0/src/dinosaurs.egg-info/entry_points.txt
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)       50 2023-05-09 10:57:25.000000 dinosaurs-2.0.0/src/dinosaurs.egg-info/requires.txt
+-rw-rw-r--   0 hargy     (1000) hargy     (1000)        1 2023-05-09 10:57:25.000000 dinosaurs-2.0.0/src/dinosaurs.egg-info/top_level.txt
```

### Comparing `dinosaurs-1.0.0/LICENSE.txt` & `dinosaurs-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dinosaurs-1.0.0/PKG-INFO` & `dinosaurs-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinosaurs
-Version: 1.0.0
+Version: 2.0.0
 Summary: A test package while printing dinosaurs
 Home-page: https://github.com/pypa/sampleproject
 Author: Nadav
 Author-email: author@example.com
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
```

### Comparing `dinosaurs-1.0.0/setup.py` & `dinosaurs-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     name="dinosaurs",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.0",  # Required
+    version="2.0.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A test package while printing dinosaurs",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `dinosaurs-1.0.0/src/dinosaurs.egg-info/PKG-INFO` & `dinosaurs-2.0.0/src/dinosaurs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinosaurs
-Version: 1.0.0
+Version: 2.0.0
 Summary: A test package while printing dinosaurs
 Home-page: https://github.com/pypa/sampleproject
 Author: Nadav
 Author-email: author@example.com
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
```

