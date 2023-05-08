# Comparing `tmp/discoger-1.1.4.tar.gz` & `tmp/discoger-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.1.4.tar", last modified: Mon May  8 21:28:04 2023, max compression
+gzip compressed data, was "discoger-1.1.5.tar", last modified: Mon May  8 22:04:39 2023, max compression
```

## Comparing `discoger-1.1.4.tar` & `discoger-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:28:04.155207 discoger-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 21:27:48.000000 discoger-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-08 21:28:04.155207 discoger-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-08 21:27:48.000000 discoger-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:28:04.155207 discoger-1.1.4/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:27:48.000000 discoger-1.1.4/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 21:27:48.000000 discoger-1.1.4/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-05-08 21:27:48.000000 discoger-1.1.4/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:28:04.155207 discoger-1.1.4/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 21:28:04.000000 discoger-1.1.4/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 21:28:04.155207 discoger-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 21:27:48.000000 discoger-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:04:39.417441 discoger-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 22:04:22.000000 discoger-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-08 22:04:39.417441 discoger-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-08 22:04:22.000000 discoger-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:04:39.417441 discoger-1.1.5/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:04:22.000000 discoger-1.1.5/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 22:04:22.000000 discoger-1.1.5/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-08 22:04:22.000000 discoger-1.1.5/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:04:39.417441 discoger-1.1.5/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 22:04:39.000000 discoger-1.1.5/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 22:04:39.417441 discoger-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-08 22:04:22.000000 discoger-1.1.5/setup.py
```

### Comparing `discoger-1.1.4/LICENSE` & `discoger-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.1.4/PKG-INFO` & `discoger-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.4
+Version: 1.1.5
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.4.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.5.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.4/README.md` & `discoger-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `discoger-1.1.4/discoger/discoger.py` & `discoger-1.1.5/discoger/discoger.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
 def process_delete_step(message):
     chat_id = message.chat.id
     id_item = message.text
     db = YamlDB(filename="%s/.config/discoger/databases/%s.yaml" % (home, chat_id))
     db["release_list"].pop(int(id_item))
     db.save()
-    bot.send_message(chat_id, "% is deleted in following list" % (id_item))
+    bot.send_message(chat_id, "%s is deleted in following list" % (id_item))
 
 
 def get_info(release_id, type_sell):
     data_last_sell = dict()
     if type_sell == 'master':
         url = f"{discogs_url}/sell/mplistrss?output=rss&master_id={release_id}&ev=mb&format=Vinyl"
     else:
```

### Comparing `discoger-1.1.4/discoger.egg-info/PKG-INFO` & `discoger-1.1.5/discoger.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.4
+Version: 1.1.5
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.4.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.1.5.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
```

### Comparing `discoger-1.1.4/setup.py` & `discoger-1.1.5/setup.py`

 * *Files identical despite different names*

