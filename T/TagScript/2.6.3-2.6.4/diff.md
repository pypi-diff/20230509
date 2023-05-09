# Comparing `tmp/TagScript-2.6.3.tar.gz` & `tmp/TagScript-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TagScript-2.6.3.tar", last modified: Wed Jan 11 08:55:40 2023, max compression
+gzip compressed data, was "TagScript-2.6.4.tar", last modified: Tue May  9 05:10:40 2023, max compression
```

## Comparing `TagScript-2.6.3.tar` & `TagScript-2.6.4.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-01-11 08:55:40.990437 TagScript-2.6.3/
--rw-r--r--   0 manansingh   (503) staff       (20)      251 2021-07-14 04:25:01.000000 TagScript-2.6.3/LICENSE
--rw-r--r--   0 manansingh   (503) staff       (20)     2519 2023-01-11 08:55:40.990660 TagScript-2.6.3/PKG-INFO
--rw-r--r--   0 manansingh   (503) staff       (20)     1819 2023-01-11 08:50:21.000000 TagScript-2.6.3/README.md
-drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-01-11 08:55:40.977168 TagScript-2.6.3/TagScript.egg-info/
--rw-r--r--   0 manansingh   (503) staff       (20)     2519 2023-01-11 08:55:40.000000 TagScript-2.6.3/TagScript.egg-info/PKG-INFO
--rw-r--r--   0 manansingh   (503) staff       (20)     1500 2023-01-11 08:55:40.000000 TagScript-2.6.3/TagScript.egg-info/SOURCES.txt
--rw-r--r--   0 manansingh   (503) staff       (20)        1 2023-01-11 08:55:40.000000 TagScript-2.6.3/TagScript.egg-info/dependency_links.txt
--rw-r--r--   0 manansingh   (503) staff       (20)       28 2023-01-11 08:55:40.000000 TagScript-2.6.3/TagScript.egg-info/requires.txt
--rw-r--r--   0 manansingh   (503) staff       (20)       16 2023-01-11 08:55:40.000000 TagScript-2.6.3/TagScript.egg-info/top_level.txt
-drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-01-11 08:55:40.978507 TagScript-2.6.3/TagScriptEngine/
--rw-r--r--   0 manansingh   (503) staff       (20)     1247 2023-01-11 08:50:21.000000 TagScript-2.6.3/TagScriptEngine/__init__.py
-drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-01-11 08:55:40.980261 TagScript-2.6.3/TagScriptEngine/adapter/
--rw-r--r--   0 manansingh   (503) staff       (20)      386 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/adapter/__init__.py
--rw-r--r--   0 manansingh   (503) staff       (20)     6466 2023-01-11 08:50:21.000000 TagScript-2.6.3/TagScriptEngine/adapter/discordadapters.py
--rw-r--r--   0 manansingh   (503) staff       (20)      427 2021-10-14 22:14:35.000000 TagScript-2.6.3/TagScriptEngine/adapter/functionadapter.py
--rw-r--r--   0 manansingh   (503) staff       (20)      371 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/adapter/intadapter.py
--rw-r--r--   0 manansingh   (503) staff       (20)      789 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/adapter/objectadapter.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1511 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/adapter/stringadapter.py
-drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-01-11 08:55:40.988602 TagScript-2.6.3/TagScriptEngine/block/
--rw-r--r--   0 manansingh   (503) staff       (20)     1512 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/__init__.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1033 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/assign.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1111 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/breakblock.py
--rw-r--r--   0 manansingh   (503) staff       (20)     2756 2023-01-11 08:50:21.000000 TagScript-2.6.3/TagScriptEngine/block/command.py
--rw-r--r--   0 manansingh   (503) staff       (20)     5261 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/control.py
--rw-r--r--   0 manansingh   (503) staff       (20)     3728 2021-08-29 09:38:36.000000 TagScript-2.6.3/TagScriptEngine/block/cooldown.py
--rw-r--r--   0 manansingh   (503) staff       (20)     6688 2021-08-29 09:37:10.000000 TagScript-2.6.3/TagScriptEngine/block/embedblock.py
--rw-r--r--   0 manansingh   (503) staff       (20)      667 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/fiftyfifty.py
--rw-r--r--   0 manansingh   (503) staff       (20)     3003 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/helpers.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1073 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/loosevariablegetter.py
--rw-r--r--   0 manansingh   (503) staff       (20)     4831 2021-10-14 22:14:35.000000 TagScript-2.6.3/TagScriptEngine/block/mathblock.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1409 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/randomblock.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1963 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/range.py
--rw-r--r--   0 manansingh   (503) staff       (20)      959 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/redirect.py
--rw-r--r--   0 manansingh   (503) staff       (20)     2821 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/replaceblock.py
--rw-r--r--   0 manansingh   (503) staff       (20)     2530 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/require_blacklist.py
--rw-r--r--   0 manansingh   (503) staff       (20)      540 2021-05-05 02:40:22.000000 TagScript-2.6.3/TagScriptEngine/block/shortcutredirect.py
--rw-r--r--   0 manansingh   (503) staff       (20)      915 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/stopblock.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1847 2021-08-31 07:12:35.000000 TagScript-2.6.3/TagScriptEngine/block/strf.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1077 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/strictvariablegetter.py
--rw-r--r--   0 manansingh   (503) staff       (20)      614 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/substr.py
--rw-r--r--   0 manansingh   (503) staff       (20)     1222 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/block/urlencodeblock.py
--rw-r--r--   0 manansingh   (503) staff       (20)     2640 2021-10-14 22:14:35.000000 TagScript-2.6.3/TagScriptEngine/exceptions.py
-drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-01-11 08:55:40.990082 TagScript-2.6.3/TagScriptEngine/interface/
--rw-r--r--   0 manansingh   (503) staff       (20)      130 2021-07-14 04:25:01.000000 TagScript-2.6.3/TagScriptEngine/interface/__init__.py
--rw-r--r--   0 manansingh   (503) staff       (20)      991 2021-10-14 22:14:35.000000 TagScript-2.6.3/TagScriptEngine/interface/adapter.py
--rw-r--r--   0 manansingh   (503) staff       (20)     3253 2021-10-14 22:14:35.000000 TagScript-2.6.3/TagScriptEngine/interface/block.py
--rw-r--r--   0 manansingh   (503) staff       (20)    13450 2022-04-15 21:32:52.000000 TagScript-2.6.3/TagScriptEngine/interpreter.py
--rw-r--r--   0 manansingh   (503) staff       (20)      886 2023-01-11 08:50:19.000000 TagScript-2.6.3/TagScriptEngine/utils.py
--rw-r--r--   0 manansingh   (503) staff       (20)     4288 2021-07-14 10:21:50.000000 TagScript-2.6.3/TagScriptEngine/verb.py
--rw-r--r--   0 manansingh   (503) staff       (20)      170 2021-07-14 04:25:01.000000 TagScript-2.6.3/pyproject.toml
--rw-r--r--   0 manansingh   (503) staff       (20)      914 2023-01-11 08:55:40.991702 TagScript-2.6.3/setup.cfg
--rw-r--r--   0 manansingh   (503) staff       (20)       38 2021-07-14 04:25:01.000000 TagScript-2.6.3/setup.py
+drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-05-09 05:10:40.590874 TagScript-2.6.4/
+-rw-r--r--   0 manansingh   (503) staff       (20)      251 2021-07-14 04:25:01.000000 TagScript-2.6.4/LICENSE
+-rw-r--r--   0 manansingh   (503) staff       (20)     2519 2023-05-09 05:10:40.591073 TagScript-2.6.4/PKG-INFO
+-rw-r--r--   0 manansingh   (503) staff       (20)     1819 2023-05-09 05:00:46.000000 TagScript-2.6.4/README.md
+drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-05-09 05:10:40.572322 TagScript-2.6.4/TagScript.egg-info/
+-rw-r--r--   0 manansingh   (503) staff       (20)     2519 2023-05-09 05:10:40.000000 TagScript-2.6.4/TagScript.egg-info/PKG-INFO
+-rw-r--r--   0 manansingh   (503) staff       (20)     1608 2023-05-09 05:10:40.000000 TagScript-2.6.4/TagScript.egg-info/SOURCES.txt
+-rw-r--r--   0 manansingh   (503) staff       (20)        1 2023-05-09 05:10:40.000000 TagScript-2.6.4/TagScript.egg-info/dependency_links.txt
+-rw-r--r--   0 manansingh   (503) staff       (20)       28 2023-05-09 05:10:40.000000 TagScript-2.6.4/TagScript.egg-info/requires.txt
+-rw-r--r--   0 manansingh   (503) staff       (20)       16 2023-05-09 05:10:40.000000 TagScript-2.6.4/TagScript.egg-info/top_level.txt
+drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-05-09 05:10:40.573932 TagScript-2.6.4/TagScriptEngine/
+-rw-r--r--   0 manansingh   (503) staff       (20)     1247 2023-05-09 05:09:34.000000 TagScript-2.6.4/TagScriptEngine/__init__.py
+drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-05-09 05:10:40.576024 TagScript-2.6.4/TagScriptEngine/adapter/
+-rw-r--r--   0 manansingh   (503) staff       (20)      386 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/adapter/__init__.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     6693 2023-05-09 05:03:52.000000 TagScript-2.6.4/TagScriptEngine/adapter/discordadapters.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      427 2021-10-14 22:14:35.000000 TagScript-2.6.4/TagScriptEngine/adapter/functionadapter.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      371 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/adapter/intadapter.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      789 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/adapter/objectadapter.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1511 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/adapter/stringadapter.py
+drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-05-09 05:10:40.586291 TagScript-2.6.4/TagScriptEngine/block/
+-rw-r--r--   0 manansingh   (503) staff       (20)     1512 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/__init__.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1033 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/assign.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1111 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/breakblock.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     2756 2023-05-09 05:00:46.000000 TagScript-2.6.4/TagScriptEngine/block/command.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     5261 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/control.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     3728 2021-08-29 09:38:36.000000 TagScript-2.6.4/TagScriptEngine/block/cooldown.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     7006 2023-05-09 05:00:46.000000 TagScript-2.6.4/TagScriptEngine/block/embedblock.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      667 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/fiftyfifty.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     3014 2023-05-09 05:00:46.000000 TagScript-2.6.4/TagScriptEngine/block/helpers.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1073 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/loosevariablegetter.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     4924 2023-05-09 05:00:46.000000 TagScript-2.6.4/TagScriptEngine/block/mathblock.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1409 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/randomblock.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1963 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/range.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      959 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/redirect.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     2821 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/replaceblock.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     2530 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/require_blacklist.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      540 2021-05-05 02:40:22.000000 TagScript-2.6.4/TagScriptEngine/block/shortcutredirect.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      915 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/stopblock.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1847 2021-08-31 07:12:35.000000 TagScript-2.6.4/TagScriptEngine/block/strf.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1077 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/strictvariablegetter.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      614 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/substr.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     1222 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/block/urlencodeblock.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     2640 2021-10-14 22:14:35.000000 TagScript-2.6.4/TagScriptEngine/exceptions.py
+drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-05-09 05:10:40.587614 TagScript-2.6.4/TagScriptEngine/interface/
+-rw-r--r--   0 manansingh   (503) staff       (20)      130 2021-07-14 04:25:01.000000 TagScript-2.6.4/TagScriptEngine/interface/__init__.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      991 2023-05-09 05:00:46.000000 TagScript-2.6.4/TagScriptEngine/interface/adapter.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     3253 2023-05-09 05:00:46.000000 TagScript-2.6.4/TagScriptEngine/interface/block.py
+-rw-r--r--   0 manansingh   (503) staff       (20)    13450 2022-04-15 21:32:52.000000 TagScript-2.6.4/TagScriptEngine/interpreter.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      992 2023-05-09 05:00:41.000000 TagScript-2.6.4/TagScriptEngine/utils.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     4288 2021-07-14 10:21:50.000000 TagScript-2.6.4/TagScriptEngine/verb.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      170 2021-07-14 04:25:01.000000 TagScript-2.6.4/pyproject.toml
+-rw-r--r--   0 manansingh   (503) staff       (20)      914 2023-05-09 05:10:40.592019 TagScript-2.6.4/setup.cfg
+-rw-r--r--   0 manansingh   (503) staff       (20)       38 2021-07-14 04:25:01.000000 TagScript-2.6.4/setup.py
+drwxr-xr-x   0 manansingh   (503) staff       (20)        0 2023-05-09 05:10:40.590395 TagScript-2.6.4/tests/
+-rw-r--r--   0 manansingh   (503) staff       (20)     1232 2021-07-14 04:25:01.000000 TagScript-2.6.4/tests/test_adapters.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      667 2021-07-14 04:25:01.000000 TagScript-2.6.4/tests/test_basic.py
+-rw-r--r--   0 manansingh   (503) staff       (20)    14539 2021-07-14 04:25:01.000000 TagScript-2.6.4/tests/test_edgecase.py
+-rw-r--r--   0 manansingh   (503) staff       (20)      801 2021-05-05 02:22:42.000000 TagScript-2.6.4/tests/test_escapes.py
+-rw-r--r--   0 manansingh   (503) staff       (20)     3942 2021-07-14 04:25:01.000000 TagScript-2.6.4/tests/test_verbs.py
```

### Comparing `TagScript-2.6.3/PKG-INFO` & `TagScript-2.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TagScript
-Version: 2.6.3
+Version: 2.6.4
 Summary: An easy drop in user-provided Templating system.
 Home-page: https://github.com/phenom4n4n/TagScript
 Author: PhenoM4n4n
 Author-email: noumenondiscord@gmail.com
 License: Creative Commons Attribution 4.0 International License
 Keywords: tagscript
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TagScript Version: 2.6.3 Summary: An easy drop in
+Metadata-Version: 2.1 Name: TagScript Version: 2.6.4 Summary: An easy drop in
 user-provided Templating system. Home-page: https://github.com/phenom4n4n/
 TagScript Author: PhenoM4n4n Author-email: noumenondiscord@gmail.com License:
 Creative Commons Attribution 4.0 International License Keywords: tagscript
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: Freely Distributable Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3.8
```

### Comparing `TagScript-2.6.3/README.md` & `TagScript-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScript.egg-info/PKG-INFO` & `TagScript-2.6.4/TagScript.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TagScript
-Version: 2.6.3
+Version: 2.6.4
 Summary: An easy drop in user-provided Templating system.
 Home-page: https://github.com/phenom4n4n/TagScript
 Author: PhenoM4n4n
 Author-email: noumenondiscord@gmail.com
 License: Creative Commons Attribution 4.0 International License
 Keywords: tagscript
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TagScript Version: 2.6.3 Summary: An easy drop in
+Metadata-Version: 2.1 Name: TagScript Version: 2.6.4 Summary: An easy drop in
 user-provided Templating system. Home-page: https://github.com/phenom4n4n/
 TagScript Author: PhenoM4n4n Author-email: noumenondiscord@gmail.com License:
 Creative Commons Attribution 4.0 International License Keywords: tagscript
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: Freely Distributable Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3.8
```

### Comparing `TagScript-2.6.3/TagScript.egg-info/SOURCES.txt` & `TagScript-2.6.4/TagScript.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -39,8 +39,13 @@
 TagScriptEngine/block/stopblock.py
 TagScriptEngine/block/strf.py
 TagScriptEngine/block/strictvariablegetter.py
 TagScriptEngine/block/substr.py
 TagScriptEngine/block/urlencodeblock.py
 TagScriptEngine/interface/__init__.py
 TagScriptEngine/interface/adapter.py
