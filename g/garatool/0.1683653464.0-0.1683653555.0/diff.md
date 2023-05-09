# Comparing `tmp/garatool-0.1683653464.0.tar.gz` & `tmp/garatool-0.1683653555.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683653464.0.tar", last modified: Tue May  9 17:31:04 2023, max compression
+gzip compressed data, was "garatool-0.1683653555.0.tar", last modified: Tue May  9 17:32:36 2023, max compression
```

## Comparing `garatool-0.1683653464.0.tar` & `garatool-0.1683653555.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:31:04.857152 garatool-0.1683653464.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:31:04.856373 garatool-0.1683653464.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683653464.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:31:04.851610 garatool-0.1683653464.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5741 2023-05-09 17:31:03.000000 garatool-0.1683653464.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683653464.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:31:04.855400 garatool-0.1683653464.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:31:04.000000 garatool-0.1683653464.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:31:04.000000 garatool-0.1683653464.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:31:04.000000 garatool-0.1683653464.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:31:04.000000 garatool-0.1683653464.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:31:04.000000 garatool-0.1683653464.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:31:04.857293 garatool-0.1683653464.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683653464.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:32:36.062021 garatool-0.1683653555.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:32:36.061648 garatool-0.1683653555.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683653555.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:32:36.058179 garatool-0.1683653555.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5747 2023-05-09 17:32:09.000000 garatool-0.1683653555.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683653555.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:32:36.061042 garatool-0.1683653555.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:32:36.062162 garatool-0.1683653555.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683653555.0/setup.py
```

### Comparing `garatool-0.1683653464.0/garatool/__init__.py` & `garatool-0.1683653555.0/garatool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 colorama.init()
 
 def flag(str):
     return colored( str , 'yellow')
 def step(str):
     return colored( ':::::::' + str +  ':::::::', 'magenta', 'on_yellow')
 def cmd(str):
-    print('Run: ', colored(str, 'cyan'))
+    print('Run: ', colored(repr(str), 'cyan'))
     return str
 
 
 PYTHON = sys.executable
 ESPTOOL = f'"{PYTHON}" "{esptool.__file__}" '
```

### Comparing `garatool-0.1683653464.0/setup.py` & `garatool-0.1683653555.0/setup.py`

 * *Files identical despite different names*

