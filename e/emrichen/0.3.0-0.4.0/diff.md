# Comparing `tmp/emrichen-0.3.0.tar.gz` & `tmp/emrichen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emrichen-0.3.0.tar", last modified: Thu Aug 25 06:46:48 2022, max compression
+gzip compressed data, was "emrichen-0.4.0.tar", last modified: Tue May  9 06:48:59 2023, max compression
```

## Comparing `emrichen-0.3.0.tar` & `emrichen-0.4.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2022-08-25 06:46:48.535231 emrichen-0.3.0/
--rw-r--r--   0 akx        (501) staff       (20)     1128 2022-01-11 14:49:12.000000 emrichen-0.3.0/LICENSE
--rw-r--r--   0 akx        (501) staff       (20)       25 2018-08-08 14:16:13.000000 emrichen-0.3.0/MANIFEST.in
--rw-r--r--   0 akx        (501) staff       (20)    16851 2022-08-25 06:46:48.535373 emrichen-0.3.0/PKG-INFO
--rw-r--r--   0 akx        (501) staff       (20)    16515 2022-08-25 06:45:59.000000 emrichen-0.3.0/README.md
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2022-08-25 06:46:48.523166 emrichen-0.3.0/emrichen/
--rw-r--r--   0 akx        (501) staff       (20)      773 2022-08-25 06:45:20.000000 emrichen-0.3.0/emrichen/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)     1438 2022-08-25 06:44:35.000000 emrichen-0.3.0/emrichen/__main__.py
--rw-r--r--   0 akx        (501) staff       (20)     2539 2022-08-25 06:44:35.000000 emrichen-0.3.0/emrichen/cli.py
--rw-r--r--   0 akx        (501) staff       (20)     2079 2022-02-18 10:01:01.000000 emrichen-0.3.0/emrichen/context.py
--rw-r--r--   0 akx        (501) staff       (20)      448 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/documents_list.py
--rw-r--r--   0 akx        (501) staff       (20)       37 2018-09-07 10:38:29.000000 emrichen-0.3.0/emrichen/exceptions.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2022-08-25 06:46:48.525444 emrichen-0.3.0/emrichen/input/
--rw-r--r--   0 akx        (501) staff       (20)      335 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/input/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)     1153 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/input/json.py
--rw-r--r--   0 akx        (501) staff       (20)      526 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/input/utils.py
--rw-r--r--   0 akx        (501) staff       (20)     2198 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/input/yaml.py
--rw-r--r--   0 akx        (501) staff       (20)     1284 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/output.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2022-08-25 06:46:48.535066 emrichen-0.3.0/emrichen/tags/
--rw-r--r--   0 akx        (501) staff       (20)     1451 2022-08-25 06:46:02.000000 emrichen-0.3.0/emrichen/tags/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)      342 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/all.py
--rw-r--r--   0 akx        (501) staff       (20)      361 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/any.py
--rw-r--r--   0 akx        (501) staff       (20)      743 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/base.py
--rw-r--r--   0 akx        (501) staff       (20)      531 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/base64.py
--rw-r--r--   0 akx        (501) staff       (20)      712 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/compose.py
--rw-r--r--   0 akx        (501) staff       (20)      420 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/concat.py
--rw-r--r--   0 akx        (501) staff       (20)      592 2021-03-11 08:37:45.000000 emrichen-0.3.0/emrichen/tags/debug.py
--rw-r--r--   0 akx        (501) staff       (20)      864 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/defaults.py
--rw-r--r--   0 akx        (501) staff       (20)      525 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/error.py
--rw-r--r--   0 akx        (501) staff       (20)      454 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/exists.py
--rw-r--r--   0 akx        (501) staff       (20)     1334 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/filter.py
--rw-r--r--   0 akx        (501) staff       (20)     1386 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/format.py
--rw-r--r--   0 akx        (501) staff       (20)     1012 2022-08-25 06:44:35.000000 emrichen-0.3.0/emrichen/tags/hash.py
--rw-r--r--   0 akx        (501) staff       (20)      836 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/if_.py
--rw-r--r--   0 akx        (501) staff       (20)     4223 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/include.py
--rw-r--r--   0 akx        (501) staff       (20)     2727 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/index.py
--rw-r--r--   0 akx        (501) staff       (20)     1225 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/join.py
--rw-r--r--   0 akx        (501) staff       (20)     1267 2022-02-18 10:01:01.000000 emrichen-0.3.0/emrichen/tags/lookup.py
--rw-r--r--   0 akx        (501) staff       (20)     3969 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/loop.py
--rw-r--r--   0 akx        (501) staff       (20)      521 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/merge.py
--rw-r--r--   0 akx        (501) staff       (20)      345 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/not_.py
--rw-r--r--   0 akx        (501) staff       (20)     1650 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/op.py
--rw-r--r--   0 akx        (501) staff       (20)     1762 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/typeop.py
--rw-r--r--   0 akx        (501) staff       (20)     2764 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/urlencode.py
--rw-r--r--   0 akx        (501) staff       (20)      305 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/var.py
--rw-r--r--   0 akx        (501) staff       (20)      437 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/void.py
--rw-r--r--   0 akx        (501) staff       (20)      633 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/tags/with_.py
--rw-r--r--   0 akx        (501) staff       (20)     2213 2022-01-11 14:49:12.000000 emrichen-0.3.0/emrichen/template.py
--rw-r--r--   0 akx        (501) staff       (20)      111 2018-08-14 06:47:24.000000 emrichen-0.3.0/emrichen/void.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2022-08-25 06:46:48.524711 emrichen-0.3.0/emrichen.egg-info/
--rw-r--r--   0 akx        (501) staff       (20)    16851 2022-08-25 06:46:48.000000 emrichen-0.3.0/emrichen.egg-info/PKG-INFO
--rw-r--r--   0 akx        (501) staff       (20)     1205 2022-08-25 06:46:48.000000 emrichen-0.3.0/emrichen.egg-info/SOURCES.txt
--rw-r--r--   0 akx        (501) staff       (20)        1 2022-08-25 06:46:48.000000 emrichen-0.3.0/emrichen.egg-info/dependency_links.txt
--rw-r--r--   0 akx        (501) staff       (20)       52 2022-08-25 06:46:48.000000 emrichen-0.3.0/emrichen.egg-info/entry_points.txt
--rw-r--r--   0 akx        (501) staff       (20)      131 2022-08-25 06:46:48.000000 emrichen-0.3.0/emrichen.egg-info/requires.txt
--rw-r--r--   0 akx        (501) staff       (20)       15 2022-08-25 06:46:48.000000 emrichen-0.3.0/emrichen.egg-info/top_level.txt
--rw-r--r--   0 akx        (501) staff       (20)        1 2022-08-25 06:46:48.000000 emrichen-0.3.0/emrichen.egg-info/zip-safe
--rw-r--r--   0 akx        (501) staff       (20)      181 2022-01-11 14:49:12.000000 emrichen-0.3.0/pyproject.toml
--rw-r--r--   0 akx        (501) staff       (20)      856 2022-08-25 06:46:48.535904 emrichen-0.3.0/setup.cfg
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2023-05-09 06:48:59.978614 emrichen-0.4.0/
+-rw-r--r--   0 akx        (501) staff       (20)     1128 2022-01-11 14:49:12.000000 emrichen-0.4.0/LICENSE
+-rw-r--r--   0 akx        (501) staff       (20)       25 2018-08-08 14:16:13.000000 emrichen-0.4.0/MANIFEST.in
+-rw-r--r--   0 akx        (501) staff       (20)    16851 2023-05-09 06:48:59.978788 emrichen-0.4.0/PKG-INFO
+-rw-r--r--   0 akx        (501) staff       (20)    16515 2023-05-09 06:44:37.000000 emrichen-0.4.0/README.md
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2023-05-09 06:48:59.966937 emrichen-0.4.0/emrichen/
+-rw-r--r--   0 akx        (501) staff       (20)      773 2023-05-09 06:47:47.000000 emrichen-0.4.0/emrichen/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)     1438 2022-08-25 07:11:13.000000 emrichen-0.4.0/emrichen/__main__.py
+-rw-r--r--   0 akx        (501) staff       (20)     2539 2022-08-25 07:11:13.000000 emrichen-0.4.0/emrichen/cli.py
+-rw-r--r--   0 akx        (501) staff       (20)     2079 2023-05-09 06:39:17.000000 emrichen-0.4.0/emrichen/context.py
+-rw-r--r--   0 akx        (501) staff       (20)      448 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/documents_list.py
+-rw-r--r--   0 akx        (501) staff       (20)       37 2018-09-07 10:38:29.000000 emrichen-0.4.0/emrichen/exceptions.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2023-05-09 06:48:59.970001 emrichen-0.4.0/emrichen/input/
+-rw-r--r--   0 akx        (501) staff       (20)      335 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/input/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)     1153 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/input/json.py
+-rw-r--r--   0 akx        (501) staff       (20)      526 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/input/utils.py
+-rw-r--r--   0 akx        (501) staff       (20)     2198 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/input/yaml.py
+-rw-r--r--   0 akx        (501) staff       (20)     1284 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/output.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2023-05-09 06:48:59.978386 emrichen-0.4.0/emrichen/tags/
+-rw-r--r--   0 akx        (501) staff       (20)     1451 2022-08-25 06:46:02.000000 emrichen-0.4.0/emrichen/tags/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)      342 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/all.py
+-rw-r--r--   0 akx        (501) staff       (20)      361 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/any.py
+-rw-r--r--   0 akx        (501) staff       (20)      743 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/base.py
+-rw-r--r--   0 akx        (501) staff       (20)      531 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/base64.py
+-rw-r--r--   0 akx        (501) staff       (20)      712 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/compose.py
+-rw-r--r--   0 akx        (501) staff       (20)      420 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/concat.py
+-rw-r--r--   0 akx        (501) staff       (20)      592 2021-03-11 08:37:45.000000 emrichen-0.4.0/emrichen/tags/debug.py
+-rw-r--r--   0 akx        (501) staff       (20)      864 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/defaults.py
+-rw-r--r--   0 akx        (501) staff       (20)      525 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/error.py
+-rw-r--r--   0 akx        (501) staff       (20)      454 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/exists.py
+-rw-r--r--   0 akx        (501) staff       (20)     1333 2023-05-09 06:47:11.000000 emrichen-0.4.0/emrichen/tags/filter.py
+-rw-r--r--   0 akx        (501) staff       (20)     1386 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/format.py
+-rw-r--r--   0 akx        (501) staff       (20)     1012 2022-08-25 07:11:13.000000 emrichen-0.4.0/emrichen/tags/hash.py
+-rw-r--r--   0 akx        (501) staff       (20)      836 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/if_.py
+-rw-r--r--   0 akx        (501) staff       (20)     4223 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/include.py
+-rw-r--r--   0 akx        (501) staff       (20)     2725 2023-05-09 06:47:11.000000 emrichen-0.4.0/emrichen/tags/index.py
+-rw-r--r--   0 akx        (501) staff       (20)     1225 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/join.py
+-rw-r--r--   0 akx        (501) staff       (20)     1267 2023-05-09 06:39:17.000000 emrichen-0.4.0/emrichen/tags/lookup.py
+-rw-r--r--   0 akx        (501) staff       (20)     3969 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/loop.py
+-rw-r--r--   0 akx        (501) staff       (20)      521 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/merge.py
+-rw-r--r--   0 akx        (501) staff       (20)      345 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/not_.py
+-rw-r--r--   0 akx        (501) staff       (20)     1803 2023-05-09 06:39:21.000000 emrichen-0.4.0/emrichen/tags/op.py
+-rw-r--r--   0 akx        (501) staff       (20)     1762 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/typeop.py
+-rw-r--r--   0 akx        (501) staff       (20)     2764 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/urlencode.py
+-rw-r--r--   0 akx        (501) staff       (20)      305 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/var.py
+-rw-r--r--   0 akx        (501) staff       (20)      437 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/void.py
+-rw-r--r--   0 akx        (501) staff       (20)      633 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/tags/with_.py
+-rw-r--r--   0 akx        (501) staff       (20)     2213 2022-01-11 14:49:12.000000 emrichen-0.4.0/emrichen/template.py
+-rw-r--r--   0 akx        (501) staff       (20)      111 2018-08-14 06:47:24.000000 emrichen-0.4.0/emrichen/void.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2023-05-09 06:48:59.968892 emrichen-0.4.0/emrichen.egg-info/
+-rw-r--r--   0 akx        (501) staff       (20)    16851 2023-05-09 06:48:59.000000 emrichen-0.4.0/emrichen.egg-info/PKG-INFO
+-rw-r--r--   0 akx        (501) staff       (20)     1205 2023-05-09 06:48:59.000000 emrichen-0.4.0/emrichen.egg-info/SOURCES.txt
+-rw-r--r--   0 akx        (501) staff       (20)        1 2023-05-09 06:48:59.000000 emrichen-0.4.0/emrichen.egg-info/dependency_links.txt
+-rw-r--r--   0 akx        (501) staff       (20)       52 2023-05-09 06:48:59.000000 emrichen-0.4.0/emrichen.egg-info/entry_points.txt
+-rw-r--r--   0 akx        (501) staff       (20)      138 2023-05-09 06:48:59.000000 emrichen-0.4.0/emrichen.egg-info/requires.txt
+-rw-r--r--   0 akx        (501) staff       (20)       15 2023-05-09 06:48:59.000000 emrichen-0.4.0/emrichen.egg-info/top_level.txt
+-rw-r--r--   0 akx        (501) staff       (20)        1 2022-08-25 06:46:48.000000 emrichen-0.4.0/emrichen.egg-info/zip-safe
+-rw-r--r--   0 akx        (501) staff       (20)      212 2023-05-09 06:42:46.000000 emrichen-0.4.0/pyproject.toml
+-rw-r--r--   0 akx        (501) staff       (20)      863 2023-05-09 06:48:59.979483 emrichen-0.4.0/setup.cfg
```

### Comparing `emrichen-0.3.0/LICENSE` & `emrichen-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/PKG-INFO` & `emrichen-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emrichen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Template engine for YAML & JSON
 Home-page: http://github.com/con2/emrichen
 Author: Santtu Pajukanta
 Author-email: santtu@pajukanta.fi
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `emrichen-0.3.0/README.md` & `emrichen-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/__init__.py` & `emrichen-0.4.0/emrichen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TextIO, Union
 
 from .context import Context
 from .tags import Var
 from .template import Template
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 
 __all__ = ['Context', 'Template', 'Var', 'emrichen']
 
 
 def emrichen(template: Union[str, TextIO], *variable_sources, **override_variables) -> str:
     """
```

