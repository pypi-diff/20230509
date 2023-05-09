# Comparing `tmp/zope.structuredtext-4.4.tar.gz` & `tmp/zope.structuredtext-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.structuredtext-4.4.tar", last modified: Fri Mar 18 07:18:46 2022, max compression
+gzip compressed data, was "zope.structuredtext-5.0.tar", last modified: Tue May  9 06:13:18 2023, max compression
```

## Comparing `zope.structuredtext-4.4.tar` & `zope.structuredtext-5.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-18 07:18:46.236049 zope.structuredtext-4.4/
--rw-r--r--   0 mac        (513) staff       (20)     1678 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      441 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4169 2022-03-18 07:18:46.236218 zope.structuredtext-4.4/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1275 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      348 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/TODO.txt
--rw-r--r--   0 mac        (513) staff       (20)      271 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)     1011 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/convert.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-18 07:18:46.214650 zope.structuredtext-4.4/docs/
--rw-r--r--   0 mac        (513) staff       (20)     3150 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      968 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)     7186 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)     5679 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     3095 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)      197 2022-03-18 07:18:46.236720 zope.structuredtext-4.4/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2860 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-18 07:18:46.208176 zope.structuredtext-4.4/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-18 07:18:46.215007 zope.structuredtext-4.4/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-18 07:18:46.220934 zope.structuredtext-4.4/src/zope/structuredtext/
--rw-r--r--   0 mac        (513) staff       (20)     2993 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    10369 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/docbook.py
--rw-r--r--   0 mac        (513) staff       (20)    26639 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/document.py
--rw-r--r--   0 mac        (513) staff       (20)     9508 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/html.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-18 07:18:46.235817 zope.structuredtext-4.4/src/zope/structuredtext/regressions/
--rw-r--r--   0 mac        (513) staff       (20)    10732 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/Acquisition.ref
--rw-r--r--   0 mac        (513) staff       (20)     9134 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/Acquisition.stx
--rw-r--r--   0 mac        (513) staff       (20)    11997 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/Acquisition.xml
--rw-r--r--   0 mac        (513) staff       (20)    32939 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/ExtensionClass.ref
--rw-r--r--   0 mac        (513) staff       (20)    30031 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/ExtensionClass.stx
--rw-r--r--   0 mac        (513) staff       (20)    36440 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/ExtensionClass.xml
--rw-r--r--   0 mac        (513) staff       (20)      340 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/InnerLinks.ref
--rw-r--r--   0 mac        (513) staff       (20)      160 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/InnerLinks.stx
--rw-r--r--   0 mac        (513) staff       (20)      428 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/InnerLinks.xml
--rw-r--r--   0 mac        (513) staff       (20)     1067 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/Links.ref
--rw-r--r--   0 mac        (513) staff       (20)      786 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/Links.stx
--rw-r--r--   0 mac        (513) staff       (20)     1457 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/Links.xml
--rw-r--r--   0 mac        (513) staff       (20)    13530 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/MultiMapping.ref
--rw-r--r--   0 mac        (513) staff       (20)    13250 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/MultiMapping.stx
--rw-r--r--   0 mac        (513) staff       (20)    12579 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/MultiMapping.xml
--rw-r--r--   0 mac        (513) staff       (20)     1548 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples.ref
--rw-r--r--   0 mac        (513) staff       (20)     1119 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples.stx
--rw-r--r--   0 mac        (513) staff       (20)     2329 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples.xml
--rw-r--r--   0 mac        (513) staff       (20)      219 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples1.ref
--rw-r--r--   0 mac        (513) staff       (20)       98 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples1.stx
--rw-r--r--   0 mac        (513) staff       (20)      266 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples1.xml
--rw-r--r--   0 mac        (513) staff       (20)      231 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/header_example.ref
--rw-r--r--   0 mac        (513) staff       (20)      165 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/header_example.stx
--rw-r--r--   0 mac        (513) staff       (20)      333 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/header_example.xml
--rw-r--r--   0 mac        (513) staff       (20)       91 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/images.ref
--rw-r--r--   0 mac        (513) staff       (20)       39 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/images.stx
--rw-r--r--   0 mac        (513) staff       (20)      109 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/images.xml
--rw-r--r--   0 mac        (513) staff       (20)     1953 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/index.ref
--rw-r--r--   0 mac        (513) staff       (20)     1707 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/index.stx
--rw-r--r--   0 mac        (513) staff       (20)     2318 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/index.xml
--rw-r--r--   0 mac        (513) staff       (20)      194 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/numbered_example.ref
--rw-r--r--   0 mac        (513) staff       (20)      108 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/numbered_example.stx
--rw-r--r--   0 mac        (513) staff       (20)      372 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/numbered_example.xml
--rw-r--r--   0 mac        (513) staff       (20)     2740 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/table.ref
--rw-r--r--   0 mac        (513) staff       (20)     2024 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/regressions/table.stx
--rw-r--r--   0 mac        (513) staff       (20)    12019 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/stdom.py
--rw-r--r--   0 mac        (513) staff       (20)     1057 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/stletters.py
--rw-r--r--   0 mac        (513) staff       (20)    15271 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/stng.py
--rw-r--r--   0 mac        (513) staff       (20)    21596 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/src/zope/structuredtext/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-03-18 07:18:46.217317 zope.structuredtext-4.4/src/zope.structuredtext.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4169 2022-03-18 07:18:45.000000 zope.structuredtext-4.4/src/zope.structuredtext.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     2630 2022-03-18 07:18:46.000000 zope.structuredtext-4.4/src/zope.structuredtext.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-03-18 07:18:45.000000 zope.structuredtext-4.4/src/zope.structuredtext.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-03-18 07:18:45.000000 zope.structuredtext-4.4/src/zope.structuredtext.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-03-18 07:18:45.000000 zope.structuredtext-4.4/src/zope.structuredtext.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       50 2022-03-18 07:18:45.000000 zope.structuredtext-4.4/src/zope.structuredtext.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-03-18 07:18:46.000000 zope.structuredtext-4.4/src/zope.structuredtext.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1654 2022-03-18 07:18:44.000000 zope.structuredtext-4.4/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-09 06:13:18.793496 zope.structuredtext-5.0/
+-rw-r--r--   0 mac        (513) staff       (20)     1845 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      441 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     4192 2023-05-09 06:13:18.793639 zope.structuredtext-5.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1275 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      348 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/TODO.txt
+-rw-r--r--   0 mac        (513) staff       (20)      271 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     1011 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/convert.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-09 06:13:18.772930 zope.structuredtext-5.0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     3150 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/docs/Makefile
+-rw-r--r--   0 mac        (513) staff       (20)      968 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/docs/api.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/docs/changelog.rst
+-rw-r--r--   0 mac        (513) staff       (20)     7186 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)     5680 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     3095 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/docs/make.bat
+-rw-r--r--   0 mac        (513) staff       (20)      470 2023-05-09 06:13:18.794211 zope.structuredtext-5.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2716 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-09 06:13:18.765155 zope.structuredtext-5.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-09 06:13:18.773436 zope.structuredtext-5.0/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-09 06:13:18.780295 zope.structuredtext-5.0/src/zope/structuredtext/
+-rw-r--r--   0 mac        (513) staff       (20)     2993 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    10293 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/docbook.py
+-rw-r--r--   0 mac        (513) staff       (20)    26363 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/document.py
+-rw-r--r--   0 mac        (513) staff       (20)     9383 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/html.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-09 06:13:18.793188 zope.structuredtext-5.0/src/zope/structuredtext/regressions/
+-rw-r--r--   0 mac        (513) staff       (20)    10732 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/Acquisition.ref
+-rw-r--r--   0 mac        (513) staff       (20)     9134 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/Acquisition.stx
+-rw-r--r--   0 mac        (513) staff       (20)    11997 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/Acquisition.xml
+-rw-r--r--   0 mac        (513) staff       (20)    32939 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/ExtensionClass.ref
+-rw-r--r--   0 mac        (513) staff       (20)    30031 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/ExtensionClass.stx
+-rw-r--r--   0 mac        (513) staff       (20)    36440 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/ExtensionClass.xml
+-rw-r--r--   0 mac        (513) staff       (20)      340 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/InnerLinks.ref
+-rw-r--r--   0 mac        (513) staff       (20)      160 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/InnerLinks.stx
+-rw-r--r--   0 mac        (513) staff       (20)      428 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/InnerLinks.xml
+-rw-r--r--   0 mac        (513) staff       (20)     1067 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/Links.ref
+-rw-r--r--   0 mac        (513) staff       (20)      786 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/Links.stx
+-rw-r--r--   0 mac        (513) staff       (20)     1457 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/Links.xml
+-rw-r--r--   0 mac        (513) staff       (20)    13530 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/MultiMapping.ref
+-rw-r--r--   0 mac        (513) staff       (20)    13250 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/MultiMapping.stx
+-rw-r--r--   0 mac        (513) staff       (20)    12579 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/MultiMapping.xml
+-rw-r--r--   0 mac        (513) staff       (20)     1548 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples.ref
+-rw-r--r--   0 mac        (513) staff       (20)     1119 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples.stx
+-rw-r--r--   0 mac        (513) staff       (20)     2329 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples.xml
+-rw-r--r--   0 mac        (513) staff       (20)      219 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples1.ref
+-rw-r--r--   0 mac        (513) staff       (20)       98 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples1.stx
+-rw-r--r--   0 mac        (513) staff       (20)      266 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples1.xml
+-rw-r--r--   0 mac        (513) staff       (20)      231 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/header_example.ref
+-rw-r--r--   0 mac        (513) staff       (20)      165 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/header_example.stx
+-rw-r--r--   0 mac        (513) staff       (20)      333 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/header_example.xml
+-rw-r--r--   0 mac        (513) staff       (20)       91 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/images.ref
+-rw-r--r--   0 mac        (513) staff       (20)       39 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/images.stx
+-rw-r--r--   0 mac        (513) staff       (20)      109 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/images.xml
+-rw-r--r--   0 mac        (513) staff       (20)     1953 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/index.ref
+-rw-r--r--   0 mac        (513) staff       (20)     1707 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/index.stx
+-rw-r--r--   0 mac        (513) staff       (20)     2318 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/index.xml
+-rw-r--r--   0 mac        (513) staff       (20)      194 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/numbered_example.ref
+-rw-r--r--   0 mac        (513) staff       (20)      108 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/numbered_example.stx
+-rw-r--r--   0 mac        (513) staff       (20)      372 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/numbered_example.xml
+-rw-r--r--   0 mac        (513) staff       (20)     2740 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/table.ref
+-rw-r--r--   0 mac        (513) staff       (20)     2024 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/regressions/table.stx
+-rw-r--r--   0 mac        (513) staff       (20)    11753 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/stdom.py
+-rw-r--r--   0 mac        (513) staff       (20)     1057 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/stletters.py
+-rw-r--r--   0 mac        (513) staff       (20)    15033 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/stng.py
+-rw-r--r--   0 mac        (513) staff       (20)    21545 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope/structuredtext/tests.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-09 06:13:18.777209 zope.structuredtext-5.0/src/zope.structuredtext.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     4192 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope.structuredtext.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     2630 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope.structuredtext.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope.structuredtext.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope.structuredtext.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope.structuredtext.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       50 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope.structuredtext.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/src/zope.structuredtext.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1831 2023-05-09 06:13:18.000000 zope.structuredtext-5.0/tox.ini
```

### Comparing `zope.structuredtext-4.4/CHANGES.rst` & `zope.structuredtext-5.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
  Changes
 =========
 
