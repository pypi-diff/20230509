# Comparing `tmp/starrail-toolkit-0.5.0.tar.gz` & `tmp/starrail-toolkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.5.0.tar", last modified: Mon May  8 13:30:27 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.5.1.tar", last modified: Mon May  8 18:32:38 2023, max compression
```

## Comparing `starrail-toolkit-0.5.0.tar` & `starrail-toolkit-0.5.1.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.334499 starrail-toolkit-0.5.0/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     4970 2023-05-08 13:30:27.334332 starrail-toolkit-0.5.0/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     4463 2023-05-08 13:29:19.000000 starrail-toolkit-0.5.0/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-08 13:30:27.334546 starrail-toolkit-0.5.0/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.328420 starrail-toolkit-0.5.0/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1763 2023-05-08 13:18:40.000000 starrail-toolkit-0.5.0/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.329106 starrail-toolkit-0.5.0/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1803 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      965 2023-05-07 04:25:56.000000 starrail-toolkit-0.5.0/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1301 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.330488 starrail-toolkit-0.5.0/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      806 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5078 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3572 2023-05-08 11:35:55.000000 starrail-toolkit-0.5.0/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.330767 starrail-toolkit-0.5.0/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5870 2023-05-07 10:02:46.000000 starrail-toolkit-0.5.0/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.331291 starrail-toolkit-0.5.0/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:18:00.000000 starrail-toolkit-0.5.0/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-07 10:02:46.000000 starrail-toolkit-0.5.0/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      563 2023-05-08 06:27:44.000000 starrail-toolkit-0.5.0/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      333 2023-05-08 13:22:41.000000 starrail-toolkit-0.5.0/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.332101 starrail-toolkit-0.5.0/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:17:51.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-07 10:02:59.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    13038 2023-05-08 13:22:17.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2520 2023-05-07 05:24:37.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2373 2023-05-07 09:07:50.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-07 10:02:48.000000 starrail-toolkit-0.5.0/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.332479 starrail-toolkit-0.5.0/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)        6 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.333336 starrail-toolkit-0.5.0/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     2155 2023-05-08 12:49:28.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-07 05:10:36.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4541 2023-05-08 12:49:28.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.0/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-08 13:13:31.000000 starrail-toolkit-0.5.0/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:30:27.334134 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     4970 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1341 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-08 13:30:27.000000 starrail-toolkit-0.5.0/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.145310 starrail-toolkit-0.5.1/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4970 2023-05-08 18:32:38.145183 starrail-toolkit-0.5.1/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4463 2023-05-08 17:45:49.000000 starrail-toolkit-0.5.1/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-08 18:32:38.145352 starrail-toolkit-0.5.1/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.138470 starrail-toolkit-0.5.1/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1763 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.139183 starrail-toolkit-0.5.1/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1803 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      965 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1301 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.140676 starrail-toolkit-0.5.1/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      806 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5078 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3572 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.140932 starrail-toolkit-0.5.1/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5870 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.141437 starrail-toolkit-0.5.1/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      563 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      333 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.142354 starrail-toolkit-0.5.1/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    13109 2023-05-08 17:41:55.000000 starrail-toolkit-0.5.1/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2520 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2373 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.142697 starrail-toolkit-0.5.1/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 14:18:54.000000 starrail-toolkit-0.5.1/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.143154 starrail-toolkit-0.5.1/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)        6 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.144182 starrail-toolkit-0.5.1/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2155 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.1/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4685 2023-05-08 17:45:09.000000 starrail-toolkit-0.5.1/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.1/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-08 17:45:52.000000 starrail-toolkit-0.5.1/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-08 18:32:38.144989 starrail-toolkit-0.5.1/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4970 2023-05-08 18:32:38.000000 starrail-toolkit-0.5.1/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1442 2023-05-08 18:32:38.000000 starrail-toolkit-0.5.1/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-08 18:32:38.000000 starrail-toolkit-0.5.1/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-08 18:32:38.000000 starrail-toolkit-0.5.1/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-08 18:32:38.000000 starrail-toolkit-0.5.1/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-08 18:32:38.000000 starrail-toolkit-0.5.1/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.5.0/LICENSE` & `starrail-toolkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/PKG-INFO` & `starrail-toolkit-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,15 +20,15 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.0    |    0.5.0     |   0.5.0   |
+|   0.5.0    |    0.5.1     |   0.5.1   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
```

### Comparing `starrail-toolkit-0.5.0/README.md` & `starrail-toolkit-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.0    |    0.5.0     |   0.5.0   |
+|   0.5.0    |    0.5.1     |   0.5.1   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
```

### Comparing `starrail-toolkit-0.5.0/setup.py` & `starrail-toolkit-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/__init__.py` & `starrail-toolkit-0.5.1/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/config.py` & `starrail-toolkit-0.5.1/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/entry/cli.py` & `starrail-toolkit-0.5.1/starrail/entry/cli.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/entry/gui.py` & `starrail-toolkit-0.5.1/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/entry/setup.py` & `starrail-toolkit-0.5.1/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gacha/autodet.py` & `starrail-toolkit-0.5.1/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gacha/database.py` & `starrail-toolkit-0.5.1/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gacha/fetch.py` & `starrail-toolkit-0.5.1/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gacha/fileio.py` & `starrail-toolkit-0.5.1/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gacha/parse.py` & `starrail-toolkit-0.5.1/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gacha/service.py` & `starrail-toolkit-0.5.1/starrail/gacha/service.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gacha/url.py` & `starrail-toolkit-0.5.1/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gui/application.py` & `starrail-toolkit-0.5.1/starrail/gui/application.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.5.1/starrail/gui/common/stylesheet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.5.1/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.5.1/starrail/gui/interfaces/gacha_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import qfluentwidgets as qfw
 from PySide6 import QtWidgets
 from PySide6.QtCore import QEvent, QObject, Qt, QThread, Signal
 from PySide6.QtWidgets import QLabel, QTableWidgetItem, QVBoxLayout
 
 import starrail.gacha.service as service
