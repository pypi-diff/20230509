# Comparing `tmp/slashml-0.1.1.tar.gz` & `tmp/slashml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-gkluihqa/slashml-0.1.1.tar", last modified: Sat May  6 22:11:49 2023, max compression
+gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-dp1cf0fi/slashml-0.1.2.tar", last modified: Mon May  8 22:01:30 2023, max compression
```

## Comparing `slashml-0.1.1.tar` & `slashml-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-06 22:11:49.718359 slashml-0.1.1/
--rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.1.1/LICENSE.txt
--rw-r--r--   0 faizank    (501) staff       (20)      279 2023-05-06 22:11:49.718192 slashml-0.1.1/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)     6847 2023-04-24 07:51:41.000000 slashml-0.1.1/README.md
--rw-r--r--   0 faizank    (501) staff       (20)       38 2023-05-06 22:11:49.718410 slashml-0.1.1/setup.cfg
--rw-r--r--   0 faizank    (501) staff       (20)      730 2023-05-06 22:11:38.000000 slashml-0.1.1/setup.py
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-06 22:11:49.717994 slashml-0.1.1/slashml.egg-info/
--rw-r--r--   0 faizank    (501) staff       (20)      279 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)      184 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/SOURCES.txt
--rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/dependency_links.txt
--rw-r--r--   0 faizank    (501) staff       (20)       17 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/requires.txt
--rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/top_level.txt
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:01:30.046007 slashml-0.1.2/
+-rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.1.2/LICENSE.txt
+-rw-r--r--   0 faizank    (501) staff       (20)      279 2023-05-08 22:01:30.045836 slashml-0.1.2/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)     5520 2023-05-08 21:56:06.000000 slashml-0.1.2/README.md
+-rw-r--r--   0 faizank    (501) staff       (20)       38 2023-05-08 22:01:30.046058 slashml-0.1.2/setup.cfg
+-rw-r--r--   0 faizank    (501) staff       (20)      730 2023-05-08 22:01:07.000000 slashml-0.1.2/setup.py
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:01:30.045639 slashml-0.1.2/slashml.egg-info/
+-rw-r--r--   0 faizank    (501) staff       (20)      279 2023-05-08 22:01:30.000000 slashml-0.1.2/slashml.egg-info/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)      184 2023-05-08 22:01:30.000000 slashml-0.1.2/slashml.egg-info/SOURCES.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-08 22:01:30.000000 slashml-0.1.2/slashml.egg-info/dependency_links.txt
+-rw-r--r--   0 faizank    (501) staff       (20)       31 2023-05-08 22:01:30.000000 slashml-0.1.2/slashml.egg-info/requires.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-08 22:01:30.000000 slashml-0.1.2/slashml.egg-info/top_level.txt
```

### Comparing `slashml-0.1.1/LICENSE.txt` & `slashml-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slashml-0.1.1/setup.py` & `slashml-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(f"{SLASHML_DIR}requires-{req_type}.txt") as fp:  # pylint: disable=W1514
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setup(
     name="slashml",
-    version="0.1.1",
+    version="0.1.2",
     url="https://slashml.com/",
     author="eff-kay",
     author_email="faiizan14@gmail.com",
     description=(
         "A Python client for interacting with SlashML services" "Developed by SlashML."
     ),
     packages=find_packages("slashml"),
```