+5.0 (2023-05-09)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-03-18)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `zope.structuredtext-4.4/CONTRIBUTING.md` & `zope.structuredtext-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/LICENSE.txt` & `zope.structuredtext-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/PKG-INFO` & `zope.structuredtext-5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: zope.structuredtext
-Version: 4.4
+Version: 5.0
 Summary: StructuredText parser
 Home-page: http://github.com/zopefoundation/zope.structuredtext
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 =====================
  zope.structuredtext
 =====================
@@ -57,14 +54,24 @@
 Please see https://zopestructuredtext.readthedocs.org/ for documentation.
 
 
 =========
  Changes
 =========
 
+5.0 (2023-05-09)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-03-18)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -143,9 +150,7 @@
 
 
 3.0.0 (2004/11/07)
 ==================
 
 - Corresponds to the verison of the ``zope.structuredtext`` package shipped
   as part of the Zope X3.0.0 release.
-
-
```

### Comparing `zope.structuredtext-4.4/README.rst` & `zope.structuredtext-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/convert.py` & `zope.structuredtext-5.0/convert.py`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/docs/Makefile` & `zope.structuredtext-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/docs/api.rst` & `zope.structuredtext-5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/docs/conf.py` & `zope.structuredtext-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/docs/index.rst` & `zope.structuredtext-5.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 characters to spaces (assuming a tab stop every eight characters).
 
 :class:`~.StructuredTextNode` objects support the read-only subset of the
 Document Object Model (DOM) API. It should be possible to process
 :class:`~.StructuredTextNode` hierarchies using XML tools such as XSLT.
 
 The second step in using StructuredText is to apply additional
