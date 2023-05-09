# Comparing `tmp/py-spw-1.4.4.tar.gz` & `tmp/Py-SPW-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Py-SPW-1.4.4.tar", last modified: Mon Aug  1 09:38:19 2022, max compression
+gzip compressed data, was "dist/Py-SPW-1.5.0.tar", last modified: Tue May  9 09:25:47 2023, max compression
```

## Comparing `py-spw-1.4.4.tar` & `Py-SPW-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-08-01 09:38:19.281057 Py-SPW-1.4.4/
--rw-rw-rw-   0        0        0     1085 2022-07-14 14:37:00.000000 Py-SPW-1.4.4/LICENSE
--rw-rw-rw-   0        0        0      820 2022-08-01 09:38:19.282053 Py-SPW-1.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-08-01 09:38:19.251054 Py-SPW-1.4.4/Py_SPW.egg-info/
--rw-rw-rw-   0        0        0      820 2022-08-01 09:38:19.000000 Py-SPW-1.4.4/Py_SPW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2022-08-01 09:38:19.000000 Py-SPW-1.4.4/Py_SPW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-01 09:38:19.000000 Py-SPW-1.4.4/Py_SPW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-08-01 09:38:19.000000 Py-SPW-1.4.4/Py_SPW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-08-01 09:38:19.000000 Py-SPW-1.4.4/Py_SPW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      365 2022-07-21 22:40:46.000000 Py-SPW-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2022-08-01 09:38:19.276059 Py-SPW-1.4.4/pyspw/
--rw-rw-rw-   0        0        0     2070 2022-07-22 21:21:42.000000 Py-SPW-1.4.4/pyspw/Parameters.py
--rw-rw-rw-   0        0        0     3263 2022-07-22 11:36:10.000000 Py-SPW-1.4.4/pyspw/Skin.py
--rw-rw-rw-   0        0        0      917 2022-08-01 09:29:09.000000 Py-SPW-1.4.4/pyspw/User.py
--rw-rw-rw-   0        0        0      196 2022-07-22 21:21:42.000000 Py-SPW-1.4.4/pyspw/__init__.py
--rw-rw-rw-   0        0        0     9768 2022-07-22 22:17:21.000000 Py-SPW-1.4.4/pyspw/api.py
--rw-rw-rw-   0        0        0      413 2022-07-14 19:51:56.000000 Py-SPW-1.4.4/pyspw/errors.py
--rw-rw-rw-   0        0        0       42 2022-08-01 09:38:19.286054 Py-SPW-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      865 2022-08-01 09:36:58.000000 Py-SPW-1.4.4/setup.py
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-05-09 09:25:47.000000 Py-SPW-1.5.0/
+-rwxrwxr-x   0 stepan    (1000) stepan    (1000)     1085 2023-04-06 18:35:20.000000 Py-SPW-1.5.0/LICENSE
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)     1351 2023-05-09 09:25:47.000000 Py-SPW-1.5.0/PKG-INFO
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-05-09 09:25:47.000000 Py-SPW-1.5.0/Py_SPW.egg-info/
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)     1351 2023-05-09 09:25:46.000000 Py-SPW-1.5.0/Py_SPW.egg-info/PKG-INFO
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)      266 2023-05-09 09:25:46.000000 Py-SPW-1.5.0/Py_SPW.egg-info/SOURCES.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)        1 2023-05-09 09:25:46.000000 Py-SPW-1.5.0/Py_SPW.egg-info/dependency_links.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)       86 2023-05-09 09:25:46.000000 Py-SPW-1.5.0/Py_SPW.egg-info/requires.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)        6 2023-05-09 09:25:46.000000 Py-SPW-1.5.0/Py_SPW.egg-info/top_level.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      941 2023-05-08 20:22:26.000000 Py-SPW-1.5.0/README.md
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-05-09 09:25:47.000000 Py-SPW-1.5.0/pyspw/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     2661 2023-05-08 23:19:28.000000 Py-SPW-1.5.0/pyspw/Parameters.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     3634 2023-05-08 23:23:59.000000 Py-SPW-1.5.0/pyspw/User.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       42 2023-05-08 19:02:28.000000 Py-SPW-1.5.0/pyspw/__init__.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     9956 2023-05-08 23:00:18.000000 Py-SPW-1.5.0/pyspw/api.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1728 2023-05-08 23:12:43.000000 Py-SPW-1.5.0/pyspw/errors.py
+-rwxrwxr-x   0 stepan    (1000) stepan    (1000)       38 2023-05-09 09:25:47.000000 Py-SPW-1.5.0/setup.cfg
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      861 2023-05-08 20:10:39.000000 Py-SPW-1.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `Py-SPW-1.4.4/LICENSE` & `Py-SPW-1.5.0/LICENSE`

 * *Files identical despite different names*

