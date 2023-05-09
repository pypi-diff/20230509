# Comparing `tmp/interlo-0.1.tar.gz` & `tmp/interlo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interlo-0.1.tar", last modified: Mon May  8 01:49:55 2023, max compression
+gzip compressed data, was "interlo-1.0.1.tar", last modified: Tue May  9 00:14:15 2023, max compression
```

## Comparing `interlo-0.1.tar` & `interlo-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 autumn     (501) staff       (20)        0 2023-05-08 01:49:55.563108 interlo-0.1/
--rw-r--r--   0 autumn     (501) staff       (20)      102 2023-05-08 01:49:55.562789 interlo-0.1/PKG-INFO
-drwxr-xr-x   0 autumn     (501) staff       (20)        0 2023-05-08 01:49:55.562307 interlo-0.1/interlo.egg-info/
--rw-r--r--   0 autumn     (501) staff       (20)      102 2023-05-08 01:49:54.000000 interlo-0.1/interlo.egg-info/PKG-INFO
--rw-r--r--   0 autumn     (501) staff       (20)      196 2023-05-08 01:49:55.000000 interlo-0.1/interlo.egg-info/SOURCES.txt
--rw-r--r--   0 autumn     (501) staff       (20)        1 2023-05-08 01:49:54.000000 interlo-0.1/interlo.egg-info/dependency_links.txt
--rw-r--r--   0 autumn     (501) staff       (20)       41 2023-05-08 01:49:55.000000 interlo-0.1/interlo.egg-info/entry_points.txt
--rw-r--r--   0 autumn     (501) staff       (20)       31 2023-05-08 01:49:55.000000 interlo-0.1/interlo.egg-info/requires.txt
--rw-r--r--   0 autumn     (501) staff       (20)        8 2023-05-08 01:49:55.000000 interlo-0.1/interlo.egg-info/top_level.txt
--rw-r--r--   0 autumn     (501) staff       (20)       38 2023-05-08 01:49:55.563313 interlo-0.1/setup.cfg
--rw-r--r--   0 autumn     (501) staff       (20)      357 2023-05-08 01:46:47.000000 interlo-0.1/setup.py
+drwxr-xr-x   0 autumn     (501) staff       (20)        0 2023-05-09 00:14:15.701953 interlo-1.0.1/
+-rw-r--r--   0 autumn     (501) staff       (20)      104 2023-05-09 00:14:15.701667 interlo-1.0.1/PKG-INFO
+drwxr-xr-x   0 autumn     (501) staff       (20)        0 2023-05-09 00:14:15.701231 interlo-1.0.1/interlo.egg-info/
+-rw-r--r--   0 autumn     (501) staff       (20)      104 2023-05-09 00:14:14.000000 interlo-1.0.1/interlo.egg-info/PKG-INFO
+-rw-r--r--   0 autumn     (501) staff       (20)      196 2023-05-09 00:14:15.000000 interlo-1.0.1/interlo.egg-info/SOURCES.txt
+-rw-r--r--   0 autumn     (501) staff       (20)        1 2023-05-09 00:14:15.000000 interlo-1.0.1/interlo.egg-info/dependency_links.txt
+-rw-r--r--   0 autumn     (501) staff       (20)       41 2023-05-09 00:14:15.000000 interlo-1.0.1/interlo.egg-info/entry_points.txt
+-rw-r--r--   0 autumn     (501) staff       (20)       31 2023-05-09 00:14:15.000000 interlo-1.0.1/interlo.egg-info/requires.txt
+-rw-r--r--   0 autumn     (501) staff       (20)        8 2023-05-09 00:14:15.000000 interlo-1.0.1/interlo.egg-info/top_level.txt
+-rw-r--r--   0 autumn     (501) staff       (20)       38 2023-05-09 00:14:15.702071 interlo-1.0.1/setup.cfg
+-rw-r--r--   0 autumn     (501) staff       (20)      359 2023-05-09 00:11:47.000000 interlo-1.0.1/setup.py
```

