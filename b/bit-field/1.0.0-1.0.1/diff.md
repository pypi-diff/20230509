# Comparing `tmp/bit_field-1.0.0.tar.gz` & `tmp/bit_field-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bit_field-1.0.0.tar", last modified: Mon May  8 19:55:51 2023, max compression
+gzip compressed data, was "bit_field-1.0.1.tar", last modified: Tue May  9 17:31:28 2023, max compression
```

## Comparing `bit_field-1.0.0.tar` & `bit_field-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:51.107464 bit_field-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 19:55:35.000000 bit_field-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 19:55:35.000000 bit_field-1.0.0/LICENSE-ORIGINAL
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-08 19:55:51.107464 bit_field-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-08 19:55:35.000000 bit_field-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:51.107464 bit_field-1.0.0/bit_field/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/jsonml_stringify.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-08 19:55:35.000000 bit_field-1.0.0/bit_field/tspan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:55:51.107464 bit_field-1.0.0/bit_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 19:55:51.000000 bit_field-1.0.0/bit_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 19:55:35.000000 bit_field-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-08 19:55:51.111464 bit_field-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:28.566752 bit_field-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-09 17:31:12.000000 bit_field-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-09 17:31:12.000000 bit_field-1.0.1/LICENSE-ORIGINAL
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-09 17:31:28.566752 bit_field-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-09 17:31:12.000000 bit_field-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:28.558751 bit_field-1.0.1/bit_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-09 17:31:12.000000 bit_field-1.0.1/bit_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 17:31:12.000000 bit_field-1.0.1/bit_field/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-09 17:31:12.000000 bit_field-1.0.1/bit_field/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-09 17:31:12.000000 bit_field-1.0.1/bit_field/jsonml_stringify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-05-09 17:31:12.000000 bit_field-1.0.1/bit_field/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-09 17:31:12.000000 bit_field-1.0.1/bit_field/tspan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:28.566752 bit_field-1.0.1/bit_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-09 17:31:28.000000 bit_field-1.0.1/bit_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-09 17:31:28.000000 bit_field-1.0.1/bit_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:31:28.000000 bit_field-1.0.1/bit_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-09 17:31:28.000000 bit_field-1.0.1/bit_field.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 17:31:28.000000 bit_field-1.0.1/bit_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 17:31:28.000000 bit_field-1.0.1/bit_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 17:31:12.000000 bit_field-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-09 17:31:28.566752 bit_field-1.0.1/setup.cfg
```

### Comparing `bit_field-1.0.0/LICENSE` & `bit_field-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bit_field-1.0.0/LICENSE-ORIGINAL` & `bit_field-1.0.1/LICENSE-ORIGINAL`

 * *Files identical despite different names*

### Comparing `bit_field-1.0.0/PKG-INFO` & `bit_field-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bit_field
-Version: 1.0.0
+Version: 1.0.1
 Summary: A bitfield diagram renderer
 Home-page: https://github.com/Arth-ur/bitfield
 Author: Arthur Gay
 License: MIT
 Keywords: bitfield,bytefield,diagram,renderer,svg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bit_field-1.0.0/README.md` & `bit_field-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bit_field-1.0.0/bit_field/cli.py` & `bit_field-1.0.1/bit_field/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                      bits=args.bits,
                      fontfamily=args.fontfamily,
                      fontweight=args.fontweight,
                      fontsize=args.fontsize,
                      compact=args.compact,
                      hflip=args.hflip,
                      vflip=args.vflip,
-                     stroke_width=args.stroke_width,
+                     strokewidth=args.strokewidth,
                      trim=args.trim,
                      uneven=args.uneven,
                      legend={key: value for key, value in args.legend} if args.legend else None)
 
     res = jsonml_stringify(res)
     if args.beautify:
         res = beautify(res)
```

### Comparing `bit_field-1.0.0/bit_field/render.py` & `bit_field-1.0.1/bit_field/render.py`

 * *Files identical despite different names*

### Comparing `bit_field-1.0.0/bit_field/tspan.py` & `bit_field-1.0.1/bit_field/tspan.py`

 * *Files identical despite different names*

### Comparing `bit_field-1.0.0/bit_field.egg-info/PKG-INFO` & `bit_field-1.0.1/bit_field.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bit-field
-Version: 1.0.0
+Version: 1.0.1
 Summary: A bitfield diagram renderer
 Home-page: https://github.com/Arth-ur/bitfield
 Author: Arthur Gay
 License: MIT
 Keywords: bitfield,bytefield,diagram,renderer,svg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bit_field-1.0.0/setup.cfg` & `bit_field-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bit_field
-version = 1.0.0
+version = 1.0.1
 author = Arthur Gay
 description = A bitfield diagram renderer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Arth-ur/bitfield
 classifiers = 
 	Programming Language :: Python :: 3
```

