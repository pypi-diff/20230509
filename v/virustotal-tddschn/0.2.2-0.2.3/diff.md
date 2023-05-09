# Comparing `tmp/virustotal-tddschn-0.2.2.tar.gz` & `tmp/virustotal_tddschn-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virustotal-tddschn-0.2.2.tar", max compression
+gzip compressed data, was "virustotal_tddschn-0.2.3.tar", max compression
```

## Comparing `virustotal-tddschn-0.2.2.tar` & `virustotal_tddschn-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1100 2022-06-01 16:22:09.734805 virustotal-tddschn-0.2.2/LICENSE
--rw-r--r--   0        0        0     4512 2022-11-27 06:02:48.621753 virustotal-tddschn-0.2.2/README.md
--rw-r--r--   0        0        0      883 2022-11-27 06:14:16.468831 virustotal-tddschn-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2022-11-27 06:14:16.469378 virustotal-tddschn-0.2.2/virustotal_tddschn/__init__.py
--rw-r--r--   0        0        0     4848 2022-09-26 12:11:15.271283 virustotal-tddschn-0.2.2/virustotal_tddschn/brew_utils.py
--rw-r--r--   0        0        0      179 2022-06-02 09:22:55.530544 virustotal-tddschn-0.2.2/virustotal_tddschn/config.py
--rw-r--r--   0        0        0      540 2022-06-02 09:21:18.978953 virustotal-tddschn-0.2.2/virustotal_tddschn/hashing.py
--rw-r--r--   0        0        0      295 2022-09-26 11:56:31.959546 virustotal-tddschn-0.2.2/virustotal_tddschn/types.py
--rw-r--r--   0        0        0     1980 2022-09-26 09:26:01.327023 virustotal-tddschn-0.2.2/virustotal_tddschn/utils.py
--rwxr-xr-x   0        0        0     6089 2022-09-26 12:03:19.167871 virustotal-tddschn-0.2.2/virustotal_tddschn/virustotal_sum_search.py
--rw-r--r--   0        0        0     5382 1970-01-01 00:00:00.000000 virustotal-tddschn-0.2.2/setup.py
--rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 virustotal-tddschn-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-09 01:16:41.518965 virustotal_tddschn-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4512 2023-05-09 01:16:41.520275 virustotal_tddschn-0.2.3/README.md
+-rw-r--r--   0        0        0      918 2023-05-09 01:21:11.599708 virustotal_tddschn-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-09 01:21:11.600144 virustotal_tddschn-0.2.3/virustotal_tddschn/__init__.py
+-rw-r--r--   0        0        0     4848 2023-05-09 01:16:41.523977 virustotal_tddschn-0.2.3/virustotal_tddschn/brew_utils.py
+-rw-r--r--   0        0        0      302 2023-05-09 01:16:41.524135 virustotal_tddschn-0.2.3/virustotal_tddschn/config.py
+-rw-r--r--   0        0        0      540 2023-05-09 01:16:41.524317 virustotal_tddschn-0.2.3/virustotal_tddschn/hashing.py
+-rw-r--r--   0        0        0      295 2023-05-09 01:16:41.524483 virustotal_tddschn-0.2.3/virustotal_tddschn/types.py
+-rw-r--r--   0        0        0     2522 2023-05-09 01:19:27.348507 virustotal_tddschn-0.2.3/virustotal_tddschn/utils.py
+-rwxr-xr-x   0        0        0     6112 2023-05-09 01:19:53.085796 virustotal_tddschn-0.2.3/virustotal_tddschn/virustotal_sum_search.py
+-rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 virustotal_tddschn-0.2.3/PKG-INFO
```

### Comparing `virustotal-tddschn-0.2.2/LICENSE` & `virustotal_tddschn-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `virustotal-tddschn-0.2.2/README.md` & `virustotal_tddschn-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `virustotal-tddschn-0.2.2/pyproject.toml` & `virustotal_tddschn-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virustotal-tddschn"
-version = "0.2.2"
+version = "0.2.3"
 description = "VirusTotal Utility Scripts"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/virustotal-tddschn"
 repository = "https://github.com/tddschn/virustotal-tddschn"
 classifiers = ["Topic :: Utilities"]
@@ -16,18 +16,20 @@
 [tool.poetry.scripts]
 vtpy = "virustotal_tddschn.virustotal_sum_search:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/virustotal-tddschn/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
+vt-py = "^0.17.3"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.5.0"
 pytest = "^7.2.0"
 black = "^22.3.0"
 better-exceptions = "^0.3.3"
+rich = "^12.6.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `virustotal-tddschn-0.2.2/virustotal_tddschn/brew_utils.py` & `virustotal_tddschn-0.2.3/virustotal_tddschn/brew_utils.py`

 * *Files identical despite different names*

### Comparing `virustotal-tddschn-0.2.2/virustotal_tddschn/hashing.py` & `virustotal_tddschn-0.2.3/virustotal_tddschn/hashing.py`

 * *Files identical despite different names*

### Comparing `virustotal-tddschn-0.2.2/virustotal_tddschn/virustotal_sum_search.py` & `virustotal_tddschn-0.2.3/virustotal_tddschn/virustotal_sum_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,16 @@
     parser.add_argument(
         '-b',
         '--browser',
         help='Browser to open URLs',
         metavar='browser',
         type=str,
         choices=list(browser_str_to_app_name_map),
-        default='chrome',
+        # default='chrome',
+        default=None
     )
 
     parser.add_argument(
         '-B', '--no-browser', help='Do not open URLs in a browser', action='store_true'
     )
 
     if not brew_related_options_only:
```

### Comparing `virustotal-tddschn-0.2.2/PKG-INFO` & `virustotal_tddschn-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: virustotal-tddschn
-Version: 0.2.2
+Version: 0.2.3
 Summary: VirusTotal Utility Scripts
 Home-page: https://github.com/tddschn/virustotal-tddschn
 License: MIT
 Keywords: virustotal
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
+Requires-Dist: vt-py (>=0.17.3,<0.18.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/virustotal-tddschn/issues
 Project-URL: Repository, https://github.com/tddschn/virustotal-tddschn
 Description-Content-Type: text/markdown
 
 # VirusTotal Utility Library and Command Line Tools
 
 - [VirusTotal Utility Library and Command Line Tools](#virustotal-utility-library-and-command-line-tools)
```

