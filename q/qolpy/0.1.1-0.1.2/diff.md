# Comparing `tmp/qolpy-0.1.1.tar.gz` & `tmp/qolpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qolpy-0.1.1.tar", last modified: Sat Apr 15 22:40:27 2023, max compression
+gzip compressed data, was "qolpy-0.1.2.tar", last modified: Mon May  8 23:14:21 2023, max compression
```

## Comparing `qolpy-0.1.1.tar` & `qolpy-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 22:40:27.325073 qolpy-0.1.1/
--rw-rw-rw-   0        0        0      593 2023-04-15 20:11:08.000000 qolpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     9179 2023-04-15 22:40:27.324074 qolpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8373 2023-04-15 22:40:11.000000 qolpy-0.1.1/README.md
--rw-rw-rw-   0        0        0       86 2023-04-15 20:11:08.000000 qolpy-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 22:40:27.325073 qolpy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-04-15 22:38:59.000000 qolpy-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:40:27.259072 qolpy-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 22:40:27.270072 qolpy-0.1.1/src/qolpy/
--rw-rw-rw-   0        0        0      172 2023-04-15 20:19:05.000000 qolpy-0.1.1/src/qolpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:40:27.307076 qolpy-0.1.1/src/qolpy/colour/
--rw-rw-rw-   0        0        0       31 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/colour/__init__.py
--rw-rw-rw-   0        0        0      140 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/colour/interface.py
--rw-rw-rw-   0        0        0      801 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/colour/main.py
--rw-rw-rw-   0        0        0     4228 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/colour/switch.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:40:27.313071 qolpy-0.1.1/src/qolpy/date/
--rw-rw-rw-   0        0        0       77 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/date/__init__.py
--rw-rw-rw-   0        0        0     1436 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/date/interface.py
--rw-rw-rw-   0        0        0     2640 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/date/main.py
--rw-rw-rw-   0        0        0     3363 2023-04-15 20:49:38.000000 qolpy-0.1.1/src/qolpy/date/switch.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:40:27.318078 qolpy-0.1.1/src/qolpy/number/
--rw-rw-rw-   0        0        0       66 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/number/__init__.py
--rw-rw-rw-   0        0        0      113 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/number/interface.py
--rw-rw-rw-   0        0        0     1338 2023-04-15 20:11:08.000000 qolpy-0.1.1/src/qolpy/number/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:40:27.322078 qolpy-0.1.1/src/qolpy/string/
--rw-rw-rw-   0        0        0       61 2023-04-15 20:19:05.000000 qolpy-0.1.1/src/qolpy/string/__init__.py
--rw-rw-rw-   0        0        0     2265 2023-04-15 20:19:05.000000 qolpy-0.1.1/src/qolpy/string/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:40:27.299105 qolpy-0.1.1/src/qolpy.egg-info/
--rw-rw-rw-   0        0        0     9179 2023-04-15 22:40:27.000000 qolpy-0.1.1/src/qolpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2023-04-15 22:40:27.000000 qolpy-0.1.1/src/qolpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 22:40:27.000000 qolpy-0.1.1/src/qolpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 22:40:27.000000 qolpy-0.1.1/src/qolpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-15 22:40:27.000000 qolpy-0.1.1/src/qolpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 23:14:21.017488 qolpy-0.1.2/
+-rw-rw-rw-   0        0        0      593 2023-04-15 20:11:08.000000 qolpy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     9359 2023-05-08 23:14:21.015487 qolpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8545 2023-05-08 23:11:59.000000 qolpy-0.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-15 20:11:08.000000 qolpy-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 23:14:21.017488 qolpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-05-08 23:12:13.000000 qolpy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:14:20.932487 qolpy-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 23:14:20.949486 qolpy-0.1.2/src/qolpy/
+-rw-rw-rw-   0        0        0      172 2023-04-15 20:19:05.000000 qolpy-0.1.2/src/qolpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:14:20.994494 qolpy-0.1.2/src/qolpy/colour/
+-rw-rw-rw-   0        0        0       31 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/colour/__init__.py
+-rw-rw-rw-   0        0        0      140 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/colour/interface.py
+-rw-rw-rw-   0        0        0      801 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/colour/main.py
+-rw-rw-rw-   0        0        0     4241 2023-05-08 23:03:34.000000 qolpy-0.1.2/src/qolpy/colour/switch.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:14:21.001487 qolpy-0.1.2/src/qolpy/date/
+-rw-rw-rw-   0        0        0       77 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/date/__init__.py
+-rw-rw-rw-   0        0        0     1436 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/date/interface.py
+-rw-rw-rw-   0        0        0     2640 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/date/main.py
+-rw-rw-rw-   0        0        0     3363 2023-04-15 20:49:38.000000 qolpy-0.1.2/src/qolpy/date/switch.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:14:21.009487 qolpy-0.1.2/src/qolpy/number/
+-rw-rw-rw-   0        0        0       66 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/number/__init__.py
+-rw-rw-rw-   0        0        0      113 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/number/interface.py
+-rw-rw-rw-   0        0        0     1338 2023-04-15 20:11:08.000000 qolpy-0.1.2/src/qolpy/number/main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:14:21.013487 qolpy-0.1.2/src/qolpy/string/
+-rw-rw-rw-   0        0        0       61 2023-04-15 20:19:05.000000 qolpy-0.1.2/src/qolpy/string/__init__.py
+-rw-rw-rw-   0        0        0     2265 2023-04-15 20:19:05.000000 qolpy-0.1.2/src/qolpy/string/main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:14:20.986489 qolpy-0.1.2/src/qolpy.egg-info/
+-rw-rw-rw-   0        0        0     9359 2023-05-08 23:14:20.000000 qolpy-0.1.2/src/qolpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2023-05-08 23:14:20.000000 qolpy-0.1.2/src/qolpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:14:20.000000 qolpy-0.1.2/src/qolpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 23:14:20.000000 qolpy-0.1.2/src/qolpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-08 23:14:20.000000 qolpy-0.1.2/src/qolpy.egg-info/top_level.txt
```

### Comparing `qolpy-0.1.1/LICENSE` & `qolpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qolpy-0.1.1/PKG-INFO` & `qolpy-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qolpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A suite of random but useful functions that are aimed at giving you 'piece of cake' level comfortability
-Home-page: https://github.com/lewisjr/qolpy.git
+Home-page: https://github.com/cerebrusinc/qolpy.git
 Author: Cerebrus Inc | Lewis Mosho Jr
 Author-email: lewis@cerebrus.dev
