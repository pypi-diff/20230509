# Comparing `tmp/starrail-toolkit-0.5.3.tar.gz` & `tmp/starrail-toolkit-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.5.3.tar", last modified: Tue May  9 07:40:51 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.5.4.tar", last modified: Tue May  9 19:05:30 2023, max compression
```

## Comparing `starrail-toolkit-0.5.3.tar` & `starrail-toolkit-0.5.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.938082 starrail-toolkit-0.5.3/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     4970 2023-05-09 07:40:51.937962 starrail-toolkit-0.5.3/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     4463 2023-05-09 07:40:34.000000 starrail-toolkit-0.5.3/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-09 07:40:51.938120 starrail-toolkit-0.5.3/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.932680 starrail-toolkit-0.5.3/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1763 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.933128 starrail-toolkit-0.5.3/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3000 2023-05-09 07:34:09.000000 starrail-toolkit-0.5.3/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      988 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.934222 starrail-toolkit-0.5.3/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1103 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5078 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3572 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.934441 starrail-toolkit-0.5.3/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     7036 2023-05-09 07:40:03.000000 starrail-toolkit-0.5.3/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.934930 starrail-toolkit-0.5.3/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      333 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.935624 starrail-toolkit-0.5.3/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    13109 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2520 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2373 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.936038 starrail-toolkit-0.5.3/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5401 2023-05-09 07:38:54.000000 starrail-toolkit-0.5.3/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.936380 starrail-toolkit-0.5.3/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      681 2023-05-09 07:33:03.000000 starrail-toolkit-0.5.3/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.937116 starrail-toolkit-0.5.3/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     2512 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-08 13:31:32.000000 starrail-toolkit-0.5.3/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5970 2023-05-09 07:29:39.000000 starrail-toolkit-0.5.3/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-06 18:42:25.000000 starrail-toolkit-0.5.3/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-09 07:39:56.000000 starrail-toolkit-0.5.3/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 07:40:51.937777 starrail-toolkit-0.5.3/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     4970 2023-05-09 07:40:51.000000 starrail-toolkit-0.5.3/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1473 2023-05-09 07:40:51.000000 starrail-toolkit-0.5.3/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-09 07:40:51.000000 starrail-toolkit-0.5.3/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-09 07:40:51.000000 starrail-toolkit-0.5.3/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       78 2023-05-09 07:40:51.000000 starrail-toolkit-0.5.3/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-09 07:40:51.000000 starrail-toolkit-0.5.3/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.757251 starrail-toolkit-0.5.4/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5041 2023-05-09 19:05:30.757120 starrail-toolkit-0.5.4/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4534 2023-05-09 19:05:12.000000 starrail-toolkit-0.5.4/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-09 19:05:30.757286 starrail-toolkit-0.5.4/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.751750 starrail-toolkit-0.5.4/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1763 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.752210 starrail-toolkit-0.5.4/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3000 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      988 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.753214 starrail-toolkit-0.5.4/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1103 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5078 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3572 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.753465 starrail-toolkit-0.5.4/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5958 2023-05-09 18:54:42.000000 starrail-toolkit-0.5.4/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.753939 starrail-toolkit-0.5.4/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1413 2023-05-09 18:54:42.000000 starrail-toolkit-0.5.4/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.754623 starrail-toolkit-0.5.4/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    12878 2023-05-09 18:43:38.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2520 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3700 2023-05-09 19:03:50.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.755097 starrail-toolkit-0.5.4/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5401 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.755462 starrail-toolkit-0.5.4/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      937 2023-05-09 18:39:18.000000 starrail-toolkit-0.5.4/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.756207 starrail-toolkit-0.5.4/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2823 2023-05-09 19:03:15.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6502 2023-05-09 19:03:15.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.4/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-09 19:05:00.000000 starrail-toolkit-0.5.4/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-09 19:05:30.756935 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5041 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1473 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-09 19:05:30.000000 starrail-toolkit-0.5.4/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.5.3/LICENSE` & `starrail-toolkit-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/PKG-INFO` & `starrail-toolkit-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.3
+Version: 0.5.4
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,32 +20,34 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.3    |    0.5.3     |   0.5.3   |
+|   0.5.4    |    0.5.4     |   0.5.4   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
-- [ ] 实现用户界面并编译到 Windows 与 macOS 平台
+- [x] 实现用户界面并编译到 Windows 平台
 - [x] 支持自动检查更新
 
