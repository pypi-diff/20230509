# Comparing `tmp/example_qazedc-0.3.0.tar.gz` & `tmp/example_qazedc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_qazedc-0.3.0.tar", last modified: Tue May  9 07:49:56 2023, max compression
+gzip compressed data, was "example_qazedc-1.0.0.tar", last modified: Tue May  9 07:42:29 2023, max compression
```

## Comparing `example_qazedc-0.3.0.tar` & `example_qazedc-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 07:49:56.900759 example_qazedc-0.3.0/
--rw-rw-rw-   0        0        0     1053 2023-05-08 06:42:14.000000 example_qazedc-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      241 2023-05-09 07:49:56.900759 example_qazedc-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      131 2023-05-08 06:43:49.000000 example_qazedc-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 07:49:56.900759 example_qazedc-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      453 2023-05-09 07:49:44.000000 example_qazedc-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:49:56.894759 example_qazedc-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 07:49:56.897759 example_qazedc-0.3.0/src/example_package_qazedc/
--rw-rw-rw-   0        0        0       53 2023-05-09 07:49:44.000000 example_qazedc-0.3.0/src/example_package_qazedc/__init__.py
--rw-rw-rw-   0        0        0      125 2023-05-09 07:49:44.000000 example_qazedc-0.3.0/src/example_package_qazedc/example.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:49:56.899759 example_qazedc-0.3.0/src/example_qazedc.egg-info/
--rw-rw-rw-   0        0        0      241 2023-05-09 07:49:56.000000 example_qazedc-0.3.0/src/example_qazedc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-09 07:49:56.000000 example_qazedc-0.3.0/src/example_qazedc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 07:49:56.000000 example_qazedc-0.3.0/src/example_qazedc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-09 07:49:56.000000 example_qazedc-0.3.0/src/example_qazedc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 07:42:29.417904 example_qazedc-1.0.0/
+-rw-rw-rw-   0        0        0     1053 2023-05-08 06:42:14.000000 example_qazedc-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      241 2023-05-09 07:42:29.417904 example_qazedc-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2023-05-08 06:43:49.000000 example_qazedc-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 07:42:29.417904 example_qazedc-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      453 2023-05-09 07:08:49.000000 example_qazedc-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:42:29.411307 example_qazedc-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 07:42:29.413905 example_qazedc-1.0.0/src/example_package_qazedc/
+-rw-rw-rw-   0        0        0       53 2023-05-09 07:20:53.000000 example_qazedc-1.0.0/src/example_package_qazedc/__init__.py
+-rw-rw-rw-   0        0        0      125 2023-05-09 07:08:49.000000 example_qazedc-1.0.0/src/example_package_qazedc/example.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:42:29.417904 example_qazedc-1.0.0/src/example_qazedc.egg-info/
+-rw-rw-rw-   0        0        0      241 2023-05-09 07:42:29.000000 example_qazedc-1.0.0/src/example_qazedc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-09 07:42:29.000000 example_qazedc-1.0.0/src/example_qazedc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 07:42:29.000000 example_qazedc-1.0.0/src/example_qazedc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-09 07:42:29.000000 example_qazedc-1.0.0/src/example_qazedc.egg-info/top_level.txt
```

### Comparing `example_qazedc-0.3.0/LICENSE` & `example_qazedc-1.0.0/LICENSE`

 * *Files identical despite different names*