-structuring rules based on text content. A variety of differentText
+structuring rules based on text content. A variety of different text
 rules can be used.  Typically, these are used to implement a
 structured text language for producing documents, but any sort of
 structured text language could be implemented in the second
 step. For example, it is possible to use StructuredText to implement
 structured text formats for representing structured data. The second
 step, which could consist of multiple processing steps, is
 performed by processing, or "coloring", the hierarchy of generic
```

### Comparing `zope.structuredtext-4.4/docs/make.bat` & `zope.structuredtext-5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/setup.py` & `zope.structuredtext-5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# https://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.structuredtext package
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
@@ -31,51 +33,48 @@
     read('README.rst')
     + '\n\n' +
     read('CHANGES.rst')
 )
 
 setup(
     name='zope.structuredtext',
-    version='4.4',
+    version='5.0',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     description='StructuredText parser',
     long_description=long_description,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'Topic :: Software Development',
     ],
     url='http://github.com/zopefoundation/zope.structuredtext',
     license='ZPL 2.1',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope', ],
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
     ],
     extras_require={
         'test': [
             'zope.testrunner',
         ],
         'docs': [
             'Sphinx',
         ]
     },
-    test_suite='zope.structuredtext.tests.test_suite',
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/__init__.py` & `zope.structuredtext-5.0/src/zope/structuredtext/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
 """
 __docformat__ = 'restructuredtext'
 
 import re
 from string import ascii_letters
 
-from zope.structuredtext.stng import structurize
 from zope.structuredtext.document import DocumentWithImages
 from zope.structuredtext.html import HTMLWithImages
+from zope.structuredtext.stng import structurize
 
 
 def stx2html(aStructuredString, level=1, header=1):
     """A shortcut to produce HTML. """
     st = structurize(aStructuredString)
     doc = DocumentWithImages()(st)
     return HTMLWithImages()(doc, header=header, level=level)
```

#### html2text {}

```diff
@@ -22,18 +22,18 @@
 ...' >>> DocBookChapterWithFigures()(doc, level=1) '...' For HTML, there is a
 shortcut:: >>> from zope.structuredtext import stx2html >>> stx2html
 (structured_string) '
 ...' If we have references in the text we can use a different function:: >>>
 from zope.structuredtext import stx2htmlWithReferences >>>
 stx2htmlWithReferences(structured_string) '
 ...' """ __docformat__ = 'restructuredtext' import re from string import