-***BREAKING：目前用户界面的第一个版本已经实现完成，稍后将会编译到 Windows 平台，界面预览：***
+## 安装方式
 
-![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+### 下载可执行程序
 
-## 安装方式
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i3GIq0v3hbbe)，两种途径的内容相同，可以自行选择下载方式。
 
-目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
+***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
+
+![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
@@ -57,15 +59,15 @@
 
 ```shell
 git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
 cd honkai-starrail-toolkit
 python3 setup.py install
 ```
 
-## 使用指南
+##  命令行使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
```

### Comparing `starrail-toolkit-0.5.3/README.md` & `starrail-toolkit-0.5.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.3    |    0.5.3     |   0.5.3   |
+|   0.5.4    |    0.5.4     |   0.5.4   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
-- [ ] 实现用户界面并编译到 Windows 与 macOS 平台
+- [x] 实现用户界面并编译到 Windows 平台
 - [x] 支持自动检查更新
 
-***BREAKING：目前用户界面的第一个版本已经实现完成，稍后将会编译到 Windows 平台，界面预览：***
+## 安装方式
 
-![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+### 下载可执行程序
 
-## 安装方式
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i3GIq0v3hbbe)，两种途径的内容相同，可以自行选择下载方式。
 
-目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
+***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
+
+![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
@@ -42,15 +44,15 @@
 
 ```shell
 git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
 cd honkai-starrail-toolkit
 python3 setup.py install
 ```
 
-## 使用指南
+##  命令行使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
```

### Comparing `starrail-toolkit-0.5.3/setup.py` & `starrail-toolkit-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/__init__.py` & `starrail-toolkit-0.5.4/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/config.py` & `starrail-toolkit-0.5.4/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/entry/cli.py` & `starrail-toolkit-0.5.4/starrail/entry/cli.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/entry/gui.py` & `starrail-toolkit-0.5.4/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/entry/setup.py` & `starrail-toolkit-0.5.4/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gacha/autodet.py` & `starrail-toolkit-0.5.4/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gacha/database.py` & `starrail-toolkit-0.5.4/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gacha/fetch.py` & `starrail-toolkit-0.5.4/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gacha/fileio.py` & `starrail-toolkit-0.5.4/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gacha/parse.py` & `starrail-toolkit-0.5.4/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gacha/service.py` & `starrail-toolkit-0.5.4/starrail/gacha/service.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gacha/url.py` & `starrail-toolkit-0.5.4/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gui/application.py` & `starrail-toolkit-0.5.4/starrail/gui/application.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-import traceback
-
 import qfluentwidgets
 from PySide6.QtCore import QEasingCurve, Qt, Signal
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QApplication, QFrame, QHBoxLayout, QWidget
 from qfluentwidgets import NavigationInterface, NavigationItemPosition
 from qframelesswindow import FramelessWindow
 
-from starrail import __version__, digital_version
-from starrail.config import configuration as cfg
 from starrail.gui.common.icon import Icon
 from starrail.gui.common.stylesheet import StyleSheet
+from starrail.gui.common.utils import checkUpdate
 from starrail.gui.interfaces.gacha_sync import GachaSyncInterface
 from starrail.gui.interfaces.home import HomeInterface
 from starrail.gui.interfaces.setting import SettingInterface
 from starrail.gui.interfaces.users import UsersInterface
-from starrail.gui.widgets.dialog import CheckUpdateDialog
 from starrail.gui.widgets.title_bar import CustomTitleBar
 from starrail.utils import babelfish
-from starrail.utils.auto_update import check_update
 
 
 class StackedWidget(QFrame):
 
     currentWidgetChanged = Signal(QWidget)
 
     def __init__(self, parent=None):
@@ -98,41 +93,41 @@
         self.titleBar.raise_()
 
     def initNavigation(self):
         self.addSubInterface(
             self.homeInterface,
             'homeInterface',
             qfluentwidgets.FluentIcon.HOME,
-            'Home',
+            babelfish.ui_welcome(),
             NavigationItemPosition.TOP,
         )
 
         self.navigationInterface.addSeparator()
 
         self.addSubInterface(
             self.gachaSyncInterface,
             'gachaSyncInterface',
             qfluentwidgets.FluentIcon.SYNC,
-            'Gacha Sync',
+            babelfish.ui_gacha_sync(),
             NavigationItemPosition.TOP,
         )
 
         self.addSubInterface(
             self.usersInterface,
             'usersInterface',
             Icon.USER,
-            'Users',
+            babelfish.ui_users(),
             NavigationItemPosition.BOTTOM,
         )
 
         self.addSubInterface(
             self.settingInterface,
             'settingInterface',
             qfluentwidgets.FluentIcon.SETTING,
-            'Settings',
+            babelfish.ui_settings(),
             NavigationItemPosition.BOTTOM,
         )
 
         self.navigationInterface.setDefaultRouteKey(
             self.homeInterface.objectName(),
         )
         self.stackWidget.currentWidgetChanged.connect(
@@ -180,33 +175,8 @@
         StyleSheet.STAR_RAIL_TOOLKIT.apply(self)
 
     def resizeEvent(self, _):
         self.titleBar.move(46, 0)
         self.titleBar.resize(self.width() - 46, self.titleBar.height())
 
     def afterShow(self):
-        self.checkUpdate()
-
-    def checkUpdate(self):
-        if cfg.check_update:
-            try:
-                latest = check_update()
-                current = digital_version(__version__)
-                if current < digital_version(latest.version):
-                    dialog = CheckUpdateDialog(
-                        title=babelfish.ui_update_available(),
-                        content=babelfish.ui_update_desc(latest.changelog),
-                        parent=self,
-                        dist=latest.dist,
-                    )
-                    dialog.show()
-                    dialog.raise_()
-            except Exception:
-                traceback.print_exc()
-                dialog = CheckUpdateDialog(
-                    title=babelfish.ui_ooops(),
-                    content=babelfish.ui_check_update_fail(),
-                    parent=self,
-                    dist=None,
-                )
-                dialog.show()
-                dialog.raise_()
+        checkUpdate(self)
```

### Comparing `starrail-toolkit-0.5.3/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.5.4/starrail/gui/common/stylesheet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.5.4/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.5.4/starrail/gui/interfaces/gacha_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import time
 import traceback
 from typing import List
 
 import qfluentwidgets as qfw
 from PySide6 import QtWidgets
-from PySide6.QtCore import QEvent, QObject, Qt, QThread, Signal
+from PySide6.QtCore import Qt, QThread, Signal
 from PySide6.QtWidgets import QLabel, QTableWidgetItem, QVBoxLayout
 
 import starrail.gacha.service as service
 from starrail.config import configuration as cfg
 from starrail.gacha.type import GachaType
 from starrail.gui.common.stylesheet import StyleSheet
 from starrail.gui.common.utils import get_current_uid
@@ -174,19 +174,14 @@
     def setTableData(self, data: List[List[str]]):
         # data: 3x5
         logger.debug(f'[GUI] {data}')
         for idx0, row in enumerate(data):
             for idx1, item in enumerate(row):
                 self.table.setItem(idx0, idx1, QTableWidgetItem(item))
 
-    def eventFilter(self, watched: QObject, event: QEvent) -> bool:
-        if event is QEvent.Type.Scroll:
-            self.parent().eventFilter(watched, event)
-        return super().eventFilter(watched, event)
-
 
 class GachaSyncInterface(BaseInterface):
 
     def __init__(self, title, subtitle, parent):
         super().__init__(title, subtitle, parent)
 
         # Buttons
```

### Comparing `starrail-toolkit-0.5.3/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.5.4/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gui/widgets/dialog.py` & `starrail-toolkit-0.5.4/starrail/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gui/widgets/link_card.py` & `starrail-toolkit-0.5.4/starrail/gui/widgets/link_card.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.5.4/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/utils/auto_update.py` & `starrail-toolkit-0.5.4/starrail/utils/auto_update.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import easydict
 
 from starrail.gacha.fetch import fetch_json
 
 user = 'LittleNyima'
 repo = 'honkai-starrail-toolkit'
 branch = 'master'
-cdn_templ = fr'https://cdn.jsdelivr.net/gh/{user}/{repo}@{branch}/'
-# version = fr'{cdn_templ}releases/version.txt'
-distribution = fr'{cdn_templ}releases/dist.json'
+cdn_templ = dict(
+    gitee=fr'https://gitee.com/{user}/{repo}-mirror/raw/{branch}/',
+    github=fr'https://raw.githubusercontent.com/{user}/{repo}/{branch}/',
+    jsdelivr=fr'https://cdn.jsdelivr.net/gh/{user}/{repo}@{branch}/',
+)
+# jsdelivr is deprecated due to untimely synchronization
 
 
 """
 Distribution JSON Format:
 {
     'version': 'the-latest-version',
     'dist': {
@@ -19,16 +22,18 @@
         'name-2': 'url-2',
     },
     'changelog': 'desc'
 }
 """
 
 
-def get_distribution():
+def get_distribution(cdn_type):
+    distribution = fr'{cdn_templ[cdn_type]}releases/dist.json'
     return fetch_json(distribution)
 
 
 def check_update():
-    payload, _ = get_distribution()
-    if payload is not None:
-        return easydict.EasyDict(payload)
+    for cdn_type in ['github', 'gitee']:
+        payload, _ = get_distribution(cdn_type)
+        if payload is not None:
+            return easydict.EasyDict(payload)
     return None
```

### Comparing `starrail-toolkit-0.5.3/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.5.4/starrail/utils/babelfish/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 average_gacha_per_5_star = dictionary.average_gacha_per_5_star
 gacha_report = dictionary.gacha_report
 gacha_title = dictionary.gacha_title
 history_of_5_stars = dictionary.history_of_5_stars
 html_thead = dictionary.html_thead
 markdown_thead = dictionary.markdown_thead
 ui_about = dictionary.ui_about
+ui_about_this = dictionary.ui_about_this
 ui_cancel_update = dictionary.ui_cancel_update
+ui_check_update = dictionary.ui_check_update
 ui_check_update_fail = dictionary.ui_check_update_fail
+ui_copyright = dictionary.ui_copyright
+ui_current_version = dictionary.ui_current_version
 ui_downloading_gacha = dictionary.ui_downloading_gacha
 ui_extract_api_fail = dictionary.ui_extract_api_fail
 ui_extracting_api_url = dictionary.ui_extracting_api_url
 ui_fine = dictionary.ui_fine
 ui_fine1 = dictionary.ui_fine1
 ui_fine2 = dictionary.ui_fine2
 ui_gacha_basic_prob = dictionary.ui_gacha_basic_prob
@@ -30,14 +34,16 @@
 ui_github_repo = dictionary.ui_github_repo
 ui_github_repo_desc = dictionary.ui_github_repo_desc
 ui_no_data = dictionary.ui_no_data
 ui_not_good = dictionary.ui_not_good
 ui_ooops = dictionary.ui_ooops
 ui_open_docs = dictionary.ui_open_docs
 ui_open_issues = dictionary.ui_open_issues
+ui_open_repo = dictionary.ui_open_repo
+ui_open_troubleshooting = dictionary.ui_open_troubleshooting
 ui_personalization = dictionary.ui_personalization
 ui_save_data = dictionary.ui_save_data
 ui_save_success = dictionary.ui_save_success
 ui_save_success_msg = dictionary.ui_save_success_msg
 ui_send_feedback = dictionary.ui_send_feedback
 ui_send_feedback_desc = dictionary.ui_send_feedback_desc
 ui_settings = dictionary.ui_settings
@@ -51,9 +57,10 @@
 ui_troubleshooting = dictionary.ui_troubleshooting
 ui_troubleshooting_desc = dictionary.ui_troubleshooting_desc
 ui_update_available = dictionary.ui_update_available
 ui_update_desc = dictionary.ui_update_desc
 ui_users = dictionary.ui_users
 ui_users_desc = dictionary.ui_users_desc
 ui_welcome = dictionary.ui_welcome
+ui_welcome = dictionary.ui_welcome
 
 __all__ = ['constants', 'translate']
```

### Comparing `starrail-toolkit-0.5.3/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.5.4/starrail/utils/babelfish/dictionary.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,19 +40,29 @@
     ),
     zhs=(
         '| 星级 | 数量 | 基础概率 | 综合概率 | 距上次 |\n'
         '| ---- | ---- | ------ | ------- | ---- |\n'
     ),
 )
 ui_about = _MS(en='About', zhs='关于')
+ui_about_this = _MS(en='About This Application', zhs='关于本软件')
 ui_cancel_update = _MS(en='Cancel Update', zhs='暂不更新')
+ui_check_update = _MS(en='Check Update', zhs='检查更新')
 ui_check_update_fail = _MS(
     en='Check update failed. Please check your network connection.',
     zhs='检查更新失败，请检查你的网络连接并重试。（不重试也行，但是你可能没联网）',
 )
+ui_copyright = _MS(
+    en='Copyright © {} LittleNyima.',
+    zhs='版权所有 © {} LittleNyima。',
+)
+ui_current_version = _MS(
+    en='Current version: {}.',
+    zhs='当前版本：{}。',
+)
 ui_downloading_gacha = _MS(
     en='Downloading page {page} of type {name}',
     zhs='正在导出{name}的第{page}页',
 )
 ui_extract_api_fail = _MS(
     en='Extracting API URL failed. Please retry after exiting the game.',
     zhs='提取 API URL 失败，请关闭游戏或重新查询抽卡信息后重试。',
@@ -88,14 +98,16 @@
     zhs='本项目代码开源，以 GPLv3 分发。点此查看源代码。',
 )
 ui_no_data = _MS(en='No Data', zhs='暂无数据')
 ui_not_good = _MS(en='No', zhs='不好')
 ui_ooops = _MS(en='OOOPS!', zhs='出错了！')
 ui_open_docs = _MS(en='Open Documentations', zhs='打开帮助页面')
 ui_open_issues = _MS(en='Open Issue Page', zhs='打开反馈页面')
+ui_open_repo = _MS(en='Open GitHub Repo', zhs='打开代码仓库')
+ui_open_troubleshooting = _MS(en='Open Troubleshooting', zhs='打开常见问题')
 ui_personalization = _MS(en='Personalization', zhs='个性化')
 ui_save_data = _MS(en='Save As', zhs='保存数据')
 ui_save_success = _MS(en='Data Save Success', zhs='保存成功')
 ui_save_success_msg = _MS(en='Data is saved to {}', zhs='数据已保存到{}')
 ui_send_feedback = _MS(en='Send Feedback', zhs='提交反馈')
 ui_send_feedback_desc = _MS(
     en='Feedback is welcome if you encounter problems or have suggestions.',
@@ -144,9 +156,10 @@
 )
 ui_users = _MS(en='Users', zhs='用户管理')
 ui_users_desc = _MS(en='Multi-user management', zhs='如果有多个账号可以用这个切换')
 ui_welcome = _MS(
     en='Welcome to HKSR Toolkit!',
     zhs='欢迎登车！',
 )
+ui_welcome = _MS(en='Welcome', zhs='欢迎页面')
 
 # === END OF PRE-DEFINED VOCABULARIES ===
```

### Comparing `starrail-toolkit-0.5.3/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.5.4/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail/utils/loggings.py` & `starrail-toolkit-0.5.4/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.3/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.5.4/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.3
+Version: 0.5.4
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,32 +20,34 @@
 </div>
 
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.5.3    |    0.5.3     |   0.5.3   |
+|   0.5.4    |    0.5.4     |   0.5.4   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
-- [ ] 实现用户界面并编译到 Windows 与 macOS 平台
+- [x] 实现用户界面并编译到 Windows 平台
 - [x] 支持自动检查更新
 
-***BREAKING：目前用户界面的第一个版本已经实现完成，稍后将会编译到 Windows 平台，界面预览：***
+## 安装方式
 
-![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
+### 下载可执行程序
 
-## 安装方式
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/i3GIq0v3hbbe)，两种途径的内容相同，可以自行选择下载方式。
 
-目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
+***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
+
+![gui_preview](https://s1.ax1x.com/2023/05/08/p90QWex.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
@@ -57,15 +59,15 @@
 
 ```shell
 git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
 cd honkai-starrail-toolkit
 python3 setup.py install
 ```
 
-## 使用指南
+##  命令行使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
```

### Comparing `starrail-toolkit-0.5.3/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.5.4/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

