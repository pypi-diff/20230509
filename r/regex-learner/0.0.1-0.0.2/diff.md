# Comparing `tmp/regex-learner-0.0.1.tar.gz` & `tmp/regex-learner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-learner-0.0.1.tar", last modified: Tue May  9 10:55:22 2023, max compression
+gzip compressed data, was "regex-learner-0.0.2.tar", last modified: Tue May  9 12:46:27 2023, max compression
```

## Comparing `regex-learner-0.0.1.tar` & `regex-learner-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:55:22.091529 regex-learner-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 10:55:08.000000 regex-learner-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-09 10:55:22.091529 regex-learner-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-09 10:55:08.000000 regex-learner-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:55:22.091529 regex-learner-0.0.1/regex_learner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-09 10:55:22.000000 regex-learner-0.0.1/regex_learner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-09 10:55:22.000000 regex-learner-0.0.1/regex_learner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:55:22.000000 regex-learner-0.0.1/regex_learner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 10:55:22.000000 regex-learner-0.0.1/regex_learner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 10:55:22.000000 regex-learner-0.0.1/regex_learner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-09 10:55:22.095529 regex-learner-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-09 10:55:08.000000 regex-learner-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-05-09 10:55:08.000000 regex-learner-0.0.1/xsystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:46:27.588833 regex-learner-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 12:46:03.000000 regex-learner-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-09 12:46:27.588833 regex-learner-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-09 12:46:03.000000 regex-learner-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:46:27.588833 regex-learner-0.0.2/regex_learner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-09 12:46:27.000000 regex-learner-0.0.2/regex_learner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-09 12:46:27.000000 regex-learner-0.0.2/regex_learner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:46:27.000000 regex-learner-0.0.2/regex_learner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 12:46:27.000000 regex-learner-0.0.2/regex_learner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 12:46:27.000000 regex-learner-0.0.2/regex_learner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-09 12:46:27.588833 regex-learner-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-09 12:46:03.000000 regex-learner-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-05-09 12:46:03.000000 regex-learner-0.0.2/xsystem.py
```

### Comparing `regex-learner-0.0.1/LICENSE` & `regex-learner-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `regex-learner-0.0.1/PKG-INFO` & `regex-learner-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-learner
-Version: 0.0.1
+Version: 0.0.2
 Summary: The project provides a tool/library implementing an automated regular expression building mechanism.
 Home-page: https://github.com/IBM/regex-learner
 Author: Stefano Braghin, Liubov Nedoshivina
 Author-email: "Liubov Nedoshivia" <liubov.nedoshivina@ibm.com>
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `regex-learner-0.0.1/README.md` & `regex-learner-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `regex-learner-0.0.1/regex_learner.egg-info/PKG-INFO` & `regex-learner-0.0.2/regex_learner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-learner
-Version: 0.0.1
+Version: 0.0.2
 Summary: The project provides a tool/library implementing an automated regular expression building mechanism.
 Home-page: https://github.com/IBM/regex-learner
 Author: Stefano Braghin, Liubov Nedoshivina
 Author-email: "Liubov Nedoshivia" <liubov.nedoshivina@ibm.com>
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `regex-learner-0.0.1/setup.cfg` & `regex-learner-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = regex-learner
-version = 0.0.1
+version = 0.0.2
 description = The project provides a tool/library implementing an automated regular expression building mechanism.
 author = Stefano Braghin, Liubov Nedoshivina
 author_email = "Liubov Nedoshivia" <liubov.nedoshivina@ibm.com>
 long_description = long_description
 long_description_content_type = text/markdown
 url = https://github.com/IBM/regex-learner
 license = Apache License 2.0
```

### Comparing `regex-learner-0.0.1/xsystem.py` & `regex-learner-0.0.2/xsystem.py`

 * *Files identical despite different names*

