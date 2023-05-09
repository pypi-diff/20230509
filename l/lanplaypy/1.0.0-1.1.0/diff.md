# Comparing `tmp/lanplaypy-1.0.0.tar.gz` & `tmp/lanplaypy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanplaypy-1.0.0.tar", last modified: Tue May  2 04:09:12 2023, max compression
+gzip compressed data, was "lanplaypy-1.1.0.tar", last modified: Tue May  9 07:01:14 2023, max compression
```

## Comparing `lanplaypy-1.0.0.tar` & `lanplaypy-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 kilian    (1001) kilian    (1001)        0 2023-05-02 04:09:12.958139 lanplaypy-1.0.0/
--rw-r--r--   0 kilian    (1001) kilian    (1001)        0 2023-05-01 22:13:31.000000 lanplaypy-1.0.0/CHANGELOG
--rw-r--r--   0 kilian    (1001) kilian    (1001)     1075 2023-05-01 22:13:31.000000 lanplaypy-1.0.0/LICENCE
--rw-r--r--   0 kilian    (1001) kilian    (1001)     4520 2023-05-02 04:09:12.958139 lanplaypy-1.0.0/PKG-INFO
--rw-r--r--   0 kilian    (1001) kilian    (1001)     3905 2023-05-02 04:01:48.000000 lanplaypy-1.0.0/README.md
--rw-r--r--   0 kilian    (1001) kilian    (1001)      896 2023-05-02 04:09:12.958139 lanplaypy-1.0.0/setup.cfg
--rw-r--r--   0 kilian    (1001) kilian    (1001)       80 2023-05-02 04:08:16.000000 lanplaypy-1.0.0/setup.py
-drwxr-xr-x   0 kilian    (1001) kilian    (1001)        0 2023-05-02 04:09:12.948139 lanplaypy-1.0.0/src/
-drwxr-xr-x   0 kilian    (1001) kilian    (1001)        0 2023-05-02 04:09:12.958139 lanplaypy-1.0.0/src/lanplay/
--rw-r--r--   0 kilian    (1001) kilian    (1001)       22 2023-05-02 03:30:52.000000 lanplaypy-1.0.0/src/lanplay/__init__.py
--rw-r--r--   0 kilian    (1001) kilian    (1001)     7390 2023-05-02 03:11:01.000000 lanplaypy-1.0.0/src/lanplay/lanplay.py
-drwxr-xr-x   0 kilian    (1001) kilian    (1001)        0 2023-05-02 04:09:12.958139 lanplaypy-1.0.0/src/lanplaypy.egg-info/
--rw-r--r--   0 kilian    (1001) kilian    (1001)     4520 2023-05-02 04:09:12.000000 lanplaypy-1.0.0/src/lanplaypy.egg-info/PKG-INFO
--rw-r--r--   0 kilian    (1001) kilian    (1001)      313 2023-05-02 04:09:12.000000 lanplaypy-1.0.0/src/lanplaypy.egg-info/SOURCES.txt
--rw-r--r--   0 kilian    (1001) kilian    (1001)        1 2023-05-02 04:09:12.000000 lanplaypy-1.0.0/src/lanplaypy.egg-info/dependency_links.txt
--rw-r--r--   0 kilian    (1001) kilian    (1001)        1 2023-05-02 04:05:06.000000 lanplaypy-1.0.0/src/lanplaypy.egg-info/not-zip-safe
--rw-r--r--   0 kilian    (1001) kilian    (1001)       22 2023-05-02 04:09:12.000000 lanplaypy-1.0.0/src/lanplaypy.egg-info/requires.txt
--rw-r--r--   0 kilian    (1001) kilian    (1001)        8 2023-05-02 04:09:12.000000 lanplaypy-1.0.0/src/lanplaypy.egg-info/top_level.txt
+drwxr-xr-x   0 kilian    (1001) kilian    (1001)        0 2023-05-09 07:01:14.245963 lanplaypy-1.1.0/
+-rw-r--r--   0 kilian    (1001) kilian    (1001)      697 2023-05-09 06:54:09.000000 lanplaypy-1.1.0/CHANGELOG
+-rw-r--r--   0 kilian    (1001) kilian    (1001)     1075 2023-05-01 22:13:31.000000 lanplaypy-1.1.0/LICENSE
+-rw-r--r--   0 kilian    (1001) kilian    (1001)     8508 2023-05-09 07:01:14.245963 lanplaypy-1.1.0/PKG-INFO
+-rw-r--r--   0 kilian    (1001) kilian    (1001)     6099 2023-05-09 06:58:24.000000 lanplaypy-1.1.0/README.md
+-rw-r--r--   0 kilian    (1001) kilian    (1001)     1392 2023-05-09 07:01:14.245963 lanplaypy-1.1.0/setup.cfg
+-rw-r--r--   0 kilian    (1001) kilian    (1001)       80 2023-05-09 06:54:24.000000 lanplaypy-1.1.0/setup.py
+drwxr-xr-x   0 kilian    (1001) kilian    (1001)        0 2023-05-09 07:01:14.225963 lanplaypy-1.1.0/src/
+drwxr-xr-x   0 kilian    (1001) kilian    (1001)        0 2023-05-09 07:01:14.235963 lanplaypy-1.1.0/src/lanplay/
+-rw-r--r--   0 kilian    (1001) kilian    (1001)       29 2023-05-06 13:47:16.000000 lanplaypy-1.1.0/src/lanplay/__init__.py
+-rw-r--r--   0 kilian    (1001) kilian    (1001)     1449 2023-05-06 14:34:55.000000 lanplaypy-1.1.0/src/lanplay/functions.py
+-rw-r--r--   0 kilian    (1001) kilian    (1001)    12571 2023-05-09 06:47:18.000000 lanplaypy-1.1.0/src/lanplay/lanplay.py
+drwxr-xr-x   0 kilian    (1001) kilian    (1001)        0 2023-05-09 07:01:14.235963 lanplaypy-1.1.0/src/lanplaypy.egg-info/
+-rw-r--r--   0 kilian    (1001) kilian    (1001)     8508 2023-05-09 07:01:14.000000 lanplaypy-1.1.0/src/lanplaypy.egg-info/PKG-INFO
+-rw-r--r--   0 kilian    (1001) kilian    (1001)      338 2023-05-09 07:01:14.000000 lanplaypy-1.1.0/src/lanplaypy.egg-info/SOURCES.txt
+-rw-r--r--   0 kilian    (1001) kilian    (1001)        1 2023-05-09 07:01:14.000000 lanplaypy-1.1.0/src/lanplaypy.egg-info/dependency_links.txt
+-rw-r--r--   0 kilian    (1001) kilian    (1001)        1 2023-05-02 04:05:06.000000 lanplaypy-1.1.0/src/lanplaypy.egg-info/not-zip-safe
+-rw-r--r--   0 kilian    (1001) kilian    (1001)       56 2023-05-09 07:01:14.000000 lanplaypy-1.1.0/src/lanplaypy.egg-info/requires.txt
+-rw-r--r--   0 kilian    (1001) kilian    (1001)        8 2023-05-09 07:01:14.000000 lanplaypy-1.1.0/src/lanplaypy.egg-info/top_level.txt
```

### Comparing `lanplaypy-1.0.0/LICENCE` & `lanplaypy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lanplaypy-1.0.0/setup.cfg` & `lanplaypy-1.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -32,12 +32,37 @@
 
 [options.packages.find]
 where = src
 exclude = 
 	*.python-version
 	*__pycache__
 	tests
+	changelog.d
+
+[options.extras_require]
+dev = 
+	setuptools-changelog
+	build
+
+[changelog]
+changelog_fragments_path = changelog.d
+major_changes_types = 
+	epic = Epic Changes
+	breaking = Breaking Changes
+	removal = Breaking Changes
+minor_changes_types = 
+	security = Security Fixes
+	deprecation = Deprecations
+	feature = New Features
+patch_changes_types = 
+	bug = Bug Fixes
+	bugfix = Bug Fixes
+	improvement = Improvements
+	build = Build
+	doc = Documentation
+	test = Tests Suite
+	misc = Miscellaneous
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

