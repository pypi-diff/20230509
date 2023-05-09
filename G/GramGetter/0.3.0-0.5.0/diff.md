# Comparing `tmp/GramGetter-0.3.0.tar.gz` & `tmp/GramGetter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GramGetter-0.3.0.tar", last modified: Tue May  9 12:37:33 2023, max compression
+gzip compressed data, was "GramGetter-0.5.0.tar", last modified: Tue May  9 13:23:34 2023, max compression
```

## Comparing `GramGetter-0.3.0.tar` & `GramGetter-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,86 @@
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:37:33.067583 GramGetter-0.3.0/
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:37:33.063583 GramGetter-0.3.0/GramGetter/
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      228 2023-05-09 11:27:33.000000 GramGetter-0.3.0/GramGetter/AUTHORS.md
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     5661 2023-05-09 11:27:34.000000 GramGetter-0.3.0/GramGetter/CODE_OF_CONDUCT.md
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    14462 2023-05-09 12:30:13.000000 GramGetter-0.3.0/GramGetter/GramGetter.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     1131 2023-05-09 11:27:35.000000 GramGetter-0.3.0/GramGetter/LICENSE
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      440 2023-05-09 11:27:35.000000 GramGetter-0.3.0/GramGetter/Pipfile
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    52724 2023-05-09 11:27:35.000000 GramGetter-0.3.0/GramGetter/Pipfile.lock
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     5306 2023-05-09 11:27:36.000000 GramGetter-0.3.0/GramGetter/README.rst
--rw-rw-r--   0 msaid     (1043) msaid     (1044)       34 2023-05-09 12:04:03.000000 GramGetter-0.3.0/GramGetter/__init__.py
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:37:33.067583 GramGetter-0.3.0/GramGetter/instaloader/
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      853 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/__init__.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    32011 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/__main__.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     1611 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/exceptions.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    82489 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/instaloader.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    38435 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/instaloadercontext.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     4934 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/lateststamps.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    14877 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/nodeiterator.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     1940 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/sectioniterator.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    79877 2023-05-09 11:27:32.000000 GramGetter-0.3.0/GramGetter/instaloader/structures.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      107 2023-05-09 11:27:34.000000 GramGetter-0.3.0/GramGetter/my_instaloader.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     2288 2023-05-09 11:27:36.000000 GramGetter-0.3.0/GramGetter/setup.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:15:46.000000 GramGetter-0.3.0/GramGetter/test.ipynb
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:37:33.063583 GramGetter-0.3.0/GramGetter.egg-info/
--rw-r-----   0 msaid     (1043) msaid     (1044)      432 2023-05-09 12:37:32.000000 GramGetter-0.3.0/GramGetter.egg-info/PKG-INFO
--rw-r-----   0 msaid     (1043) msaid     (1044)      798 2023-05-09 12:37:33.000000 GramGetter-0.3.0/GramGetter.egg-info/SOURCES.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)        1 2023-05-09 12:37:32.000000 GramGetter-0.3.0/GramGetter.egg-info/dependency_links.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)       14 2023-05-09 12:37:32.000000 GramGetter-0.3.0/GramGetter.egg-info/requires.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)       11 2023-05-09 12:37:32.000000 GramGetter-0.3.0/GramGetter.egg-info/top_level.txt
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      316 2023-05-09 12:36:44.000000 GramGetter-0.3.0/MANIFEST.in
--rw-r-----   0 msaid     (1043) msaid     (1044)      432 2023-05-09 12:37:33.067583 GramGetter-0.3.0/PKG-INFO
--rw-rw-r--   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:33:47.000000 GramGetter-0.3.0/README
--rw-r-----   0 msaid     (1043) msaid     (1044)       38 2023-05-09 12:37:33.067583 GramGetter-0.3.0/setup.cfg
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      710 2023-05-09 12:37:31.000000 GramGetter-0.3.0/setup.py
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.813211 GramGetter-0.5.0/
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.805211 GramGetter-0.5.0/GramGetter/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      228 2023-05-09 11:27:33.000000 GramGetter-0.5.0/GramGetter/AUTHORS.md
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     5661 2023-05-09 11:27:34.000000 GramGetter-0.5.0/GramGetter/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    14452 2023-05-09 13:23:00.000000 GramGetter-0.5.0/GramGetter/GramGetter.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1131 2023-05-09 11:27:35.000000 GramGetter-0.5.0/GramGetter/LICENSE
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      440 2023-05-09 11:27:35.000000 GramGetter-0.5.0/GramGetter/Pipfile
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    52724 2023-05-09 11:27:35.000000 GramGetter-0.5.0/GramGetter/Pipfile.lock
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     5306 2023-05-09 11:27:36.000000 GramGetter-0.5.0/GramGetter/README.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)       34 2023-05-09 12:04:03.000000 GramGetter-0.5.0/GramGetter/__init__.py
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.805211 GramGetter-0.5.0/GramGetter/deploy/
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.809211 GramGetter-0.5.0/GramGetter/deploy/arch/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      789 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/deploy/arch/PKGBUILD.template
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1043 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/deploy/arch/deploy.sh
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     4944 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/deploy/arch/id_rsa_AUR.enc
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.809211 GramGetter-0.5.0/GramGetter/deploy/windows/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     2273 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/deploy/windows/create_exe.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      728 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/deploy/windows/instaloader.spec
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.809211 GramGetter-0.5.0/GramGetter/docs/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     8061 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/Makefile
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      327 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/README.md
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.809211 GramGetter-0.5.0/GramGetter/docs/_static/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    78686 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/_static/instaloaderdoc.css
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    52009 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/_static/instaloaderdoc.js
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.809211 GramGetter-0.5.0/GramGetter/docs/_templates/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     3396 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/_templates/layout.html
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      227 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/_templates/page.html
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      946 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/_templates/search.html
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     3320 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/as-module.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    12618 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/basic-usage.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    11264 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/cli-options.rst
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.809211 GramGetter-0.5.0/GramGetter/docs/codesnippets/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      390 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets/113_only_one_per_user.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      739 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets/120_ghost_followers.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      431 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets/121_since_until.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      594 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets/194_top_x_of_user.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1187 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets/56_track_deleted.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     2113 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets/615_import_firefox_session.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      783 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets/666_historical_hashtag_data.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      144 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets/README.md
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     4601 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/codesnippets.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    11647 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/conf.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     5592 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/contributing.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)   337840 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/favicon.ico
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     2841 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/index.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1386 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/installation.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     5164 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/logo.png
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    19053 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/logo.svg
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     8473 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/logo_heading.png
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.809211 GramGetter-0.5.0/GramGetter/docs/module/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1126 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/module/exceptions.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      180 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/module/instaloader.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      438 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/module/instaloadercontext.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      988 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/module/nodeiterator.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1553 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/module/structures.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)       23 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/requirements.txt
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    10724 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/sphinx_autodoc_typehints.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      914 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/sponsors.rst
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     3636 2023-05-09 11:27:31.000000 GramGetter-0.5.0/GramGetter/docs/troubleshooting.rst
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.813211 GramGetter-0.5.0/GramGetter/instaloader/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      853 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/__init__.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    32011 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/__main__.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1611 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/exceptions.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    82489 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/instaloader.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    38435 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/instaloadercontext.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     4934 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/lateststamps.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    14877 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/nodeiterator.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/py.typed
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1940 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/sectioniterator.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    79877 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/instaloader/structures.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      107 2023-05-09 11:27:34.000000 GramGetter-0.5.0/GramGetter/instaloader.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     2288 2023-05-09 11:27:36.000000 GramGetter-0.5.0/GramGetter/setup.py
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.813211 GramGetter-0.5.0/GramGetter/test/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     8346 2023-05-09 11:27:32.000000 GramGetter-0.5.0/GramGetter/test/instaloader_unittests.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:15:46.000000 GramGetter-0.5.0/GramGetter/test.ipynb
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 13:23:34.809211 GramGetter-0.5.0/GramGetter.egg-info/
+-rw-r-----   0 msaid     (1043) msaid     (1044)      432 2023-05-09 13:23:34.000000 GramGetter-0.5.0/GramGetter.egg-info/PKG-INFO
+-rw-r-----   0 msaid     (1043) msaid     (1044)     2422 2023-05-09 13:23:34.000000 GramGetter-0.5.0/GramGetter.egg-info/SOURCES.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)        1 2023-05-09 13:23:34.000000 GramGetter-0.5.0/GramGetter.egg-info/dependency_links.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)       14 2023-05-09 13:23:34.000000 GramGetter-0.5.0/GramGetter.egg-info/requires.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)       11 2023-05-09 13:23:34.000000 GramGetter-0.5.0/GramGetter.egg-info/top_level.txt
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      316 2023-05-09 12:36:44.000000 GramGetter-0.5.0/MANIFEST.in
+-rw-r-----   0 msaid     (1043) msaid     (1044)      432 2023-05-09 13:23:34.813211 GramGetter-0.5.0/PKG-INFO
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:33:47.000000 GramGetter-0.5.0/README
+-rw-r-----   0 msaid     (1043) msaid     (1044)       38 2023-05-09 13:23:34.813211 GramGetter-0.5.0/setup.cfg
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      687 2023-05-09 13:23:30.000000 GramGetter-0.5.0/setup.py
```

### Comparing `GramGetter-0.3.0/GramGetter/CODE_OF_CONDUCT.md` & `GramGetter-0.5.0/GramGetter/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/GramGetter.py` & `GramGetter-0.5.0/GramGetter/GramGetter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import my_instaloader as instaloader
+from .instaloader import *
 import time
 from datetime import datetime, timedelta
 import warnings
 warnings.filterwarnings("ignore")
 
 class GramGetter:
     def __init__(self, username, cookie_dict):