+from starrail.config import configuration as cfg
 from starrail.gacha.type import GachaType
 from starrail.gui.common.stylesheet import StyleSheet
 from starrail.gui.common.utils import get_current_uid
 from starrail.gui.interfaces.base import BaseInterface
 from starrail.utils import babelfish, loggings
 
 AF = Qt.AlignmentFlag
@@ -321,14 +322,15 @@
     def setToolTipContentSlot(self, tooltip: qfw.StateToolTip, content: str):
         tooltip.setContent(content)
 
     def syncSuccessSlot(self, uid: int):
         logger.info('[GUI] Gacha data synchronization success')
 
         self.uid = uid
+        cfg.uid = uid
 
         self.syncToolTip.setTitle(babelfish.ui_sync_gacha_success())
         self.syncToolTip.setContent('')
         self.syncToolTip.setState(True)
         self.syncToolTip = None
         self.syncThread = None
```

### Comparing `starrail-toolkit-0.5.0/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.5.1/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.5.1/starrail/gui/interfaces/setting.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.5.1/starrail/utils/babelfish/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.5.1/starrail/utils/babelfish/dictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,19 @@
     zhs='正在提取 API URL',
 )
 ui_gacha_basic_prob = _MS(en='Basic Prob.', zhs='基础概率')
 ui_gacha_count = _MS(en='Count', zhs='数量')
 ui_gacha_since_last = _MS(en='Since Last', zhs='距上次')
 ui_gacha_sync = _MS(en='Sync Gacha Data', zhs='抽卡数据同步')
 ui_gacha_sync_desc = _MS(
-    en='Let\'s fetch something!',
-    zhs='让我看看谁又歪了？',
+    en=(
+        'First query warp record in the game, then close the game and click '
+        'the sync button.'
+    ),
+    zhs='先在游戏里查询一次抽卡记录，然后退出游戏，点击同步按钮。',
 )
 ui_gacha_true_prob = _MS(en='True Prob.', zhs='综合概率')
 ui_gacha_type = _MS(en='Type', zhs='星级')
 ui_get_started = _MS(en='Get Started', zhs='开始使用')
 ui_get_started_desc = _MS(
     en='Learning how to use the toolkit.',
     zhs='学习本工具箱的基本使用方法。',
```

### Comparing `starrail-toolkit-0.5.0/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.5.1/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail/utils/loggings.py` & `starrail-toolkit-0.5.1/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.0/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.5.1/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,15 +20,15 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.0    |    0.5.0     |   0.5.0   |
+|   0.5.0    |    0.5.1     |   0.5.1   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
```

### Comparing `starrail-toolkit-0.5.0/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.5.1/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 starrail/gui/common/utils.py
 starrail/gui/interfaces/__init__.py
 starrail/gui/interfaces/base.py
 starrail/gui/interfaces/gacha_sync.py
 starrail/gui/interfaces/home.py
 starrail/gui/interfaces/setting.py
 starrail/gui/interfaces/users.py
+starrail/gui/widgets/__init__.py
+starrail/gui/widgets/link_card.py
+starrail/gui/widgets/title_bar.py
 starrail/utils/__init__.py
 starrail/utils/auto_update.py
 starrail/utils/loggings.py
 starrail/utils/babelfish/__init__.py
 starrail/utils/babelfish/constants.py
 starrail/utils/babelfish/dictionary.py
 starrail/utils/babelfish/locale.py
```

