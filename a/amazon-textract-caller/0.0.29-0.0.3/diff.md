# Comparing `tmp/amazon-textract-caller-0.0.29.tar.gz` & `tmp/amazon-textract-caller-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-caller-0.0.29.tar", last modified: Tue May  9 21:28:14 2023, max compression
+gzip compressed data, was "dist/amazon-textract-caller-0.0.3.tar", last modified: Mon Apr 12 20:14:14 2021, max compression
```

## Comparing `amazon-textract-caller-0.0.29.tar` & `amazon-textract-caller-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-05-09 21:28:14.608815 amazon-textract-caller-0.0.29/
--rw-r--r--   0 schadem    (504) staff       (20)    10142 2022-09-08 17:40:40.000000 amazon-textract-caller-0.0.29/LICENSE
--rw-r--r--   0 schadem    (504) staff       (20)      161 2022-09-08 17:40:40.000000 amazon-textract-caller-0.0.29/MANIFEST.in
--rw-r--r--   0 schadem    (504) staff       (20)     6839 2023-05-09 21:28:14.608923 amazon-textract-caller-0.0.29/PKG-INFO
--rw-r--r--   0 schadem    (504) staff       (20)     4867 2022-09-08 17:40:40.000000 amazon-textract-caller-0.0.29/README.md
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-05-09 21:28:14.608159 amazon-textract-caller-0.0.29/amazon_textract_caller.egg-info/
--rw-r--r--   0 schadem    (504) staff       (20)     6839 2023-05-09 21:28:14.000000 amazon-textract-caller-0.0.29/amazon_textract_caller.egg-info/PKG-INFO
--rw-r--r--   0 schadem    (504) staff       (20)      356 2023-05-09 21:28:14.000000 amazon-textract-caller-0.0.29/amazon_textract_caller.egg-info/SOURCES.txt
--rw-r--r--   0 schadem    (504) staff       (20)        1 2023-05-09 21:28:14.000000 amazon-textract-caller-0.0.29/amazon_textract_caller.egg-info/dependency_links.txt
--rw-r--r--   0 schadem    (504) staff       (20)      114 2023-05-09 21:28:14.000000 amazon-textract-caller-0.0.29/amazon_textract_caller.egg-info/requires.txt
--rw-r--r--   0 schadem    (504) staff       (20)       15 2023-05-09 21:28:14.000000 amazon-textract-caller-0.0.29/amazon_textract_caller.egg-info/top_level.txt
--rw-r--r--   0 schadem    (504) staff       (20)      400 2023-05-09 21:28:14.609243 amazon-textract-caller-0.0.29/setup.cfg
--rw-r--r--   0 schadem    (504) staff       (20)     2076 2023-05-09 21:28:03.000000 amazon-textract-caller-0.0.29/setup.py
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-05-09 21:28:14.608659 amazon-textract-caller-0.0.29/textractcaller/
--rw-r--r--   0 schadem    (504) staff       (20)      569 2023-05-09 21:27:50.000000 amazon-textract-caller-0.0.29/textractcaller/__init__.py
--rw-r--r--   0 schadem    (504) staff       (20)       24 2023-05-09 21:28:03.000000 amazon-textract-caller-0.0.29/textractcaller/_version.py
--rw-r--r--   0 schadem    (504) staff       (20)    31507 2023-05-09 21:27:50.000000 amazon-textract-caller-0.0.29/textractcaller/t_call.py
+drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-12 20:14:14.826155 amazon-textract-caller-0.0.3/
+-rw-r--r--   0 schadem  (1964830885) staff       (20)    10142 2021-04-02 00:17:18.000000 amazon-textract-caller-0.0.3/LICENSE
+-rw-r--r--   0 schadem  (1964830885) staff       (20)      161 2021-04-05 21:52:38.000000 amazon-textract-caller-0.0.3/MANIFEST.in
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     3835 2021-04-12 20:14:14.826386 amazon-textract-caller-0.0.3/PKG-INFO
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     2469 2021-04-05 21:08:52.000000 amazon-textract-caller-0.0.3/README.md
+drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-12 20:14:14.824392 amazon-textract-caller-0.0.3/amazon_textract_caller.egg-info/
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     3835 2021-04-12 20:14:14.000000 amazon-textract-caller-0.0.3/amazon_textract_caller.egg-info/PKG-INFO
+-rw-r--r--   0 schadem  (1964830885) staff       (20)      356 2021-04-12 20:14:14.000000 amazon-textract-caller-0.0.3/amazon_textract_caller.egg-info/SOURCES.txt
+-rw-r--r--   0 schadem  (1964830885) staff       (20)        1 2021-04-12 20:14:14.000000 amazon-textract-caller-0.0.3/amazon_textract_caller.egg-info/dependency_links.txt
+-rw-r--r--   0 schadem  (1964830885) staff       (20)       15 2021-04-12 20:14:14.000000 amazon-textract-caller-0.0.3/amazon_textract_caller.egg-info/requires.txt
+-rw-r--r--   0 schadem  (1964830885) staff       (20)       15 2021-04-12 20:14:14.000000 amazon-textract-caller-0.0.3/amazon_textract_caller.egg-info/top_level.txt
+-rw-r--r--   0 schadem  (1964830885) staff       (20)      399 2021-04-12 20:14:14.827158 amazon-textract-caller-0.0.3/setup.cfg
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     1921 2021-04-12 20:14:04.000000 amazon-textract-caller-0.0.3/setup.py
+drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-12 20:14:14.825780 amazon-textract-caller-0.0.3/textractcaller/
+-rw-r--r--   0 schadem  (1964830885) staff       (20)      137 2021-04-05 22:06:44.000000 amazon-textract-caller-0.0.3/textractcaller/__init__.py
+-rw-r--r--   0 schadem  (1964830885) staff       (20)       23 2021-04-12 20:14:04.000000 amazon-textract-caller-0.0.3/textractcaller/_version.py
+-rw-r--r--   0 schadem  (1964830885) staff       (20)    12547 2021-04-12 20:02:06.000000 amazon-textract-caller-0.0.3/textractcaller/t_call.py
```

### Comparing `amazon-textract-caller-0.0.29/LICENSE` & `amazon-textract-caller-0.0.3/LICENSE`

 * *Files identical despite different names*

