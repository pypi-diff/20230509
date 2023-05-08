# Comparing `tmp/oexp-0.2.2.tar.gz` & `tmp/oexp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.2.2.tar", last modified: Wed Apr 12 04:06:24 2023, max compression
+gzip compressed data, was "oexp-0.3.0.tar", last modified: Mon May  8 23:04:19 2023, max compression
```

## Comparing `oexp-0.2.2.tar` & `oexp-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:06:24.622341 oexp-0.2.2/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-04-12 04:06:24.622179 oexp-0.2.2/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.2.2/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:06:24.621272 oexp-0.2.2/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      127 2023-03-14 19:30:00.000000 oexp-0.2.2/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)      399 2023-03-18 02:41:19.000000 oexp-0.2.2/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     7596 2023-03-31 14:49:58.000000 oexp-0.2.2/oexp/oexp.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:06:24.622013 oexp-0.2.2/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      206 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-04-12 04:06:24.000000 oexp-0.2.2/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-04-12 04:06:20.000000 oexp-0.2.2/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-04-12 04:06:24.622382 oexp-0.2.2/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-08 23:04:19.975768 oexp-0.3.0/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-08 23:04:19.975582 oexp-0.3.0/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.3.0/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-08 23:04:19.974447 oexp-0.3.0/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.3.0/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    71050 2023-05-08 23:03:51.000000 oexp-0.3.0/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-08 23:03:35.000000 oexp-0.3.0/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     4740 2023-05-08 19:15:04.000000 oexp-0.3.0/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-08 23:04:19.975369 oexp-0.3.0/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-08 23:04:14.000000 oexp-0.3.0/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-08 23:04:19.975816 oexp-0.3.0/setup.cfg
```

