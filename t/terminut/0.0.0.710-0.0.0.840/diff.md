# Comparing `tmp/terminut-0.0.0.710.tar.gz` & `tmp/terminut-0.0.0.840.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminut-0.0.0.710.tar", last modified: Mon May  8 23:58:37 2023, max compression
+gzip compressed data, was "terminut-0.0.0.840.tar", last modified: Tue May  9 01:04:03 2023, max compression
```

## Comparing `terminut-0.0.0.710.tar` & `terminut-0.0.0.840.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:58:37.206208 terminut-0.0.0.710/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.710/LICENSE
--rw-rw-rw-   0        0        0     1996 2023-05-08 23:58:37.206208 terminut-0.0.0.710/PKG-INFO
--rw-rw-rw-   0        0        0      816 2023-05-08 01:53:38.000000 terminut-0.0.0.710/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.710/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 23:58:37.206208 terminut-0.0.0.710/setup.cfg
--rw-rw-rw-   0        0        0     1600 2023-05-08 23:58:26.000000 terminut-0.0.0.710/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:58:37.193597 terminut-0.0.0.710/terminut/
--rw-rw-rw-   0        0        0      363 2023-05-08 23:41:45.000000 terminut-0.0.0.710/terminut/__init__.py
--rw-rw-rw-   0        0        0     3786 2023-05-08 23:58:14.000000 terminut-0.0.0.710/terminut/console.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:58:37.205210 terminut-0.0.0.710/terminut.egg-info/
--rw-rw-rw-   0        0        0     1996 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 23:58:37.000000 terminut-0.0.0.710/terminut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 01:04:03.340566 terminut-0.0.0.840/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.840/LICENSE
+-rw-rw-rw-   0        0        0     2618 2023-05-09 01:04:03.339568 terminut-0.0.0.840/PKG-INFO
+-rw-rw-rw-   0        0        0     1438 2023-05-09 01:03:28.000000 terminut-0.0.0.840/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.840/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 01:04:03.340566 terminut-0.0.0.840/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2023-05-09 01:03:48.000000 terminut-0.0.0.840/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:04:03.325085 terminut-0.0.0.840/terminut/
+-rw-rw-rw-   0        0        0      363 2023-05-09 00:09:38.000000 terminut-0.0.0.840/terminut/__init__.py
+-rw-rw-rw-   0        0        0     7386 2023-05-09 00:58:53.000000 terminut-0.0.0.840/terminut/console.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:04:03.338572 terminut-0.0.0.840/terminut.egg-info/
+-rw-rw-rw-   0        0        0     2618 2023-05-09 01:04:03.000000 terminut-0.0.0.840/terminut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-09 01:04:03.000000 terminut-0.0.0.840/terminut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 01:04:03.000000 terminut-0.0.0.840/terminut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-09 01:04:03.000000 terminut-0.0.0.840/terminut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 01:04:03.000000 terminut-0.0.0.840/terminut.egg-info/top_level.txt
```

### Comparing `terminut-0.0.0.710/LICENSE` & `terminut-0.0.0.840/LICENSE`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.710/PKG-INFO` & `terminut-0.0.0.840/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.710
+Version: 0.0.0.840
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
@@ -36,26 +36,42 @@
                 And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
-! package not available yet for non-personal use !
+! package NOT FULLY available for non-personal use !
+~ use at the knowledge of knowing it may break ~
+
+pip install terminut
 ```
 
 ### Usage
 ```py
-from terminut.console import printf as print, inputf as input, init
+# default shit if u want to only import for ease - auto switches #
+
+from terminut import printf as print, inputf as input, init
+init(debug=True)
 
-init(
-    gradient=True,
-    showTimestamp=True,
-    madeBy="vast#1337"
-)
+print("[DEBUG] Should Not Show")
+print("[INFO] Should Show")
 
-print("Cool Stuff")
+# --------------------------------------------------------- #
+
+# this is for custom cool stuff as seen here: 
+# https://cdn.discordapp.com/attachments/1099515953223569420/1105295220414885998/2023-05-08_20-46-22.mp4
+
+import time
+from terminut import BetaConsole
+c = BetaConsole(speed=2)
+while True:
+    try:
+        timestamp = c.getTimestamp()
+        c.alphaPrint("[INF]", f"[{timestamp}] made by vast :D", increment=False)
+        time.sleep(0.001)
+    except KeyboardInterrupt: exit(0)
 ```
 
 ---
 
 ## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

