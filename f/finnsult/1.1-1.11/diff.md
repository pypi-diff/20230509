# Comparing `tmp/finnsult-1.1.tar.gz` & `tmp/finnsult-1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finnsult-1.1.tar", last modified: Tue May  9 12:59:24 2023, max compression
+gzip compressed data, was "finnsult-1.11.tar", last modified: Tue May  9 13:02:19 2023, max compression
```

## Comparing `finnsult-1.1.tar` & `finnsult-1.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 realfinnventor   (502) staff       (20)        0 2023-05-09 12:59:24.534730 finnsult-1.1/
--rw-r--r--   0 realfinnventor   (502) staff       (20)     1071 2023-04-16 19:32:24.000000 finnsult-1.1/LICENSE.txt
--rw-r--r--   0 realfinnventor   (502) staff       (20)       46 2023-05-09 00:45:23.000000 finnsult-1.1/MANIFEST.in
--rw-r--r--   0 realfinnventor   (502) staff       (20)     1700 2023-05-09 12:59:24.533858 finnsult-1.1/PKG-INFO
--rw-r--r--   0 realfinnventor   (502) staff       (20)     1288 2023-05-09 12:54:05.000000 finnsult-1.1/README.md
--rw-r--r--   0 realfinnventor   (502) staff       (20)       38 2023-05-09 12:59:24.535036 finnsult-1.1/setup.cfg
--rw-r--r--   0 realfinnventor   (502) staff       (20)      837 2023-05-09 12:58:59.000000 finnsult-1.1/setup.py
-drwxr-xr-x   0 realfinnventor   (502) staff       (20)        0 2023-05-09 12:59:24.517214 finnsult-1.1/src/
-drwxr-xr-x   0 realfinnventor   (502) staff       (20)        0 2023-05-09 12:59:24.525697 finnsult-1.1/src/finnsult.egg-info/
--rw-r--r--   0 realfinnventor   (502) staff       (20)     1700 2023-05-09 12:59:24.000000 finnsult-1.1/src/finnsult.egg-info/PKG-INFO
--rw-r--r--   0 realfinnventor   (502) staff       (20)      328 2023-05-09 12:59:24.000000 finnsult-1.1/src/finnsult.egg-info/SOURCES.txt
--rw-r--r--   0 realfinnventor   (502) staff       (20)        1 2023-05-09 12:59:24.000000 finnsult-1.1/src/finnsult.egg-info/dependency_links.txt
--rw-r--r--   0 realfinnventor   (502) staff       (20)       39 2023-05-09 12:59:24.000000 finnsult-1.1/src/finnsult.egg-info/entry_points.txt
--rw-r--r--   0 realfinnventor   (502) staff       (20)        7 2023-05-09 12:59:24.000000 finnsult-1.1/src/finnsult.egg-info/requires.txt
--rw-r--r--   0 realfinnventor   (502) staff       (20)        7 2023-05-09 12:59:24.000000 finnsult-1.1/src/finnsult.egg-info/top_level.txt
-drwxr-xr-x   0 realfinnventor   (502) staff       (20)        0 2023-05-09 12:59:24.531353 finnsult-1.1/src/insult/
--rw-r--r--   0 realfinnventor   (502) staff       (20)       21 2023-05-09 00:37:19.000000 finnsult-1.1/src/insult/__init__.py
--rwxr-xr-x   0 realfinnventor   (502) staff       (20)     2512 2023-05-09 00:49:55.000000 finnsult-1.1/src/insult/insult.py
--rw-r--r--   0 realfinnventor   (502) staff       (20)      951 2023-04-11 01:56:14.000000 finnsult-1.1/src/insult/settings.yml
+drwxr-xr-x   0 realfinnventor   (502) staff       (20)        0 2023-05-09 13:02:19.175943 finnsult-1.11/
+-rw-r--r--   0 realfinnventor   (502) staff       (20)     1071 2023-04-16 19:32:24.000000 finnsult-1.11/LICENSE.txt
+-rw-r--r--   0 realfinnventor   (502) staff       (20)       46 2023-05-09 00:45:23.000000 finnsult-1.11/MANIFEST.in
+-rw-r--r--   0 realfinnventor   (502) staff       (20)     1702 2023-05-09 13:02:19.175206 finnsult-1.11/PKG-INFO
+-rw-r--r--   0 realfinnventor   (502) staff       (20)     1289 2023-05-09 13:01:24.000000 finnsult-1.11/README.md
+-rw-r--r--   0 realfinnventor   (502) staff       (20)       38 2023-05-09 13:02:19.176191 finnsult-1.11/setup.cfg
+-rw-r--r--   0 realfinnventor   (502) staff       (20)      837 2023-05-09 13:01:31.000000 finnsult-1.11/setup.py
+drwxr-xr-x   0 realfinnventor   (502) staff       (20)        0 2023-05-09 13:02:19.158283 finnsult-1.11/src/
+drwxr-xr-x   0 realfinnventor   (502) staff       (20)        0 2023-05-09 13:02:19.167885 finnsult-1.11/src/finnsult.egg-info/
+-rw-r--r--   0 realfinnventor   (502) staff       (20)     1702 2023-05-09 13:02:19.000000 finnsult-1.11/src/finnsult.egg-info/PKG-INFO
+-rw-r--r--   0 realfinnventor   (502) staff       (20)      328 2023-05-09 13:02:19.000000 finnsult-1.11/src/finnsult.egg-info/SOURCES.txt
+-rw-r--r--   0 realfinnventor   (502) staff       (20)        1 2023-05-09 13:02:19.000000 finnsult-1.11/src/finnsult.egg-info/dependency_links.txt
+-rw-r--r--   0 realfinnventor   (502) staff       (20)       39 2023-05-09 13:02:19.000000 finnsult-1.11/src/finnsult.egg-info/entry_points.txt
+-rw-r--r--   0 realfinnventor   (502) staff       (20)        7 2023-05-09 13:02:19.000000 finnsult-1.11/src/finnsult.egg-info/requires.txt
+-rw-r--r--   0 realfinnventor   (502) staff       (20)        7 2023-05-09 13:02:19.000000 finnsult-1.11/src/finnsult.egg-info/top_level.txt
+drwxr-xr-x   0 realfinnventor   (502) staff       (20)        0 2023-05-09 13:02:19.173163 finnsult-1.11/src/insult/
+-rw-r--r--   0 realfinnventor   (502) staff       (20)       21 2023-05-09 00:37:19.000000 finnsult-1.11/src/insult/__init__.py
+-rwxr-xr-x   0 realfinnventor   (502) staff       (20)     2512 2023-05-09 00:49:55.000000 finnsult-1.11/src/insult/insult.py
+-rw-r--r--   0 realfinnventor   (502) staff       (20)      951 2023-04-11 01:56:14.000000 finnsult-1.11/src/insult/settings.yml
```

### Comparing `finnsult-1.1/LICENSE.txt` & `finnsult-1.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finnsult-1.1/PKG-INFO` & `finnsult-1.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finnsult
-Version: 1.1
+Version: 1.11
 Summary: A program to insult people
 Home-page: https://the-real-finnventor.github.io/insult/
 Author: Finn Everspaugh
 Author-email: finnventor@everspaugh.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -39,15 +39,15 @@
 
 ## Installation (if you don't care about the settings)
 ```
 pip3 install finnsult
 open ~/.zprofile
 ```
 
