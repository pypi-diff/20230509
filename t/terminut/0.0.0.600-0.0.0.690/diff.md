# Comparing `tmp/terminut-0.0.0.600.tar.gz` & `tmp/terminut-0.0.0.690.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminut-0.0.0.600.tar", last modified: Mon May  8 23:04:13 2023, max compression
+gzip compressed data, was "terminut-0.0.0.690.tar", last modified: Mon May  8 23:15:16 2023, max compression
```

## Comparing `terminut-0.0.0.600.tar` & `terminut-0.0.0.690.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:04:13.046951 terminut-0.0.0.600/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.600/LICENSE
--rw-rw-rw-   0        0        0     1996 2023-05-08 23:04:13.045954 terminut-0.0.0.600/PKG-INFO
--rw-rw-rw-   0        0        0      816 2023-05-08 01:53:38.000000 terminut-0.0.0.600/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.600/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 23:04:13.046951 terminut-0.0.0.600/setup.cfg
--rw-rw-rw-   0        0        0     1600 2023-05-08 23:03:58.000000 terminut-0.0.0.600/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:04:13.030800 terminut-0.0.0.600/terminut/
--rw-rw-rw-   0        0        0      335 2023-05-08 02:35:20.000000 terminut-0.0.0.600/terminut/__init__.py
--rw-rw-rw-   0        0        0     2574 2023-05-08 23:02:03.000000 terminut-0.0.0.600/terminut/console.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:04:13.045954 terminut-0.0.0.600/terminut.egg-info/
--rw-rw-rw-   0        0        0     1996 2023-05-08 23:04:13.000000 terminut-0.0.0.600/terminut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-08 23:04:13.000000 terminut-0.0.0.600/terminut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:04:13.000000 terminut-0.0.0.600/terminut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-08 23:04:13.000000 terminut-0.0.0.600/terminut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 23:04:13.000000 terminut-0.0.0.600/terminut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 23:15:16.614605 terminut-0.0.0.690/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.690/LICENSE
+-rw-rw-rw-   0        0        0     1996 2023-05-08 23:15:16.613607 terminut-0.0.0.690/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2023-05-08 01:53:38.000000 terminut-0.0.0.690/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.690/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 23:15:16.614605 terminut-0.0.0.690/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2023-05-08 23:15:05.000000 terminut-0.0.0.690/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:15:16.601131 terminut-0.0.0.690/terminut/
+-rw-rw-rw-   0        0        0      335 2023-05-08 02:35:20.000000 terminut-0.0.0.690/terminut/__init__.py
+-rw-rw-rw-   0        0        0     2546 2023-05-08 23:14:39.000000 terminut-0.0.0.690/terminut/console.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:15:16.612609 terminut-0.0.0.690/terminut.egg-info/
+-rw-rw-rw-   0        0        0     1996 2023-05-08 23:15:16.000000 terminut-0.0.0.690/terminut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-08 23:15:16.000000 terminut-0.0.0.690/terminut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:15:16.000000 terminut-0.0.0.690/terminut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-08 23:15:16.000000 terminut-0.0.0.690/terminut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 23:15:16.000000 terminut-0.0.0.690/terminut.egg-info/top_level.txt
```

### Comparing `terminut-0.0.0.600/LICENSE` & `terminut-0.0.0.690/LICENSE`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.600/PKG-INFO` & `terminut-0.0.0.690/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.600
+Version: 0.0.0.690
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
```

### Comparing `terminut-0.0.0.600/README.md` & `terminut-0.0.0.690/README.md`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.600/setup.py` & `terminut-0.0.0.690/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.600"
+vers = "0.0.0.690"
     
 setup(name="terminut",
       version=vers,
       description="Terminut // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `terminut-0.0.0.600/terminut/console.py` & `terminut-0.0.0.690/terminut/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,16 @@
         or ("(-)" in content)
         or ("(~)" in content) 
         or ("debug" in content.lower())
         ) and (Settings.debug == False): return
     
     timestamp = f'{Settings.c_SECO}{datetime.fromtimestamp(time()).strftime("%H:%M:%S")}{Fore.RESET} ' if Settings.timestamp else ''
     
-    content   = sub(r'\[.*?\]', f"[{Settings.c_SECO}][{Settings.c_MAIN}]", content)
+    content   = sub(r'\[(.*?)]', rf'{Settings.c_SECO}[{Settings.c_MAIN}\1{Settings.c_SECO}]{Fore.RESET}', content)
     content   = content\
-        .replace("]", f"{Settings.c_SECO}]{Fore.RESET}")\
         .replace("|", f"{Settings.c_SECO}|{Settings.c_MAIN}")\
         .replace("->", f"{Settings.c_SECO}->{Settings.c_MAIN}")\
         .replace("(+)", f"{Settings.c_SECO}({Fore.GREEN}+{Settings.c_SECO}){Settings.c_MAIN}")\
         .replace("($)", f"{Settings.c_SECO}({Fore.GREEN}${Settings.c_SECO}){Settings.c_MAIN}")\
         .replace("(-)", f"{Settings.c_SECO}({Fore.RED}-{Settings.c_SECO}){Settings.c_MAIN}")\
         .replace("(!)", f"{Settings.c_SECO}({Fore.RED}!{Settings.c_SECO}){Settings.c_MAIN}")\
         .replace("(~)", f"{Settings.c_SECO}({Fore.YELLOW}~{Settings.c_SECO}){Settings.c_MAIN}")\
```

### Comparing `terminut-0.0.0.600/terminut.egg-info/PKG-INFO` & `terminut-0.0.0.690/terminut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.600
+Version: 0.0.0.690
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
```

