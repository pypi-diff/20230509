# Comparing `tmp/bambooai-0.1.0.tar.gz` & `tmp/bambooai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.1.0.tar", last modified: Tue May  9 12:42:48 2023, max compression
+gzip compressed data, was "bambooai-0.1.1.tar", last modified: Tue May  9 12:58:14 2023, max compression
```

## Comparing `bambooai-0.1.0.tar` & `bambooai-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 12:42:48.165822 bambooai-0.1.0/
--rw-rw-rw-   0        0        0     5507 2023-05-09 12:42:48.163813 bambooai-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5015 2023-05-09 08:27:19.000000 bambooai-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 12:42:48.155911 bambooai-0.1.0/bambooai/
--rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.1.0/bambooai/__init__.py
--rw-rw-rw-   0        0        0     7736 2023-05-09 12:31:21.000000 bambooai-0.1.0/bambooai/bambooai.py
-drwxrwxrwx   0        0        0        0 2023-05-09 12:42:48.162293 bambooai-0.1.0/bambooai.egg-info/
--rw-rw-rw-   0        0        0     5507 2023-05-09 12:42:48.000000 bambooai-0.1.0/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-09 12:42:48.000000 bambooai-0.1.0/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 12:42:48.000000 bambooai-0.1.0/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-09 12:42:48.000000 bambooai-0.1.0/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 12:42:48.000000 bambooai-0.1.0/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 12:42:48.166010 bambooai-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-05-09 12:40:58.000000 bambooai-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:58:14.028590 bambooai-0.1.1/
+-rw-rw-rw-   0        0        0     5507 2023-05-09 12:58:14.028590 bambooai-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5015 2023-05-09 08:27:19.000000 bambooai-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 12:58:13.997590 bambooai-0.1.1/bambooai/
+-rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.1.1/bambooai/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-05-09 12:51:42.000000 bambooai-0.1.1/bambooai/bambooai.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:58:14.026589 bambooai-0.1.1/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     5507 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 12:58:14.029589 bambooai-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-05-09 12:54:11.000000 bambooai-0.1.1/setup.py
```

### Comparing `bambooai-0.1.0/PKG-INFO` & `bambooai-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bambooai-0.1.0/README.md` & `bambooai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bambooai-0.1.0/bambooai/bambooai.py` & `bambooai-0.1.1/bambooai/bambooai.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         content = response.choices[0].message.content.strip()
         tokens_used = response.usage.total_tokens
 
         return content, tokens_used
     
     # Function to sanitize the output from the LLM
-    def _extract_code(response: str, separator: str = "```") -> str:
+    def _extract_code(self,response: str, separator: str = "```") -> str:
 
         # Define a blacklist of Python keywords and functions that are not allowed
         blacklist = ['os','subprocess','sys','eval','exec','file','open','socket','urllib']
 
         # Set the initial value of code to the response
         code = response
```

### Comparing `bambooai-0.1.0/bambooai.egg-info/PKG-INFO` & `bambooai-0.1.1/bambooai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bambooai-0.1.0/setup.py` & `bambooai-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='bambooai',
-    version='0.1.0',
+    version='0.1.1',
     description='A lightweight library for working with pandas dataframes using natural language queries',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         'openai',
         'pandas',
```

