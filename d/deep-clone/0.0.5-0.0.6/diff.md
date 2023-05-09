# Comparing `tmp/deep-clone-0.0.5.tar.gz` & `tmp/deep-clone-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep-clone-0.0.5.tar", last modified: Wed May  3 17:48:13 2023, max compression
+gzip compressed data, was "deep-clone-0.0.6.tar", last modified: Tue May  9 09:21:36 2023, max compression
```

## Comparing `deep-clone-0.0.5.tar` & `deep-clone-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:48:13.479968 deep-clone-0.0.5/
--rw-rw-rw-   0        0        0     1092 2023-05-03 14:09:43.000000 deep-clone-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      918 2023-05-03 17:48:13.478964 deep-clone-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-05-03 14:08:07.000000 deep-clone-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 17:48:13.477974 deep-clone-0.0.5/deep_clone.egg-info/
--rw-rw-rw-   0        0        0      918 2023-05-03 17:48:13.000000 deep-clone-0.0.5/deep_clone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-05-03 17:48:13.000000 deep-clone-0.0.5/deep_clone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:48:13.000000 deep-clone-0.0.5/deep_clone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-03 17:48:13.000000 deep-clone-0.0.5/deep_clone.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 17:48:13.000000 deep-clone-0.0.5/deep_clone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 17:48:13.480961 deep-clone-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-03 17:47:43.000000 deep-clone-0.0.5/setup.py
+drwxrwxrwx   0 rajan     (1000) rajan     (1000)        0 2023-05-09 09:21:36.323710 deep-clone-0.0.6/
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)     1092 2023-05-03 14:09:43.000000 deep-clone-0.0.6/LICENSE
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)      882 2023-05-09 09:21:36.317706 deep-clone-0.0.6/PKG-INFO
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)      422 2023-05-03 14:08:07.000000 deep-clone-0.0.6/README.md
+drwxrwxrwx   0 rajan     (1000) rajan     (1000)        0 2023-05-09 09:21:36.288342 deep-clone-0.0.6/deep_clone.egg-info/
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)      882 2023-05-09 09:21:35.000000 deep-clone-0.0.6/deep_clone.egg-info/PKG-INFO
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)      199 2023-05-09 09:21:35.000000 deep-clone-0.0.6/deep_clone.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)        1 2023-05-09 09:21:35.000000 deep-clone-0.0.6/deep_clone.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)       53 2023-05-09 09:21:35.000000 deep-clone-0.0.6/deep_clone.egg-info/entry_points.txt
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)       11 2023-05-09 09:21:35.000000 deep-clone-0.0.6/deep_clone.egg-info/top_level.txt
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)       38 2023-05-09 09:21:36.325709 deep-clone-0.0.6/setup.cfg
+-rwxrwxrwx   0 rajan     (1000) rajan     (1000)      739 2023-05-09 09:18:48.000000 deep-clone-0.0.6/setup.py
```

### Comparing `deep-clone-0.0.5/LICENSE` & `deep-clone-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deep-clone-0.0.5/PKG-INFO` & `deep-clone-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: deep-clone
-Version: 0.0.5
-Summary: Deep clone specific folder from a GitHub repo
-Home-page: https://github.com/rajan-personal/deep-clone
-Author: Rajan Gupta
-Author-email: 96rajangupta@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Deep Clone GitHub Repo - Readme
-
-This repository contains a Python script for deep cloning a specific folder within a GitHub repository, rather than cloning the entire repository.
-
-## Features
-
-- Deep clone a specific folder within a GitHub repository
-- Must specify a specific branch
-- Lightweight cloning, only retrieves the required folder
-
-## Requirements
-
-- Python 3.6 or later
-- Git
-
-## Usage
-
-deep_clone url dir
-
-
-
+Metadata-Version: 2.1
+Name: deep-clone
+Version: 0.0.6
+Summary: Deep clone specific folder from a GitHub repo
+Home-page: https://github.com/rajan-personal/deep-clone
+Author: Rajan Gupta
+Author-email: 96rajangupta@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Deep Clone GitHub Repo - Readme
+
+This repository contains a Python script for deep cloning a specific folder within a GitHub repository, rather than cloning the entire repository.
+
+## Features
+
+- Deep clone a specific folder within a GitHub repository
+- Must specify a specific branch
+- Lightweight cloning, only retrieves the required folder
+
+## Requirements
+
+- Python 3.6 or later
+- Git
+
+## Usage
+
+deep_clone url dir
+
+
+
```

### Comparing `deep-clone-0.0.5/deep_clone.egg-info/PKG-INFO` & `deep-clone-0.0.6/deep_clone.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: deep-clone
-Version: 0.0.5
-Summary: Deep clone specific folder from a GitHub repo
-Home-page: https://github.com/rajan-personal/deep-clone
-Author: Rajan Gupta
-Author-email: 96rajangupta@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Deep Clone GitHub Repo - Readme
-
-This repository contains a Python script for deep cloning a specific folder within a GitHub repository, rather than cloning the entire repository.
-
-## Features
-
-- Deep clone a specific folder within a GitHub repository
-- Must specify a specific branch
-- Lightweight cloning, only retrieves the required folder
-
-## Requirements
-
-- Python 3.6 or later
-- Git
-
-## Usage
-
-deep_clone url dir
-
-
-
+Metadata-Version: 2.1
+Name: deep-clone
+Version: 0.0.6
+Summary: Deep clone specific folder from a GitHub repo
+Home-page: https://github.com/rajan-personal/deep-clone
+Author: Rajan Gupta
+Author-email: 96rajangupta@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Deep Clone GitHub Repo - Readme
+
+This repository contains a Python script for deep cloning a specific folder within a GitHub repository, rather than cloning the entire repository.
+
+## Features
+
+- Deep clone a specific folder within a GitHub repository
+- Must specify a specific branch
+- Lightweight cloning, only retrieves the required folder
+
+## Requirements
+
+- Python 3.6 or later
+- Git
+
+## Usage
+
+deep_clone url dir
+
+
+
```

### Comparing `deep-clone-0.0.5/setup.py` & `deep-clone-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="deep-clone",
-    version="0.0.5",
+    version="0.0.6",
     py_modules=["deep-clone"],
     install_requires=[],
     entry_points={
         "console_scripts": [
-            "deepclone=deepclone.main:main",
+            "deep-clone=deep_clone.main:main",
         ],
     },
     author="Rajan Gupta",
     author_email="96rajangupta@gmail.com",
     description="Deep clone specific folder from a GitHub repo",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