### Comparing `terminut-0.0.0.710/setup.py` & `terminut-0.0.0.840/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.710"
+vers = "0.0.0.840"
     
 setup(name="terminut",
       version=vers,
       description="Terminut // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `terminut-0.0.0.710/terminut/console.py` & `terminut-0.0.0.840/terminut/console.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,81 @@
-from colorama import Fore
+from colorama import Fore, Style
 from datetime import datetime
 from time     import time
 from re       import sub
 from colorsys import hsv_to_rgb
+from shutil   import get_terminal_size
 
 
 class Settings:
     initialized = False
     debug = True 
     timestamp = True
     c_MAIN = Fore.LIGHTBLUE_EX
     c_SECO = Fore.LIGHTBLACK_EX
 
+
+
+
+def init(
+    debug: bool = True,
+    showTimestamp: bool = True,
+    colMain = Fore.LIGHTBLUE_EX,
+    colSeco = Fore.LIGHTBLACK_EX,
+    madeBy = "vast#1337"
+):
+    Settings.initialized = True
+    Settings.debug = debug
+    Settings.timestamp = showTimestamp
+    Settings.c_MAIN = colMain
+    Settings.c_SECO = colSeco
+
+
+@staticmethod
+def printf(content: str, mainCol=None, showTimestamp=None):
+    if showTimestamp is None: showTimestamp = Settings.timestamp
+    if mainCol is None: mainCol = Settings.c_MAIN
+    if type(content) != str: return print(content)
+    if (
+        ("(!)" in content)
+        or ("(-)" in content)
+        or ("(~)" in content) 
+        or ("debug" in content.lower())
+        ) and (Settings.debug == False): return
+    
+    timestamp = f'{Settings.c_SECO}{datetime.fromtimestamp(time()).strftime("%H:%M:%S")}{Fore.RESET} ' if (showTimestamp) else ''
+    
+    content   = sub(r'\[(.*?)]', rf'{Settings.c_SECO}[{mainCol}\1{Settings.c_SECO}]{Fore.RESET}', content)
+    content   = content\
+        .replace("|", f"{Settings.c_SECO}|{mainCol}")\
+        .replace("->", f"{Settings.c_SECO}->{mainCol}")\
+        .replace("(+)", f"{Settings.c_SECO}({Fore.GREEN}+{Settings.c_SECO}){mainCol}")\
+        .replace("($)", f"{Settings.c_SECO}({Fore.GREEN}${Settings.c_SECO}){mainCol}")\
+        .replace("(-)", f"{Settings.c_SECO}({Fore.RED}-{Settings.c_SECO}){mainCol}")\
+        .replace("(!)", f"{Settings.c_SECO}({Fore.RED}!{Settings.c_SECO}){mainCol}")\
+        .replace("(~)", f"{Settings.c_SECO}({Fore.YELLOW}~{Settings.c_SECO}){mainCol}")\
+        .replace("(#)", f"{Settings.c_SECO}({Fore.BLUE}#{Settings.c_SECO}){mainCol}")\
+        .replace("(*)", f"{Settings.c_SECO}({Fore.CYAN}*{Settings.c_SECO}){mainCol}")
+    
+        # .replace("(", f"{Settings.c_SECO}({Fore.RESET}").replace(")", f"{Settings.c_SECO}){Fore.RESET}")
+        # .replace("[", f"{Settings.c_SECO}[{mainCol}")\
+        
+    return print(timestamp + content, end=f"{Fore.RESET}\n")
+    
+    
+@staticmethod
+def inputf(content: str):
+    if "(?)" not in content: x = f"{Settings.c_SECO}({Settings.c_MAIN}?{Settings.c_SECO}){Fore.RESET} "
+    else: x = ""
+    content = x + content\
+        .replace("(", f"{Settings.c_SECO}({Settings.c_MAIN}").replace(")", f"{Settings.c_SECO}){Settings.c_MAIN}")\
+        .replace(">", f"{Settings.c_SECO}>{Fore.RESET}")
+    return input(content)
+
+
 class Console:
     def init(
         debug: bool = True,
         showTimestamp: bool = True,
         colMain = Fore.LIGHTBLUE_EX,
         colSeco = Fore.LIGHTBLACK_EX,
         madeBy = "vast#1337"
@@ -73,14 +133,16 @@
 
 class BetaConsole:
     def __init__(self, speed: int = 2, showMS: int = 4):
         self.colHue = 120
         self.speed = speed
         self.direction = self.speed
         self.showMS = showMS
+        self.extraSpace = 0
+        self.incrementing = True
 
     def getTimestamp(self):
         rgb = hsv_to_rgb(self.colHue / 360, 1, 1)
         red = int(rgb[0] * 255)
         green = int(rgb[1] * 255)
         blue = int(rgb[2] * 255)
 
@@ -91,10 +153,35 @@
         if self.colHue >= 240:
             self.direction = -self.speed
         elif self.colHue <= 120:
             self.direction = self.speed
 
         return timestamp
 
-    def alphaPrint(self):
-        print(self.getTimestamp())
+    def alphaPrint(self, type, text, increment:bool=False):
+        if increment:
+            if self.extraSpace == 0: self.incrementing = True
+            elif self.extraSpace == 10: self.incrementing = False
+            if self.incrementing: self.extraSpace += 1
+            else: self.extraSpace -= 1
+
+        console_width = get_terminal_size().columns
+
+        other_len = 28 # avg of # len(text.split("\x1b[0m] ")[0])
+        text_length = len(text.split("\x1b[0m] ")[1]) # keeps changing cuz of colors
+        type_length = len(type)
+        
+        spaces = max(0, console_width - (text_length - type_length + other_len + self.extraSpace))
+        
+        if "err" in type.lower():
+            form_color = Fore.RED
+        elif "inf" in type.lower():
+            form_color = Fore.LIGHTCYAN_EX
+        else:
+            form_color = Fore.GREEN
+        formatted_info = type.replace("[", f"{Fore.LIGHTBLACK_EX}[{form_color}").replace("]", f"{Fore.LIGHTBLACK_EX}]{Style.RESET_ALL}")
+
+
+        output = f"{text}{' ' * spaces}{formatted_info}"
 
+        print(output)
+        return
```

### Comparing `terminut-0.0.0.710/terminut.egg-info/PKG-INFO` & `terminut-0.0.0.840/terminut.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.710
+Version: 0.0.0.840
 Summary: Terminut // vast#1337
 Home-page: http://pypi.python.org/pypi/terminut
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
@@ -36,26 +36,42 @@
                 And Available To Anyone Else Who Wants To Use <
 ```
 
 ---
 
 ### Installation
 ```yaml
-! package not available yet for non-personal use !
+! package NOT FULLY available for non-personal use !
+~ use at the knowledge of knowing it may break ~
+
+pip install terminut
 ```
 
 ### Usage
 ```py
-from terminut.console import printf as print, inputf as input, init
+# default shit if u want to only import for ease - auto switches #
+
+from terminut import printf as print, inputf as input, init
+init(debug=True)
 
-init(
-    gradient=True,
-    showTimestamp=True,
-    madeBy="vast#1337"
-)
+print("[DEBUG] Should Not Show")
+print("[INFO] Should Show")
 
-print("Cool Stuff")
+# --------------------------------------------------------- #
+
+# this is for custom cool stuff as seen here: 
+# https://cdn.discordapp.com/attachments/1099515953223569420/1105295220414885998/2023-05-08_20-46-22.mp4
+
+import time
+from terminut import BetaConsole
+c = BetaConsole(speed=2)
+while True:
+    try:
+        timestamp = c.getTimestamp()
+        c.alphaPrint("[INF]", f"[{timestamp}] made by vast :D", increment=False)
+        time.sleep(0.001)
+    except KeyboardInterrupt: exit(0)
 ```
 
 ---
 
 ## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