-TagScriptEngine/interface/block.py
+TagScriptEngine/interface/block.py
+tests/test_adapters.py
+tests/test_basic.py
+tests/test_edgecase.py
+tests/test_escapes.py
+tests/test_verbs.py
```

### Comparing `TagScript-2.6.3/TagScriptEngine/__init__.py` & `TagScript-2.6.4/TagScriptEngine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .block import *
 from .exceptions import *
 from .interface import *
 from .interpreter import *
 from .utils import *
 from .verb import Verb
 
-__version__ = "2.6.3"
+__version__ = "2.6.4"
 
 
 class VersionInfo(namedtuple("VersionInfo", "major minor micro")):
     """
     Version information.
 
     Attributes
```

### Comparing `TagScript-2.6.3/TagScriptEngine/adapter/discordadapters.py` & `TagScript-2.6.4/TagScriptEngine/adapter/discordadapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from random import choice
 
-from discord import TextChannel
+import discord
 
 from ..interface import Adapter
-from ..utils import escape_content
+from ..utils import DPY2, escape_content
 from ..verb import Verb
 
 __all__ = (
     "AttributeAdapter",
     "MemberAdapter",
     "ChannelAdapter",
     "GuildAdapter",
@@ -15,18 +15,19 @@
 
 
 class AttributeAdapter(Adapter):
     __slots__ = ("object", "_attributes", "_methods")
 
     def __init__(self, base):
         self.object = base
+        created_at = getattr(base, "created_at", None) or discord.utils.snowflake_time(base.id)
         self._attributes = {
             "id": base.id,
-            "created_at": base.created_at,
-            "timestamp": int(base.created_at.timestamp()),
+            "created_at": created_at,
+            "timestamp": int(created_at.timestamp()),
             "name": getattr(base, "name", str(base)),
         }
         self._methods = {}
         self.update_attributes()
         self.update_methods()
 
     def __repr__(self):
@@ -103,26 +104,27 @@
     top_role
         The author's top role.
     roleids
         A list of the author's role IDs, split by spaces.
     """
 
     def update_attributes(self):