### Comparing `emrichen-0.3.0/emrichen/__main__.py` & `emrichen-0.4.0/emrichen/__main__.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/cli.py` & `emrichen-0.4.0/emrichen/cli.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/context.py` & `emrichen-0.4.0/emrichen/context.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/input/json.py` & `emrichen-0.4.0/emrichen/input/json.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/input/utils.py` & `emrichen-0.4.0/emrichen/input/utils.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/input/yaml.py` & `emrichen-0.4.0/emrichen/input/yaml.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/output.py` & `emrichen-0.4.0/emrichen/output.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/__init__.py` & `emrichen-0.4.0/emrichen/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/base.py` & `emrichen-0.4.0/emrichen/tags/base.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/base64.py` & `emrichen-0.4.0/emrichen/tags/base64.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/compose.py` & `emrichen-0.4.0/emrichen/tags/compose.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/debug.py` & `emrichen-0.4.0/emrichen/tags/debug.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/defaults.py` & `emrichen-0.4.0/emrichen/tags/defaults.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/error.py` & `emrichen-0.4.0/emrichen/tags/error.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/filter.py` & `emrichen-0.4.0/emrichen/tags/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     example: See `tests/test_cond.py`
     description: Takes in a list and only returns elements that pass a predicate.
     """
 
     value_types = (dict,)
 
     def enrich(self, context: Context):
-
         as_ = str(self.data.get('as', 'item'))
         index_as = str(self.data.get('index_as') or '')
         test = self.data.get('test', Var(as_))
         iterable, is_mapping = get_iterable(self, self.data['over'], context)
 
         output: Union[OrderedDict, list] = OrderedDict() if is_mapping else []
```

### Comparing `emrichen-0.3.0/emrichen/tags/format.py` & `emrichen-0.4.0/emrichen/tags/format.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/hash.py` & `emrichen-0.4.0/emrichen/tags/hash.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/if_.py` & `emrichen-0.4.0/emrichen/tags/if_.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/include.py` & `emrichen-0.4.0/emrichen/tags/include.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/index.py` & `emrichen-0.4.0/emrichen/tags/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         if 'template' not in data:
             as_ = data.get('as', 'item')
             data = dict(data, template=Var(as_))
 
         super().__init__(data)
 
     def process_item(self, context: Context, output: dict, value, result) -> None:
-
         by = self.data['by']
         result_as = self.data.get('result_as')
 
         if result_as:
             context = Context(context, {result_as: result})
 
         key = context.enrich(by)
@@ -68,15 +67,14 @@
         `result_as`: (optional, string) When evaluating `by`, the enriched `template` is available under this name.
 
     example: TBD
     description: Makes a dict out of a list. Keys are determined by `by`. Items with the same key are grouped in a list.
     """
 
     def process_item(self, context: Context, output: dict, value, result) -> None:
-
         by = self.data['by']
         result_as = self.data.get('result_as')
 
         if result_as:
             context = Context(context, {result_as: result})
 
         key = context.enrich(by)
```

### Comparing `emrichen-0.3.0/emrichen/tags/join.py` & `emrichen-0.4.0/emrichen/tags/join.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/lookup.py` & `emrichen-0.4.0/emrichen/tags/lookup.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/loop.py` & `emrichen-0.4.0/emrichen/tags/loop.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/merge.py` & `emrichen-0.4.0/emrichen/tags/merge.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/op.py` & `emrichen-0.4.0/emrichen/tags/op.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import operator
+from typing import Any, Callable, Dict, List, Tuple
 
 from ..context import Context
 from .base import BaseTag
 
-operator_list = [
+OpFunc = Callable[[Any, Any], Any]
+
+operator_list: List[Tuple[Tuple[str, ...], OpFunc]] = [
     (('=', '==', '===', 'eq'), operator.eq),
     (('≠', '!=', '!==', 'ne'), operator.ne),
+    (('<=', 'le', 'lte'), operator.le),
     (('>=', 'ge', 'gte'), operator.ge),
-    (('>', 'gt'), operator.gt),
     (('<', 'lt'), operator.lt),
     (('>', 'gt'), operator.gt),
     (('in', '∈'), operator.contains),
     (('not in', '∉'), lambda a, b: not operator.contains(a, b)),
     (('+', 'plus', 'add'), operator.add),
     (('-', 'minus', 'sub', 'subtract'), operator.sub),
     (('*', '×', 'mul', 'times'), operator.mul),
     (('/', '÷', 'div', 'divide', 'truediv'), operator.truediv),
     (('//', 'floordiv'), operator.floordiv),
 ]
 
-operators = {}
+operators: Dict[str, OpFunc] = {}
 for aliases, func in operator_list:
     for alias in aliases:
         operators[alias] = func
 
 
 class Op(BaseTag):
     """
```

### Comparing `emrichen-0.3.0/emrichen/tags/typeop.py` & `emrichen-0.4.0/emrichen/tags/typeop.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/urlencode.py` & `emrichen-0.4.0/emrichen/tags/urlencode.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/tags/with_.py` & `emrichen-0.4.0/emrichen/tags/with_.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen/template.py` & `emrichen-0.4.0/emrichen/template.py`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/emrichen.egg-info/PKG-INFO` & `emrichen-0.4.0/emrichen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emrichen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Template engine for YAML & JSON
 Home-page: http://github.com/con2/emrichen
 Author: Santtu Pajukanta
 Author-email: santtu@pajukanta.fi
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `emrichen-0.3.0/emrichen.egg-info/SOURCES.txt` & `emrichen-0.4.0/emrichen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emrichen-0.3.0/setup.cfg` & `emrichen-0.4.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 [options]
 packages = find:
 zip_safe = True
 python_requires = >=3.6
 install_requires = 
 	PyYAML
-	pyaml
+	pyaml~=21.10
 	jsonpath-rw~=1.4.0
 
 [options.entry_points]
 console_scripts = 
 	emrichen = emrichen.__main__:main
 
 [options.extras_require]
 test = 
 	pytest~=6.2.3
 	pytest-cov~=2.0
 lint = 
-	black>=21.7b0
+	black==23.3.0
 	flake8>=3.9.2
-	mypy>=0.910
+	mypy>=0.971
 	isort>=5.9.2
 
 [tool:pytest]
 addopts = --verbose
 python_files = tests/*.py
 
 [flake8]
```

