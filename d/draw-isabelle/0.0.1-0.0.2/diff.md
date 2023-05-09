# Comparing `tmp/draw-isabelle-0.0.1.tar.gz` & `tmp/draw-isabelle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draw-isabelle-0.0.1.tar", last modified: Tue May  9 19:18:06 2023, max compression
+gzip compressed data, was "draw-isabelle-0.0.2.tar", last modified: Tue May  9 19:22:03 2023, max compression
```

## Comparing `draw-isabelle-0.0.1.tar` & `draw-isabelle-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-09 19:18:06.156362 draw-isabelle-0.0.1/
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1261 2023-05-09 19:18:06.156362 draw-isabelle-0.0.1/PKG-INFO
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      950 2023-05-09 19:12:28.000000 draw-isabelle-0.0.1/README.md
-drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-09 19:18:06.153029 draw-isabelle-0.0.1/draw_isabelle/
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-09 19:00:25.000000 draw-isabelle-0.0.1/draw_isabelle/__init__.py
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      360 2023-05-09 19:17:13.000000 draw-isabelle-0.0.1/draw_isabelle/__main__.py
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1520 2023-05-09 19:00:15.000000 draw-isabelle-0.0.1/draw_isabelle/parsing.py
-drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-09 19:18:06.156362 draw-isabelle-0.0.1/draw_isabelle.egg-info/
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1261 2023-05-09 19:18:06.000000 draw-isabelle-0.0.1/draw_isabelle.egg-info/PKG-INFO
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      319 2023-05-09 19:18:06.000000 draw-isabelle-0.0.1/draw_isabelle.egg-info/SOURCES.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        1 2023-05-09 19:18:06.000000 draw-isabelle-0.0.1/draw_isabelle.egg-info/dependency_links.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       70 2023-05-09 19:18:06.000000 draw-isabelle-0.0.1/draw_isabelle.egg-info/entry_points.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       18 2023-05-09 19:18:06.000000 draw-isabelle-0.0.1/draw_isabelle.egg-info/requires.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       14 2023-05-09 19:18:06.000000 draw-isabelle-0.0.1/draw_isabelle.egg-info/top_level.txt
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       38 2023-05-09 19:18:06.156362 draw-isabelle-0.0.1/setup.cfg
--rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      836 2023-05-09 19:16:28.000000 draw-isabelle-0.0.1/setup.py
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-09 19:22:03.648831 draw-isabelle-0.0.2/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1178 2023-05-09 19:22:03.648831 draw-isabelle-0.0.2/PKG-INFO
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      853 2023-05-09 19:19:47.000000 draw-isabelle-0.0.2/README.md
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-09 19:22:03.648831 draw-isabelle-0.0.2/draw_isabelle/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-09 19:00:25.000000 draw-isabelle-0.0.2/draw_isabelle/__init__.py
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      360 2023-05-09 19:17:13.000000 draw-isabelle-0.0.2/draw_isabelle/__main__.py
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1520 2023-05-09 19:00:15.000000 draw-isabelle-0.0.2/draw_isabelle/parsing.py
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-09 19:22:03.648831 draw-isabelle-0.0.2/draw_isabelle.egg-info/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1178 2023-05-09 19:22:03.000000 draw-isabelle-0.0.2/draw_isabelle.egg-info/PKG-INFO
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      319 2023-05-09 19:22:03.000000 draw-isabelle-0.0.2/draw_isabelle.egg-info/SOURCES.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        1 2023-05-09 19:22:03.000000 draw-isabelle-0.0.2/draw_isabelle.egg-info/dependency_links.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       70 2023-05-09 19:22:03.000000 draw-isabelle-0.0.2/draw_isabelle.egg-info/entry_points.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       18 2023-05-09 19:22:03.000000 draw-isabelle-0.0.2/draw_isabelle.egg-info/requires.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       14 2023-05-09 19:22:03.000000 draw-isabelle-0.0.2/draw_isabelle.egg-info/top_level.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       38 2023-05-09 19:22:03.648831 draw-isabelle-0.0.2/setup.cfg
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      850 2023-05-09 19:21:14.000000 draw-isabelle-0.0.2/setup.py
```

### Comparing `draw-isabelle-0.0.1/PKG-INFO` & `draw-isabelle-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: draw-isabelle
-Version: 0.0.1
+Version: 0.0.2
 Summary: Viz Isabelle ⟨l, a, r⟩ graphs
