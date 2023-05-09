# Comparing `tmp/zoterotex-0.0.1a9.tar.gz` & `tmp/zoterotex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a9.tar", last modified: Mon May  8 23:22:28 2023, max compression
+gzip compressed data, was "zoterotex-0.1.1.tar", last modified: Tue May  9 00:10:31 2023, max compression
```

## Comparing `zoterotex-0.0.1a9.tar` & `zoterotex-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 23:22:28.844753 zoterotex-0.0.1a9/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-08 23:22:28.844519 zoterotex-0.0.1a9/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-08 23:18:50.000000 zoterotex-0.0.1a9/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-08 23:22:28.844805 zoterotex-0.0.1a9/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 23:22:28.841826 zoterotex-0.0.1a9/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142      149 2023-05-08 23:10:07.000000 zoterotex-0.0.1a9/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142      643 2023-05-08 23:21:03.000000 zoterotex-0.0.1a9/zoterotex/__main__.py
--rw-r--r--   0 galer    (1959091754) 1971611142      975 2023-05-08 23:21:03.000000 zoterotex-0.0.1a9/zoterotex/_header.py
--rw-r--r--   0 galer    (1959091754) 1971611142     1691 2023-05-08 23:21:03.000000 zoterotex-0.0.1a9/zoterotex/_sync.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 23:22:28.844193 zoterotex-0.0.1a9/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      298 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-09 00:10:31.479727 zoterotex-0.1.1/
+-rw-r--r--   0 galer    (1959091754) 1971611142     1340 2023-05-09 00:10:31.479525 zoterotex-0.1.1/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      930 2023-05-08 23:58:38.000000 zoterotex-0.1.1/README.md
+-rw-r--r--   0 galer    (1959091754) 1971611142      695 2023-05-08 23:50:23.000000 zoterotex-0.1.1/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-09 00:10:31.479788 zoterotex-0.1.1/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-09 00:10:31.477328 zoterotex-0.1.1/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142       92 2023-05-09 00:09:01.000000 zoterotex-0.1.1/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142      996 2023-05-09 00:08:13.000000 zoterotex-0.1.1/zoterotex/__main__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     2700 2023-05-09 00:08:33.000000 zoterotex-0.1.1/zoterotex/_sync.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-09 00:10:31.479272 zoterotex-0.1.1/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142     1340 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      287 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/top_level.txt
```

