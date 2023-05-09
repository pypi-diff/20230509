# Comparing `tmp/venakatest-0.1.28.tar.gz` & `tmp/venakatest-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venakatest-0.1.28.tar", last modified: Tue May  9 03:56:20 2023, max compression
+gzip compressed data, was "venakatest-0.1.29.tar", last modified: Tue May  9 03:58:35 2023, max compression
```

## Comparing `venakatest-0.1.28.tar` & `venakatest-0.1.29.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 03:56:20.652093 venakatest-0.1.28/
--rw-rw-rw-   0        0        0       94 2023-05-09 03:56:20.651105 venakatest-0.1.28/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.28/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 03:56:20.652093 venakatest-0.1.28/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-05-09 03:56:15.000000 venakatest-0.1.28/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:56:20.630092 venakatest-0.1.28/venakatest/
--rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.28/venakatest/__init__.py
--rw-rw-rw-   0        0        0     2634 2023-05-09 03:51:07.000000 venakatest-0.1.28/venakatest/test.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:56:20.650093 venakatest-0.1.28/venakatest.egg-info/
--rw-rw-rw-   0        0        0       94 2023-05-09 03:56:20.000000 venakatest-0.1.28/venakatest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-09 03:56:20.000000 venakatest-0.1.28/venakatest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 03:56:20.000000 venakatest-0.1.28/venakatest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-09 03:56:20.000000 venakatest-0.1.28/venakatest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 03:56:20.000000 venakatest-0.1.28/venakatest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 03:56:20.000000 venakatest-0.1.28/venakatest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 03:58:35.479515 venakatest-0.1.29/
+-rw-rw-rw-   0        0        0       94 2023-05-09 03:58:35.478515 venakatest-0.1.29/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.29/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 03:58:35.479515 venakatest-0.1.29/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-05-09 03:58:33.000000 venakatest-0.1.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:58:35.461516 venakatest-0.1.29/venakatest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.29/venakatest/__init__.py
+-rw-rw-rw-   0        0        0     2634 2023-05-09 03:51:07.000000 venakatest-0.1.29/venakatest/test.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:58:35.477516 venakatest-0.1.29/venakatest.egg-info/
+-rw-rw-rw-   0        0        0       94 2023-05-09 03:58:35.000000 venakatest-0.1.29/venakatest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-09 03:58:35.000000 venakatest-0.1.29/venakatest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 03:58:35.000000 venakatest-0.1.29/venakatest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-09 03:58:35.000000 venakatest-0.1.29/venakatest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 03:58:35.000000 venakatest-0.1.29/venakatest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 03:58:35.000000 venakatest-0.1.29/venakatest.egg-info/top_level.txt
```

### Comparing `venakatest-0.1.28/venakatest/test.py` & `venakatest-0.1.29/venakatest/test.py`

 * *Files identical despite different names*