```

### Comparing `GramGetter-0.3.0/GramGetter/LICENSE` & `GramGetter-0.5.0/GramGetter/LICENSE`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/Pipfile.lock` & `GramGetter-0.5.0/GramGetter/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/README.rst` & `GramGetter-0.5.0/GramGetter/README.rst`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/__init__.py` & `GramGetter-0.5.0/GramGetter/instaloader/__init__.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/__main__.py` & `GramGetter-0.5.0/GramGetter/instaloader/__main__.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/exceptions.py` & `GramGetter-0.5.0/GramGetter/instaloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/instaloader.py` & `GramGetter-0.5.0/GramGetter/instaloader/instaloader.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/instaloadercontext.py` & `GramGetter-0.5.0/GramGetter/instaloader/instaloadercontext.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/lateststamps.py` & `GramGetter-0.5.0/GramGetter/instaloader/lateststamps.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/nodeiterator.py` & `GramGetter-0.5.0/GramGetter/instaloader/nodeiterator.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/sectioniterator.py` & `GramGetter-0.5.0/GramGetter/instaloader/sectioniterator.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/instaloader/structures.py` & `GramGetter-0.5.0/GramGetter/instaloader/structures.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/GramGetter/setup.py` & `GramGetter-0.5.0/GramGetter/setup.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.3.0/setup.py` & `GramGetter-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 requirements = ['requests>=2.4']
 setup(
     name='GramGetter',
-    version='0.3.0',    # Update this for new versions
-    packages=find_packages(include=['GramGetter*']),
-    include_package_data=True,
+    version='0.5.0',    # Update this for new versions
     description='A crawler for scraping instagram content',
     author='Mohamed Amine Said',
     author_email='amine8said@gmail.com',
     url='https://github.com/instaloader/instaloader',
     python_requires='>=3.8',
     install_requires=requirements,
+    package_data={'': ['*']},
+    include_package_data=True,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

