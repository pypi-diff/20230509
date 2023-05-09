# Comparing `tmp/pytzen-0.0.111.tar.gz` & `tmp/pytzen-0.0.112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytzen-0.0.111.tar", last modified: Thu Apr 20 19:33:26 2023, max compression
+gzip compressed data, was "pytzen-0.0.112.tar", last modified: Tue May  9 20:27:59 2023, max compression
```

## Comparing `pytzen-0.0.111.tar` & `pytzen-0.0.112.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-04-20 19:33:26.528080 pytzen-0.0.111/
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1063 2023-02-07 08:42:41.000000 pytzen-0.0.111/LICENSE
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1703 2023-04-20 19:33:26.528080 pytzen-0.0.111/PKG-INFO
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1343 2023-04-20 19:30:08.000000 pytzen-0.0.111/README.md
--rwxrwxr-x   0 pytzen    (1000) pytzen    (1000)       84 2023-03-17 18:47:24.000000 pytzen-0.0.111/pyproject.toml
--rwxrwxr-x   0 pytzen    (1000) pytzen    (1000)      505 2023-04-20 19:33:26.528080 pytzen-0.0.111/setup.cfg
-drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-04-20 19:33:26.524080 pytzen-0.0.111/src/
-drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-04-20 19:33:26.528080 pytzen-0.0.111/src/pytzen/
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)      148 2023-04-20 19:33:22.000000 pytzen-0.0.111/src/pytzen/__init__.py
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1561 2023-03-20 15:07:47.000000 pytzen-0.0.111/src/pytzen/ai_joke_generator.py
-drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-04-20 19:33:26.528080 pytzen-0.0.111/src/pytzen/system_info/
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)        0 2023-03-20 15:00:30.000000 pytzen-0.0.111/src/pytzen/system_info/__init__.py
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     2977 2023-03-20 19:10:35.000000 pytzen-0.0.111/src/pytzen/system_info/get_info.py
-drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-04-20 19:33:26.528080 pytzen-0.0.111/src/pytzen.egg-info/
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1703 2023-04-20 19:33:26.000000 pytzen-0.0.111/src/pytzen.egg-info/PKG-INFO
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)      303 2023-04-20 19:33:26.000000 pytzen-0.0.111/src/pytzen.egg-info/SOURCES.txt
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)        1 2023-04-20 19:33:26.000000 pytzen-0.0.111/src/pytzen.egg-info/dependency_links.txt
--rw-rw-r--   0 pytzen    (1000) pytzen    (1000)        7 2023-04-20 19:33:26.000000 pytzen-0.0.111/src/pytzen.egg-info/top_level.txt
+drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-05-09 20:27:59.500184 pytzen-0.0.112/
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1063 2023-02-07 08:42:41.000000 pytzen-0.0.112/LICENSE
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1156 2023-05-09 20:27:59.500184 pytzen-0.0.112/PKG-INFO
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)      840 2023-05-09 20:26:54.000000 pytzen-0.0.112/README.md
+-rwxrwxr-x   0 pytzen    (1000) pytzen    (1000)       84 2023-03-17 18:47:24.000000 pytzen-0.0.112/pyproject.toml
+-rwxrwxr-x   0 pytzen    (1000) pytzen    (1000)      456 2023-05-09 20:27:59.500184 pytzen-0.0.112/setup.cfg
+drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-05-09 20:27:59.496185 pytzen-0.0.112/src/
+drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-05-09 20:27:59.500184 pytzen-0.0.112/src/pytzen/
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)      148 2023-05-09 20:27:54.000000 pytzen-0.0.112/src/pytzen/__init__.py
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1561 2023-03-20 15:07:47.000000 pytzen-0.0.112/src/pytzen/ai_joke_generator.py
+drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-05-09 20:27:59.500184 pytzen-0.0.112/src/pytzen/system_info/
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)        0 2023-03-20 15:00:30.000000 pytzen-0.0.112/src/pytzen/system_info/__init__.py
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     2977 2023-03-20 19:10:35.000000 pytzen-0.0.112/src/pytzen/system_info/get_info.py
+drwxrwxr-x   0 pytzen    (1000) pytzen    (1000)        0 2023-05-09 20:27:59.500184 pytzen-0.0.112/src/pytzen.egg-info/
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)     1156 2023-05-09 20:27:59.000000 pytzen-0.0.112/src/pytzen.egg-info/PKG-INFO
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)      303 2023-05-09 20:27:59.000000 pytzen-0.0.112/src/pytzen.egg-info/SOURCES.txt
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)        1 2023-05-09 20:27:59.000000 pytzen-0.0.112/src/pytzen.egg-info/dependency_links.txt
+-rw-rw-r--   0 pytzen    (1000) pytzen    (1000)        7 2023-05-09 20:27:59.000000 pytzen-0.0.112/src/pytzen.egg-info/top_level.txt
```

### Comparing `pytzen-0.0.111/LICENSE` & `pytzen-0.0.112/LICENSE`

 * *Files identical despite different names*

### Comparing `pytzen-0.0.111/src/pytzen/ai_joke_generator.py` & `pytzen-0.0.112/src/pytzen/ai_joke_generator.py`

 * *Files identical despite different names*

### Comparing `pytzen-0.0.111/src/pytzen/system_info/get_info.py` & `pytzen-0.0.112/src/pytzen/system_info/get_info.py`

 * *Files identical despite different names*