-ascii_letters from zope.structuredtext.stng import structurize from
-zope.structuredtext.document import DocumentWithImages from
-zope.structuredtext.html import HTMLWithImages def stx2html(aStructuredString,
-level=1, header=1): """A shortcut to produce HTML. """ st = structurize
-(aStructuredString) doc = DocumentWithImages()(st) return HTMLWithImages()(doc,
-header=header, level=level) def stx2htmlWithReferences(text, level=1,
-header=1): """A shortcut to produce HTML with references""" text = re.sub( r'
-[\000\n]\.\. \[([0-9_%s-]+)\]' % ascii_letters, r'\n [\1]', text) text = re.sub
-( r'([\000- ,])\[(?P[0-9_%s-]+)\]([\000- ,.:])' % ascii_letters, r'\1[\2]\3',
-text) text = re.sub( r'([\000- ,])\[([^]]+)\.html\]([\000- ,.:])', r'\1[\2]\3',
-text) return stx2html(text, level=level, header=header)
+ascii_letters from zope.structuredtext.document import DocumentWithImages from
+zope.structuredtext.html import HTMLWithImages from zope.structuredtext.stng
+import structurize def stx2html(aStructuredString, level=1, header=1): """A
+shortcut to produce HTML. """ st = structurize(aStructuredString) doc =
+DocumentWithImages()(st) return HTMLWithImages()(doc, header=header,
+level=level) def stx2htmlWithReferences(text, level=1, header=1): """A shortcut
+to produce HTML with references""" text = re.sub( r'[\000\n]\.\. \[([0-9_%s-
+]+)\]' % ascii_letters, r'\n [\1]', text) text = re.sub( r'([\000- ,])\[(?P[0-
+9_%s-]+)\]([\000- ,.:])' % ascii_letters, r'\1[\2]\3', text) text = re.sub( r'(
+[\000- ,])\[([^]]+)\.html\]([\000- ,.:])', r'\1[\2]\3', text) return stx2html
+(text, level=level, header=header)
```

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/docbook.py` & `zope.structuredtext-5.0/src/zope/structuredtext/docbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 """ Render STX document as docbook.
 """
-from __future__ import print_function
 
-__metaclass__ = type
 
-
-class DocBook(object):
+class DocBook:
     """ Structured text document renderer for Docbook.
     """
     element_types = {
         '#text': '_text',
         'StructuredTextDocument': 'document',
         'StructuredTextParagraph': 'paragraph',
         'StructuredTextExample': 'example',
@@ -268,15 +265,15 @@
                    children[0].getChildNodes()[0].getNodeValue())
         for c in children:
             getattr(self, self.element_types[c.getNodeName()]
                     )(c, level, output)
         output('</article>\n')
 
 
-class DocBookBook(object):
+class DocBookBook:
 
     def __init__(self, title=''):
         self.title = title
         self.chapters = []
 
     def addChapter(self, chapter):
         self.chapters.append(chapter)
```

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/document.py` & `zope.structuredtext-5.0/src/zope/structuredtext/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,49 +10,42 @@
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 """ Structured text document parser
 """
 import re
 
+from zope.structuredtext.stletters import dbl_quoted_punc
 from zope.structuredtext.stletters import letters
 from zope.structuredtext.stletters import literal_punc
-from zope.structuredtext.stletters import under_punc
-from zope.structuredtext.stletters import strongem_punc
 from zope.structuredtext.stletters import phrase_delimiters
-from zope.structuredtext.stletters import dbl_quoted_punc
+from zope.structuredtext.stletters import strongem_punc
+from zope.structuredtext.stletters import under_punc
 from zope.structuredtext.stng import StructuredTextBullet
 from zope.structuredtext.stng import StructuredTextDescription
 from zope.structuredtext.stng import StructuredTextDocument
 from zope.structuredtext.stng import StructuredTextEmphasis
 from zope.structuredtext.stng import StructuredTextExample
 from zope.structuredtext.stng import StructuredTextImage
 from zope.structuredtext.stng import StructuredTextInnerLink
 from zope.structuredtext.stng import StructuredTextLink
+from zope.structuredtext.stng import StructuredTextLiteral
 from zope.structuredtext.stng import StructuredTextNamedLink
 from zope.structuredtext.stng import StructuredTextNumbered
-from zope.structuredtext.stng import StructuredTextLiteral
 from zope.structuredtext.stng import StructuredTextParagraph
-from zope.structuredtext.stng import StructuredTextSGML
 from zope.structuredtext.stng import StructuredTextSection
