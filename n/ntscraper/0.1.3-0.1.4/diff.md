# Comparing `tmp/ntscraper-0.1.3.tar.gz` & `tmp/ntscraper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntscraper-0.1.3.tar", last modified: Sat May  6 07:28:01 2023, max compression
+gzip compressed data, was "ntscraper-0.1.4.tar", last modified: Tue May  9 07:58:58 2023, max compression
```

## Comparing `ntscraper-0.1.3.tar` & `ntscraper-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:28:01.262889 ntscraper-0.1.3/
--rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3485 2023-05-06 07:28:01.262889 ntscraper-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2559 2023-05-06 07:24:10.000000 ntscraper-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 07:28:01.230866 ntscraper-0.1.3/ntscraper/
--rw-rw-rw-   0        0        0       26 2023-01-31 13:55:18.000000 ntscraper-0.1.3/ntscraper/__init__.py
--rw-rw-rw-   0        0        0    27229 2023-05-06 07:24:10.000000 ntscraper-0.1.3/ntscraper/nitter.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:28:01.258874 ntscraper-0.1.3/ntscraper.egg-info/
--rw-rw-rw-   0        0        0     3485 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 07:28:01.262889 ntscraper-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-05-06 07:24:10.000000 ntscraper-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:58:58.438847 ntscraper-0.1.4/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3485 2023-05-09 07:58:58.436843 ntscraper-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2559 2023-05-06 07:24:10.000000 ntscraper-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 07:58:58.392840 ntscraper-0.1.4/ntscraper/
+-rw-rw-rw-   0        0        0       26 2023-01-31 13:55:18.000000 ntscraper-0.1.4/ntscraper/__init__.py
+-rw-rw-rw-   0        0        0    27292 2023-05-08 09:45:29.000000 ntscraper-0.1.4/ntscraper/nitter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:58:58.434843 ntscraper-0.1.4/ntscraper.egg-info/
+-rw-rw-rw-   0        0        0     3485 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 07:58:58.438847 ntscraper-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-05-08 09:46:48.000000 ntscraper-0.1.4/setup.py
```

### Comparing `ntscraper-0.1.3/LICENSE.txt` & `ntscraper-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ntscraper-0.1.3/PKG-INFO` & `ntscraper-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
```

### Comparing `ntscraper-0.1.3/README.md` & `ntscraper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ntscraper-0.1.3/ntscraper/nitter.py` & `ntscraper-0.1.4/ntscraper/nitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,14 +329,15 @@
         """
         return (
             tweet.find("div", class_="tweet-content media-body")
             .text.strip()
             .replace("\n", " ")
             if tweet.find("div", class_="tweet-content media-body")
             else tweet.find("div", class_="quote-text").text.strip().replace("\n", " ")
+            if tweet.find("div", class_="quote-text") else ""
         )
 
     def __get_tweet_link(self, tweet):
         """
         Extract link from a tweet
 
         :param tweet: tweet to extract link from
```

### Comparing `ntscraper-0.1.3/ntscraper.egg-info/PKG-INFO` & `ntscraper-0.1.4/ntscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
```

### Comparing `ntscraper-0.1.3/setup.py` & `ntscraper-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ntscraper",
-    version="0.1.3",
+    version="0.1.4",
     description="Unofficial library to scrape Twitter profiles and posts from Nitter instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Homepage': 'https://github.com/bocchilorenzo/ntscraper',
         'Source': 'https://github.com/bocchilorenzo/ntscraper',
         'Documentation': 'https://github.com/bocchilorenzo/ntscraper'
```

