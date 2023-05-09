# Comparing `tmp/ReverseTwitterScraper-0.5.tar.gz` & `tmp/ReverseTwitterScraper-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseTwitterScraper-0.5.tar", last modified: Thu May  4 15:27:20 2023, max compression
+gzip compressed data, was "ReverseTwitterScraper-0.6.tar", last modified: Tue May  9 20:19:30 2023, max compression
```

## Comparing `ReverseTwitterScraper-0.5.tar` & `ReverseTwitterScraper-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 15:27:20.936016 ReverseTwitterScraper-0.5/
--rw-rw-rw-   0        0        0     1090 2023-03-08 21:13:40.000000 ReverseTwitterScraper-0.5/LICENSE
--rw-rw-rw-   0        0        0     7671 2023-05-04 15:27:20.935516 ReverseTwitterScraper-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7176 2023-05-04 15:26:42.000000 ReverseTwitterScraper-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 15:27:20.910510 ReverseTwitterScraper-0.5/ReverseTwitterScraper/
--rw-rw-rw-   0        0        0    20330 2023-05-04 15:21:46.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper/Scraper.py
--rw-rw-rw-   0        0        0       37 2023-03-09 02:04:31.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:27:20.934014 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/
--rw-rw-rw-   0        0        0     7671 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-04 15:27:20.000000 ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 15:27:20.936016 ReverseTwitterScraper-0.5/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-05-04 15:26:31.000000 ReverseTwitterScraper-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:19:30.383320 ReverseTwitterScraper-0.6/
+-rw-rw-rw-   0        0        0     1090 2023-03-08 21:13:40.000000 ReverseTwitterScraper-0.6/LICENSE
+-rw-rw-rw-   0        0        0     7671 2023-05-09 20:19:30.383320 ReverseTwitterScraper-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7176 2023-05-04 15:26:42.000000 ReverseTwitterScraper-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 20:19:30.363316 ReverseTwitterScraper-0.6/ReverseTwitterScraper/
+-rw-rw-rw-   0        0        0    20330 2023-05-04 15:21:46.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper/Scraper.py
+-rw-rw-rw-   0        0        0       37 2023-03-09 02:04:31.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:19:30.382320 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/
+-rw-rw-rw-   0        0        0     7671 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-09 20:19:30.000000 ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 20:19:30.383320 ReverseTwitterScraper-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-05-09 20:18:46.000000 ReverseTwitterScraper-0.6/setup.py
```

### Comparing `ReverseTwitterScraper-0.5/LICENSE` & `ReverseTwitterScraper-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseTwitterScraper-0.5/PKG-INFO` & `ReverseTwitterScraper-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseTwitterScraper
-Version: 0.5
+Version: 0.6
 Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
 Home-page: https://github.com/1220moritz/reverse-twitter-scraper
 Author: 1220moritz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `ReverseTwitterScraper-0.5/README.md` & `ReverseTwitterScraper-0.6/README.md`

 * *Files identical despite different names*

### Comparing `ReverseTwitterScraper-0.5/ReverseTwitterScraper/Scraper.py` & `ReverseTwitterScraper-0.6/ReverseTwitterScraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `ReverseTwitterScraper-0.5/ReverseTwitterScraper.egg-info/PKG-INFO` & `ReverseTwitterScraper-0.6/ReverseTwitterScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseTwitterScraper
-Version: 0.5
+Version: 0.6
 Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
 Home-page: https://github.com/1220moritz/reverse-twitter-scraper
 Author: 1220moritz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `ReverseTwitterScraper-0.5/setup.py` & `ReverseTwitterScraper-0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ReverseTwitterScraper",
-    version="0.5",
+    version="0.6",
     author="1220moritz",
     description="A Python package for scraping Twitter data without API. With proxy and account-cookie support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/1220moritz/reverse-twitter-scraper",
       install_requires=[
           'selenium-wire',
           'selenium',
           "httpx",
-          "asyncio",
-          "traceback"
+          "asyncio"
       ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