+from zope.structuredtext.stng import StructuredTextSGML
 from zope.structuredtext.stng import StructuredTextStrong
 from zope.structuredtext.stng import StructuredTextTable
 from zope.structuredtext.stng import StructuredTextUnderline
 from zope.structuredtext.stng import StructuredTextXref
 from zope.structuredtext.stng import structurize
 
-if bytes is not str:  # pragma: PY3
-    string_types = (str,)
-else:  # pragma: PY2
-    string_types = (unicode, str)  # noqa: F821 undefined name 'unicode'
-
-__metaclass__ = type
-
 
-class Document(object):
+class Document:
     """
     Class instance calls [ex.=> x()] require a structured text
     structure. Doc will then parse each paragraph in the structure
     and will find the special structures within each paragraph.
     Each special structure will be stored as an instance. Special
     structures within another special structure are stored within
     the 'top' structure
@@ -83,15 +76,15 @@
         'doc_emphasize',
         'doc_underline',
         'doc_sgml',
         'doc_xref',
     ]
 
     def __call__(self, doc):
-        if isinstance(doc, string_types):
+        if isinstance(doc, str):
             doc = structurize(doc)
             doc.setSubparagraphs(self.color_paragraphs(
                 doc.getSubparagraphs()))
         else:
             doc = StructuredTextDocument(self.color_paragraphs(
                 doc.getSubparagraphs()))
         return doc
@@ -106,28 +99,28 @@
 
         If no instances of expr are found, raw_string is returned.
         Otherwise a list of substrings and instances is returned
         """
 
         tmp = []    # the list to be returned if raw_string is split
 
-        if isinstance(text_type, string_types):
+        if isinstance(text_type, str):
             text_type = getattr(self, text_type)
 
         while True:
             t = text_type(raw_string)
             if not t:
                 break
             # an instance of expr was found
             t, start, end = t
 
             if start:
                 tmp.append(raw_string[:start])
 
-            if isinstance(t, string_types):
+            if isinstance(t, str):
                 # if we get a string back, add it to text to be parsed
                 raw_string = t + raw_string[end:len(raw_string)]
             else:
                 if isinstance(t, list):
                     # is we get a list, append it's elements
                     tmp.extend(t)
                 else:
@@ -149,21 +142,21 @@
         """Search the paragraph for each special structure
         """
         if types is None:
             types = self.text_types
 
         for text_type in types:
 
-            if isinstance(text, string_types):
+            if isinstance(text, str):
                 text = self.parse(text, text_type)
             elif isinstance(text, list):  # Waaaa
                 result = []
 
                 for s in text:
-                    if isinstance(s, string_types):
+                    if isinstance(s, str):
                         s = self.parse(s, text_type)
                         if isinstance(s, list):
                             result.extend(s)
                         else:
                             result.append(s)
                     else:
                         s.setColorizableTexts(
@@ -180,15 +173,15 @@
                 text.setColorizableTexts(result)
 
         return text
 
     def color_paragraphs(self, raw_paragraphs,
                          type=type,
                          sequence_types=(tuple, list),
-                         sts=string_types):
+                         sts=str):
         result = []
         for paragraph in raw_paragraphs:
             if paragraph.getNodeName() != 'StructuredTextParagraph':
                 result.append(paragraph)
                 continue
 
             for pt in self.paragraph_types:
@@ -206,16 +199,15 @@
                             paragraph.getSubparagraphs()
                         )
                         paragraph.setSubparagraphs(subs)
                     break
             else:
                 # copy, retain attributes
                 atts = getattr(paragraph, '_attributes', [])
-                kw = dict([(att, getattr(paragraph, att))
-                           for att in atts])
+                kw = {att: getattr(paragraph, att) for att in atts}
                 subs = self.color_paragraphs(paragraph.getSubparagraphs())
                 new_paragraphs = StructuredTextParagraph(
                     paragraph.getColorizableTexts()[0], subs, **kw),
 
             # color the inline StructuredText types
             # for each StructuredTextParagraph
             for paragraph in new_paragraphs:
