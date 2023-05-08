# Comparing `tmp/terminut-0.0.0.4.tar.gz` & `tmp/terminut-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminut-0.0.0.4.tar", last modified: Mon May  8 22:42:25 2023, max compression
+gzip compressed data, was "terminut-0.0.0.5.tar", last modified: Mon May  8 22:47:44 2023, max compression
```

## Comparing `terminut-0.0.0.4.tar` & `terminut-0.0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 22:42:25.618160 terminut-0.0.0.4/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1994 2023-05-08 22:42:25.617164 terminut-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      816 2023-05-08 01:53:38.000000 terminut-0.0.0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 22:42:25.618160 terminut-0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1598 2023-05-08 02:34:01.000000 terminut-0.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:42:25.602472 terminut-0.0.0.4/terminut/
--rw-rw-rw-   0        0        0      335 2023-05-08 02:35:20.000000 terminut-0.0.0.4/terminut/__init__.py
--rw-rw-rw-   0        0        0     2418 2023-05-08 02:23:50.000000 terminut-0.0.0.4/terminut/console.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:42:25.616166 terminut-0.0.0.4/terminut.egg-info/
--rw-rw-rw-   0        0        0     1994 2023-05-08 22:42:25.000000 terminut-0.0.0.4/terminut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-08 22:42:25.000000 terminut-0.0.0.4/terminut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 22:42:25.000000 terminut-0.0.0.4/terminut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-08 22:42:25.000000 terminut-0.0.0.4/terminut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 22:42:25.000000 terminut-0.0.0.4/terminut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:44.180588 terminut-0.0.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1994 2023-05-08 22:47:44.180588 terminut-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2023-05-08 01:53:38.000000 terminut-0.0.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 22:47:44.180588 terminut-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1598 2023-05-08 22:47:16.000000 terminut-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:44.163638 terminut-0.0.0.5/terminut/
+-rw-rw-rw-   0        0        0      335 2023-05-08 02:35:20.000000 terminut-0.0.0.5/terminut/__init__.py
+-rw-rw-rw-   0        0        0     2467 2023-05-08 22:47:09.000000 terminut-0.0.0.5/terminut/console.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:44.179578 terminut-0.0.0.5/terminut.egg-info/
+-rw-rw-rw-   0        0        0     1994 2023-05-08 22:47:44.000000 terminut-0.0.0.5/terminut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-08 22:47:44.000000 terminut-0.0.0.5/terminut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 22:47:44.000000 terminut-0.0.0.5/terminut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-08 22:47:44.000000 terminut-0.0.0.5/terminut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 22:47:44.000000 terminut-0.0.0.5/terminut.egg-info/top_level.txt
```

### Comparing `terminut-0.0.0.4/LICENSE` & `terminut-0.0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.4/PKG-INFO` & `terminut-0.0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
```

### Comparing `terminut-0.0.0.4/README.md` & `terminut-0.0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.4/setup.py` & `terminut-0.0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.4"
+vers = "0.0.0.5"
     
 setup(name="terminut",
       version=vers,
       description="Terminut // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `terminut-0.0.0.4/terminut/console.py` & `terminut-0.0.0.5/terminut/console.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,31 +27,32 @@
         ("(!)" in content)
         or ("(-)" in content)
         or ("(~)" in content) 
         or ("debug" in content.lower())
         ) and (Settings.debug == False): return
     
     timestamp = f'{Settings.c_SECO}{datetime.fromtimestamp(time()).strftime("%H:%M:%S")}{Fore.RESET} ' if Settings.timestamp else ''
-    print(
-        timestamp + 
-        content
-        .replace("[", f"{Settings.c_SECO}[{Settings.c_MAIN}")
-        .replace("]", f"{Settings.c_SECO}]{Fore.RESET}")
-        .replace("|", f"{Settings.c_SECO}|{Settings.c_MAIN}")
-        .replace("->", f"{Settings.c_SECO}->{Settings.c_MAIN}")
-
-        # .replace("(", f"{Settings.c_SECO}({Fore.RESET}").replace(")", f"{Settings.c_SECO}){Fore.RESET}")
-        .replace("(+)", f"{Settings.c_SECO}({Fore.GREEN}+{Settings.c_SECO}){Settings.c_MAIN}")
-        .replace("($)", f"{Settings.c_SECO}({Fore.GREEN}${Settings.c_SECO}){Settings.c_MAIN}")
-        .replace("(-)", f"{Settings.c_SECO}({Fore.RED}-{Settings.c_SECO}){Settings.c_MAIN}")
-        .replace("(!)", f"{Settings.c_SECO}({Fore.RED}!{Settings.c_SECO}){Settings.c_MAIN}")
-        .replace("(~)", f"{Settings.c_SECO}({Fore.YELLOW}~{Settings.c_SECO}){Settings.c_MAIN}")
-        .replace("(#)", f"{Settings.c_SECO}({Fore.BLUE}#{Settings.c_SECO}){Settings.c_MAIN}")
+    content   = content\
+        .replace("[", f"{Settings.c_SECO}[{Settings.c_MAIN}")\
+        .replace("]", f"{Settings.c_SECO}]{Fore.RESET}")\
+        .replace("|", f"{Settings.c_SECO}|{Settings.c_MAIN}")\
+        .replace("->", f"{Settings.c_SECO}->{Settings.c_MAIN}")\
+        .replace("(+)", f"{Settings.c_SECO}({Fore.GREEN}+{Settings.c_SECO}){Settings.c_MAIN}")\
+        .replace("($)", f"{Settings.c_SECO}({Fore.GREEN}${Settings.c_SECO}){Settings.c_MAIN}")\
+        .replace("(-)", f"{Settings.c_SECO}({Fore.RED}-{Settings.c_SECO}){Settings.c_MAIN}")\
+        .replace("(!)", f"{Settings.c_SECO}({Fore.RED}!{Settings.c_SECO}){Settings.c_MAIN}")\
+        .replace("(~)", f"{Settings.c_SECO}({Fore.YELLOW}~{Settings.c_SECO}){Settings.c_MAIN}")\
+        .replace("(#)", f"{Settings.c_SECO}({Fore.BLUE}#{Settings.c_SECO}){Settings.c_MAIN}")\
         .replace("(*)", f"{Settings.c_SECO}({Fore.CYAN}*{Settings.c_SECO}){Settings.c_MAIN}")
-    , end=f"{Fore.RESET}\n")
+    
+        # .replace("(", f"{Settings.c_SECO}({Fore.RESET}").replace(")", f"{Settings.c_SECO}){Fore.RESET}")
+        
+        
+    return print( timestamp + content, end=f"{Fore.RESET}\n" )
+    
     
 @staticmethod
 def inputf(content: str):
     if "(?)" not in content: x = f"{Settings.c_SECO}({Settings.c_MAIN}?{Settings.c_SECO}){Fore.RESET} "
     else: x = ""
     content = x + content\
         .replace("(", f"{Settings.c_SECO}({Settings.c_MAIN}").replace(")", f"{Settings.c_SECO}){Settings.c_MAIN}")\
```

### Comparing `terminut-0.0.0.4/terminut.egg-info/PKG-INFO` & `terminut-0.0.0.5/terminut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
```

