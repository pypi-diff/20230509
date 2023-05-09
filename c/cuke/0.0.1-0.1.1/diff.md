# Comparing `tmp/Cuke-0.0.1.tar.gz` & `tmp/cuke-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cuke-0.0.1.tar", last modified: Thu Sep 29 06:03:33 2022, max compression
+gzip compressed data, was "cuke-0.1.1.tar", max compression
```

## Comparing `Cuke-0.0.1.tar` & `cuke-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,6 @@
-drwxr-xr-x   0 boab      (1000) boab      (1000)        0 2022-09-29 06:03:33.271255 Cuke-0.0.1/
--rw-r--r--   0 boab      (1000) boab      (1000)      249 2022-09-29 06:03:33.271255 Cuke-0.0.1/PKG-INFO
--rw-r--r--   0 boab      (1000) boab      (1000)       35 2022-09-29 06:03:01.000000 Cuke-0.0.1/README.md
-drwxr-xr-x   0 boab      (1000) boab      (1000)        0 2022-09-29 06:03:33.271255 Cuke-0.0.1/cuke/
-drwxr-xr-x   0 boab      (1000) boab      (1000)        0 2022-09-29 06:03:33.271255 Cuke-0.0.1/cuke/Cuke.egg-info/
--rw-r--r--   0 boab      (1000) boab      (1000)      249 2022-09-29 06:03:32.000000 Cuke-0.0.1/cuke/Cuke.egg-info/PKG-INFO
--rw-r--r--   0 boab      (1000) boab      (1000)      192 2022-09-29 06:03:33.000000 Cuke-0.0.1/cuke/Cuke.egg-info/SOURCES.txt
--rw-r--r--   0 boab      (1000) boab      (1000)        1 2022-09-29 06:03:32.000000 Cuke-0.0.1/cuke/Cuke.egg-info/dependency_links.txt
--rw-r--r--   0 boab      (1000) boab      (1000)        7 2022-09-29 06:03:33.000000 Cuke-0.0.1/cuke/Cuke.egg-info/requires.txt
--rw-r--r--   0 boab      (1000) boab      (1000)        1 2022-09-29 06:03:33.000000 Cuke-0.0.1/cuke/Cuke.egg-info/top_level.txt
--rw-r--r--   0 boab      (1000) boab      (1000)       79 2022-09-29 06:03:33.271255 Cuke-0.0.1/setup.cfg
--rw-r--r--   0 boab      (1000) boab      (1000)      391 2022-09-29 06:02:21.000000 Cuke-0.0.1/setup.py
+-rw-r--r--   0        0        0       37 2023-05-09 03:30:00.925539 cuke-0.1.1/README.md
+-rw-r--r--   0        0        0    12131 2023-05-09 03:30:00.925539 cuke-0.1.1/cuke/__init__.py
+-rw-r--r--   0        0        0      655 2023-05-09 03:30:00.925539 cuke-0.1.1/cuke/errors.py
+-rw-r--r--   0        0        0     1702 2023-05-09 03:30:00.925539 cuke-0.1.1/cuke/util.py
+-rw-r--r--   0        0        0      557 2023-05-09 03:30:00.925539 cuke-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 cuke-0.1.1/PKG-INFO
```