```

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/html.py` & `zope.structuredtext-5.0/src/zope/structuredtext/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,22 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 """ HTML renderer for STX documents.
 """
+from functools import partial
+from html import escape
 
-try:
-    from html import escape
-except ImportError:  # pragma: PY2
-    from cgi import escape
-else:  # pragma: PY3
-    from functools import partial
-    escape = partial(escape, quote=False)
 
-__metaclass__ = type
+escape = partial(escape, quote=False)
 
 
-class HTML(object):
+class HTML:
 
     paragraph_nestable = {
         '#text': '_text',
         'StructuredTextLiteral': 'literal',
         'StructuredTextEmphasis': 'emphasis',
         'StructuredTextStrong': 'strong',
         'StructuredTextLink': 'link',
@@ -220,15 +215,15 @@
     def sgml(self, doc, level, output):
         for c in doc.getChildNodes():
             getattr(self, self.element_types[c.getNodeName()]
                     )(c, level, output)
 
     def xref(self, doc, level, output):
         val = doc.getNodeValue()
-        output('<a href="#ref%s">[%s]</a>' % (val, val))
+        output('<a href="#ref{}">[{}]</a>'.format(val, val))
 
     def table(self, doc, level, output):
         """
         A StructuredTextTable holds StructuredTextRow(s) which
         holds StructuredTextColumn(s). A StructuredTextColumn
         is a type of StructuredTextParagraph and thus holds
         the actual data.
```

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/Acquisition.ref` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/Acquisition.ref`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/Acquisition.stx` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/Acquisition.stx`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/Acquisition.xml` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/Acquisition.xml`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/ExtensionClass.ref` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/ExtensionClass.ref`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/ExtensionClass.stx` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/ExtensionClass.stx`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/ExtensionClass.xml` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/ExtensionClass.xml`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/Links.ref` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/Links.ref`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/Links.stx` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/Links.stx`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/Links.xml` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/Links.xml`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/MultiMapping.ref` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/MultiMapping.ref`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/MultiMapping.stx` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/MultiMapping.stx`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/MultiMapping.xml` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/MultiMapping.xml`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples.ref` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples.ref`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples.stx` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples.stx`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/examples.xml` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/examples.xml`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/index.ref` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/index.ref`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/index.stx` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/index.stx`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/index.xml` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/index.xml`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/table.ref` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/table.ref`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/regressions/table.stx` & `zope.structuredtext-5.0/src/zope/structuredtext/regressions/table.stx`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/stdom.py` & `zope.structuredtext-5.0/src/zope/structuredtext/stdom.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,14 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 """DOM implementation in StructuredText: read-only methods
 """
 
-if bytes is not str:  # pragma: PY3
-    string_types = (str,)
-else:  # pragma: PY2
-    string_types = (unicode, str)  # noqa: F821 undefined name 'unicode'
-
-__metaclass__ = type
-
 # Node type codes
 # ---------------
 
 ELEMENT_NODE = 1
 ATTRIBUTE_NODE = 2
 TEXT_NODE = 3
 CDATA_SECTION_NODE = 4
@@ -97,41 +90,41 @@
 class InUseAttributeException(DOMException):
     code = INUSE_ATTRIBUTE_ERR
 
 # Node classes
 # ------------
 
 
-class ParentNode(object):
+class ParentNode:
     """
     A node that can have children, or, more precisely, that implements
     the child access methods of the DOM.
     """
 
-    def getChildNodes(self, type=type, sts=string_types):
+    def getChildNodes(self, type=type, sts=str):
         """
         Returns a NodeList that contains all children of this node.
         If there are no children, this is a empty NodeList
         """
         r = []
         for n in self.getChildren():
             if isinstance(n, sts):
                 n = TextNode(n)
             r.append(n.__of__(self))
 
         return NodeList(r)
 
-    def getFirstChild(self, type=type, sts=string_types):
+    def getFirstChild(self, type=type, sts=str):
         """
         The first child of this node. If there is no such node
         this returns None
         """
         raise NotImplementedError()
 
-    def getLastChild(self, type=type, sts=string_types):
+    def getLastChild(self, type=type, sts=str):
         """
         The last child of this node.  If there is no such node
         this returns None.
         """
         raise NotImplementedError()
 
 
@@ -184,15 +177,15 @@
         if index < 0:
             return None
         try:
             n = children[index]
         except IndexError:  # pragma: no cover
             return None
         else:
-            if isinstance(n, string_types):
+            if isinstance(n, str):
                 n = TextNode(n)
             n._DOMIndex = index
             return n.__of__(self)
 
     def getNextSibling(self):
         """
         The node immediately preceding this node.  If
@@ -210,15 +203,15 @@
 
         index = index + 1
         try:
             n = children[index]
         except IndexError:  # pragma: no cover
             return None
         else:
-            if isinstance(n, string_types):  # pragma: no cover
+            if isinstance(n, str):  # pragma: no cover
                 n = TextNode(n)
             n._DOMIndex = index
             return n.__of__(self)
 
     def getOwnerDocument(self):
         """
         The Document object associated with this node, if any.
@@ -322,15 +315,15 @@
     getNodeName = getTagName
 
     _NODE_TYPE = ELEMENT_NODE
 
     def getNodeValue(self):
         r = []
         for c in self.getChildren():
-            if not isinstance(c, string_types):
+            if not isinstance(c, str):
                 c = c.getNodeValue()
             r.append(c)
         return ''.join(r)
 
     def getParentNode(self):
         """
         The parent of this node.  All nodes except Document
@@ -365,26 +358,26 @@
         preorder traversal of the Document tree.  Parameter: tagname
         The name of the tag to match (* = all tags). Return Value: A new
         NodeList object containing all the matched Elements.
         """
         raise NotImplementedError()
 
 
-class NodeList(object):
+class NodeList:
     """NodeList interface - Provides the abstraction of an ordered
     collection of nodes.
 
     Python extensions: can use sequence-style 'len', 'getitem', and
     'for..in' constructs.
     """
 
     def __init__(self, list=None):
         self._data = list or []
 
-    def __getitem__(self, index, type=type, sts=string_types):
+    def __getitem__(self, index, type=type, sts=str):
         return self._data[index]
 
     def item(self, index):
         """Returns the index-th item in the collection
         """
         raise NotImplementedError()
 
@@ -392,15 +385,15 @@
         """The length of the NodeList
         """
         return len(self._data)
 
     __len__ = getLength
 
 
-class NamedNodeMap(object):
+class NamedNodeMap:
     """
     NamedNodeMap interface - Is used to represent collections
     of nodes that can be accessed by name.  NamedNodeMaps are not
     maintained in any particular order.
 
     Python extensions: can use sequence-style 'len', 'getitem', and
     'for..in' constructs, and mapping-style 'getitem'.
```

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/stletters.py` & `zope.structuredtext-5.0/src/zope/structuredtext/stletters.py`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/stng.py` & `zope.structuredtext-5.0/src/zope/structuredtext/stng.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 """ Core document model.
 """
-from __future__ import print_function
 
 import re
-from . import stdom
 
-__metaclass__ = type
+from . import stdom
 
 
 def indention(str, front=re.compile(r"^\s+").match):
     """Find the number of leading spaces. If none, return 0.
     """
     result = front(str)
     if result is not None:
@@ -116,15 +114,15 @@
     currentindent = 0
     levels = {0: 0}
     level = 0        # which header are we under
     struct = []       # the structure to be returned
     run = struct
 
     paragraphs = paragraphs.expandtabs()
-    paragraphs = '%s%s%s' % ('\n\n', paragraphs, '\n\n')
+    paragraphs = '{}{}{}'.format('\n\n', paragraphs, '\n\n')
     paragraphs = delimiter.split(paragraphs)
     paragraphs = [x for x in paragraphs if x.strip()]
 
     if not paragraphs:
         return StructuredTextDocument()
 
     ind = []     # structure based on indention levels
@@ -225,15 +223,15 @@
 class StructuredTextDocument(StructuredTextParagraph):
     """A StructuredTextDocument holds StructuredTextParagraphs
     as its subparagraphs.
     """
     _attributes = ()
 
     def __init__(self, subs=None, **kw):
-        super(StructuredTextDocument, self).__init__('', subs, **kw)
+        super().__init__('', subs, **kw)
 
     def getChildren(self):
         return self._subs
 
     def getColorizableTexts(self):
         return ()
 
@@ -253,15 +251,15 @@
 class StructuredTextExample(StructuredTextParagraph):
     """Represents a section of document with literal text, as for examples"""
 
     def __init__(self, subs, **kw):
         t = []
         for s in subs:
             flatten(s, t.append)
-        super(StructuredTextExample, self).__init__('\n\n'.join(t), (), **kw)
+        super().__init__('\n\n'.join(t), (), **kw)
 
     def getColorizableTexts(self):
         return ()
 
     def setColorizableTexts(self, src):
         pass  # never color examples
 
@@ -287,15 +285,15 @@
 
 
 class StructuredTextDescription(StructuredTextParagraph):
     """Represents a section of a document with a title and a body
     """
 
     def __init__(self, title, src, subs, **kw):
-        super(StructuredTextDescription, self).__init__(src, subs, **kw)
+        super().__init__(src, subs, **kw)
         self._title = title
 
     def getColorizableTexts(self):
         return self._title, self._src
 
     def setColorizableTexts(self, src):
         self._title, self._src = src
@@ -309,15 +307,15 @@
     """Represents a section of a document with a title and a body"""
 
 
 class StructuredTextSection(StructuredTextParagraph):
     """Represents a section of a document with a title and a body"""
 
     def __init__(self, src, subs=None, **kw):
-        super(StructuredTextSection, self).__init__(
+        super().__init__(
             StructuredTextSectionTitle(src), subs, **kw)
 
     def getColorizableTexts(self):
         return self._src.getColorizableTexts()
 
     def setColorizableTexts(self, src):
         self._src.setColorizableTexts(src)
@@ -330,15 +328,15 @@
     rows is a list of lists containing tuples, which
     represent the columns/cells in each rows.
     EX
     rows = [[('row 1:column1',1)],[('row2:column1',1)]]
     """
 
     def __init__(self, rows, src, subs, **kw):
-        super(StructuredTextTable, self).__init__(subs, **kw)
+        super().__init__(subs, **kw)
         self._rows = []
         for row in rows:
             if row:
                 self._rows.append(StructuredTextRow(row, kw))
 
     def getRows(self):
         return [self._rows]
@@ -398,15 +396,15 @@
         """
         row is a list of tuples, where each tuple is
         the raw text for a cell/column and the span
         of that cell/column.
         EX
         [('this is column one',1), ('this is column two',1)]
         """
-        super(StructuredTextRow, self).__init__([], **kw)
+        super().__init__([], **kw)
 
         self._columns = []
         for column in row:
             self._columns.append(StructuredTextColumn(column[0],
                                                       column[1],
                                                       column[2],
                                                       column[3],
@@ -430,15 +428,15 @@
     StructuredTextColumn is a cell/column in a table.
     A cell can hold multiple paragraphs. The cell
     is either classified as a StructuredTextTableHeader
     or StructuredTextTableData.
     """
 
     def __init__(self, text, span, align, valign, typ, kw):
-        super(StructuredTextColumn, self).__init__(text, [], **kw)
+        super().__init__(text, [], **kw)
         self._span = span
         self._align = align
         self._valign = valign
         self._type = typ
 
     def getSpan(self):
         return self._span
@@ -486,15 +484,15 @@
     def getColorizableTexts(self):
         return self._value,
 
     def setColorizableTexts(self, v):
         self._value = v[0]
 
     def __repr__(self):
-        return '%s(%s)' % (self.__class__.__name__, repr(self._value))
+        return '{}({})'.format(self.__class__.__name__, repr(self._value))
 
 
 class StructuredTextLiteral(StructuredTextMarkup):
     def getColorizableTexts(self):
         return ()
 
     def setColorizableTexts(self, v):
```

