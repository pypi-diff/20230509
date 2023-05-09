# Comparing `tmp/PyHarshit-0.0.1.tar.gz` & `tmp/PyHarshit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHarshit-0.0.1.tar", last modified: Tue May  9 10:38:35 2023, max compression
+gzip compressed data, was "PyHarshit-0.0.2.tar", last modified: Tue May  9 13:40:37 2023, max compression
```

## Comparing `PyHarshit-0.0.1.tar` & `PyHarshit-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 10:38:35.884178 PyHarshit-0.0.1/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      477 2023-05-09 10:38:35.884178 PyHarshit-0.0.1/PKG-INFO
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 10:38:35.884178 PyHarshit-0.0.1/PyHarshit/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-09 10:37:48.000000 PyHarshit-0.0.1/PyHarshit/__init__.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      170 2023-05-09 10:37:48.000000 PyHarshit-0.0.1/PyHarshit/anim.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       19 2023-05-09 10:37:48.000000 PyHarshit-0.0.1/PyHarshit/boolset.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      106 2023-05-09 10:37:48.000000 PyHarshit-0.0.1/PyHarshit/charset.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      313 2023-05-09 10:37:48.000000 PyHarshit-0.0.1/PyHarshit/maths.py
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 10:38:35.884178 PyHarshit-0.0.1/PyHarshit.egg-info/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      477 2023-05-09 10:38:35.000000 PyHarshit-0.0.1/PyHarshit.egg-info/PKG-INFO
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      251 2023-05-09 10:38:35.000000 PyHarshit-0.0.1/PyHarshit.egg-info/SOURCES.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-09 10:38:35.000000 PyHarshit-0.0.1/PyHarshit.egg-info/dependency_links.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       10 2023-05-09 10:38:35.000000 PyHarshit-0.0.1/PyHarshit.egg-info/top_level.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      263 2023-05-09 10:37:48.000000 PyHarshit-0.0.1/README.md
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       38 2023-05-09 10:38:35.884178 PyHarshit-0.0.1/setup.cfg
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      545 2023-05-09 10:37:48.000000 PyHarshit-0.0.1/setup.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 13:40:37.730635 PyHarshit-0.0.2/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      669 2023-05-09 13:40:37.730635 PyHarshit-0.0.2/PKG-INFO
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 13:40:37.730635 PyHarshit-0.0.2/PyHarshit/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/PyHarshit/__init__.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      170 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/PyHarshit/anim.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       19 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/PyHarshit/boolset.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      106 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/PyHarshit/charset.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      313 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/PyHarshit/maths.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      305 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/PyHarshit/tools.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      588 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/PyHarshit/utils.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 13:40:37.730635 PyHarshit-0.0.2/PyHarshit.egg-info/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      669 2023-05-09 13:40:37.000000 PyHarshit-0.0.2/PyHarshit.egg-info/PKG-INFO
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      321 2023-05-09 13:40:37.000000 PyHarshit-0.0.2/PyHarshit.egg-info/SOURCES.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-09 13:40:37.000000 PyHarshit-0.0.2/PyHarshit.egg-info/dependency_links.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        5 2023-05-09 13:40:37.000000 PyHarshit-0.0.2/PyHarshit.egg-info/requires.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       10 2023-05-09 13:40:37.000000 PyHarshit-0.0.2/PyHarshit.egg-info/top_level.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      455 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/README.md
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       38 2023-05-09 13:40:37.730635 PyHarshit-0.0.2/setup.cfg
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      545 2023-05-09 13:38:44.000000 PyHarshit-0.0.2/setup.py
```

### Comparing `PyHarshit-0.0.1/setup.py` & `PyHarshit-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     page_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="PyHarshit",
-    version="0.0.1",
+    version="0.0.2",
     author="Harshit Shrivastav",
     author_email="itsharshit@yandex.com",
     description="Utlity file for my codes",
     long_description=page_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
```