-Project-URL: Bug Tracker, https://github.com/lewisjr/qolpy/issues
+Project-URL: Bug Tracker, https://github.com/cerebrusinc/qolpy/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
@@ -18,19 +18,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img src="https://drive.google.com/uc?id=1r9L_Kjdm1i4lCYOCq-bngr-yTl6OZ_lu" alt="py-qol logo" width="250" height="250" />
 </p>
 
-# qolpy v0.1.1
+# qolpy v0.1.2
 
 Are you tired of making the same module in every project? Not a problem! Qol has your back.
 
-A suite of random but useful functions that are aimed at giving you "piece of cake" level comfortability. This is a python port of the [javascript quality of life](https://github.com/lewisjr/qol) and [javascript fstring](https://github.com/lewisjr/fstring) package
+A suite of random but useful functions that are aimed at giving you "piece of cake" level comfortability. This is a python port of the [javascript quality of life](https://github.com/cerebrusinc/qol) and [javascript fstring](https://github.com/cerebrusinc/fstring) package
 
 # Installation
 
     pip install qolpy
 
 or
 
@@ -57,15 +57,15 @@
 ```python
 c = random_colour()
 c_rgb = random_colour("rgb")
 c_cmyk = random_colour("cmyk")
 c_hsv = random_colour("hsv")
 c_hsl = random_colour("hsl")
 
-print(c, c_rgb, c_cmyk, c_hsv, c_hsl);
+print(c, c_rgb, c_cmyk, c_hsv, c_hsl)
 # #f7f7f7, rgb(247,247,247), cmyk(0%,0%,0%,3%), hsv(0,0%,97%), hsl(0,0%,97%)
 ```
 
 <details>
 <summary><strong>Params</strong></summary>
 
 | Parameter | Default Setting | Required? | Definition                                 | Options                            |
@@ -153,15 +153,15 @@
 
 <details>
 <summary><strong>Params</strong></summary>
 
 | Parameter | Default Setting | Required? | Definition                       | Options                                                    |
 | --------- | --------------- | --------- | -------------------------------- | ---------------------------------------------------------- |
 | value     | `undefined`     | Yes       | The number you want to be parsed | `none`                                                     |
-| setting   | `undefined`     | Yes       | The delimiter for the number     | `space`, `comma`, `punct`, any other delimiter as a string |
+| setting   | `comma`         | No        | The delimiter for the number     | `space`, `comma`, `punct`, any other delimiter as a string |
 
 </details>
 <br />
 
 ## abbreviate
 
 ```python
@@ -237,14 +237,23 @@
 <br />
 
 # Changelog
 
 ## v0.1.x
 
 <details open>
+<summary><strong>v0.1.2</strong></summary>
+
+- README updated
+  - Repo links updated
+- `color` dir typing fixed; No more import error
+
+</details>
+
+<details>
 <summary><strong>v0.1.1</strong></summary>
 
 - README completed
 - `parse_date` error fixed
   - Used tp return `month` object when `nll` was specifically set as an arg for `c_format`
 - Moved codebase into `src` folder
```

### Comparing `qolpy-0.1.1/README.md` & `qolpy-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <p align="center">
     <img src="https://drive.google.com/uc?id=1r9L_Kjdm1i4lCYOCq-bngr-yTl6OZ_lu" alt="py-qol logo" width="250" height="250" />
 </p>
 
-# qolpy v0.1.1
+# qolpy v0.1.2
 
 Are you tired of making the same module in every project? Not a problem! Qol has your back.
 
-A suite of random but useful functions that are aimed at giving you "piece of cake" level comfortability. This is a python port of the [javascript quality of life](https://github.com/lewisjr/qol) and [javascript fstring](https://github.com/lewisjr/fstring) package
+A suite of random but useful functions that are aimed at giving you "piece of cake" level comfortability. This is a python port of the [javascript quality of life](https://github.com/cerebrusinc/qol) and [javascript fstring](https://github.com/cerebrusinc/fstring) package
 
 # Installation
 
     pip install qolpy
 
 or
 
@@ -37,15 +37,15 @@
 ```python
 c = random_colour()
 c_rgb = random_colour("rgb")
 c_cmyk = random_colour("cmyk")
 c_hsv = random_colour("hsv")
 c_hsl = random_colour("hsl")
 
-print(c, c_rgb, c_cmyk, c_hsv, c_hsl);
+print(c, c_rgb, c_cmyk, c_hsv, c_hsl)
 # #f7f7f7, rgb(247,247,247), cmyk(0%,0%,0%,3%), hsv(0,0%,97%), hsl(0,0%,97%)
 ```
 
 <details>
 <summary><strong>Params</strong></summary>
 
 | Parameter | Default Setting | Required? | Definition                                 | Options                            |
@@ -133,15 +133,15 @@
 
 <details>
 <summary><strong>Params</strong></summary>
 
 | Parameter | Default Setting | Required? | Definition                       | Options                                                    |
 | --------- | --------------- | --------- | -------------------------------- | ---------------------------------------------------------- |
 | value     | `undefined`     | Yes       | The number you want to be parsed | `none`                                                     |
-| setting   | `undefined`     | Yes       | The delimiter for the number     | `space`, `comma`, `punct`, any other delimiter as a string |
+| setting   | `comma`         | No        | The delimiter for the number     | `space`, `comma`, `punct`, any other delimiter as a string |
 
 </details>
 <br />
 
 ## abbreviate
 
 ```python
@@ -217,14 +217,23 @@
 <br />
 
 # Changelog
 
 ## v0.1.x
 
 <details open>
+<summary><strong>v0.1.2</strong></summary>
+
+- README updated
+  - Repo links updated
+- `color` dir typing fixed; No more import error
+
+</details>
+
+<details>
 <summary><strong>v0.1.1</strong></summary>
 
 - README completed
 - `parse_date` error fixed
   - Used tp return `month` object when `nll` was specifically set as an arg for `c_format`
 - Moved codebase into `src` folder
```

### Comparing `qolpy-0.1.1/setup.py` & `qolpy-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="qolpy",
-    version="0.1.1",
+    version="0.1.2",
     description="A suite of random but useful functions that are aimed at giving you 'piece of cake' level comfortability",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/lewisjr/qolpy.git",
+    url="https://github.com/cerebrusinc/qolpy.git",
     project_urls={
-        "Bug Tracker": "https://github.com/lewisjr/qolpy/issues",
+        "Bug Tracker": "https://github.com/cerebrusinc/qolpy/issues",
     },
     author = "Cerebrus Inc | Lewis Mosho Jr",
     author_email = "lewis@cerebrus.dev",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

### Comparing `qolpy-0.1.1/src/qolpy/colour/main.py` & `qolpy-0.1.2/src/qolpy/colour/main.py`

 * *Files identical despite different names*

### Comparing `qolpy-0.1.1/src/qolpy/colour/switch.py` & `qolpy-0.1.2/src/qolpy/colour/switch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import Literal, Union, Any
+from typing import Union, Literal, Any, List, Tuple
 from .interface import Colour_Setting
 
 class FauxSwitch(object):
     """A lambda class based switch to change hex to other colour format"""
     def switch(self, setting: Colour_Setting, r_hex: str) -> Union[Any, Literal[False]]:
         """A lambda class based switch to change hex to other colour format"""
         formated_setting: str = f"__to_{setting}__"
         colour_switch = getattr(self, formated_setting, lambda r_hex=r_hex: False)
         return colour_switch(r_hex)
     
     @staticmethod
-    def __compute_colour__(r: int, g: int, b: int, setting: Literal["cmyk", "hs*"]) -> list[float]:
+    def __compute_colour__(r: int, g: int, b: int, setting: Literal["cmyk", "hs*"]) -> List[float]:
         if setting == "cmyk":
             cc: float = 1 - r / 255
             cm: float = 1 - g / 255
             cy: float = 1 - b / 255
             ck: float = min(cc, cm, cy)
             return [cc, cm, cy, ck]
         
         cr: float = r / 255
         cg: float = g / 255
         cb: float = b / 255
         c_min: float = min(cr, cg, cb)
         c_max: float = max(cr, cg, cb)
         return [cr, cg, cb, c_min, c_max]
     
-    def __to_rgb__(self, r_hex: str) -> tuple[str, int, int, int]:
+    def __to_rgb__(self, r_hex: str) -> Tuple[str, int, int, int]:
         """
         Convert a hex to RGB
     
         Args:
 		    hex: the colour as a hex
         
         Returns:
@@ -39,15 +39,15 @@
         g = int(r_hex[2:4], 16)
         b = int(r_hex[4:6], 16)
 
         as_string: str = f"rbg({r}, {g}, {b})"
 
         return (as_string, r, g, b)
 
-    def __to_cmyk__(self, r_hex: str) -> tuple[str, float, float, float, float]:
+    def __to_cmyk__(self, r_hex: str) -> Tuple[str, float, float, float, float]:
         """
         Convert a hex to CMYK
 	
         Args:
             hex: the colour as a hex
 
         Returns:
@@ -69,15 +69,15 @@
         y: float = dy * 100
         k: float = ck * 100
 
         as_string: str = f"cmyk({c}%, {m}%, {y}%, {k}%)"
 
         return (as_string, c, m, y, k)
     
-    def __to_hsv__(self, r_hex: str) -> tuple[str, float, float, float]:
+    def __to_hsv__(self, r_hex: str) -> Tuple[str, float, float, float]:
         """
         Convert a hex to HSV
 	
         Args:
             hex: the colour as a hex
 
         Returns:
@@ -96,15 +96,15 @@
         s: float = cS * 100
         v: float = cv * 100
 
         as_string: str = f"hsv({h}, {s}%, {v}%)"
 
         return (as_string, h, s, v)
 
-    def __to_hsl__(self, r_hex: str) -> tuple[str, float, float, float]:
+    def __to_hsl__(self, r_hex: str) -> Tuple[str, float, float, float]:
         """
 	    Convert a hex to HSL
 
         Args:
         	hex: the colour as a hex
 
         Returns:
```

### Comparing `qolpy-0.1.1/src/qolpy/date/interface.py` & `qolpy-0.1.2/src/qolpy/date/interface.py`

 * *Files identical despite different names*

### Comparing `qolpy-0.1.1/src/qolpy/date/main.py` & `qolpy-0.1.2/src/qolpy/date/main.py`

 * *Files identical despite different names*

### Comparing `qolpy-0.1.1/src/qolpy/date/switch.py` & `qolpy-0.1.2/src/qolpy/date/switch.py`

 * *Files identical despite different names*

### Comparing `qolpy-0.1.1/src/qolpy/number/main.py` & `qolpy-0.1.2/src/qolpy/number/main.py`

 * *Files identical despite different names*

### Comparing `qolpy-0.1.1/src/qolpy/string/main.py` & `qolpy-0.1.2/src/qolpy/string/main.py`

 * *Files identical despite different names*

### Comparing `qolpy-0.1.1/src/qolpy.egg-info/PKG-INFO` & `qolpy-0.1.2/src/qolpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qolpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A suite of random but useful functions that are aimed at giving you 'piece of cake' level comfortability
-Home-page: https://github.com/lewisjr/qolpy.git
+Home-page: https://github.com/cerebrusinc/qolpy.git
 Author: Cerebrus Inc | Lewis Mosho Jr
 Author-email: lewis@cerebrus.dev
-Project-URL: Bug Tracker, https://github.com/lewisjr/qolpy/issues
+Project-URL: Bug Tracker, https://github.com/cerebrusinc/qolpy/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
@@ -18,19 +18,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img src="https://drive.google.com/uc?id=1r9L_Kjdm1i4lCYOCq-bngr-yTl6OZ_lu" alt="py-qol logo" width="250" height="250" />
 </p>
 
-# qolpy v0.1.1
+# qolpy v0.1.2
 
 Are you tired of making the same module in every project? Not a problem! Qol has your back.
 
-A suite of random but useful functions that are aimed at giving you "piece of cake" level comfortability. This is a python port of the [javascript quality of life](https://github.com/lewisjr/qol) and [javascript fstring](https://github.com/lewisjr/fstring) package
+A suite of random but useful functions that are aimed at giving you "piece of cake" level comfortability. This is a python port of the [javascript quality of life](https://github.com/cerebrusinc/qol) and [javascript fstring](https://github.com/cerebrusinc/fstring) package
 
 # Installation
 
     pip install qolpy
 
 or
 
@@ -57,15 +57,15 @@
 ```python
 c = random_colour()
 c_rgb = random_colour("rgb")
 c_cmyk = random_colour("cmyk")
 c_hsv = random_colour("hsv")
 c_hsl = random_colour("hsl")
 
-print(c, c_rgb, c_cmyk, c_hsv, c_hsl);
+print(c, c_rgb, c_cmyk, c_hsv, c_hsl)
 # #f7f7f7, rgb(247,247,247), cmyk(0%,0%,0%,3%), hsv(0,0%,97%), hsl(0,0%,97%)
 ```
 
 <details>
 <summary><strong>Params</strong></summary>
 
 | Parameter | Default Setting | Required? | Definition                                 | Options                            |
@@ -153,15 +153,15 @@
 
 <details>
 <summary><strong>Params</strong></summary>
 
 | Parameter | Default Setting | Required? | Definition                       | Options                                                    |
 | --------- | --------------- | --------- | -------------------------------- | ---------------------------------------------------------- |
 | value     | `undefined`     | Yes       | The number you want to be parsed | `none`                                                     |
-| setting   | `undefined`     | Yes       | The delimiter for the number     | `space`, `comma`, `punct`, any other delimiter as a string |
+| setting   | `comma`         | No        | The delimiter for the number     | `space`, `comma`, `punct`, any other delimiter as a string |
 
 </details>
 <br />
 
 ## abbreviate
 
 ```python
@@ -237,14 +237,23 @@
 <br />
 
 # Changelog
 
 ## v0.1.x
 
 <details open>
+<summary><strong>v0.1.2</strong></summary>
+
+- README updated
+  - Repo links updated
+- `color` dir typing fixed; No more import error
+
+</details>
+
+<details>
 <summary><strong>v0.1.1</strong></summary>
 
 - README completed
 - `parse_date` error fixed
   - Used tp return `month` object when `nll` was specifically set as an arg for `c_format`
 - Moved codebase into `src` folder
```

### Comparing `qolpy-0.1.1/src/qolpy.egg-info/SOURCES.txt` & `qolpy-0.1.2/src/qolpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