### Comparing `zope.structuredtext-4.4/src/zope/structuredtext/tests.py` & `zope.structuredtext-5.0/src/zope/structuredtext/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,35 +6,36 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
-from __future__ import print_function
+
 import doctest
-import unittest
 import glob
 import os
+import unittest
 
-from zope.structuredtext import stng
 from zope.structuredtext import stdom
-from zope.structuredtext.document import DocumentWithImages
-from zope.structuredtext.html import HTMLWithImages
+from zope.structuredtext import stng
 from zope.structuredtext.docbook import DocBook
 from zope.structuredtext.docbook import DocBookChapterWithFigures
+from zope.structuredtext.document import DocumentWithImages
+from zope.structuredtext.html import HTMLWithImages
+
 
 here = os.path.dirname(__file__)
 regressions = os.path.join(here, 'regressions')
 
 files = glob.glob(regressions + '/*stx')
 
 
 def readFile(dirname, fname):
-    with open(os.path.join(dirname, fname), "r") as myfile:
+    with open(os.path.join(dirname, fname)) as myfile:
         lines = myfile.readlines()
     return ''.join(lines)
 
 
 def structurizedFile(f):
     raw_text = readFile(regressions, f)
     text = stng.structurize(raw_text)
@@ -42,15 +43,15 @@
 
 
 def structurizedFiles():
     for f in files:
         yield structurizedFile(f)
 
 