+        avatar_url = self.object.display_avatar.url if DPY2 else self.object.avatar_url
         joined_at = getattr(self.object, "joined_at", self.object.created_at)
         additional_attributes = {
             "color": self.object.color,
             "colour": self.object.color,
             "nick": self.object.display_name,
-            "avatar": (self.object.avatar_url, False),
+            "avatar": (avatar_url, False),
             "discriminator": self.object.discriminator,
             "joined_at": joined_at,
             "joinstamp": int(joined_at.timestamp()),
             "mention": self.object.mention,
             "bot": self.object.bot,
-            "top_role": getattr(self.object, "top_role", None),
+            "top_role": getattr(self.object, "top_role", ""),
         }
         if roleids := getattr(self.object, "_roles", None):
             additional_attributes["roleids"] = " ".join(str(r) for r in roleids)
         self._attributes.update(additional_attributes)
 
 
 class ChannelAdapter(AttributeAdapter):
@@ -152,19 +154,19 @@
     mention
         A formatted text that pings the channel.
     topic
         The channel's topic.
     """
 
     def update_attributes(self):
-        if isinstance(self.object, TextChannel):
+        if isinstance(self.object, discord.TextChannel):
             additional_attributes = {
                 "nsfw": self.object.nsfw,
                 "mention": self.object.mention,
-                "topic": self.object.topic or None,
+                "topic": self.object.topic or "",
             }
             self._attributes.update(additional_attributes)
 
 
 class GuildAdapter(AttributeAdapter):
     """
     The ``{server}`` block with no parameters returns the server's name
