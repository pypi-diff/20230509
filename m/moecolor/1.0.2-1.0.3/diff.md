# Comparing `tmp/moecolor-1.0.2.tar.gz` & `tmp/moecolor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\moecolor-1.0.2.tar", last modified: Sun Apr 30 05:51:49 2023, max compression
+gzip compressed data, was "dist\moecolor-1.0.3.tar", last modified: Tue May  9 00:44:11 2023, max compression
```

## Comparing `moecolor-1.0.2.tar` & `moecolor-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 05:51:49.000000 moecolor-1.0.2/
--rw-rw-rw-   0        0        0     7518 2023-04-30 05:51:49.000000 moecolor-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5728 2023-01-04 04:46:32.000000 moecolor-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 05:51:49.000000 moecolor-1.0.2/moecolor/
--rw-rw-rw-   0        0        0     5660 2023-01-04 04:46:32.000000 moecolor-1.0.2/moecolor/README.py
--rw-rw-rw-   0        0        0      152 2023-02-22 01:27:35.000000 moecolor-1.0.2/moecolor/__init__.py
--rw-rw-rw-   0        0        0     9652 2023-04-30 05:51:24.000000 moecolor-1.0.2/moecolor/main.py
--rw-rw-rw-   0        0        0     1196 2023-04-30 05:51:38.000000 moecolor-1.0.2/moecolor/version.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:51:49.000000 moecolor-1.0.2/moecolor.egg-info/
--rw-rw-rw-   0        0        0     7518 2023-04-30 05:51:49.000000 moecolor-1.0.2/moecolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-30 05:51:49.000000 moecolor-1.0.2/moecolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 05:51:49.000000 moecolor-1.0.2/moecolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 05:51:49.000000 moecolor-1.0.2/moecolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 05:51:49.000000 moecolor-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1245 2023-02-22 04:15:58.000000 moecolor-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:44:11.000000 moecolor-1.0.3/
+-rw-rw-rw-   0        0        0     7518 2023-05-09 00:44:11.000000 moecolor-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5728 2023-01-04 04:46:32.000000 moecolor-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 00:44:11.000000 moecolor-1.0.3/moecolor/
+-rw-rw-rw-   0        0        0     5660 2023-01-04 04:46:32.000000 moecolor-1.0.3/moecolor/README.py
+-rw-rw-rw-   0        0        0      152 2023-02-22 01:27:35.000000 moecolor-1.0.3/moecolor/__init__.py
+-rw-rw-rw-   0        0        0     9859 2023-05-07 06:30:02.000000 moecolor-1.0.3/moecolor/main.py
+-rw-rw-rw-   0        0        0     1196 2023-05-07 06:31:45.000000 moecolor-1.0.3/moecolor/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:44:11.000000 moecolor-1.0.3/moecolor.egg-info/
+-rw-rw-rw-   0        0        0     7518 2023-05-09 00:44:11.000000 moecolor-1.0.3/moecolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-09 00:44:11.000000 moecolor-1.0.3/moecolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 00:44:11.000000 moecolor-1.0.3/moecolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 00:44:11.000000 moecolor-1.0.3/moecolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 00:44:11.000000 moecolor-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1245 2023-02-22 04:15:58.000000 moecolor-1.0.3/setup.py
```

### Comparing `moecolor-1.0.2/PKG-INFO` & `moecolor-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moecolor
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Libary to print colored and styled text in terminal. Offers color-specific configuration by providing 24bit hex or RGB values as well 256-color mode.
 Home-page: https://github.com/mhamdan91/moecolor
 Author: mhamdan91 (Hamdan, Muhammad)
 Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Moecolor (Flexible terminal text coloring and styling)
         =======================================================
```

### Comparing `moecolor-1.0.2/README.md` & `moecolor-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `moecolor-1.0.2/moecolor/README.py` & `moecolor-1.0.3/moecolor/README.py`

 * *Files identical despite different names*

### Comparing `moecolor-1.0.2/moecolor/main.py` & `moecolor-1.0.3/moecolor/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,25 +203,33 @@
             sw = set(cw)
             # calculate word length
             lw = sum(c*c for c in cw.values())**0.5
             return (sw, cw, lw)
 
         v1 = word2vec(word)
         for color in available_colors:
-            v2 = word2vec(color)
-            shared = v1[0].intersection(v2[0])
-            # Cos(x, y) = x . y / ||x|| * ||y||
-            scores[color] = sum(v1[1][ch]*v2[1][ch] for ch in shared)/v1[2]/v2[2]
+            try:
+                v2 = word2vec(color)
+                shared = v1[0].intersection(v2[0])
+                # Cos(x, y) = x . y / ||x|| * ||y||
+                score = sum(v1[1][ch]*v2[1][ch] for ch in shared) / v1[2]/v2[2]
+            except Exception:
+                score = 0.5
+            scores[color] = score
         scores = sorted(scores.items(), key=lambda item:item[1], reverse=True)
         return AVAILABLE_COLORS[scores[0][0]] if scores[0][1] > 0.5 else -1
 
 def print(text: str='', *args, color: typing.Any='', attr: typing.Iterable=[], **kwargs):
     possible_help = ['h', 'usage', 'show_help', 'help_me', 'use', 'help']
     if set(possible_help).intersection(kwargs):
         osprint(LONG_DESCRIPTION)
         return
-    text = (text + ' ' + ' '.join(args)).strip()
-    ft = FormatText(text, color, attr=attr) if color or attr else text
-    osprint(ft, **kwargs)
+    try:
+        text = (str(text) + ' ' + ' '.join(args)).strip()
+        ft = FormatText(text, color, attr=attr) if color or attr else text
+    except:
+        osprint(text, **kwargs)
+    else:
+        osprint(ft, **kwargs)
 
 print.__doc__ = LONG_DESCRIPTION
 FormatText.__doc__ = LONG_DESCRIPTION
```

### Comparing `moecolor-1.0.2/moecolor/version.py` & `moecolor-1.0.3/moecolor/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = "Muhammad Hamdan <mhamdan.dev@gmail.com>"
 __copyright__ = """
 MIT License
 
 Copyright (c) 2022 Muhammad Hamdan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `moecolor-1.0.2/moecolor.egg-info/PKG-INFO` & `moecolor-1.0.3/moecolor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moecolor
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Libary to print colored and styled text in terminal. Offers color-specific configuration by providing 24bit hex or RGB values as well 256-color mode.
 Home-page: https://github.com/mhamdan91/moecolor
 Author: mhamdan91 (Hamdan, Muhammad)
 Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Moecolor (Flexible terminal text coloring and styling)
         =======================================================
```

### Comparing `moecolor-1.0.2/setup.py` & `moecolor-1.0.3/setup.py`

 * *Files identical despite different names*