-class MockParagraph(object):
+class MockParagraph:
 
     co_texts = ()
     sub_paragraphs = ()
     indent = 0
     node_type = stdom.TEXT_NODE
     node_value = ''
     node_name = None
@@ -83,15 +84,15 @@
 
     maxDiff = None
 
     def _compare(self, filename, output, expected_extension=".ref"):
         expected_filename = filename.replace('.stx', expected_extension)
         try:
             expected = readFile(regressions, expected_filename)
-        except IOError:  # pragma: no cover
+        except OSError:  # pragma: no cover
             full_expected_fname = os.path.join(regressions, expected_filename)
             if not os.path.exists(full_expected_fname):
                 with open(full_expected_fname, 'w') as f:
                     f.write(output)
         else:
             self.assertEqual(expected.strip(), output.strip())
 
@@ -488,16 +489,16 @@
 <p>            first paragraph</p>
 <h2>            Subtitle</h2>
 <p>                second paragraph</p>"""))
 
     def testUnicodeContent(self):
         # This fails because ST uses the default locale to get "letters"
         # whereas it should use \w+ and re.U if the string is Unicode.
-        self._test(u"h\xe9 **y\xe9** xx",
-                   u"h\xe9 <strong>y\xe9</strong> xx")
+        self._test("h\xe9 **y\xe9** xx",
+                   "h\xe9 <strong>y\xe9</strong> xx")
 
     def test_paragraph_not_nestable(self):
         first_child_not_nestable = MockParagraph(
             node_name='not nestable or known')
         second_child_nestable = MockParagraph(node_name="#text")
         third_child_not_nestable = MockParagraph(
             node_name='not nestable or known')
```

### Comparing `zope.structuredtext-4.4/src/zope.structuredtext.egg-info/PKG-INFO` & `zope.structuredtext-5.0/src/zope.structuredtext.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: zope.structuredtext
-Version: 4.4
+Version: 5.0
 Summary: StructuredText parser
 Home-page: http://github.com/zopefoundation/zope.structuredtext
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 =====================
  zope.structuredtext
 =====================
@@ -57,14 +54,24 @@
 Please see https://zopestructuredtext.readthedocs.org/ for documentation.
 
 
 =========
  Changes
 =========
 
+5.0 (2023-05-09)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-03-18)
 ================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -143,9 +150,7 @@
 
 
 3.0.0 (2004/11/07)
 ==================
 
 - Corresponds to the verison of the ``zope.structuredtext`` package shipped
   as part of the Zope X3.0.0 release.
-
-
```

### Comparing `zope.structuredtext-4.4/src/zope.structuredtext.egg-info/SOURCES.txt` & `zope.structuredtext-5.0/src/zope.structuredtext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.structuredtext-4.4/tox.ini` & `zope.structuredtext-5.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
-    !py27-!pypy: sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
+    sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
 extras =
     test
     docs
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
 basepython = python3
 skip_install = false
 commands_pre =
 commands =
     sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
@@ -49,25 +57,23 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage run -a -m sphinx -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
-    coverage html
-    coverage report -m --fail-under=99
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=99
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.structuredtext
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