@@ -209,16 +211,17 @@
         humans = 0
         for m in guild.members:
             if m.bot:
                 bots += 1
             else:
                 humans += 1
         member_count = guild.member_count
+        icon_url = getattr(guild.icon, "url", "") if DPY2 else guild.icon_url
         additional_attributes = {
-            "icon": (guild.icon_url, False),
+            "icon": (icon_url, False),
             "member_count": member_count,
             "members": member_count,
             "bots": bots,
             "humans": humans,
             "description": guild.description or "No description.",
         }
         self._attributes.update(additional_attributes)
```

### Comparing `TagScript-2.6.3/TagScriptEngine/adapter/objectadapter.py` & `TagScript-2.6.4/TagScriptEngine/adapter/objectadapter.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/adapter/stringadapter.py` & `TagScript-2.6.4/TagScriptEngine/adapter/stringadapter.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/__init__.py` & `TagScript-2.6.4/TagScriptEngine/block/__init__.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/assign.py` & `TagScript-2.6.4/TagScriptEngine/block/assign.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/breakblock.py` & `TagScript-2.6.4/TagScriptEngine/block/breakblock.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/command.py` & `TagScript-2.6.4/TagScriptEngine/block/command.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/control.py` & `TagScript-2.6.4/TagScriptEngine/block/control.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/cooldown.py` & `TagScript-2.6.4/TagScriptEngine/block/cooldown.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/embedblock.py` & `TagScript-2.6.4/TagScriptEngine/block/embedblock.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,30 +35,38 @@
 
 def set_dynamic_url(embed: Embed, attribute: str, value: str):
     method = getattr(embed, f"set_{attribute}")
     method(url=value)
 
 
 def add_field(embed: Embed, _: str, payload: str):
