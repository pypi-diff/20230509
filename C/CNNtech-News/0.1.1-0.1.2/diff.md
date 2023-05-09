# Comparing `tmp/CNNtech_News-0.1.1.tar.gz` & `tmp/CNNtech_News-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CNNtech_News-0.1.1.tar", last modified: Mon May  8 23:46:11 2023, max compression
+gzip compressed data, was "CNNtech_News-0.1.2.tar", last modified: Tue May  9 07:26:23 2023, max compression
```

## Comparing `CNNtech_News-0.1.1.tar` & `CNNtech_News-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:46:11.566957 CNNtech_News-0.1.1/
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:46:11.565516 CNNtech_News-0.1.1/CNNtech_News.egg-info/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1122 2023-05-08 23:46:11.000000 CNNtech_News-0.1.1/CNNtech_News.egg-info/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      197 2023-05-08 23:46:11.000000 CNNtech_News-0.1.1/CNNtech_News.egg-info/SOURCES.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-08 23:46:11.000000 CNNtech_News-0.1.1/CNNtech_News.egg-info/dependency_links.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       15 2023-05-08 23:46:11.000000 CNNtech_News-0.1.1/CNNtech_News.egg-info/top_level.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-08 23:18:31.000000 CNNtech_News-0.1.1/LICENSE
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1122 2023-05-08 23:46:11.566592 CNNtech_News-0.1.1/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      518 2023-05-08 23:41:16.000000 CNNtech_News-0.1.1/README.md
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-08 23:46:11.567049 CNNtech_News-0.1.1/setup.cfg
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      984 2023-05-08 23:41:51.000000 CNNtech_News-0.1.1/setup.py
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:46:11.566057 CNNtech_News-0.1.1/updateTechnews/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2263 2023-05-08 23:41:16.000000 CNNtech_News-0.1.1/updateTechnews/__init__.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-09 07:26:23.476890 CNNtech_News-0.1.2/
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-09 07:26:23.475710 CNNtech_News-0.1.2/CNNtech_News.egg-info/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1122 2023-05-09 07:26:23.000000 CNNtech_News-0.1.2/CNNtech_News.egg-info/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      197 2023-05-09 07:26:23.000000 CNNtech_News-0.1.2/CNNtech_News.egg-info/SOURCES.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-09 07:26:23.000000 CNNtech_News-0.1.2/CNNtech_News.egg-info/dependency_links.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       15 2023-05-09 07:26:23.000000 CNNtech_News-0.1.2/CNNtech_News.egg-info/top_level.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-08 23:18:31.000000 CNNtech_News-0.1.2/LICENSE
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1122 2023-05-09 07:26:23.476582 CNNtech_News-0.1.2/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      518 2023-05-08 23:41:16.000000 CNNtech_News-0.1.2/README.md
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-09 07:26:23.477021 CNNtech_News-0.1.2/setup.cfg
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      984 2023-05-09 07:25:27.000000 CNNtech_News-0.1.2/setup.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-09 07:26:23.476122 CNNtech_News-0.1.2/updateTechnews/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2262 2023-05-08 23:51:22.000000 CNNtech_News-0.1.2/updateTechnews/__init__.py
```

### Comparing `CNNtech_News-0.1.1/CNNtech_News.egg-info/PKG-INFO` & `CNNtech_News-0.1.2/CNNtech_News.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNNtech-News
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package will provide you the most update of CNN Tech News
 Home-page: https://github.com/ganirh0612/CNNtech_News
 Author: Hasan Gani Rachmatullah
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `CNNtech_News-0.1.1/LICENSE` & `CNNtech_News-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CNNtech_News-0.1.1/PKG-INFO` & `CNNtech_News-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNNtech_News
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package will provide you the most update of CNN Tech News
 Home-page: https://github.com/ganirh0612/CNNtech_News
 Author: Hasan Gani Rachmatullah
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `CNNtech_News-0.1.1/README.md` & `CNNtech_News-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `CNNtech_News-0.1.1/setup.py` & `CNNtech_News-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CNNtech_News",
-    version="0.1.1",
+    version="0.1.2",
     author="Hasan Gani Rachmatullah",
     author_email="ganirh0612@gmail.com",
     description="This package will provide you the most update of CNN Tech News",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ganirh0612/CNNtech_News",
     project_urls={
```

### Comparing `CNNtech_News-0.1.1/updateTechnews/__init__.py` & `CNNtech_News-0.1.2/updateTechnews/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         tech['newsEight'] = newsEight
 
         return tech
 
     else:
         return None
 
-
 def show_news(result):
     if result is None:
         print("Update News Not Found")
         return
 
     print(description)
     print("Most Updates Technology News Today")
```

