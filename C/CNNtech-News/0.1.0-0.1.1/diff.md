# Comparing `tmp/CNNtech_News-0.1.0.tar.gz` & `tmp/CNNtech_News-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CNNtech_News-0.1.0.tar", last modified: Mon May  8 23:35:42 2023, max compression
+gzip compressed data, was "CNNtech_News-0.1.1.tar", last modified: Mon May  8 23:46:11 2023, max compression
```

## Comparing `CNNtech_News-0.1.0.tar` & `CNNtech_News-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:35:42.405679 CNNtech_News-0.1.0/
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:35:42.404366 CNNtech_News-0.1.0/CNNtech_News.egg-info/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1118 2023-05-08 23:35:42.000000 CNNtech_News-0.1.0/CNNtech_News.egg-info/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      197 2023-05-08 23:35:42.000000 CNNtech_News-0.1.0/CNNtech_News.egg-info/SOURCES.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-08 23:35:42.000000 CNNtech_News-0.1.0/CNNtech_News.egg-info/dependency_links.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       15 2023-05-08 23:35:42.000000 CNNtech_News-0.1.0/CNNtech_News.egg-info/top_level.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-08 23:18:31.000000 CNNtech_News-0.1.0/LICENSE
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1118 2023-05-08 23:35:42.405274 CNNtech_News-0.1.0/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      514 2023-05-08 23:30:57.000000 CNNtech_News-0.1.0/README.md
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-08 23:35:42.405803 CNNtech_News-0.1.0/setup.cfg
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      984 2023-05-08 23:35:27.000000 CNNtech_News-0.1.0/setup.py
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:35:42.404807 CNNtech_News-0.1.0/updateTechnews/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2264 2023-05-08 23:30:57.000000 CNNtech_News-0.1.0/updateTechnews/__init__.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:46:11.566957 CNNtech_News-0.1.1/
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:46:11.565516 CNNtech_News-0.1.1/CNNtech_News.egg-info/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1122 2023-05-08 23:46:11.000000 CNNtech_News-0.1.1/CNNtech_News.egg-info/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      197 2023-05-08 23:46:11.000000 CNNtech_News-0.1.1/CNNtech_News.egg-info/SOURCES.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-08 23:46:11.000000 CNNtech_News-0.1.1/CNNtech_News.egg-info/dependency_links.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       15 2023-05-08 23:46:11.000000 CNNtech_News-0.1.1/CNNtech_News.egg-info/top_level.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-08 23:18:31.000000 CNNtech_News-0.1.1/LICENSE
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1122 2023-05-08 23:46:11.566592 CNNtech_News-0.1.1/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      518 2023-05-08 23:41:16.000000 CNNtech_News-0.1.1/README.md
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-08 23:46:11.567049 CNNtech_News-0.1.1/setup.cfg
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      984 2023-05-08 23:41:51.000000 CNNtech_News-0.1.1/setup.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-08 23:46:11.566057 CNNtech_News-0.1.1/updateTechnews/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2263 2023-05-08 23:41:16.000000 CNNtech_News-0.1.1/updateTechnews/__init__.py
```

### Comparing `CNNtech_News-0.1.0/CNNtech_News.egg-info/PKG-INFO` & `CNNtech_News-0.1.1/CNNtech_News.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNNtech-News
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package will provide you the most update of CNN Tech News
 Home-page: https://github.com/ganirh0612/CNNtech_News
 Author: Hasan Gani Rachmatullah
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 # How It Works
 This Package will scrape from https://edition.cnn.com/business/tech
 
 This package will use BeautifulSoup4 and Request, to then produce in the form of JSON that is ready to be used in web or mobile applications.
 
 # How to Use This Package?
 ```
-import updateTech
+import updateTechnews
 
 if __name__ == '__main__':
     print('Deskription Package:', description)
     result = news_data()
     show_news(result)
 ```
```

### Comparing `CNNtech_News-0.1.0/LICENSE` & `CNNtech_News-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CNNtech_News-0.1.0/PKG-INFO` & `CNNtech_News-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNNtech_News
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package will provide you the most update of CNN Tech News
 Home-page: https://github.com/ganirh0612/CNNtech_News
 Author: Hasan Gani Rachmatullah
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 # How It Works
 This Package will scrape from https://edition.cnn.com/business/tech
 
 This package will use BeautifulSoup4 and Request, to then produce in the form of JSON that is ready to be used in web or mobile applications.
 
 # How to Use This Package?
 ```
-import updateTech
+import updateTechnews
 
 if __name__ == '__main__':
     print('Deskription Package:', description)
     result = news_data()
     show_news(result)
 ```
```

### Comparing `CNNtech_News-0.1.0/README.md` & `CNNtech_News-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # How It Works
 This Package will scrape from https://edition.cnn.com/business/tech
 
 This package will use BeautifulSoup4 and Request, to then produce in the form of JSON that is ready to be used in web or mobile applications.
 
 # How to Use This Package?
 ```
-import updateTech
+import updateTechnews
 
 if __name__ == '__main__':
     print('Deskription Package:', description)
     result = news_data()
     show_news(result)
 ```
```

### Comparing `CNNtech_News-0.1.0/setup.py` & `CNNtech_News-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CNNtech_News",
-    version="0.1.0",
+    version="0.1.1",
     author="Hasan Gani Rachmatullah",
     author_email="ganirh0612@gmail.com",
     description="This package will provide you the most update of CNN Tech News",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ganirh0612/CNNtech_News",
     project_urls={
```

### Comparing `CNNtech_News-0.1.0/updateTechnews/__init__.py` & `CNNtech_News-0.1.1/updateTechnews/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,12 +73,11 @@
     print(f"News 3 > {result['newsThree']}")
     print(f"News 4 > {result['newsFour']}")
     print(f"News 5 > {result['newsFive']}")
     print(f"News 6 > {result['newsSix']}")
     print(f"News 7 > {result['newsSeven']}")
     print(f"News 8 > {result['newsEight']}")
 
-
 if __name__ == '__main__':
     print('Deskription Package:', description)
     result = news_data()
     show_news(result)
```