+    if (data := helper_split(payload, 3)) is None:
+        raise EmbedParseError("`add_field` payload was not split by |")
     try:
-        name, value, _inline = helper_split(payload, 3)
+        name, value, _inline = data
         inline = implicit_bool(_inline)
         if inline is None:
             raise EmbedParseError(
-                f"`inline` argument for `add_field` is not a boolean value (_inline)"
+                "`inline` argument for `add_field` is not a boolean value (_inline)"
             )
     except ValueError:
-        try:
-            name, value = helper_split(payload, 2)
-        except ValueError as exc:
-            raise EmbedParseError("`add_field` payload was not split by |") from exc
+        name, value = helper_split(payload, 2)
         inline = False
     embed.add_field(name=name, value=value, inline=inline)
 
 
+def set_footer(embed: Embed, _: str, payload: str):
+    data = helper_split(payload, 2)
+    if data is None:
+        embed.set_footer(text=payload)
+    else:
+        text, icon_url = data
+        embed.set_footer(text=text, icon_url=icon_url)
+
+
 class EmbedBlock(Block):
     """
     An embed block will send an embed in the tag response.
     There are two ways to use the embed block, either by using properly
     formatted embed JSON from an embed generator or manually inputting
     the accepted embed attributes.
 
@@ -89,14 +97,15 @@
 
     *   ``title``
     *   ``description``
     *   ``color``
     *   ``url``
     *   ``thumbnail``
     *   ``image``
+    *   ``footer``
     *   ``field`` - (See below)
 
     Adding a field to an embed requires the payload to be split by ``|``, into
     either 2 or 3 parts. The first part is the name of the field, the second is
     the text of the field, and the third optionally specifies whether the field
     should be inline.
 
@@ -108,14 +117,15 @@
 
     **Examples:** ::
 
         {embed(color):#37b2cb}
         {embed(title):Rules}
         {embed(description):Follow these rules to ensure a good experience in our server!}
         {embed(field):Rule 1|Respect everyone you speak to.|false}
+        {embed(footer):Thanks for reading!|{guild(icon)}}
 
     Both methods can be combined to create an embed in a tag.
     The following tagscript uses JSON to create an embed with fields and later
     set the embed title.
 
     ::
 
@@ -130,14 +140,15 @@
         "title": setattr,
         "color": set_color,
         "colour": set_color,
         "url": setattr,
         "thumbnail": set_dynamic_url,
         "image": set_dynamic_url,
         "field": add_field,
+        "footer": set_footer,
     }
 
     @staticmethod
     def get_embed(ctx: Context) -> Embed:
         return ctx.response.actions.get("embed", Embed())
 
     @staticmethod
```

### Comparing `TagScript-2.6.3/TagScriptEngine/block/fiftyfifty.py` & `TagScript-2.6.4/TagScriptEngine/block/fiftyfifty.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/helpers.py` & `TagScript-2.6.4/TagScriptEngine/block/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,19 @@
 
     >>> helper_split("this, should|work")
     ["this, should", "work"]
     """
     args = (maxsplit,) if maxsplit is not None else ()
     if "|" in split_string:
         return SPLIT_REGEX.split(split_string, *args)
