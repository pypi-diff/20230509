# Comparing `tmp/elm-messenger-0.1.3.tar.gz` & `tmp/elm-messenger-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.1.3.tar", last modified: Sun May  7 08:28:02 2023, max compression
+gzip compressed data, was "elm-messenger-0.1.4.tar", last modified: Tue May  9 06:58:18 2023, max compression
```

## Comparing `elm-messenger-0.1.3.tar` & `elm-messenger-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9317 2023-05-07 08:25:40.000000 elm-messenger-0.1.3/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-09 06:58:18.000000 elm-messenger-0.1.4/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9308 2023-05-09 01:19:04.000000 elm-messenger-0.1.4/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-09 06:58:18.261228 elm-messenger-0.1.4/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.4/setup.py
```

### Comparing `elm-messenger-0.1.3/messengercli/messenger.py` & `elm-messenger-0.1.4/messengercli/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,21 +217,19 @@
                 ),
             )
             self.update_rep_next(
                 f"src/Scenes/{scene}/Model.elm",
                 2,
                 ",\n".join(
                     [
-                        f"""( "{l}"
-          , let
+                        f"""let
                 x =
                     {l}.layer
             in
-            {l}G.getLayerT {{ x | data = {l}.layer.init t NullLayerMsg initCommonData }}
-          )"""
+            {l}G.getLayerT {{ x | data = {l}.layer.init (addCommonData nullCommonData env) NullLayerInitData }}"""
                         for l in layers
                     ]
                 ),
             )
 
 
 @app.command()
```

