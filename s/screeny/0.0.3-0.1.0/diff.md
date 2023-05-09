# Comparing `tmp/screeny-0.0.3.tar.gz` & `tmp/screeny-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screeny-0.0.3.tar", last modified: Fri Apr 28 22:35:10 2023, max compression
+gzip compressed data, was "screeny-0.1.0.tar", last modified: Tue May  9 14:23:29 2023, max compression
```

## Comparing `screeny-0.0.3.tar` & `screeny-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-28 22:35:10.684476 screeny-0.0.3/
--rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.0.3/LICENSE
--rw-r--r--   0 paulpol    (501) staff       (20)    23170 2023-04-28 17:23:31.000000 screeny-0.0.3/LICENSE-3RD-Party.txt
--rw-r--r--   0 paulpol    (501) staff       (20)      451 2023-04-28 22:35:10.684645 screeny-0.0.3/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)       71 2023-04-27 17:09:15.000000 screeny-0.0.3/README.md
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-28 22:35:10.681933 screeny-0.0.3/Screeny.egg-info/
--rw-r--r--   0 paulpol    (501) staff       (20)      451 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      411 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/SOURCES.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/dependency_links.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       32 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/requires.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/top_level.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-04-28 18:10:34.000000 screeny-0.0.3/pyproject.toml
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-28 22:35:10.683324 screeny-0.0.3/screeny/
--rw-r--r--   0 paulpol    (501) staff       (20)       28 2023-04-28 18:03:41.000000 screeny-0.0.3/screeny/__init__.py
--rw-r--r--   0 paulpol    (501) staff       (20)      727 2023-04-27 19:39:34.000000 screeny-0.0.3/screeny/screeny.py
--rw-r--r--   0 paulpol    (501) staff       (20)      503 2023-04-28 22:35:10.685281 screeny-0.0.3/setup.cfg
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-09 14:23:29.895242 screeny-0.1.0/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.1.0/LICENSE
+-rw-r--r--   0 paulpol    (501) staff       (20)    23170 2023-04-28 17:23:31.000000 screeny-0.1.0/LICENSE-3RD-Party.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)      887 2023-05-09 14:23:29.895377 screeny-0.1.0/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      507 2023-05-09 14:18:43.000000 screeny-0.1.0/README.md
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-09 14:23:29.892131 screeny-0.1.0/Screeny.egg-info/
+-rw-r--r--   0 paulpol    (501) staff       (20)      887 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      428 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       32 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/requires.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-09 14:23:29.000000 screeny-0.1.0/Screeny.egg-info/top_level.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-04-28 18:10:34.000000 screeny-0.1.0/pyproject.toml
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-09 14:23:29.894260 screeny-0.1.0/screeny/
+-rw-r--r--   0 paulpol    (501) staff       (20)       28 2023-04-28 18:03:41.000000 screeny-0.1.0/screeny/__init__.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      448 2023-05-09 13:48:00.000000 screeny-0.1.0/screeny/mouse.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     1139 2023-05-09 14:12:55.000000 screeny-0.1.0/screeny/screeny.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      503 2023-05-09 14:23:29.895947 screeny-0.1.0/setup.cfg
```

### Comparing `screeny-0.0.3/LICENSE` & `screeny-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screeny-0.0.3/LICENSE-3RD-Party.txt` & `screeny-0.1.0/LICENSE-3RD-Party.txt`

 * *Files identical despite different names*