-    if easy and "~" in split_string:
-        return split_string.split("~", *args)
-    if easy and "," in split_string:
-        return split_string.split(",", *args)
+    if easy:
+        if "~" in split_string:
+            return split_string.split("~", *args)
+        if "," in split_string:
+            return split_string.split(",", *args)
     return
 
 
 def helper_parse_list_if(if_string):
     split = helper_split(if_string, False)
     if split is None:
         return [helper_parse_if(if_string)]
```

### Comparing `TagScript-2.6.3/TagScriptEngine/block/loosevariablegetter.py` & `TagScript-2.6.4/TagScriptEngine/block/loosevariablegetter.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/mathblock.py` & `TagScript-2.6.4/TagScriptEngine/block/mathblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
             "^": operator.pow,
             "%": operator.mod,
         }
         self.fn = {
             "sin": math.sin,
             "cos": math.cos,
             "tan": math.tan,
+            "sinh": math.sinh,
+            "cosh": math.cosh,
+            "tanh": math.tanh,
             "exp": math.exp,
             "abs": abs,
             "trunc": lambda a: int(a),
             "round": round,
             "sgn": lambda a: abs(a) > epsilon and ((a > 0) - (a < 0)) or 0,
             "log": lambda a: math.log(a, 10),
             "ln": math.log,
```

### Comparing `TagScript-2.6.3/TagScriptEngine/block/randomblock.py` & `TagScript-2.6.4/TagScriptEngine/block/randomblock.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/range.py` & `TagScript-2.6.4/TagScriptEngine/block/range.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/redirect.py` & `TagScript-2.6.4/TagScriptEngine/block/redirect.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/replaceblock.py` & `TagScript-2.6.4/TagScriptEngine/block/replaceblock.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/require_blacklist.py` & `TagScript-2.6.4/TagScriptEngine/block/require_blacklist.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/shortcutredirect.py` & `TagScript-2.6.4/TagScriptEngine/block/shortcutredirect.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/stopblock.py` & `TagScript-2.6.4/TagScriptEngine/block/stopblock.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/strf.py` & `TagScript-2.6.4/TagScriptEngine/block/strf.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/strictvariablegetter.py` & `TagScript-2.6.4/TagScriptEngine/block/strictvariablegetter.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/substr.py` & `TagScript-2.6.4/TagScriptEngine/block/substr.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/block/urlencodeblock.py` & `TagScript-2.6.4/TagScriptEngine/block/urlencodeblock.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/exceptions.py` & `TagScript-2.6.4/TagScriptEngine/exceptions.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/interface/adapter.py` & `TagScript-2.6.4/TagScriptEngine/interface/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     from ..interpreter import Context
 
 
 class Adapter:
     """
```

### Comparing `TagScript-2.6.3/TagScriptEngine/interface/block.py` & `TagScript-2.6.4/TagScriptEngine/interface/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from functools import lru_cache
-from typing import Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     from ..interpreter import Context
 
 
 __all__ = ("Block", "verb_required_block")
```

### Comparing `TagScript-2.6.3/TagScriptEngine/interpreter.py` & `TagScript-2.6.4/TagScriptEngine/interpreter.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/TagScriptEngine/utils.py` & `TagScript-2.6.4/TagScriptEngine/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import re
 from inspect import isawaitable
-from typing import Any, Awaitable, Callable, Union
+from typing import Any, Awaitable, Callable, T, TypeVar, Union
 
-__all__ = ("escape_content", "maybe_await")
+import discord
+
+__all__ = ("escape_content", "maybe_await", "DPY2")
+
+T = TypeVar("T")
+
+DPY2 = discord.version_info >= (2, 0, 0, "alpha", 0)
 
 pattern = re.compile(r"(?<!\\)([{():|}])")
 
 
 def _sub_match(match: re.Match) -> str:
-    return "\\" + match.group(1)
+    return "\\" + match[1]
 
 
 def escape_content(string: str) -> str:
     """
     Escapes given input to avoid tampering with engine/block behavior.
 
     Returns
@@ -21,15 +27,15 @@
         The escaped content.
     """
     if string is None:
         return
     return pattern.sub(_sub_match, string)
 
 
-async def maybe_await(func: Union[Callable[..., Any], Awaitable[Any]], *args, **kwargs) -> Any:
+async def maybe_await(func: Callable[..., Union[T, Awaitable[T]]], *args: Any, **kwargs: Any) -> T:
     """
     Await the given function if it is awaitable or call it synchronously.
 
     Returns
     -------
     Any
         The result of the awaitable function.
```

### Comparing `TagScript-2.6.3/TagScriptEngine/verb.py` & `TagScript-2.6.4/TagScriptEngine/verb.py`

 * *Files identical despite different names*

### Comparing `TagScript-2.6.3/setup.cfg` & `TagScript-2.6.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 keywords = tagscript,
 
 [options]
 packages = find_namespace:
 install_requires = 
-	discord.py==1.7.3
+	discord.py==2.2.3
 	pyparsing
 python_requires = >=3.8
 
 [options.packages.find]
 include = 
 	TagScriptEngine
 	TagScriptEngine.*
```

