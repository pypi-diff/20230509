# Comparing `tmp/garatool-0.1683653262.0.tar.gz` & `tmp/garatool-0.1683653360.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683653262.0.tar", last modified: Tue May  9 17:27:42 2023, max compression
+gzip compressed data, was "garatool-0.1683653360.0.tar", last modified: Tue May  9 17:29:20 2023, max compression
```

## Comparing `garatool-0.1683653262.0.tar` & `garatool-0.1683653360.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:27:42.638134 garatool-0.1683653262.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:27:42.637791 garatool-0.1683653262.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683653262.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:27:42.634691 garatool-0.1683653262.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5741 2023-05-09 17:27:40.000000 garatool-0.1683653262.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683653262.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:27:42.637189 garatool-0.1683653262.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:27:42.000000 garatool-0.1683653262.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:27:42.000000 garatool-0.1683653262.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:27:42.000000 garatool-0.1683653262.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:27:42.000000 garatool-0.1683653262.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:27:42.000000 garatool-0.1683653262.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:27:42.638246 garatool-0.1683653262.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683653262.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:29:20.661382 garatool-0.1683653360.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:29:20.660985 garatool-0.1683653360.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683653360.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:29:20.657544 garatool-0.1683653360.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5743 2023-05-09 17:29:18.000000 garatool-0.1683653360.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683653360.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:29:20.660520 garatool-0.1683653360.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:29:20.000000 garatool-0.1683653360.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:29:20.000000 garatool-0.1683653360.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:29:20.000000 garatool-0.1683653360.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:29:20.000000 garatool-0.1683653360.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:29:20.000000 garatool-0.1683653360.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:29:20.661510 garatool-0.1683653360.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683653360.0/setup.py
```

### Comparing `garatool-0.1683653262.0/garatool/__init__.py` & `garatool-0.1683653360.0/garatool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     return colored( ':::::::' + str +  ':::::::', 'magenta', 'on_yellow')
 def cmd(str):
     print('Run: ', colored(str, 'cyan'))
     return str
 
 
 PYTHON = sys.executable
-ESPTOOL = f'"{PYTHON}" "{esptool.__file__}" '
+ESPTOOL = f'r"{PYTHON}" r"{esptool.__file__}" '
 
 
 class Board(Enum):
     CreatorPlus: str = 'plus'
     CreatorIoT : str = 'iot'
     def __str__(self):
         return self.name
```

### Comparing `garatool-0.1683653262.0/setup.py` & `garatool-0.1683653360.0/setup.py`

 * *Files identical despite different names*