-Now find `${PATH}`. Put your cursor before that and paste this: `/Users/INSERT_YOUR_USERNAME_HERE/Library/Python/3.9/bin:`. Then replace `INSERT_YOUR_USERNAME_HERE` with your username (eg. finneverspaugh). If you are unsure of you username at any time in the terminal (unless the terminal is activly doing something) it should say `username@computername.
+Now find `${PATH}`. Put your cursor before that and paste this: `/Users/INSERT_YOUR_USERNAME_HERE/Library/Python/3.9/bin:`. Then replace `INSERT_YOUR_USERNAME_HERE` with your username (eg. finneverspaugh). If you are unsure of you username at any time in the terminal (unless the terminal is activly doing something) it should say `username@computername`.
 
 ## Run (at any time open a terminal and run)
 ```
 insult
 ```
 
 # DISCLAIMER:
```

### Comparing `finnsult-1.1/README.md` & `finnsult-1.11/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ## Installation (if you don't care about the settings)
 ```
 pip3 install finnsult
 open ~/.zprofile
 ```
 
-Now find `${PATH}`. Put your cursor before that and paste this: `/Users/INSERT_YOUR_USERNAME_HERE/Library/Python/3.9/bin:`. Then replace `INSERT_YOUR_USERNAME_HERE` with your username (eg. finneverspaugh). If you are unsure of you username at any time in the terminal (unless the terminal is activly doing something) it should say `username@computername.
+Now find `${PATH}`. Put your cursor before that and paste this: `/Users/INSERT_YOUR_USERNAME_HERE/Library/Python/3.9/bin:`. Then replace `INSERT_YOUR_USERNAME_HERE` with your username (eg. finneverspaugh). If you are unsure of you username at any time in the terminal (unless the terminal is activly doing something) it should say `username@computername`.
 
 ## Run (at any time open a terminal and run)
 ```
 insult
 ```
 
 # DISCLAIMER:
```

### Comparing `finnsult-1.1/setup.py` & `finnsult-1.11/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "finnsult",
-    version = "1.01",
+    version = "1.11",
     author = "Finn Everspaugh",
     author_email = "finnventor@everspaugh.com",
     description = "A program to insult people",
     entry_points={
         'console_scripts': [
             'insult = insult:main',
        ],
```

### Comparing `finnsult-1.1/src/finnsult.egg-info/PKG-INFO` & `finnsult-1.11/src/finnsult.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finnsult
-Version: 1.1
+Version: 1.11
 Summary: A program to insult people
 Home-page: https://the-real-finnventor.github.io/insult/
 Author: Finn Everspaugh
 Author-email: finnventor@everspaugh.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -39,15 +39,15 @@
 
 ## Installation (if you don't care about the settings)
 ```
 pip3 install finnsult
 open ~/.zprofile
 ```
 
-Now find `${PATH}`. Put your cursor before that and paste this: `/Users/INSERT_YOUR_USERNAME_HERE/Library/Python/3.9/bin:`. Then replace `INSERT_YOUR_USERNAME_HERE` with your username (eg. finneverspaugh). If you are unsure of you username at any time in the terminal (unless the terminal is activly doing something) it should say `username@computername.
+Now find `${PATH}`. Put your cursor before that and paste this: `/Users/INSERT_YOUR_USERNAME_HERE/Library/Python/3.9/bin:`. Then replace `INSERT_YOUR_USERNAME_HERE` with your username (eg. finneverspaugh). If you are unsure of you username at any time in the terminal (unless the terminal is activly doing something) it should say `username@computername`.
 
 ## Run (at any time open a terminal and run)
 ```
 insult
 ```
 
 # DISCLAIMER:
```

### Comparing `finnsult-1.1/src/insult/insult.py` & `finnsult-1.11/src/insult/insult.py`

 * *Files identical despite different names*

### Comparing `finnsult-1.1/src/insult/settings.yml` & `finnsult-1.11/src/insult/settings.yml`

 * *Files identical despite different names*

