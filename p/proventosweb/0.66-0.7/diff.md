# Comparing `tmp/proventosweb-0.66.tar.gz` & `tmp/proventosweb-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.66.tar", last modified: Tue May  9 18:07:16 2023, max compression
+gzip compressed data, was "proventosweb-0.7.tar", last modified: Tue May  9 18:04:31 2023, max compression
```

## Comparing `proventosweb-0.66.tar` & `proventosweb-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 18:07:16.668293 proventosweb-0.66/
--rw-rw-rw-   0        0        0      265 2023-05-09 18:07:16.667295 proventosweb-0.66/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 18:07:16.641365 proventosweb-0.66/proventosweb/
--rw-rw-rw-   0        0        0       44 2023-05-09 18:01:30.000000 proventosweb-0.66/proventosweb/__init__.py
--rw-rw-rw-   0        0        0    12340 2023-05-09 18:02:59.000000 proventosweb-0.66/proventosweb/proventosweb.py
-drwxrwxrwx   0        0        0        0 2023-05-09 18:07:16.665300 proventosweb-0.66/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      265 2023-05-09 18:07:16.000000 proventosweb-0.66/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-09 18:07:16.000000 proventosweb-0.66/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 18:07:16.000000 proventosweb-0.66/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.66/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-09 18:07:16.000000 proventosweb-0.66/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-09 18:07:16.000000 proventosweb-0.66/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 18:07:16.669290 proventosweb-0.66/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-09 18:07:00.000000 proventosweb-0.66/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:04:31.038541 proventosweb-0.7/
+-rw-rw-rw-   0        0        0      264 2023-05-09 18:04:31.037544 proventosweb-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 18:04:30.998090 proventosweb-0.7/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-09 18:01:30.000000 proventosweb-0.7/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    12340 2023-05-09 18:02:59.000000 proventosweb-0.7/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:04:31.035550 proventosweb-0.7/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.7/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-09 18:04:30.000000 proventosweb-0.7/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 18:04:31.038541 proventosweb-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-05-09 18:03:32.000000 proventosweb-0.7/setup.py
```

### Comparing `proventosweb-0.66/proventosweb/proventosweb.py` & `proventosweb-0.7/proventosweb/proventosweb.py`

 * *Files identical despite different names*