-Home-page: https://github.com/sorenmulli
-Download-URL: https://pypi.org/project/draw_isabelle
+Home-page: https://github.com/sorenmulli/draw-isabelle
+Download-URL: https://pypi.org/project/draw-isabelle
 Author: Søren Winkel Holm
 Author-email: swholm@protonmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # draw-isabelle
 
 Quick visualization tool for nested Isabelle trees which are defined by the angle brace Isabelle syntax `⟨l, a, r⟩`.
 
 
 ## Install and usage
 
 ```console
-$ pip install draw-isabelle # or alternatively, clone repo and run make
-$ draw-isabelle '⟨⟨⟨⟨⟩, a, ⟨⟩⟩, a, ⟨⟨⟩, a, ⟨⟩⟩⟩, a, ⟨⟨⟩, a, ⟨⟩⟩⟩' # or alternatively, call with python -m draw_isabelle
+$ pip install draw-isabelle
+$ draw-isabelle '⟨⟨⟨⟨⟩, a, ⟨⟩⟩, a, ⟨⟨⟩, a, ⟨⟩⟩⟩, a, ⟨⟨⟩, a, ⟨⟩⟩⟩'
 ```
 
 will output
 ```
           ________a___
          /            \
      ___a___          _a
     /       \        /  \
   _a        _a      ⟨⟩   ⟨⟩
  /  \      /  \
 ⟨⟩   ⟨⟩   ⟨⟩   ⟨⟩
 ```
 
+
 ## Contributing
 Please open PR's with fixes and code improvements; could be cool to also support the Node/Leaf syntax or maybe other useful structures.
 
 Code is also pretty untested so please LMK with breaking examples.
 
 Might also make sense to code the ASCII tree representation in this repo to remove the binarytree dependency.
```

### Comparing `draw-isabelle-0.0.1/draw_isabelle/parsing.py` & `draw-isabelle-0.0.2/draw_isabelle/parsing.py`

 * *Files identical despite different names*

### Comparing `draw-isabelle-0.0.1/draw_isabelle.egg-info/PKG-INFO` & `draw-isabelle-0.0.2/draw_isabelle.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: draw-isabelle
-Version: 0.0.1
+Version: 0.0.2
 Summary: Viz Isabelle ⟨l, a, r⟩ graphs
-Home-page: https://github.com/sorenmulli
-Download-URL: https://pypi.org/project/draw_isabelle
+Home-page: https://github.com/sorenmulli/draw-isabelle
+Download-URL: https://pypi.org/project/draw-isabelle
 Author: Søren Winkel Holm
 Author-email: swholm@protonmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # draw-isabelle
 
 Quick visualization tool for nested Isabelle trees which are defined by the angle brace Isabelle syntax `⟨l, a, r⟩`.
 
 
 ## Install and usage
 
 ```console
-$ pip install draw-isabelle # or alternatively, clone repo and run make
-$ draw-isabelle '⟨⟨⟨⟨⟩, a, ⟨⟩⟩, a, ⟨⟨⟩, a, ⟨⟩⟩⟩, a, ⟨⟨⟩, a, ⟨⟩⟩⟩' # or alternatively, call with python -m draw_isabelle
+$ pip install draw-isabelle
+$ draw-isabelle '⟨⟨⟨⟨⟩, a, ⟨⟩⟩, a, ⟨⟨⟩, a, ⟨⟩⟩⟩, a, ⟨⟨⟩, a, ⟨⟩⟩⟩'
 ```
 
 will output
 ```
           ________a___
          /            \
      ___a___          _a
     /       \        /  \
   _a        _a      ⟨⟩   ⟨⟩
  /  \      /  \
 ⟨⟩   ⟨⟩   ⟨⟩   ⟨⟩
 ```
 
+
 ## Contributing
 Please open PR's with fixes and code improvements; could be cool to also support the Node/Leaf syntax or maybe other useful structures.
 
 Code is also pretty untested so please LMK with breaking examples.
 
 Might also make sense to code the ASCII tree representation in this repo to remove the binarytree dependency.
```

### Comparing `draw-isabelle-0.0.1/setup.py` & `draw-isabelle-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 required = [
     "binarytree~=6.5.1",
 ]
 
 # pylint: disable=use-dict-literal
 setup_args = dict(
     name="draw-isabelle",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     author="Søren Winkel Holm",
     author_email="swholm@protonmail.com",
-    url="https://github.com/sorenmulli",
-    download_url="https://pypi.org/project/draw_isabelle",
+    url="https://github.com/sorenmulli/draw-isabelle",
+    download_url="https://pypi.org/project/draw-isabelle",
     install_requires=required,
     description="Viz Isabelle ⟨l, a, r⟩ graphs",
     long_description_content_type="text/markdown",
     long_description=readme,
     license="MIT",
     entry_points={
         "console_scripts": [
```

