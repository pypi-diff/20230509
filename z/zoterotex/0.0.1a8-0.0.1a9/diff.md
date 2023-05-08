# Comparing `tmp/zoterotex-0.0.1a8.tar.gz` & `tmp/zoterotex-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a8.tar", last modified: Mon May  8 22:39:18 2023, max compression
+gzip compressed data, was "zoterotex-0.0.1a9.tar", last modified: Mon May  8 23:22:28 2023, max compression
```

## Comparing `zoterotex-0.0.1a8.tar` & `zoterotex-0.0.1a9.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 22:39:18.558654 zoterotex-0.0.1a8/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-08 22:39:18.558417 zoterotex-0.0.1a8/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-08 22:34:18.000000 zoterotex-0.0.1a8/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-08 22:39:18.558711 zoterotex-0.0.1a8/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 22:39:18.555525 zoterotex-0.0.1a8/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a8/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     3115 2023-05-08 22:33:05.000000 zoterotex-0.0.1a8/zoterotex/__main__.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 22:39:18.558099 zoterotex-0.0.1a8/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 23:22:28.844753 zoterotex-0.0.1a9/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-08 23:22:28.844519 zoterotex-0.0.1a9/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-08 23:18:50.000000 zoterotex-0.0.1a9/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-08 23:22:28.844805 zoterotex-0.0.1a9/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 23:22:28.841826 zoterotex-0.0.1a9/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142      149 2023-05-08 23:10:07.000000 zoterotex-0.0.1a9/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142      643 2023-05-08 23:21:03.000000 zoterotex-0.0.1a9/zoterotex/__main__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142      975 2023-05-08 23:21:03.000000 zoterotex-0.0.1a9/zoterotex/_header.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     1691 2023-05-08 23:21:03.000000 zoterotex-0.0.1a9/zoterotex/_sync.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 23:22:28.844193 zoterotex-0.0.1a9/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      298 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-08 23:22:28.000000 zoterotex-0.0.1a9/zoterotex.egg-info/top_level.txt
```

