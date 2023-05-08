# Comparing `tmp/zoterotex-0.0.1a7.tar.gz` & `tmp/zoterotex-0.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a7.tar", last modified: Fri May  5 00:29:54 2023, max compression
+gzip compressed data, was "zoterotex-0.0.1a8.tar", last modified: Mon May  8 22:39:18 2023, max compression
```

## Comparing `zoterotex-0.0.1a7.tar` & `zoterotex-0.0.1a8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:29:54.967843 zoterotex-0.0.1a7/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:29:54.967598 zoterotex-0.0.1a7/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-05 00:18:06.000000 zoterotex-0.0.1a7/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-05 00:29:54.967888 zoterotex-0.0.1a7/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:29:54.964851 zoterotex-0.0.1a7/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a7/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     2154 2023-05-05 00:29:26.000000 zoterotex-0.0.1a7/zoterotex/__main__.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:29:54.967286 zoterotex-0.0.1a7/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 22:39:18.558654 zoterotex-0.0.1a8/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-08 22:39:18.558417 zoterotex-0.0.1a8/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-08 22:34:18.000000 zoterotex-0.0.1a8/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-08 22:39:18.558711 zoterotex-0.0.1a8/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 22:39:18.555525 zoterotex-0.0.1a8/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a8/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     3115 2023-05-08 22:33:05.000000 zoterotex-0.0.1a8/zoterotex/__main__.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-08 22:39:18.558099 zoterotex-0.0.1a8/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-08 22:39:18.000000 zoterotex-0.0.1a8/zoterotex.egg-info/top_level.txt
```

