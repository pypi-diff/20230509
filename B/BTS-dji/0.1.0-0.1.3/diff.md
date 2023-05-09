# Comparing `tmp/BTS_dji-0.1.0.tar.gz` & `tmp/BTS_dji-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTS_dji-0.1.0.tar", last modified: Tue May  9 01:43:11 2023, max compression
+gzip compressed data, was "BTS_dji-0.1.3.tar", last modified: Tue May  9 03:53:49 2023, max compression
```

## Comparing `BTS_dji-0.1.0.tar` & `BTS_dji-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 01:43:11.785516 BTS_dji-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:43:11.772365 BTS_dji-0.1.0/BTS_dji/
--rw-rw-rw-   0        0        0        0 2023-05-09 01:23:28.000000 BTS_dji-0.1.0/BTS_dji/__init__.py
--rw-rw-rw-   0        0        0     2774 2023-05-09 01:24:05.000000 BTS_dji-0.1.0/BTS_dji/kbd.py
-drwxrwxrwx   0        0        0        0 2023-05-09 01:43:11.784522 BTS_dji-0.1.0/BTS_dji.egg-info/
--rw-rw-rw-   0        0        0      509 2023-05-09 01:43:11.000000 BTS_dji-0.1.0/BTS_dji.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-09 01:43:11.000000 BTS_dji-0.1.0/BTS_dji.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 01:43:11.000000 BTS_dji-0.1.0/BTS_dji.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 01:43:11.000000 BTS_dji-0.1.0/BTS_dji.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 01:43:11.000000 BTS_dji-0.1.0/BTS_dji.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      509 2023-05-09 01:43:11.785019 BTS_dji-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-05-09 00:40:43.000000 BTS_dji-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 01:43:11.785516 BTS_dji-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1133 2023-05-09 01:42:24.000000 BTS_dji-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:53:49.380252 BTS_dji-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:53:49.380252 BTS_dji-0.1.3/BTS_dji/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-09 03:53:38.000000 BTS_dji-0.1.3/BTS_dji/Robomaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 03:53:38.000000 BTS_dji-0.1.3/BTS_dji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-05-09 03:53:38.000000 BTS_dji-0.1.3/BTS_dji/controler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-09 03:53:38.000000 BTS_dji-0.1.3/BTS_dji/kbd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:53:49.380252 BTS_dji-0.1.3/BTS_dji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 03:53:49.000000 BTS_dji-0.1.3/BTS_dji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 03:53:49.000000 BTS_dji-0.1.3/BTS_dji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:53:49.000000 BTS_dji-0.1.3/BTS_dji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 03:53:49.000000 BTS_dji-0.1.3/BTS_dji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 03:53:49.000000 BTS_dji-0.1.3/BTS_dji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 03:53:49.380252 BTS_dji-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 03:53:38.000000 BTS_dji-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:53:49.380252 BTS_dji-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-09 03:53:38.000000 BTS_dji-0.1.3/setup.py
```

