# Comparing `tmp/botcity-framework-core-1.1.0.tar.gz` & `tmp/botcity-framework-core-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/botcity-framework-core-python/botcity-framework-core-python/dist/.tmp-c8bcn57k/botcity-framework-core-1.1.0.t", last modified: Thu Mar 23 19:13:20 2023, max compression
+gzip compressed data, was "/home/runner/work/botcity-framework-core-python/botcity-framework-core-python/dist/.tmp-eiumycgb/botcity-framework-core-1.1.1.t", last modified: Tue May  9 21:27:55 2023, max compression
```

## Comparing `botcity-framework-core-1.1.0.tar` & `botcity-framework-core-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity/core/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity/core/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity/core/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/application/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/application/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    54451 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/cv2find.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/os_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/botcity/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity_framework_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity_framework_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity_framework_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity_framework_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity_framework_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/botcity_framework_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-23 19:13:20.000000 botcity-framework-core-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-03-23 19:13:06.000000 botcity-framework-core-1.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/core/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/core/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/application/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/application/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54451 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/cv2find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/os_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/botcity/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/botcity_framework_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-09 21:27:55.000000 botcity-framework-core-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-09 21:27:44.000000 botcity-framework-core-1.1.1/versioneer.py
```

### Comparing `botcity-framework-core-1.1.0/LICENSE` & `botcity-framework-core-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/PKG-INFO` & `botcity-framework-core-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-framework-core
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://www.github.com/botcity-dev/botcity-framework-core-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <h1 align="center">BotCity Framework Core - Python</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botcity-framework-core Version: 1.1.0 Home-page:
+Metadata-Version: 2.1 Name: botcity-framework-core Version: 1.1.1 Home-page:
 https://www.github.com/botcity-dev/botcity-framework-core-python Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                  ****** BotCity Framework Core - Python ******
                          Â« Explore Framework docs Â»
 
 ## Summary  - [ð¤ Computer-vision based UI Automation](#-computer-vision-
 based-ui-automation) - [ð Generate Python Code while Interacting with your
```

### Comparing `botcity-framework-core-1.1.0/README.md` & `botcity-framework-core-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/botcity/core/application/functions.py` & `botcity-framework-core-1.1.1/botcity/core/application/functions.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/botcity/core/application/utils.py` & `botcity-framework-core-1.1.1/botcity/core/application/utils.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/botcity/core/bot.py` & `botcity-framework-core-1.1.1/botcity/core/bot.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/botcity/core/cv2find.py` & `botcity-framework-core-1.1.1/botcity/core/cv2find.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/botcity/core/input_utils.py` & `botcity-framework-core-1.1.1/botcity/core/input_utils.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/botcity/core/os_compat.py` & `botcity-framework-core-1.1.1/botcity/core/os_compat.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/botcity_framework_core.egg-info/PKG-INFO` & `botcity-framework-core-1.1.1/botcity_framework_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-framework-core
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://www.github.com/botcity-dev/botcity-framework-core-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <h1 align="center">BotCity Framework Core - Python</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botcity-framework-core Version: 1.1.0 Home-page:
+Metadata-Version: 2.1 Name: botcity-framework-core Version: 1.1.1 Home-page:
 https://www.github.com/botcity-dev/botcity-framework-core-python Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                  ****** BotCity Framework Core - Python ******
                          Â« Explore Framework docs Â»
 
 ## Summary  - [ð¤ Computer-vision based UI Automation](#-computer-vision-
 based-ui-automation) - [ð Generate Python Code while Interacting with your
```

### Comparing `botcity-framework-core-1.1.0/botcity_framework_core.egg-info/SOURCES.txt` & `botcity-framework-core-1.1.1/botcity_framework_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/setup.py` & `botcity-framework-core-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-core-1.1.0/versioneer.py` & `botcity-framework-core-1.1.1/versioneer.py`

 * *Files identical despite different names*

