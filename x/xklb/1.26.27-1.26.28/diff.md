# Comparing `tmp/xklb-1.26.27.tar.gz` & `tmp/xklb-1.26.28.tar.gz`

## Comparing `xklb-1.26.27.tar` & `xklb-1.26.28.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.27/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.27/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.27/Windows.md
--rw-r--r--   0        0        0   420714 2020-02-02 00:00:00.000000 xklb-1.26.27/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.27/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.27/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.27/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.27/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.26.27/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.26.27/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/books.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/consts.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/dl_config.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/hn_extract.py
--rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/lb.py
--rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/playback.py
--rw-r--r--   0        0        0    26772 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/praw_extract.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21844 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.27/xklb/scripts/mining/words.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.27/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.27/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.27/LICENSE
--rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.27/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.27/pyproject.toml
--rw-r--r--   0        0        0    44039 2020-02-02 00:00:00.000000 xklb-1.26.27/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.28/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.28/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.28/Windows.md
+-rw-r--r--   0        0        0   419424 2020-02-02 00:00:00.000000 xklb-1.26.28/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.28/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.28/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.28/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.28/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.26.28/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.26.28/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/books.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/consts.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/dl_config.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/lb.py
+-rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/playback.py
+-rw-r--r--   0        0        0    26800 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21844 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.28/xklb/scripts/mining/words.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.28/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.28/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.28/LICENSE
+-rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.28/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.28/pyproject.toml
+-rw-r--r--   0        0        0    44039 2020-02-02 00:00:00.000000 xklb-1.26.28/PKG-INFO
```

### Comparing `xklb-1.26.27/Windows.md` & `xklb-1.26.28/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/pdm.lock` & `xklb-1.26.28/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     "pychromecast<13,>=12.1.4",
     "requests>=2.23.0",
     "yt-dlp>=2022.6.22.1",
 ]
 
 [[package]]
 name = "certifi"
-version = "2022.12.7"
+version = "2023.5.7"
 requires_python = ">=3.6"
 summary = "Python package for providing Mozilla's CA Bundle."
 
 [[package]]
 name = "cffi"
 version = "1.15.1"
 summary = "Foreign Function Interface for Python calling C code."
@@ -302,15 +302,15 @@
 name = "future"
 version = "0.18.3"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Clean single-source support for Python 3 and 2"
 
 [[package]]
 name = "gallery-dl"
-version = "1.25.3"
+version = "1.25.4"
 requires_python = ">=3.4"
 summary = "Command-line program to download image galleries and collections from several image hosting sites"
 dependencies = [
     "requests>=2.11.0",
 ]
 
 [[package]]
@@ -516,16 +516,16 @@
 name = "olefile"
 version = "0.46"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Python package to parse, read and write Microsoft OLE2 files (Structured Storage or Compound Document, Microsoft Office)"
 
 [[package]]
 name = "orjson"
-version = "3.8.11"
-requires_python = ">= 3.7"
+version = "3.8.12"
+requires_python = ">=3.7"
 summary = "Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy"
 
 [[package]]
 name = "packaging"
 version = "23.1"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
@@ -821,15 +821,15 @@
     "markdown-it-py<3.0.0,>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.264"
+version = "0.0.265"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
 name = "scalene"
 version = "1.5.19"
 requires_python = ">=3.8"
@@ -877,17 +877,17 @@
 [[package]]
 name = "sqlite-fts4"
 version = "1.0.3"
 summary = "Python functions for working with SQLite FTS4 search"
 
 [[package]]
 name = "sqlite-utils"
-version = "3.30"
-requires_python = ">=3.6"
-summary = "CLI tool and Python utility functions for manipulating SQLite databases"
+version = "3.31"
+requires_python = ">=3.7"
+summary = "CLI tool and Python library for manipulating SQLite databases"
 dependencies = [
     "click",
     "click-default-group-wheel",
     "python-dateutil",
     "sqlite-fts4",
     "tabulate",
 ]
@@ -1028,21 +1028,21 @@
 name = "websocket-client"
 version = "1.5.1"
 requires_python = ">=3.7"
 summary = "WebSocket client for Python with low level API options"
 
 [[package]]
 name = "websockets"
-version = "11.0.2"
+version = "11.0.3"
 requires_python = ">=3.7"
 summary = "An implementation of the WebSocket Protocol (RFC 6455 & 7692)"
 
 [[package]]
 name = "werkzeug"
-version = "2.3.3"
+version = "2.3.4"
 requires_python = ">=3.8"
 summary = "The comprehensive WSGI web application library."
 dependencies = [
     "MarkupSafe>=2.1.1",
 ]
 
 [[package]]
@@ -1408,17 +1408,17 @@
     {url = "https://files.pythonhosted.org/packages/0a/d2/0f5006892e07ea342d57dbeda46027e99a097ffb6218bee1e37f9776ed95/casttube-0.2.1-py3-none-any.whl", hash = "sha256:36f118007f9eead3959cf30de03c1640b53a263569ff2a3971c0521826c835b2"},
     {url = "https://files.pythonhosted.org/packages/78/54/f7e80d701c587940cf1c871fb6327b4a2682df4287896fbf9400cd0bbf21/casttube-0.2.1.tar.gz", hash = "sha256:54d2af8c7949aa9c5db87fb11ef0a478a5d3e7ac6d2d2ac8dd1711e3a516fc82"},
 ]
 "catt 0.12.10" = [
     {url = "https://files.pythonhosted.org/packages/0c/6d/be6e8682f6d33f763cab155e77879329b78ccd59b096dea01c2bac2d4f13/catt-0.12.10-py3-none-any.whl", hash = "sha256:0f51120b307671d671fcd2cbc3686c1df584e7a78d1589dc1b6468d25a6cd7b1"},
     {url = "https://files.pythonhosted.org/packages/fa/df/4d1503bf067b3d28b90b0c9ddf8cc4c5430bdc104da5ac7b16c8eddc8f0b/catt-0.12.10.tar.gz", hash = "sha256:a462f126ad2630ef7f57ea66ca3808eee7620b25de74d76a9204c8a87e874c1f"},
 ]
-"certifi 2022.12.7" = [
-    {url = "https://files.pythonhosted.org/packages/37/f7/2b1b0ec44fdc30a3d31dfebe52226be9ddc40cd6c0f34ffc8923ba423b69/certifi-2022.12.7.tar.gz", hash = "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3"},
-    {url = "https://files.pythonhosted.org/packages/71/4c/3db2b8021bd6f2f0ceb0e088d6b2d49147671f25832fb17970e9b583d742/certifi-2022.12.7-py3-none-any.whl", hash = "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"},
+"certifi 2023.5.7" = [
+    {url = "https://files.pythonhosted.org/packages/93/71/752f7a4dd4c20d6b12341ed1732368546bc0ca9866139fe812f6009d9ac7/certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
+    {url = "https://files.pythonhosted.org/packages/9d/19/59961b522e6757f0c9097e4493fa906031b95b3ebe9360b2c3083561a6b4/certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
 ]
 "cffi 1.15.1" = [
     {url = "https://files.pythonhosted.org/packages/00/05/23a265a3db411b0bfb721bf7a116c7cecaf3eb37ebd48a6ea4dfb0a3244d/cffi-1.15.1-cp27-cp27m-win_amd64.whl", hash = "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e"},
     {url = "https://files.pythonhosted.org/packages/03/7b/259d6e01a6083acef9d3c8c88990c97d313632bb28fa84d6ab2bb201140a/cffi-1.15.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405"},
     {url = "https://files.pythonhosted.org/packages/0e/65/0d7b5dad821ced4dcd43f96a362905a68ce71e6b5f5cfd2fada867840582/cffi-1.15.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e"},
     {url = "https://files.pythonhosted.org/packages/0e/e2/a23af3d81838c577571da4ff01b799b0c2bbde24bd924d97e228febae810/cffi-1.15.1-cp310-cp310-win_amd64.whl", hash = "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d"},
     {url = "https://files.pythonhosted.org/packages/10/72/617ee266192223a38b67149c830bd9376b69cf3551e1477abc72ff23ef8e/cffi-1.15.1-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9"},
@@ -1740,17 +1740,17 @@
 "ftfy 6.1.1" = [
     {url = "https://files.pythonhosted.org/packages/97/16/79c6e17bd3465f6498282dd23813846c68cd0989fe60bfef68bb1918d041/ftfy-6.1.1.tar.gz", hash = "sha256:bfc2019f84fcd851419152320a6375604a0f1459c281b5b199b2cd0d2e727f8f"},
     {url = "https://files.pythonhosted.org/packages/e1/1e/bf736f9576a8979752b826b75cbd83663ff86634ea3055a766e2d8ad3ee5/ftfy-6.1.1-py3-none-any.whl", hash = "sha256:0ffd33fce16b54cccaec78d6ec73d95ad370e5df5a25255c8966a6147bd667ca"},
 ]
 "future 0.18.3" = [
     {url = "https://files.pythonhosted.org/packages/8f/2e/cf6accf7415237d6faeeebdc7832023c90e0282aa16fd3263db0eb4715ec/future-0.18.3.tar.gz", hash = "sha256:34a17436ed1e96697a86f9de3d15a3b0be01d8bc8de9c1dffd59fb8234ed5307"},
 ]
-"gallery-dl 1.25.3" = [
-    {url = "https://files.pythonhosted.org/packages/2d/7b/759ffa14f2b0152b1a71671fb92da305f07bb035d3fb52fddcfe97b3fcc9/gallery_dl-1.25.3-py3-none-any.whl", hash = "sha256:9604690a4584069fb69f220f455a899ea3b323a3eafeb25f173470faf575aaee"},
-    {url = "https://files.pythonhosted.org/packages/be/05/db6932f3f27b24fd33dcc924584bbe8401211120763a8dc0733eaa8bc6a2/gallery_dl-1.25.3.tar.gz", hash = "sha256:6a8b1a03c17c4d5067634333f936d16108d55b91540e24a2a2197feefa97c22b"},
+"gallery-dl 1.25.4" = [
+    {url = "https://files.pythonhosted.org/packages/18/fc/a4af2c1e8de06c46464d67b3cf3993914d9a9b1ce1d6e3840ae82a90f09b/gallery_dl-1.25.4.tar.gz", hash = "sha256:e31d178d7ae21002564a66c68c15b16795895bdaee184f7056b7596137bac04e"},
+    {url = "https://files.pythonhosted.org/packages/4a/03/52dc3552087349a63eb94b6b9c6591205284ba9f93c9b999fb08f3b57146/gallery_dl-1.25.4-py3-none-any.whl", hash = "sha256:62396d46abe38c7f14c27e86734b14bcec9c395a76eb02a40a46f66cf6238fe2"},
 ]
 "guessit 3.7.1" = [
     {url = "https://files.pythonhosted.org/packages/96/5f/64304acee35bac703cee51656a5caf37bd18c9490561fbff225922f41d39/guessit-3.7.1.tar.gz", hash = "sha256:2c18d982ee6db30db5d59557add0324a2b49bf3940a752947510632a2b58a3c1"},
     {url = "https://files.pythonhosted.org/packages/db/5e/eec6416047845a745b1d2aee181244b380e59158e29d814021d2e511b267/guessit-3.7.1-py3-none-any.whl", hash = "sha256:c3be280ee8ec581a45ca6a654a92e317bf89567fdc55e7167452226f4f5b8b38"},
 ]
 "humanize 4.6.0" = [
     {url = "https://files.pythonhosted.org/packages/06/b1/9e491df2ee1c919d67ee328d8bc9f17b7a9af68e4077f3f5fac83a4488c9/humanize-4.6.0.tar.gz", hash = "sha256:5f1f22bc65911eb1a6ffe7659bd6598e33dcfeeb904eb16ee1e705a09bf75916"},
@@ -2068,66 +2068,61 @@
     {url = "https://files.pythonhosted.org/packages/f0/e8/1ea9adebdccaadfc208c7517e09f5145ed5a73069779ff436393085d47a2/numpy-1.24.3-cp311-cp311-win_amd64.whl", hash = "sha256:5342cf6aad47943286afa6f1609cad9b4266a05e7f2ec408e2cf7aea7ff69d80"},
     {url = "https://files.pythonhosted.org/packages/f3/23/7cc851bae09cf4db90d42a701dfe525780883ada86bece45e3da7a07e76b/numpy-1.24.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:3c1104d3c036fb81ab923f507536daedc718d0ad5a8707c6061cdfd6d184e570"},
     {url = "https://files.pythonhosted.org/packages/fa/7d/8dfb40eecbb6bc83ca00ef979f5cdeca5909a250cb8b642dcf1fbd34c078/numpy-1.24.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7"},
 ]
 "olefile 0.46" = [
     {url = "https://files.pythonhosted.org/packages/34/81/e1ac43c6b45b4c5f8d9352396a14144bba52c8fec72a80f425f6a4d653ad/olefile-0.46.zip", hash = "sha256:133b031eaf8fd2c9399b78b8bc5b8fcbe4c31e85295749bb17a87cba8f3c3964"},
 ]
-"orjson 3.8.11" = [
-    {url = "https://files.pythonhosted.org/packages/00/32/b6fac1a93ac31829f7263dc070551a60a0c710c131b0cb58ba41a200d941/orjson-3.8.11-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:6d7b050135669d2335e40120215ad4120e29958c139f8bab68ce06a1cb1a1b2c"},
-    {url = "https://files.pythonhosted.org/packages/00/8a/ca729b5af5972cff989197681f965c590f6120f43eb64e2e6e9abce96e28/orjson-3.8.11-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:358e515b8b19a275b259f5ee1e0efa2859b1d976b5ed5d016ac59f9e6c8788a3"},
-    {url = "https://files.pythonhosted.org/packages/03/1e/728747da836829b358fcc451c0274a3c38e060eea4654793ca6b74636c85/orjson-3.8.11-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bf48ed8d4b6ab9f23b7ee642462369d7133412d72824bad89f9bf4311c06c6a1"},
-    {url = "https://files.pythonhosted.org/packages/13/1e/c9345602fda75f228179b6d3c1c1292adc4f40e260f4536cb2b4044b7d17/orjson-3.8.11-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:7e4ded77ac7432a155d1d27a83bcadf722750aea3b9e6c4d47f2a92054ab71cb"},
-    {url = "https://files.pythonhosted.org/packages/16/45/a05192669185bd7734ebd64ee636a7b200762c6da67894cd6311d00502dd/orjson-3.8.11-cp37-cp37m-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:71a656f1c62e84c69060093e20cedff6a92e472d53ff5b8b9026b1b298542a68"},
-    {url = "https://files.pythonhosted.org/packages/17/7d/4301a4c3c9908e46a5c1186c5232d83b15af7d265817d7553b70197fd009/orjson-3.8.11-cp39-cp39-manylinux_2_28_x86_64.whl", hash = "sha256:714c3e2be6ed7e4ff6e887926d6e171bfd94fdee76d7d3bfa74ee19237a2d49d"},
-    {url = "https://files.pythonhosted.org/packages/32/7f/2e0b9ad9ab068ea32b57ae140e15e7303c2ecf86e1214ce69c8c3ee9ea9b/orjson-3.8.11-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:b369019e597b59c4b97e9f925a3b725321fa1481c129d76c74c6ea3823f5d1e8"},
-    {url = "https://files.pythonhosted.org/packages/37/b1/4dcae237c6498f0cd2afa990bb2d93eb90c5d41a1056f5ca297d2239aa37/orjson-3.8.11-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2fc050f8e7f2e4061c8c9968ad0be745b11b03913b77ffa8ceca65914696886c"},
-    {url = "https://files.pythonhosted.org/packages/3c/4b/67d4a9cbb504817c35e7cb31f4ef006195372497a623618665151b3a14d6/orjson-3.8.11-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3afccf7f8684dca7f017837a315de0a1ab5c095de22a4eed206d079f9325ed72"},
-    {url = "https://files.pythonhosted.org/packages/3e/28/71a77cf7db5c9debc152d411f1da0a5c3a3197a3a1e298464e070f37de00/orjson-3.8.11-cp310-cp310-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:9fa900bdd84b4576c8dd6f3e2a00b35797f29283af328c6e3d70addfa4c2d599"},
-    {url = "https://files.pythonhosted.org/packages/3e/93/08e22637abab902e18780a6b07a7407a68caf9cb872ac79df8e0955d97a5/orjson-3.8.11-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:37f38c8194ce086e6a9816b4b8dde5e7f383feeed92feec0385d99baf64f9b6e"},
-    {url = "https://files.pythonhosted.org/packages/49/f1/f375e5621e79d28ee989cbddf99b4e819b43b741e55ab7935fc9cc6ce08e/orjson-3.8.11-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:7c7b4fae3b8fc69c8e76f1c0694f3decfe8a57f87e7ac7779ebb59cd71135438"},
-    {url = "https://files.pythonhosted.org/packages/52/ae/4c2c3022d8d30cacd87baf955fcee3c986594dd2f103c78631f1c922389f/orjson-3.8.11-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d47f97b99beb9bcac6e288a76b559543a61e0187443d8089204b757726b1d000"},
-    {url = "https://files.pythonhosted.org/packages/67/28/2a968fe292e85bab916db3cb8dd84a722425f4967cd92dd15f12897c1339/orjson-3.8.11-cp38-cp38-manylinux_2_28_x86_64.whl", hash = "sha256:ef52f1d5a2f89ef9049781c90ea35d5edf74374ed6ed515c286a706d1b290267"},
-    {url = "https://files.pythonhosted.org/packages/68/4c/d6e0c378686fc567790c701ada6a9616b201d4a54552bc45b4dbd2b14545/orjson-3.8.11-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:4118dcd2b5a27a22af5ad92414073f25d93bca1868f1f580056003c84841062f"},
-    {url = "https://files.pythonhosted.org/packages/72/bc/e0cf777c3d81af5be4c08df9dae968a5da14f9d2b97f6f590005c83dbd2d/orjson-3.8.11-cp37-none-win_amd64.whl", hash = "sha256:b68a07794834b7bd53ae2a8b4fe4bf010734cae3f0917d434c83b97acf8e5bce"},
-    {url = "https://files.pythonhosted.org/packages/7c/6c/c7c32c67bd8e4a589a905e1a6131a1b7cfe534cff31e66fdce1c3b11de87/orjson-3.8.11-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:d7d5aecccfaf2052cd07ed5bec8efba9ddfea055682fcd346047b1a3e9da3034"},
-    {url = "https://files.pythonhosted.org/packages/7d/8e/53878064fdc3d63acd8bdda4a161cef7eb2e0409cc0f4849752c9867fd80/orjson-3.8.11-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0a53b3c02a38aadc5302661c2ca18645093971488992df77ce14fef16f598b2e"},
-    {url = "https://files.pythonhosted.org/packages/83/07/218d156fd331bf024347239492c6c08a2995ecbfa88bccf11947508256a1/orjson-3.8.11-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:1e97fdbb779a3b8f5d9fc7dfddef5325f81ee45897eb7cb4638d5d9734d42514"},
-    {url = "https://files.pythonhosted.org/packages/85/f9/b0a1736100fa455de898ccc57a54c07612c4919f7eaa761bbc1e5e099254/orjson-3.8.11-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9486963d2e65482c565dacb366adb36d22aa22acf7274b61490244c3d87fa631"},
-    {url = "https://files.pythonhosted.org/packages/86/b1/6042c73cae624793f182f16d7976e42835de2c0421efbe1f431b7f8360d5/orjson-3.8.11-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e14903bfeb591a9117b7d40d81e3ebca9700b4e77bd829d6f22ea57941bb0ebf"},
-    {url = "https://files.pythonhosted.org/packages/87/ea/03502809586741c18fcf6845622ba4a6ca0e77891a3f01ec46281714deae/orjson-3.8.11-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:f4e4a1001933166fd1c257b920b241b35322bef99ed7329338bf266ac053abe7"},
-    {url = "https://files.pythonhosted.org/packages/88/3f/ee2ad2408b1f87b0fef04891151441d2a9951203460953d195c78258860a/orjson-3.8.11-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:c2d3e6b65458ed71b6797f321d6e8bfeeadee9d3d31cac47806a608ea745edd7"},
-    {url = "https://files.pythonhosted.org/packages/88/90/f3c96affce81d08d56434a84c8130da6073fab560622b3a3893c4be59ffa/orjson-3.8.11-cp39-none-win_amd64.whl", hash = "sha256:0bc3d1b93a73b46a698c054697eb2d27bdedbc5ea0d11ec5f1a6bfbec36346b5"},
-    {url = "https://files.pythonhosted.org/packages/8b/90/fd5a7d1a9b1065f3ebae6b227e25fbef8d4454ceac6cd02ae0f9d228f6b3/orjson-3.8.11-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3b65424ceee82b94e3613233b67ef110dc58f9d83b0076ec47a506289552a861"},
-    {url = "https://files.pythonhosted.org/packages/95/00/df4a035a1edba0ee1ae89152312ae837aa0b6cdcc3ac7895409cb1eca6fa/orjson-3.8.11-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f2ef933da50b31c112b252be03d1ef59e0d0552c1a08e48295bd529ce42aaab8"},
-    {url = "https://files.pythonhosted.org/packages/95/4c/61734f64828ac9e0d39382863c0b916e91661d988bb9b654168f34440a3b/orjson-3.8.11-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1103e597c16f82c241e1b02beadc9c91cecd93e60433ca73cb6464dcc235f37c"},
-    {url = "https://files.pythonhosted.org/packages/98/36/3fc17daadc49735a530ac559c037c81edc5dce0763c72b069db401f1dfc0/orjson-3.8.11-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:382f15861a4bf447ab9d07106010e61b217ef6d4245c6cf64af0c12c4c5e2346"},
-    {url = "https://files.pythonhosted.org/packages/98/bc/ad2e5a1411976153621699bc460549691fd19a96eef15faa518162665e5b/orjson-3.8.11-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:5c3b5405edc3a5f9e34516ee1a729f6c46aecf6de960ae07a7b3e95ebdd0e1d9"},
-    {url = "https://files.pythonhosted.org/packages/9e/1d/1e223d0c5eb8093ad9acdaec7f61f5ad041862fe6a27db68dbf4629c4ea1/orjson-3.8.11-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:04b60dfc1251742e79bb075d7a7c4e37078b932a02e6f005c45761bd90c69189"},
-    {url = "https://files.pythonhosted.org/packages/a2/88/90cd28ee83856171f247fca9523857a6c8aad59bad811a25d1388a5c136c/orjson-3.8.11-cp38-cp38-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:98befa717efaab7ddb847ebe47d473f6bd6f0cb53e98e6c3d487c7c58ba2e174"},
-    {url = "https://files.pythonhosted.org/packages/a2/8c/2fb31949136215c828f1ecc266720afbc36b8a80aa299e6e6f3ec9c00632/orjson-3.8.11-cp37-cp37m-manylinux_2_28_x86_64.whl", hash = "sha256:235926b38ed9b76ab2bca99ff26ece79c1c46bc10079b06e660b087aecffbe69"},
-    {url = "https://files.pythonhosted.org/packages/a5/4f/7498b3ec54017a09de2563a4c85c81dcb73894110bc3ecba3580af397445/orjson-3.8.11-cp310-none-win_amd64.whl", hash = "sha256:62eb8bdcf6f4cdbe12743e88ad98696277a75f91a35e8fb93a7ea2b9f4a7000c"},
-    {url = "https://files.pythonhosted.org/packages/a6/85/90b299ff58f851847ba9c149f563c6f18fb9fd054c17f7fe07751eadf844/orjson-3.8.11-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:176d742f53434541e50a5e659694073aa51dcbd8f29a1708a4fa1a320193c615"},
-    {url = "https://files.pythonhosted.org/packages/a9/87/7dd79550c902916ec0aa99c6dd91c5531d48e1d86befa09069ca93848fa8/orjson-3.8.11-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:3c55065bc2075a5ea6ffb30462d84fd3aa5bbb7ae600855c325ee5753feec715"},
-    {url = "https://files.pythonhosted.org/packages/aa/9f/b6f78ff25edadf02fdb9d521268245f6d554ee20353594e9492a455bd874/orjson-3.8.11-cp311-cp311-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:982ab319b7a5ece4199caf2a2b3a28e62a8e289cb6418548ef98bced7e2a6cfe"},
-    {url = "https://files.pythonhosted.org/packages/b5/c4/6d6e4d68a789c807f615d5f9ffceead50b3df733ac0c7fc19d47b7a4cbf7/orjson-3.8.11-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0f9415b86ef154bf247fa78a6918aac50089c296e26fb6cf15bc9d7e6402a1f8"},
-    {url = "https://files.pythonhosted.org/packages/b7/43/dffa4fcdcc7d39ccf8509896523359d1c5aa02e25088b1ee2ebaf53118fa/orjson-3.8.11-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:3485c458670c0edb79ca149fe201f199dd9ccfe7ca3acbdef617e3c683e7b97f"},
-    {url = "https://files.pythonhosted.org/packages/b8/ef/4bedd95b595776c4745c8bff77aa00f755cc88cc6b94bd9e8b5595dd1a0e/orjson-3.8.11.tar.gz", hash = "sha256:882c77126c42dd93bb35288632d69b1e393863a2b752de3e5fe0112833609496"},
-    {url = "https://files.pythonhosted.org/packages/c4/07/f29b03ddbf98828aa84549a810ba13770a2a61e08621009e581152f19534/orjson-3.8.11-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:173b8f8c750590f432757292cfb197582e5c14347b913b4017561d47af0e759b"},
-    {url = "https://files.pythonhosted.org/packages/cd/7a/bbcc6b07d078a877dc6bd56aa3b0b97c2e463800986cd7edf26605080a2d/orjson-3.8.11-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:66f0c9e4e8f6641497a7dc50591af3704b11468e9fc90cfb5874f28b0a61edb5"},
-    {url = "https://files.pythonhosted.org/packages/d9/f2/e051be62f8e415edd72328a0a14ee028432ff89cd20f3c808f27587e1fad/orjson-3.8.11-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1fedcc428416e23a6c9de62a000c22ae33bbe0108302ad5d5935e29ea739bf37"},
-    {url = "https://files.pythonhosted.org/packages/da/c3/5ed5c85029d814408bb841a77b566eb777d6855b13c9c45ddeac87343b64/orjson-3.8.11-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:d70b6db9d4e1e6057829cd7fe119c217cebaf989f88d14b2445fa69fc568d03e"},
-    {url = "https://files.pythonhosted.org/packages/dc/7f/2647741a99d42422ad82e8c9424b5ee4443951c2ae5f743d1dd4a6719551/orjson-3.8.11-cp311-none-win_amd64.whl", hash = "sha256:12f647d4da0aab1997e25bed4fa2b76782b5b9d2d1bf3066b5f0a57d34d833c4"},
-    {url = "https://files.pythonhosted.org/packages/ec/5a/6e791896f99ca1f5bb5da5327143cda69b4dc62bfe1088e5e60817f1bc6a/orjson-3.8.11-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:08729e339ff3146e6de56c1166f014c3d2ec3e79ffb76d6c55d52cc892e5e477"},
-    {url = "https://files.pythonhosted.org/packages/ec/db/c9f42566e339faa5cd840c73e7698f439ec916626d79bfee8a4e7c078020/orjson-3.8.11-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cdf201e77d3fac9d8d6f68d872ef45dccfe46f30b268bb88b6c5af5065b433aa"},
-    {url = "https://files.pythonhosted.org/packages/ed/7e/e614a9d5f0a5f35b47a650cb5e01d1dfee83e0b69232f5f5474d1969b94f/orjson-3.8.11-cp39-cp39-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:c67ac094a4dde914297543af19f22532d7124f3a35245580d8b756c4ff2f5884"},
-    {url = "https://files.pythonhosted.org/packages/f5/d6/366c09102f8a41b168e537db866f1b681cb037c0ceb036c3b908921030ee/orjson-3.8.11-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:58c068f93d701f9466f667bf3b5cb4e4946aee940df2b07ca5101f1cf1b60ce4"},
-    {url = "https://files.pythonhosted.org/packages/f7/d5/ca8ab6e8b04bc62f605c488759cdfc3ba815ab9a18573e65d97dd763b409/orjson-3.8.11-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f7aeefac55848aeb29f20b91fa55f9e488f446201bb1bb31dc17480d113d8955"},
-    {url = "https://files.pythonhosted.org/packages/fa/84/bd6533b9c2eeda75df9502c6514e557083f0834daa85ce89fe1c5d5b490b/orjson-3.8.11-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:553fdaf9f4b5060a0dcc517ae0c511c289c184a83d6719d03c5602ed0eef0390"},
-    {url = "https://files.pythonhosted.org/packages/fc/47/1cd81f3a396ef3a3883378c3bad80509c0f14429d62a3100d5b26f82d870/orjson-3.8.11-cp38-none-win_amd64.whl", hash = "sha256:5ff10789cbc08a9fd94507c907ba55b9315e99f20345ff8ef34fac432dacd948"},
+"orjson 3.8.12" = [
+    {url = "https://files.pythonhosted.org/packages/01/af/f0f1583194cb2b4e28b11e9c423d336e10ffee09939d86fa54ade60fe3ff/orjson-3.8.12-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:efb3a10030462a22c731682434df5c137a67632a8339f821cd501920b169007e"},
+    {url = "https://files.pythonhosted.org/packages/10/72/3e0c81df350632898725ca542538e648e28f6268542eff3fe0129290916c/orjson-3.8.12-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:6d1acf52d3a4b9384af09a5c2658c3a7a472a4d62a0ad1fe2c8fab8ef460c9b4"},
+    {url = "https://files.pythonhosted.org/packages/14/b7/18c54b14bdf6b1a805b706adfae2cc1a460de344ae1f6f8d5e1419093afe/orjson-3.8.12-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a72b50719bdd6bb0acfca3d4d1c841aa4b191f3ff37268e7aba04e5d6be44ccd"},
+    {url = "https://files.pythonhosted.org/packages/15/87/cd5a506935f80a75b0675aa06106efefb1379c1ed9bbb942794073cd8793/orjson-3.8.12-cp311-cp311-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:9a6c1594d5a9ff56e5babc4a87ac372af38d37adef9e06744e9f158431e33f43"},
+    {url = "https://files.pythonhosted.org/packages/16/f2/459afafc84fe178e30f593468d65a687449a49253ef217be151f398a0e0f/orjson-3.8.12-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:77710774faed337ac4ad919dadc5f3b655b0cd40518e5386e6f1f116de9c6c25"},
+    {url = "https://files.pythonhosted.org/packages/17/29/369a64bf87e66886e66962a1dd859b420bd79fec6771efffad94d56bd296/orjson-3.8.12-cp38-cp38-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:062e67108c218fdb9475edd5272b1629c05b56c66416fa915de5656adde30e73"},
+    {url = "https://files.pythonhosted.org/packages/17/68/bb2b4056589896f7500ac536331c713181bda9d29af8649bbdb359a5bc03/orjson-3.8.12-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:96fb1eb82b578eb6c0e53e3cf950839fe98ea210626f87c8204bd4fc2cc6ba02"},
+    {url = "https://files.pythonhosted.org/packages/18/22/440bd56050eb12ec7e4adf87386836385582d3801dcd4a6b00564d553559/orjson-3.8.12-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:4fd240e736ce52cd757d74142d9933fd35a3184396be887c435f0574e0388654"},
+    {url = "https://files.pythonhosted.org/packages/1a/ad/023133cbd08249a040fb4c422f8f527d557c9984eab83b2b5c9558c258b6/orjson-3.8.12-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f568205519bb0197ca91915c5da6058cfbb59993e557b02dfc3b2718b34770a"},
+    {url = "https://files.pythonhosted.org/packages/26/2b/8f00f06ea857f00c3521e6a3fadf7e838a01faec7591cdbf217b25ad955d/orjson-3.8.12-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:becbd5af6d035a7ec2ee3239d4700929d52d8517806b97dd04efcc37289403f7"},
+    {url = "https://files.pythonhosted.org/packages/29/07/593edef4aefa554a7fb83d8616bffb76de0b6188b963dc74f75065668654/orjson-3.8.12-cp39-none-win_amd64.whl", hash = "sha256:82d65e478a21f98107b4eb8390104746bb3024c27084b57edab7d427385f1f70"},
+    {url = "https://files.pythonhosted.org/packages/29/9f/91d73b05f1bca62b815425e655e2b6d7da85f7f152955ca86a14af1c4db8/orjson-3.8.12-cp39-cp39-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:aff761de5ed5543a0a51e9f703668624749aa2239de5d7d37d9c9693daeaf5dc"},
+    {url = "https://files.pythonhosted.org/packages/2d/47/78b9f77454e5ba2adf527da5a4acb98e6d6291e162c0345649fe7f28b551/orjson-3.8.12-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:2ad149ed76dce2bbdfbadd61c35959305e77141badf364a158beb4ef3d88ec37"},
+    {url = "https://files.pythonhosted.org/packages/32/2f/6bd7d4e90dfe7d21a410907caceb9192c6595b1f8e3fca2a13c86e35cb34/orjson-3.8.12-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:62f999798f2fa55e567d483864ebfc30120fb055c2696a255979439323a5b15c"},
+    {url = "https://files.pythonhosted.org/packages/33/a5/a90f88d7e5c2d4281ee0a0fbf78dff31d1da8762787610924392200913ec/orjson-3.8.12-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ebb03e4c7648f7bb299872002a6120082da018f41ba7a9ebf4ceae8d765443d2"},
+    {url = "https://files.pythonhosted.org/packages/35/f0/07ee02d463bc8964e723cdac48a6d928dcc021778b2eacd338339f6e67e1/orjson-3.8.12-cp37-none-win_amd64.whl", hash = "sha256:6f1b01f641f5e87168b819ac1cbd81aa6278e7572c326f3d27e92dea442a2c0d"},
+    {url = "https://files.pythonhosted.org/packages/3e/1d/e5628cd5828a325db7c1b3c241c99b76b1640ec2fd7b6eb6bd9895879e6b/orjson-3.8.12.tar.gz", hash = "sha256:9f0f042cf002a474a6aea006dd9f8d7a5497e35e5fb190ec78eb4d232ec19955"},
+    {url = "https://files.pythonhosted.org/packages/48/51/e1efdcaa98fd77527d3e46c9081d113c866af7f60317bdfc305c82e9fbca/orjson-3.8.12-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8682f752c19f6a7d9fc727fd98588b4c8b0dce791b5794bb814c7379ccd64a79"},
+    {url = "https://files.pythonhosted.org/packages/4f/fd/b8b27f9dce9e6b72968c5c955ca738c5a7cd3c0e98c48223151f587ea85f/orjson-3.8.12-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0ba645c92801417933fa74448622ba614a275ea82df05e888095c7742d913bb4"},
+    {url = "https://files.pythonhosted.org/packages/5a/98/98954742d267ed528c9a7a7317a165cdfd47c46cf32e71233925da1486b6/orjson-3.8.12-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:135f29cf936283a0cd1b8bce86540ca181108f2a4d4483eedad6b8026865d2a9"},
+    {url = "https://files.pythonhosted.org/packages/69/25/ed824928caac9ce7e609f023c8084fc61f4f21d106adaa724e0789a49836/orjson-3.8.12-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:44f7bb4c995652106276442de1147c9993716d1e2d79b7fd435afa154ff236b9"},
+    {url = "https://files.pythonhosted.org/packages/6b/df/bfba654be34cda184e7345606471f6f5320034d783bd0c9444e2be6858c7/orjson-3.8.12-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:834b50df79f1fe89bbaced3a1c1d8c8c92cc99e84cdcd374d8da4974b3560d2a"},
+    {url = "https://files.pythonhosted.org/packages/6e/ff/a2bd5781213b9770e7bb3beb1995ca1a4681d7a35bd00e6d1c65b5437063/orjson-3.8.12-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:355055e0977c43b0e5325b9312b7208c696fe20cd54eed1d6fc80b0a4d6721f5"},
+    {url = "https://files.pythonhosted.org/packages/70/54/2f31265e4021872397dec7d7d0b2baed6d59c7aa4910df73fae5fb6fdfcb/orjson-3.8.12-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c6390ce0bce24c107fc275736aa8a4f768ef7eb5df935d7dca0cc99815eb5d99"},
+    {url = "https://files.pythonhosted.org/packages/79/1e/50cf4ba0dc3a90233a0d4c75eae8fe7eb344a7f0638f61463a2cac13265f/orjson-3.8.12-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6cae2ff288a80e81ce30313e735c5436495ab58cf8d4fbe84900e616d0ee7a78"},
+    {url = "https://files.pythonhosted.org/packages/7b/fa/5011e7e3945147a61b2f5a798f6e5570fff5d7324bb8fa6a5a150dafdcd1/orjson-3.8.12-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:de3d096dde3e46d01841abc1982b906694ab3c92f338d37a2e6184739dc8a958"},
+    {url = "https://files.pythonhosted.org/packages/81/cb/5fe6078cd7425ddcbbf48aa5001bbf4cf7bfcd83992af4ded037b401b1b4/orjson-3.8.12-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:7e549468867991f6f9cfbd9c5bbc977330173bd8f6ceb79973bbd4634e13e1b9"},
+    {url = "https://files.pythonhosted.org/packages/a5/63/a28607d7a7142a4e70d5571a2d3252de660f4cfc6b5e6e03efc608e3f4e6/orjson-3.8.12-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:397670665f94cf5cff779054781d80395084ba97191d82f7b3a86f0a20e6102b"},
+    {url = "https://files.pythonhosted.org/packages/a5/d3/cb28e1fccaa0740ed0f8562153651caabcd44589b6ee6960a0bf4f5e327d/orjson-3.8.12-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:d937503e4dfba5edc8d5e0426d3cc97ed55716e93212b2e12a198664487b9965"},
+    {url = "https://files.pythonhosted.org/packages/b0/e6/3242d5681358f65ead018d834d0e01f55c49347b06ba132931da49947a8e/orjson-3.8.12-cp310-none-win_amd64.whl", hash = "sha256:06e528f9a84fbb4000fd0eee573b5db543ee70ae586fdbc53e740b0ac981701c"},
+    {url = "https://files.pythonhosted.org/packages/b7/27/545b49651dca71eb92134935c49942c7be43672659c8db1b23d78c8d5a6d/orjson-3.8.12-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8d153b228b6e24f8bccf732a51e01e8e938eef59efed9030c5c257778fbe0804"},
+    {url = "https://files.pythonhosted.org/packages/bc/fe/b623cfe25ca9bdc3cb6cbefc6871ce3785363bfd38a30102dda44fbf4671/orjson-3.8.12-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:7e405d54c84c30d9b1c918c290bcf4ef484a45c69d5583a95db81ffffba40b44"},
+    {url = "https://files.pythonhosted.org/packages/bd/99/cfd8ef1b184ab9973517d450256d4f3a5b07ee958b0482819441c46cd7c3/orjson-3.8.12-cp37-cp37m-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:dc27a8ec13f28e92dc1ea89bf1232d77e7d3ebfd5c1ccf4f3729a70561cb63bd"},
+    {url = "https://files.pythonhosted.org/packages/bd/9d/6361f9333d9ec3593164e0cee538f66c1cdba317ff5f2d6e7debd5501541/orjson-3.8.12-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f480ae7b84369b1860d8867f0baf8d885fede400fda390ce088bfa8edf97ffdc"},
+    {url = "https://files.pythonhosted.org/packages/c5/76/1be359006bb9369ce52119ca6d0c30a408ecfb8726bdc61b7f444b53a046/orjson-3.8.12-cp38-none-win_amd64.whl", hash = "sha256:710c40c214b753392e46f9275fd795e9630dd737a5ab4ac6e4ee1a02fe83cc0d"},
+    {url = "https://files.pythonhosted.org/packages/c9/9e/1de9209a233ebaa6a013473bf17af25f1bd4b66653540dcf2f5618f633d0/orjson-3.8.12-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f4e22b0aa70c963ac01fcd620de15be21a5027711b0e5d4b96debcdeea43e3ae"},
+    {url = "https://files.pythonhosted.org/packages/cc/08/a921138667cc064cee508e74a4c2e99afead8961552b047f3cbceb6dafaf/orjson-3.8.12-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:7d50d9b1ae409ea15534365fec0ce8a5a5f7dc94aa790aacfb8cfec87ab51aa4"},
+    {url = "https://files.pythonhosted.org/packages/cd/5e/f388c8f606c5c2aa047f93759ab94b1ff739cc99a9b95e507ca4bd242171/orjson-3.8.12-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:7d63f524048825e05950db3b6998c756d5377a5e8c469b2e3bdb9f3217523d74"},
+    {url = "https://files.pythonhosted.org/packages/cf/78/8f74d1670446455420c270792da794a8bc11bffc1f13fb2fa6803bd46837/orjson-3.8.12-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:8f00038bf5d07439d13c0c2c5cd6ad48eb86df7dbd7a484013ce6a113c421b14"},
+    {url = "https://files.pythonhosted.org/packages/d4/58/33619aab5d51f1948ab21aa7b26698a76ec9b1f2b5fb2af96dc3fd9a6833/orjson-3.8.12-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:cd6fbd1413559572e81b5ac64c45388147c3ba85cc3df2eaa11002945e0dbd1f"},
+    {url = "https://files.pythonhosted.org/packages/d6/18/e39890cbc4d2a6c4d7bc2202b960c3a6035df8f26b261d72da7b580f35ee/orjson-3.8.12-cp311-none-win_amd64.whl", hash = "sha256:eb16e0195febd24b44f4db1ab3be85ecf6038f92fd511370cebc004b3d422294"},
+    {url = "https://files.pythonhosted.org/packages/d7/b0/9ccdd107dc875e603edf9fa024680a2d63ab3e23464a4e78d5d1b8ecdde4/orjson-3.8.12-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:83e8c740a718fa6d511a82e463adc7ab17631c6eea81a716b723e127a9c51d57"},
+    {url = "https://files.pythonhosted.org/packages/d8/11/a9598459031b6601186352ad1441ae17ba8963b9dc7f7806b40dcedeff02/orjson-3.8.12-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:ec4f0130d9a27cb400423e09e0f9e46480e9e977f05fdcf663a7a2c68735513e"},
+    {url = "https://files.pythonhosted.org/packages/df/a1/5ec3a96568c40aa2ecf0220872691ef271454cadec1a6b761ae52f67bcbf/orjson-3.8.12-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3fa58ca064c640fa9d823f98fbbc8e71940ecb78cea3ac2507da1cbf49d60b51"},
+    {url = "https://files.pythonhosted.org/packages/e6/a7/d716cf8836515a85c349ad7fb1279536b7d59a1187b596a69cee66708e75/orjson-3.8.12-cp310-cp310-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:c84046e890e13a119404a83f2e09e622509ed4692846ff94c4ca03654fbc7fb5"},
+    {url = "https://files.pythonhosted.org/packages/f8/28/a1be6e66721ee95cff620a305447520e4c360bd8b9c9c7ba64c725262873/orjson-3.8.12-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:29706dd8189835bcf1781faed286e99ae54fd6165437d364dfdbf0276bf39b19"},
 ]
 "packaging 23.1" = [
     {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 "pandas 2.0.1" = [
     {url = "https://files.pythonhosted.org/packages/16/75/924e3a52c35cb105a152d29622d0f06bb0f48a677e77ddd6e11ef0004164/pandas-2.0.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e09a53a4fe8d6ae2149959a2d02e1ef2f4d2ceb285ac48f74b79798507e468b4"},
@@ -2570,32 +2565,32 @@
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
 "rich 13.3.5" = [
     {url = "https://files.pythonhosted.org/packages/39/03/6de23bdd88f5ee7f8b03f94f6e88108f5d7ffe6d207e95cdb06d9aa4cd57/rich-13.3.5-py3-none-any.whl", hash = "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"},
     {url = "https://files.pythonhosted.org/packages/3d/0b/8dd34d20929c4b5e474db2e64426175469c2b7fea5ba71c6d4b3397a9729/rich-13.3.5.tar.gz", hash = "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c"},
 ]
-"ruff 0.0.264" = [
-    {url = "https://files.pythonhosted.org/packages/1e/0e/375fde351cb0531470ad6b437cb1bbb6ce83cb0f6e01d0fd68680e3cfeff/ruff-0.0.264-py3-none-win32.whl", hash = "sha256:5a8658ebcc37d62f72840cbdf564171c1a2b6831db482b4d917962541a2f4a44"},
-    {url = "https://files.pythonhosted.org/packages/23/dc/51ee0cd6d2c3c8e0ddc6531c7a8909c5df5f5f21d091854e9ff4293a7466/ruff-0.0.264-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:d628de91e2be7a83128526636097d2dd890669a06143f826f6c591d79aeefbc4"},
-    {url = "https://files.pythonhosted.org/packages/31/84/b47957fa69018359dfbc350e28404a78f20a6cf213b580eff737784e3389/ruff-0.0.264-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:cd4f60ffc3eb15802c554a9c8581bf2117c4d3d06fbc57e0ba58f04cb1aaa47f"},
-    {url = "https://files.pythonhosted.org/packages/37/6f/4aeda64a401beecf560381961efd8a01d6d53d1e095b084b77f31e410dca/ruff-0.0.264-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:91c6eb4f979b661a2dd850d9ac803842bb7b66d4926de84f09c787af82590f73"},
-    {url = "https://files.pythonhosted.org/packages/37/f1/c4023c9dc501d7e49fe939fd86a287c02cf044be6f6cece359218c2ea025/ruff-0.0.264-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:71fd865ebacc1083259b3fb7e3eb45235a86e62e21830b8a6b067be0ec54aa2e"},
-    {url = "https://files.pythonhosted.org/packages/57/eb/ec0dd02cfd07b7f725d5ba18edcbe1f1228b89d650eb72f50049c75f1df2/ruff-0.0.264-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:04ec5d75e4bca754cedd20d53e2ba4920d6259e7579abfb2e8e30c3c80e41b17"},
-    {url = "https://files.pythonhosted.org/packages/64/a9/0ab814985bc90c19e7ac8ba53406c8f2f535739fff3a749e83a0573420ae/ruff-0.0.264-py3-none-musllinux_1_2_i686.whl", hash = "sha256:484e395d1984ab9e1e66bd42e7a5192decfee86998d07d36ee50b2fadccc8734"},
-    {url = "https://files.pythonhosted.org/packages/68/1d/f6fbf3b023b0c86c372ebe31907e18a3fc22ee3f6e00ea534e530aa48466/ruff-0.0.264-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4564e0f245eb515c6ed63988c21e9c40bcfd485cd1ec63bdd790f9a81d301f15"},
-    {url = "https://files.pythonhosted.org/packages/6a/18/9809f9c1008a9f0cf1cbfc400b46649f1631eebe4dc6f9421f7178c361f8/ruff-0.0.264-py3-none-win_arm64.whl", hash = "sha256:3e2c38449548e122f2612843a7c04e22b4fd491656955c57b8cb05df11639ad6"},
-    {url = "https://files.pythonhosted.org/packages/78/40/6a33d40d0bd48adce97775ed68b06922c95dba8076bb6db7ab320f6b9002/ruff-0.0.264-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:323ae6c1702b26c96d0fbf939c5959c37e79021f86b70f63634df918bc77f36e"},
-    {url = "https://files.pythonhosted.org/packages/8a/e0/3cc67b6f9b9f20c04f1237a6192b19343309d3c2605930ea2472eb2f81fe/ruff-0.0.264-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:18a29ed37bf8cfe6dce8a2db56c313a64c0804095108753621f3c3321e0c9c5f"},
-    {url = "https://files.pythonhosted.org/packages/a3/82/2cb89c8afffb03201cbdd19529ed5b3338705d5c6fb2b76830d3d1955f17/ruff-0.0.264-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:d97ba8db0fb601ffe9ee996ebb97c698e427a2fd4514fefbe7b803111354f783"},
-    {url = "https://files.pythonhosted.org/packages/b2/95/bb0befe3eb5fc7ae4bfde2f4162323bf55136a106fd0685378c35a89e1bb/ruff-0.0.264-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:67326fdc9ac0a1b13e229c6e24e8d115863c52cd710faaaaa588851535281d6c"},
-    {url = "https://files.pythonhosted.org/packages/be/b3/bcf54b0ddf6e0e75ebe7fbe3bb1c7786647f1aac3ed60e128863129b3b4a/ruff-0.0.264-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:ec2fa192c035b8b68cc2b91049c561cd69543e2b8c4d157d9aa7727320bedcca"},
-    {url = "https://files.pythonhosted.org/packages/c2/a9/7c1b194946f1460ffbf26d9d25649c6ec4119982552936b3ce4425b7cae7/ruff-0.0.264-py3-none-win_amd64.whl", hash = "sha256:068a82a29d80848a56e3d9d4308e6e0ca8b2ecdaf5ac342a292545a59b7f2c21"},
-    {url = "https://files.pythonhosted.org/packages/c6/06/3ed1d46e1e2a71d5b88b0087a994642730e5c1396425dd31d017463e0614/ruff-0.0.264.tar.gz", hash = "sha256:8fcd4b693ca1374eb7a5796581c90689f884f98f388740d94f0702fd30f8f78f"},
-    {url = "https://files.pythonhosted.org/packages/fb/60/2f4f5170c58d70e4600d71c91e76b83a25ec31dfd2eb939e0805c1bbe6d2/ruff-0.0.264-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:05ee163a046fc593d150179d23f4af447fb82f3e59cd34e031ea0868c65bb8e8"},
+"ruff 0.0.265" = [
+    {url = "https://files.pythonhosted.org/packages/27/ee/674d3816cbffa55e4fad4446e2815c783ca0648180a905418edfd664bc50/ruff-0.0.265-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:30ddfe22de6ce4eb1260408f4480bbbce998f954dbf470228a21a9b2c45955e4"},
+    {url = "https://files.pythonhosted.org/packages/40/8d/fbd44882b6ef61c8be8fa9ce6448bb99ff105816ac22e2f2116473809c6d/ruff-0.0.265-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:1d5a8de2fbaf91ea5699451a06f4074e7a312accfa774ad9327cde3e4fda2081"},
+    {url = "https://files.pythonhosted.org/packages/41/33/f9043ba8a20a667d888adc81768ebdaadaa0d2b760da61912682d62bbff8/ruff-0.0.265-py3-none-win_amd64.whl", hash = "sha256:f54facf286103006171a00ce20388d88ed1d6732db3b49c11feb9bf3d46f90e9"},
+    {url = "https://files.pythonhosted.org/packages/77/cc/8806e6aaf8dc0cd4f41444f5423c31d691b7acf0386665406823f9528e45/ruff-0.0.265-py3-none-win_arm64.whl", hash = "sha256:c78470656e33d32ddc54e8482b1b0fc6de58f1195586731e5ff1405d74421499"},
+    {url = "https://files.pythonhosted.org/packages/94/67/f875768b8ecfbc6264a9fc5e10735359f23b2ac98194bf0512555225b987/ruff-0.0.265-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:5028950f7af9b119d43d91b215d5044976e43b96a0d1458d193ef0dd3c587bf8"},
+    {url = "https://files.pythonhosted.org/packages/9d/07/7178c1b251c2bfed0676e7f8cd76d6107a5e89b2d1b7b464c084b311dfe6/ruff-0.0.265-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b279fa55ea175ef953208a6d8bfbcdcffac1c39b38cdb8c2bfafe9222add70bb"},
+    {url = "https://files.pythonhosted.org/packages/9e/35/fb24000483a56339ffe3c00c8b0d12c4ca99201f7f2f30f4799202a20a83/ruff-0.0.265-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:a8b44a245b60512403a6a03a5b5212da274d33862225c5eed3bcf12037eb19bb"},
+    {url = "https://files.pythonhosted.org/packages/a1/00/135639453182b6c64c507f448764d78f8df90bcd19e4b0e16427407709e0/ruff-0.0.265-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:9ac13b11d9ad3001de9d637974ec5402a67cefdf9fffc3929ab44c2fcbb850a1"},
+    {url = "https://files.pythonhosted.org/packages/b2/bc/b14c0de95721ef6bd3a1dcfe7b4ce9f368c72a2d5aed7c98e767771c860c/ruff-0.0.265-py3-none-musllinux_1_2_i686.whl", hash = "sha256:d0f9967f84da42d28e3d9d9354cc1575f96ed69e6e40a7d4b780a7a0418d9409"},
+    {url = "https://files.pythonhosted.org/packages/b3/1d/0e544e4b73bafbe88f6c39bce5306fdbf5af07e9d004fe023eeedf9ee548/ruff-0.0.265-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:d586e69ab5cbf521a1910b733412a5735936f6a610d805b89d35b6647e2a66aa"},
+    {url = "https://files.pythonhosted.org/packages/b4/c4/7b8b05279a11ba30cf99eb628dbfd2fbf7219c192eb78f9585280bc3ae69/ruff-0.0.265-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:62a9578b48cfd292c64ea3d28681dc16b1aa7445b7a7709a2884510fc0822118"},
+    {url = "https://files.pythonhosted.org/packages/c7/87/9b9d14b1778edb4ce03e0e80ab9378e12e402dce2b5cd27403b6670b6ed6/ruff-0.0.265-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:4057eb539a1d88eb84e9f6a36e0a999e0f261ed850ae5d5817e68968e7b89ed9"},
+    {url = "https://files.pythonhosted.org/packages/d1/c3/2aeec2adaff3cfa95d713283089568ee905f759e18d034646e3aa85a6282/ruff-0.0.265.tar.gz", hash = "sha256:53c17f0dab19ddc22b254b087d1381b601b155acfa8feed514f0d6a413d0ab3a"},
+    {url = "https://files.pythonhosted.org/packages/e3/d1/433db20e8ef8f67ff7cfa32fdf6b9adb0592a1269fd93e230fd0dfbf64f2/ruff-0.0.265-py3-none-win32.whl", hash = "sha256:9e9db5ccb810742d621f93272e3cc23b5f277d8d00c4a79668835d26ccbe48dd"},
+    {url = "https://files.pythonhosted.org/packages/e7/c3/157c421412809780430110b766f8bdad65b55f0671c00c778d827dbb6f35/ruff-0.0.265-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2a9b38bdb40a998cbc677db55b6225a6c4fadcf8819eb30695e1b8470942426b"},
+    {url = "https://files.pythonhosted.org/packages/f4/1c/5161404f7231c37e951f7dce3a4f623733a6563c17724189d003602ce55f/ruff-0.0.265-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:aa17b13cd3f29fc57d06bf34c31f21d043735cc9a681203d634549b0e41047d1"},
+    {url = "https://files.pythonhosted.org/packages/fd/ac/1c40dc44ed92744c3a9ca6f07ed2d83f0431d71a02766a7a478e2112fb59/ruff-0.0.265-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:a11bd0889e88d3342e7bc514554bb4461bf6cc30ec115821c2425cfaac0b1b6a"},
 ]
 "scalene 1.5.19" = [
     {url = "https://files.pythonhosted.org/packages/11/19/c973ecc43b18076df6c7efff7bec280d02d48d8245f46d94b7e90cf306f2/scalene-1.5.19-cp39-cp39-win_amd64.whl", hash = "sha256:d1fd5d83f3c022ddc46049f29823351b8dbdb8590f5803358fa6034784601f24"},
     {url = "https://files.pythonhosted.org/packages/19/54/d89426ab970f1cb3850b0374967ae22d831d0091efeb2c1d8e8d02ac2a19/scalene-1.5.19-cp39-cp39-macosx_11_7_universal2.whl", hash = "sha256:6c08f3bc0b6355db3c34f0e9aea1b291e64675bb832e19758ee751918787cac0"},
     {url = "https://files.pythonhosted.org/packages/49/11/5a2fa4567eee217609e0a627534f5fb60d0c1f768b43a93145a2ea24e39b/scalene-1.5.19-cp38-cp38-manylinux_2_24_x86_64.whl", hash = "sha256:f67f39321548c06de440319bdd70c41c14b6c50d4748226a101402995677cade"},
     {url = "https://files.pythonhosted.org/packages/5e/3c/b1f159a11f0949f3f27b18af1cc68ee301088a7337efc7d961684bdd3f46/scalene-1.5.19-cp37-cp37m-macosx_10_15_universal2.whl", hash = "sha256:58fb40d031081a55e813f292b2d85b64d7558a372832d8e456f7fe2113adf182"},
     {url = "https://files.pythonhosted.org/packages/65/c3/ebaf00eef807b8da6c5b0c4eb6627f0a67538a25ac7e3858347e15c55d22/scalene-1.5.19-cp38-cp38-win_amd64.whl", hash = "sha256:7a1d452ad4d32cf8adb8b86cae4e5b9c7bff866fff1c43618f9ad114b9ecac32"},
@@ -2629,17 +2624,17 @@
 "speechrecognition 3.8.1" = [
     {url = "https://files.pythonhosted.org/packages/26/e1/7f5678cd94ec1234269d23756dbdaa4c8cfaed973412f88ae8adf7893a50/SpeechRecognition-3.8.1-py2.py3-none-any.whl", hash = "sha256:4d8f73a0c05ec70331c3bacaa89ecc06dfa8d9aba0899276664cda06ab597e8e"},
 ]
 "sqlite-fts4 1.0.3" = [
     {url = "https://files.pythonhosted.org/packages/51/29/0096e8b1811aaa78cfb296996f621f41120c21c2f5cd448ae1d54979d9fc/sqlite_fts4-1.0.3-py3-none-any.whl", hash = "sha256:0359edd8dea6fd73c848989e1e2b1f31a50fe5f9d7272299ff0e8dbaa62d035f"},
     {url = "https://files.pythonhosted.org/packages/c2/6d/9dad6c3b433ab8912ace969c66abd595f8e0a2ccccdb73602b1291dbda29/sqlite-fts4-1.0.3.tar.gz", hash = "sha256:78b05eeaf6680e9dbed8986bde011e9c086a06cb0c931b3cf7da94c214e8930c"},
 ]
-"sqlite-utils 3.30" = [
-    {url = "https://files.pythonhosted.org/packages/0c/d4/4e27f7aeeda5b0ed9da7cacffe81f2e48cd5a4f347c72011390f04267ac4/sqlite_utils-3.30-py3-none-any.whl", hash = "sha256:e2113e5ce8e9c69822fff419145d7144034b0bd7bb6bf9b8bf92bcc6de859705"},
-    {url = "https://files.pythonhosted.org/packages/ba/8d/9660dc531135779a1980e670d78d1402506e02fc1aaa10556da6ecf9960c/sqlite-utils-3.30.tar.gz", hash = "sha256:30005c12d5f13445659f791766beb6a9900c25f442bea1f980f21d38b75f6e33"},
+"sqlite-utils 3.31" = [
+    {url = "https://files.pythonhosted.org/packages/61/c9/99abf36fcef22959316cff00a7f07b413256ad97ab803ee45d6de78f2a52/sqlite_utils-3.31-py3-none-any.whl", hash = "sha256:95849cf62a9d6aa7df2dd27dfc615c0ee71c515516284a7d85e2c061021893c9"},
+    {url = "https://files.pythonhosted.org/packages/e8/da/6f34fd782e805f275ac17ecaba247db6c53eeaf340907c0e536366b6de1b/sqlite-utils-3.31.tar.gz", hash = "sha256:54989f3d09ed121f9df97831d041738ae48771d3ca85008946f1bc1884109a8a"},
 ]
 "ssort 0.11.6" = [
     {url = "https://files.pythonhosted.org/packages/27/c6/4fdb102b282380d5b4791d90302ba8778689f24bef118707fd50f037752e/ssort-0.11.6.tar.gz", hash = "sha256:21fec493487f32dff50d30efa5b6aad18286e9817600b64bfe686ae062bae7ae"},
 ]
 "stack-data 0.6.2" = [
     {url = "https://files.pythonhosted.org/packages/6a/81/aa96c25c27f78cdc444fec27d80f4c05194c591465e491a1358d8a035bc1/stack_data-0.6.2-py3-none-any.whl", hash = "sha256:cbb2a53eb64e5785878201a97ed7c7b94883f48b87bfb0bbe8b623c74679e4a8"},
     {url = "https://files.pythonhosted.org/packages/db/18/aa7f2b111aeba2cd83503254d9133a912d7f61f459a0c8561858f0d72a56/stack_data-0.6.2.tar.gz", hash = "sha256:32d2dd0376772d01b6cb9fc996f3c8b57a357089dec328ed4b6553d037eaf815"},
@@ -2696,89 +2691,89 @@
     {url = "https://files.pythonhosted.org/packages/20/f4/c0584a25144ce20bfcf1aecd041768b8c762c1eb0aa77502a3f0baa83f11/wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {url = "https://files.pythonhosted.org/packages/5e/5f/1e4bd82a9cc1f17b2c2361a2d876d4c38973a997003ba5eb400e8a932b6c/wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
 "websocket-client 1.5.1" = [
     {url = "https://files.pythonhosted.org/packages/6d/9a/6c793729c9d48fcca155ce55e4dfafacffb7fb52a62e3ae2198846c31af6/websocket_client-1.5.1-py3-none-any.whl", hash = "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"},
     {url = "https://files.pythonhosted.org/packages/8b/94/696484b0c13234c91b316bc3d82d432f9b589a9ef09d016875a31c670b76/websocket-client-1.5.1.tar.gz", hash = "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40"},
 ]
-"websockets 11.0.2" = [
-    {url = "https://files.pythonhosted.org/packages/07/55/1187816ffb02a5366839ec10069441188a4645c5f206c04ce702527adcb2/websockets-11.0.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:232b6ba974f5d09b1b747ac232f3a3d8f86de401d7b565e837cc86988edf37ac"},
-    {url = "https://files.pythonhosted.org/packages/0e/74/787fce70aae0fd9ff90bf77432039d1939438a125773156cf0324715c591/websockets-11.0.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:3ffe251a31f37e65b9b9aca5d2d67fd091c234e530f13d9dce4a67959d5a3fba"},
-    {url = "https://files.pythonhosted.org/packages/14/ca/87f36bc5758c1ca28494914f2c13942755a841cc481583356663cd5f11d4/websockets-11.0.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e37a76ccd483a6457580077d43bc3dfe1fd784ecb2151fcb9d1c73f424deaeba"},
-    {url = "https://files.pythonhosted.org/packages/19/69/b7fd42aa6f119828c13a578c4be861d2ee37d6c6142481b4c293a8a96ab5/websockets-11.0.2-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2acdc82099999e44fa7bd8c886f03c70a22b1d53ae74252f389be30d64fd6004"},
-    {url = "https://files.pythonhosted.org/packages/1a/7f/6d62388722b39ecf990e7d17559f22258d477a0348abe78dd85094f8b8b4/websockets-11.0.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7742cd4524622cc7aa71734b51294644492a961243c4fe67874971c4d3045982"},
-    {url = "https://files.pythonhosted.org/packages/2a/02/1b5e07f6cc7db9165d5007eba59d08c1ace5e30b0b7fab23cd4ca3be991d/websockets-11.0.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:adf6385f677ed2e0b021845b36f55c43f171dab3a9ee0ace94da67302f1bc364"},
-    {url = "https://files.pythonhosted.org/packages/2e/8b/dab160db6ff385efe034ae4907893720b4a5f23fb282f124f5a375827b72/websockets-11.0.2-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:ce69f5c742eefd039dce8622e99d811ef2135b69d10f9aa79fbf2fdcc1e56cd7"},
-    {url = "https://files.pythonhosted.org/packages/30/cc/b119fab11fcd2f065ea0eb7cbf4fd1559187acdc7455baefebf4a79f11d9/websockets-11.0.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:87c69f50281126dcdaccd64d951fb57fbce272578d24efc59bce72cf264725d0"},
-    {url = "https://files.pythonhosted.org/packages/32/ff/03941fb1c875594b39ea1ca902b673517ff4f87b4ce7a58282f1159e5c7d/websockets-11.0.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:3a2100b02d1aaf66dc48ff1b2a72f34f6ebc575a02bc0350cc8e9fbb35940166"},
-    {url = "https://files.pythonhosted.org/packages/33/ed/d9dab6cbbc400d4e63acc6060f0bd2a8fa9e938b24d5a66f7847d1f19403/websockets-11.0.2-cp37-cp37m-win32.whl", hash = "sha256:5875f623a10b9ba154cb61967f940ab469039f0b5e61c80dd153a65f024d9fb7"},
-    {url = "https://files.pythonhosted.org/packages/37/3b/6765dbaf2f245b710519893e46e39f40b279072664cc2e65f9915fcf02b6/websockets-11.0.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:2eb042734e710d39e9bc58deab23a65bd2750e161436101488f8af92f183c239"},
-    {url = "https://files.pythonhosted.org/packages/3b/c5/0c98276e1f4d1db4b82f61e91fc99451fa7e303add19b688fa07dd900620/websockets-11.0.2-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3e79065ff6549dd3c765e7916067e12a9c91df2affea0ac51bcd302aaf7ad207"},
-    {url = "https://files.pythonhosted.org/packages/3b/ed/14377de838c057ee35f4bdac3f470c48b70982c5cdbc6d00cec5c3fbb18d/websockets-11.0.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ede13a6998ba2568b21825809d96e69a38dc43184bdeebbde3699c8baa21d015"},
-    {url = "https://files.pythonhosted.org/packages/3b/f4/47c57f2c91fc45b04f892208cb33d499002abdb1f539918769d5681c6406/websockets-11.0.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:95c09427c1c57206fe04277bf871b396476d5a8857fa1b99703283ee497c7a5d"},
-    {url = "https://files.pythonhosted.org/packages/3d/29/9ac6cfd99afdd3ba2c836e4d683ced7ade3cd1a286a026f4740eea931707/websockets-11.0.2-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:752fbf420c71416fb1472fec1b4cb8631c1aa2be7149e0a5ba7e5771d75d2bb9"},
-    {url = "https://files.pythonhosted.org/packages/41/51/582b3d67979cae83a3015f6551f83587e222854515e3c6b0f091a58d777e/websockets-11.0.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ca9b2dced5cbbc5094678cc1ec62160f7b0fe4defd601cd28a36fde7ee71bbb5"},
-    {url = "https://files.pythonhosted.org/packages/42/c0/f5fa70aae7a6983f35380cff5843b18fbb20077558aeaf34be845e0529a9/websockets-11.0.2-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:b444366b605d2885f0034dd889faf91b4b47668dd125591e2c64bfde611ac7e1"},
-    {url = "https://files.pythonhosted.org/packages/42/e8/65d921f856ac3bb0e5aa3382b58d9016cdd8a97355045ac758bbed3e3469/websockets-11.0.2-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d6b2bfa1d884c254b841b0ff79373b6b80779088df6704f034858e4d705a4802"},
-    {url = "https://files.pythonhosted.org/packages/44/8b/1186b15bd47078fb57f3354000c37eb3d7af90e2813d696b54cb95025f74/websockets-11.0.2-cp310-cp310-win_amd64.whl", hash = "sha256:3b87cd302f08ea9e74fdc080470eddbed1e165113c1823fb3ee6328bc40ca1d3"},
-    {url = "https://files.pythonhosted.org/packages/49/16/5cb977c3184f56f9bb5b269654374e150c88df15b5ca611d7211ec9add09/websockets-11.0.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:3565a8f8c7bdde7c29ebe46146bd191290413ee6f8e94cf350609720c075b0a1"},
-    {url = "https://files.pythonhosted.org/packages/4a/81/2e080177189909fc8361f288154068f93d0e966be39b89426b4c89a50295/websockets-11.0.2-cp311-cp311-win32.whl", hash = "sha256:2174a75d579d811279855df5824676d851a69f52852edb0e7551e0eeac6f59a4"},
-    {url = "https://files.pythonhosted.org/packages/4b/00/862efcce079d2ca56c7a6ec8c829f232000566b40305dc962d49f3250e6c/websockets-11.0.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:320ddceefd2364d4afe6576195201a3632a6f2e6d207b0c01333e965b22dbc84"},
-    {url = "https://files.pythonhosted.org/packages/4b/84/a1d7881bf310dd19d72108e7d503644e1b0d6088a60decb7fab92bbccf16/websockets-11.0.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:cb46d2c7631b2e6f10f7c8bac7854f7c5e5288f024f1c137d4633c79ead1e3c0"},
-    {url = "https://files.pythonhosted.org/packages/50/52/0e7e12f35035f031f0e0a7eff80b605d6b5e651f8254f3c0a73fab580a58/websockets-11.0.2-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d70a438ef2a22a581d65ad7648e949d4ccd20e3c8ed7a90bbc46df4e60320891"},
-    {url = "https://files.pythonhosted.org/packages/50/8d/5d8f0d54f759845cd630943b3de062f4e7ea0fdd83e1372e380170848286/websockets-11.0.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:cf45d273202b0c1cec0f03a7972c655b93611f2e996669667414557230a87b88"},
-    {url = "https://files.pythonhosted.org/packages/54/d7/b194887d5a56aa819da5081b82d0224e119f460424d6082f076a3c9a7945/websockets-11.0.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:25aae96c1060e85836552a113495db6d857400288161299d77b7b20f2ac569f2"},
-    {url = "https://files.pythonhosted.org/packages/59/ca/cbde2c49cc95675a37914fe54d0e4ba7d3d3e99b6cb0aae36a6eef4e2607/websockets-11.0.2-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:46388a050d9e40316e58a3f0838c63caacb72f94129eb621a659a6e49bad27ce"},
-    {url = "https://files.pythonhosted.org/packages/6b/70/56e924042d71d35bb4e5da9f80526679023fb324380c21ae5c6510531dd8/websockets-11.0.2-cp37-cp37m-win_amd64.whl", hash = "sha256:634239bc844131863762865b75211a913c536817c0da27f691400d49d256df1d"},
-    {url = "https://files.pythonhosted.org/packages/74/4b/cc47a4df634b1d8dcb0a8e2ff69888e52e2bf848fecb8ccb8fb2669d4009/websockets-11.0.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:1df2413266bf48430ef2a752c49b93086c6bf192d708e4a9920544c74cd2baa6"},
-    {url = "https://files.pythonhosted.org/packages/75/3b/c0a17f1e5c453708f6b60095f34dc7f7362ca264c09ad406cc6446eee233/websockets-11.0.2-cp311-cp311-win_amd64.whl", hash = "sha256:c78ca3037a954a4209b9f900e0eabbc471fb4ebe96914016281df2c974a93e3e"},
-    {url = "https://files.pythonhosted.org/packages/75/bf/eb54d8ff54a13fc788599f0cbc12ad2d6a23c11e6f813f0677f8008a3f8a/websockets-11.0.2-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:dd906b0cdc417ea7a5f13bb3c6ca3b5fd563338dc596996cb0fdd7872d691c0a"},
-    {url = "https://files.pythonhosted.org/packages/77/2e/821acedf0717f36e2b9ae6f8ba76c3c4389bd0bf823cc9b730bdf5970bcf/websockets-11.0.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:0fb4480556825e4e6bf2eebdbeb130d9474c62705100c90e59f2f56459ddab42"},
-    {url = "https://files.pythonhosted.org/packages/79/f9/5ddb516bab32607763ce06291adf33d0a8845f03b5a84af3e3dd479540fe/websockets-11.0.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:3a09cce3dacb6ad638fdfa3154d9e54a98efe7c8f68f000e55ca9c716496ca67"},
-    {url = "https://files.pythonhosted.org/packages/7b/51/d5c9c4f7028274199bff159ef31ce4edd7738de1869fd27187c563ddbbfe/websockets-11.0.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:d3cc3e48b6c9f7df8c3798004b9c4b92abca09eeea5e1b0a39698f05b7a33b9d"},
-    {url = "https://files.pythonhosted.org/packages/7c/92/48c9e2b0a8de05bba6823ca14bd58b581f2158fbce38a8ca8dccacf4eccb/websockets-11.0.2-pp37-pypy37_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1b52def56d2a26e0e9c464f90cadb7e628e04f67b0ff3a76a4d9a18dfc35e3dd"},
-    {url = "https://files.pythonhosted.org/packages/7d/43/a0a37ccc9fd16686d8dbde253516e9a3ccd699619d7a7b4a10925bdc022d/websockets-11.0.2-cp39-cp39-win32.whl", hash = "sha256:d1881518b488a920434a271a6e8a5c9481a67c4f6352ebbdd249b789c0467ddc"},
-    {url = "https://files.pythonhosted.org/packages/7f/63/58a365e9f610fc02bc32ab5fb5ab88869d5d52dbec61efcdee8d36a8c6f3/websockets-11.0.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:58477b041099bb504e1a5ddd8aa86302ed1d5c6995bdd3db2b3084ef0135d277"},
-    {url = "https://files.pythonhosted.org/packages/81/ca/2ce8945870f08c0d856b55e6bc812551130189de27a971902e7b9528b5df/websockets-11.0.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:4c54086b2d2aec3c3cb887ad97e9c02c6be9f1d48381c7419a4aa932d31661e4"},
-    {url = "https://files.pythonhosted.org/packages/82/1a/1e3a9a94451e104748304598ceca69e68b9a3db3dcc026cea47d5968dd4d/websockets-11.0.2-cp39-cp39-win_amd64.whl", hash = "sha256:25e265686ea385f22a00cc2b719b880797cd1bb53b46dbde969e554fb458bfde"},
-    {url = "https://files.pythonhosted.org/packages/83/8f/9a1c3e8e805053619f21c6cb15ddbc7876bf883a28fa99503fa58b4a8405/websockets-11.0.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dca9708eea9f9ed300394d4775beb2667288e998eb6f542cdb6c02027430c599"},
-    {url = "https://files.pythonhosted.org/packages/8c/2e/2ff028546cb1e5dcf2c3161c953406c781f30450eee087b9b831015ae39a/websockets-11.0.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8f392587eb2767afa8a34e909f2fec779f90b630622adc95d8b5e26ea8823cb8"},
-    {url = "https://files.pythonhosted.org/packages/8c/62/1c966e6feed8c89faa79714ed3053fa0afd1b106bf0c44156c833f28c36a/websockets-11.0.2-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a4fe2442091ff71dee0769a10449420fd5d3b606c590f78dd2b97d94b7455640"},
-    {url = "https://files.pythonhosted.org/packages/91/bc/0c09be051a99b1ecae063d7f03da33546610158dca6d55b4ab508ba7fedf/websockets-11.0.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:34a6f8996964ccaa40da42ee36aa1572adcb1e213665e24aa2f1037da6080909"},
-    {url = "https://files.pythonhosted.org/packages/96/42/ff89b6738393fc4ddf4ee0c4feedb68cd5ee834e89c52ec1916eb93b55e7/websockets-11.0.2-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b985ba2b9e972cf99ddffc07df1a314b893095f62c75bc7c5354a9c4647c6503"},
-    {url = "https://files.pythonhosted.org/packages/98/93/bcf5ee63aad37e4a7b675eae39d55411611274fd4891e2c920cea9a3ff55/websockets-11.0.2-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e8b967a4849db6b567dec3f7dd5d97b15ce653e3497b8ce0814e470d5e074750"},
-    {url = "https://files.pythonhosted.org/packages/9c/c8/fbd583360155c9869750558c6408714b92fb5695a56772f493ed78408c5c/websockets-11.0.2-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:6d872c972c87c393e6a49c1afbdc596432df8c06d0ff7cd05aa18e885e7cfb7c"},
-    {url = "https://files.pythonhosted.org/packages/9d/67/68e568bb4a0617529db2723c75958223b70b95921cd114b5fd13567db4d8/websockets-11.0.2.tar.gz", hash = "sha256:b1a69701eb98ed83dd099de4a686dc892c413d974fa31602bc00aca7cb988ac9"},
-    {url = "https://files.pythonhosted.org/packages/9e/78/edb34f8c1fae5427d6fc44f85c0f70daa1082bccc88178ba2e656c9151d2/websockets-11.0.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:808b8a33c961bbd6d33c55908f7c137569b09ea7dd024bce969969aa04ecf07c"},
-    {url = "https://files.pythonhosted.org/packages/a2/bd/d20b428950e6965bb6e0489c7e5508e6791b8989d1b9f84047765c28c213/websockets-11.0.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:954eb789c960fa5daaed3cfe336abc066941a5d456ff6be8f0e03dd89886bb4c"},
-    {url = "https://files.pythonhosted.org/packages/a7/10/971a38996b8044209f527a01563accb479e7f52bd6e2b77a55c31cf8423f/websockets-11.0.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:392d409178db1e46d1055e51cc850136d302434e12d412a555e5291ab810f622"},
-    {url = "https://files.pythonhosted.org/packages/aa/80/ec21babff00cc5cb27c10a99e4c03b670a9e27f26439091f979fee74538a/websockets-11.0.2-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:3178d965ec204773ab67985a09f5696ca6c3869afeed0bb51703ea404a24e975"},
-    {url = "https://files.pythonhosted.org/packages/ac/3c/e5b6ea6b8b0b238d8d66a6d0ed32b466b40d8e417af73a4091db10ed1beb/websockets-11.0.2-cp310-cp310-win32.whl", hash = "sha256:8f24cd758cbe1607a91b720537685b64e4d39415649cac9177cd1257317cf30c"},
-    {url = "https://files.pythonhosted.org/packages/b3/bd/65e44c75f0aa9b782bbfc11eded7f7f5b702b4e43c47d680006258136dac/websockets-11.0.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:ec00401846569aaf018700249996143f567d50050c5b7b650148989f956547af"},
-    {url = "https://files.pythonhosted.org/packages/b6/fa/96b64fea54542630a7c79e784f7514228b91138720858c820e3bc157e43b/websockets-11.0.2-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:502683c5dedfc94b9f0f6790efb26aa0591526e8403ad443dce922cd6c0ec83b"},
-    {url = "https://files.pythonhosted.org/packages/ba/d2/cc7369f01a294005b86cecb103ce0e57ed976783161bf93caa7d54b9558f/websockets-11.0.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:580cc95c58118f8c39106be71e24d0b7e1ad11a155f40a2ee687f99b3e5e432e"},
-    {url = "https://files.pythonhosted.org/packages/be/ef/618a403b112a66058dedab15ab4167f13a414943c244540cb470ba375507/websockets-11.0.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8df63dcd955eb6b2e371d95aacf8b7c535e482192cff1b6ce927d8f43fb4f552"},
-    {url = "https://files.pythonhosted.org/packages/c1/a9/17672f611f8955dad4345a56438b0dc710f9be75ca47957779ee6b2f14f7/websockets-11.0.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:955fcdb304833df2e172ce2492b7b47b4aab5dcc035a10e093d911a1916f2c87"},
-    {url = "https://files.pythonhosted.org/packages/c3/91/08c0ee33324f2648dcb9d96bd8c78cbbc20e5d7770917cc5176ba9663ea3/websockets-11.0.2-pp38-pypy38_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5c7de298371d913824f71b30f7685bb07ad13969c79679cca5b1f7f94fec012f"},
-    {url = "https://files.pythonhosted.org/packages/c3/9b/8aeb56224cf2933d2c1a178cd422ada37f74d0cda542f373183769953611/websockets-11.0.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:f97e03d4d5a4f0dca739ea274be9092822f7430b77d25aa02da6775e490f6846"},
-    {url = "https://files.pythonhosted.org/packages/ce/f4/698cf3587d4e2c469bb0fb79395bbbb6f35b6f8714da7e72dff94f7b6356/websockets-11.0.2-cp38-cp38-win_amd64.whl", hash = "sha256:220d5b93764dd70d7617f1663da64256df7e7ea31fc66bc52c0e3750ee134ae3"},
-    {url = "https://files.pythonhosted.org/packages/d0/5b/713dc7ca860e3a5bebff1204176cabbcca46747120e5fb59d13d8daad121/websockets-11.0.2-cp38-cp38-win32.whl", hash = "sha256:aa7b33c1fb2f7b7b9820f93a5d61ffd47f5a91711bc5fa4583bbe0c0601ec0b2"},
-    {url = "https://files.pythonhosted.org/packages/d8/73/0de2391aa2fdc833032bfef415adf90193177263e9436f3c06fbbbadebe0/websockets-11.0.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2abeeae63154b7f63d9f764685b2d299e9141171b8b896688bd8baec6b3e2303"},
-    {url = "https://files.pythonhosted.org/packages/dd/b7/ed3575a038d2d7b242fb8ced354c7dbcc8c8ea170b7cf33b62f31df7896c/websockets-11.0.2-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:daa1e8ea47507555ed7a34f8b49398d33dff5b8548eae3de1dc0ef0607273a33"},
-    {url = "https://files.pythonhosted.org/packages/df/25/3f044ffe1099fd9edf3c5b7ef1f98d8ef139f43582ca118dc903c980806e/websockets-11.0.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:46dda4bc2030c335abe192b94e98686615f9274f6b56f32f2dd661fb303d9d12"},
-    {url = "https://files.pythonhosted.org/packages/df/8f/064d879849112d09df9fd2a797668c011fbd33420d15e469435da903dc22/websockets-11.0.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e0eeeea3b01c97fd3b5049a46c908823f68b59bf0e18d79b231d8d6764bc81ee"},
-    {url = "https://files.pythonhosted.org/packages/e7/55/883b3d2fb2435d4d80cbe39237d0a1ad7f6014f05de21926e3b410a1eae6/websockets-11.0.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:13bd5bebcd16a4b5e403061b8b9dcc5c77e7a71e3c57e072d8dff23e33f70fba"},
-    {url = "https://files.pythonhosted.org/packages/ea/8a/32116db59137262378ba72a124e5ee28f78f8a3a621281cfbddb6a634b37/websockets-11.0.2-py3-none-any.whl", hash = "sha256:5004c087d17251938a52cce21b3dbdabeecbbe432ce3f5bbbf15d8692c36eac9"},
-    {url = "https://files.pythonhosted.org/packages/f0/61/c1a45650b8526b19f2aeb9f3e03532e493e6470bd99c4f67c66f5e20915b/websockets-11.0.2-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b2a573c8d71b7af937852b61e7ccb37151d719974146b5dc734aad350ef55a02"},
-    {url = "https://files.pythonhosted.org/packages/f8/cb/1178fe699508fc820eead75a8f1848dbc95acdd9fb2530b784db1e4a8f58/websockets-11.0.2-pp39-pypy39_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:518ed6782d9916c5721ebd61bb7651d244178b74399028302c8617d0620af291"},
-    {url = "https://files.pythonhosted.org/packages/f8/e9/885a685ddf6a4f9033b6254cb742e4f2f47acee10e5d068f0a7ea8592e52/websockets-11.0.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:143782041e95b63083b02107f31cda999f392903ae331de1307441f3a4557d51"},
-]
-"werkzeug 2.3.3" = [
-    {url = "https://files.pythonhosted.org/packages/52/82/bc77d22189679940b9f73685451167221ec5348e08c6d2594f1070767124/Werkzeug-2.3.3.tar.gz", hash = "sha256:a987caf1092edc7523edb139edb20c70571c4a8d5eed02e0b547b4739174d091"},
-    {url = "https://files.pythonhosted.org/packages/d1/3d/2f818de3e6f693f215f1de41604ab8fad5c215b1b18eec70a2cc5900ff6c/Werkzeug-2.3.3-py3-none-any.whl", hash = "sha256:4866679a0722de00796a74086238bb3b98d90f423f05de039abb09315487254a"},
+"websockets 11.0.3" = [
+    {url = "https://files.pythonhosted.org/packages/03/28/3a51ffcf51ac45746639f83128908bbb1cd212aa631e42d15a7acebce5cb/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e052b8467dd07d4943936009f46ae5ce7b908ddcac3fda581656b1b19c083d9b"},
+    {url = "https://files.pythonhosted.org/packages/0a/84/68b848a373493b58615d6c10e9e8ccbaadfd540f84905421739a807704f8/websockets-11.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aa5003845cdd21ac0dc6c9bf661c5beddd01116f6eb9eb3c8e272353d45b3288"},
+    {url = "https://files.pythonhosted.org/packages/0f/d8/a997d3546aef9cc995a1126f7d7ade96c0e16c1a0efb9d2d430aee57c925/websockets-11.0.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:619d9f06372b3a42bc29d0cd0354c9bb9fb39c2cbc1a9c5025b4538738dbffaf"},
+    {url = "https://files.pythonhosted.org/packages/14/fc/5cbbf439c925e1e184a0392ec477a30cee2fabc0e63807c1d4b6d570fb52/websockets-11.0.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:b30c6590146e53149f04e85a6e4fcae068df4289e31e4aee1fdf56a0dead8f97"},
+    {url = "https://files.pythonhosted.org/packages/16/49/ae616bd221efba84a3d78737b417f704af1ffa36f40dcaba5eb954dd4753/websockets-11.0.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e848f46a58b9fcf3d06061d17be388caf70ea5b8cc3466251963c8345e13f7eb"},
+    {url = "https://files.pythonhosted.org/packages/19/d3/2ea3f95d83033675144b0848a0ae2e4998b3f763da09ec3df6bce97ea4e6/websockets-11.0.3-cp37-cp37m-win32.whl", hash = "sha256:e590228200fcfc7e9109509e4d9125eace2042fd52b595dd22bbc34bb282307f"},
+    {url = "https://files.pythonhosted.org/packages/1b/3d/3dc77699fa4d003f2e810c321592f80f62b81d7b78483509de72ffe581fd/websockets-11.0.3-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:0ee68fe502f9031f19d495dae2c268830df2760c0524cbac5d759921ba8c8e82"},
+    {url = "https://files.pythonhosted.org/packages/20/62/5c6039c4069912adb27889ddd000403a2de9e0fe6aebe439b4e6b128a6b8/websockets-11.0.3-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:e6316827e3e79b7b8e7d8e3b08f4e331af91a48e794d5d8b099928b6f0b85f20"},
+    {url = "https://files.pythonhosted.org/packages/25/25/48540419005d07ed2d368a7eafb44ed4f33a2691ae4c210850bf31123c4a/websockets-11.0.3-cp38-cp38-win_amd64.whl", hash = "sha256:03aae4edc0b1c68498f41a6772d80ac7c1e33c06c6ffa2ac1c27a07653e79d6f"},
+    {url = "https://files.pythonhosted.org/packages/27/e9/605b0618d0864e9be7c2a78f22bff57aba9cf56b9fccde3205db9023ae22/websockets-11.0.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:92b2065d642bf8c0a82d59e59053dd2fdde64d4ed44efe4870fa816c1232647b"},
+    {url = "https://files.pythonhosted.org/packages/30/a5/d641f2a9a4b4079cfddbb0726fc1b914be76a610aaedb45e4760899a4ce1/websockets-11.0.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:bee9fcb41db2a23bed96c6b6ead6489702c12334ea20a297aa095ce6d31370d0"},
+    {url = "https://files.pythonhosted.org/packages/32/2c/ab8ea64e9a7d8bf62a7ea7a037fb8d328d8bd46dbfe083787a9d452a148e/websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b67c6f5e5a401fc56394f191f00f9b3811fe843ee93f4a70df3c389d1adf857d"},
+    {url = "https://files.pythonhosted.org/packages/36/19/0da435afb26a6c47c0c045a82e414912aa2ac10de5721276a342bd9fdfee/websockets-11.0.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:332d126167ddddec94597c2365537baf9ff62dfcc9db4266f263d455f2f031cb"},
+    {url = "https://files.pythonhosted.org/packages/38/30/01a10fbf4cc1e7ffa07be9b0401501918fc9433d71fb7da4cfcef3bd26ca/websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8531fdcad636d82c517b26a448dcfe62f720e1922b33c81ce695d0edb91eb931"},
+    {url = "https://files.pythonhosted.org/packages/38/ed/b8b133416536b6816e480594864e5950051db522714623eefc9e5275ec04/websockets-11.0.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:6505c1b31274723ccaf5f515c1824a4ad2f0d191cec942666b3d0f3aa4cb4007"},
+    {url = "https://files.pythonhosted.org/packages/44/a8/66c3a66b70b01a6c55fde486298766177fa11dd0d3a2c1cfc6820f25b4dc/websockets-11.0.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2529338a6ff0eb0b50c7be33dc3d0e456381157a31eefc561771ee431134a97f"},
+    {url = "https://files.pythonhosted.org/packages/47/96/9d5749106ff57629b54360664ae7eb9afd8302fad1680ead385383e33746/websockets-11.0.3-py3-none-any.whl", hash = "sha256:6681ba9e7f8f3b19440921e99efbb40fc89f26cd71bf539e45d8c8a25c976dc6"},
+    {url = "https://files.pythonhosted.org/packages/58/05/2efb520317340ece74bfc4d88e8f011dd71a4e6c263000bfffb71a343685/websockets-11.0.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e1a99a7a71631f0efe727c10edfba09ea6bee4166a6f9c19aafb6c0b5917d09c"},
+    {url = "https://files.pythonhosted.org/packages/58/0a/7570e15661a0a546c3a1152d95fe8c05480459bab36247f0acbf41f01a41/websockets-11.0.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bceab846bac555aff6427d060f2fcfff71042dba6f5fca7dc4f75cac815e57ca"},
+    {url = "https://files.pythonhosted.org/packages/58/68/9403771de1b1c21a2e878e4841815af8c9f8893b094654934e2a5ee4dbc8/websockets-11.0.3-cp38-cp38-win32.whl", hash = "sha256:f61bdb1df43dc9c131791fbc2355535f9024b9a04398d3bd0684fc16ab07df74"},
+    {url = "https://files.pythonhosted.org/packages/66/89/799f595c67b97a8a17e13d2764e088f631616bd95668aaa4c04b7cada136/websockets-11.0.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:df41b9bc27c2c25b486bae7cf42fccdc52ff181c8c387bfd026624a491c2671b"},
+    {url = "https://files.pythonhosted.org/packages/6b/ca/65d6986665888494eca4d5435a9741c822022996f0f4200c57ce4b9242f7/websockets-11.0.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:660e2d9068d2bedc0912af508f30bbeb505bbbf9774d98def45f68278cea20d3"},
+    {url = "https://files.pythonhosted.org/packages/70/fc/71377f36ef3049f3bc7db7c0f3a7696929d5f836d7a18777131d994192a9/websockets-11.0.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:34fd59a4ac42dff6d4681d8843217137f6bc85ed29722f2f7222bd619d15e95b"},
+    {url = "https://files.pythonhosted.org/packages/72/89/0d150939f2e592ed78c071d69237ac1c872462cc62a750c5f592f3d4ab18/websockets-11.0.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:97b52894d948d2f6ea480171a27122d77af14ced35f62e5c892ca2fae9344311"},
+    {url = "https://files.pythonhosted.org/packages/78/b2/df5452031b02b857851139806308f2af7c749069e25bfe15f2d559ade6e7/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0ac56b661e60edd453585f4bd68eb6a29ae25b5184fd5ba51e97652580458998"},
+    {url = "https://files.pythonhosted.org/packages/82/3c/00f051abcf88aec5e952a8840076749b0b26a30c219dcae8ba70200998aa/websockets-11.0.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:86d2a77fd490ae3ff6fae1c6ceaecad063d3cc2320b44377efdde79880e11526"},
+    {url = "https://files.pythonhosted.org/packages/89/8f/707a05d5725f956c78d252a5fd73b89fa3ac57dd3959381c2d1acb41cb13/websockets-11.0.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:01f5567d9cf6f502d655151645d4e8b72b453413d3819d2b6f1185abc23e82dd"},
+    {url = "https://files.pythonhosted.org/packages/8a/77/a04d2911f6e2b9e781ce7ffc1e8516b54b85f985369eec8c853fd619d8e8/websockets-11.0.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:69269f3a0b472e91125b503d3c0b3566bda26da0a3261c49f0027eb6075086d1"},
+    {url = "https://files.pythonhosted.org/packages/8a/bd/a5e5973899d78d44a540f50a9e30b01c6771e8bf7883204ee762060cf95a/websockets-11.0.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4841ed00f1026dfbced6fca7d963c4e7043aa832648671b5138008dc5a8f6d99"},
+    {url = "https://files.pythonhosted.org/packages/8b/97/34178f5f7c29e679372d597cebfeff2aa45991d741d938117d4616e81a74/websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1d5023a4b6a5b183dc838808087033ec5df77580485fc533e7dab2567851b0a4"},
+    {url = "https://files.pythonhosted.org/packages/8c/a8/e81533499f84ef6cdd95d11d5b05fa827c0f097925afd86f16e6a2631d8e/websockets-11.0.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b58cbf0697721120866820b89f93659abc31c1e876bf20d0b3d03cef14faf84d"},
+    {url = "https://files.pythonhosted.org/packages/8f/7b/4d4ecd29be7d08486e38f987a6603c491296d1e33fe55127d79aebb0333e/websockets-11.0.3-cp310-cp310-win32.whl", hash = "sha256:2d903ad4419f5b472de90cd2d40384573b25da71e33519a67797de17ef849b69"},
+    {url = "https://files.pythonhosted.org/packages/8f/f2/8a3eb016be19743c7eb9e67c855df0fdfa5912534ffaf83a05b62667d761/websockets-11.0.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8c82f11964f010053e13daafdc7154ce7385ecc538989a354ccc7067fd7028fd"},
+    {url = "https://files.pythonhosted.org/packages/94/8c/266155c14b7a26deca6fa4c4d5fd15b0ab32725d78a2acfcf6b24943585d/websockets-11.0.3-cp37-cp37m-win_amd64.whl", hash = "sha256:b16fff62b45eccb9c7abb18e60e7e446998093cdcb50fed33134b9b6878836de"},
+    {url = "https://files.pythonhosted.org/packages/98/a7/0ed69892981351e5acf88fac0ff4c801fabca2c3bdef9fca4c7d3fde8c53/websockets-11.0.3-cp310-cp310-win_amd64.whl", hash = "sha256:1d2256283fa4b7f4c7d7d3e84dc2ece74d341bce57d5b9bf385df109c2a1a82f"},
+    {url = "https://files.pythonhosted.org/packages/99/23/43071c989c0f87f612e7bccee98d00b04bddd3aca0cdc1ffaf31f6f8a4b4/websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c114e8da9b475739dde229fd3bc6b05a6537a88a578358bc8eb29b4030fac9c9"},
+    {url = "https://files.pythonhosted.org/packages/9a/6e/0fd7274042f46acb589161407f4b505b44c68d369437ce919bae1fa9b8c4/websockets-11.0.3-cp39-cp39-win32.whl", hash = "sha256:c7f3cb904cce8e1be667c7e6fef4516b98d1a6a0635a58a57528d577ac18a128"},
+    {url = "https://files.pythonhosted.org/packages/a0/1a/3da73e69ebc00649d11ed836541c92c1a2df0b8a8aa641a2c8746e7c2b9c/websockets-11.0.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3580dd9c1ad0701169e4d6fc41e878ffe05e6bdcaf3c412f9d559389d0c9e016"},
+    {url = "https://files.pythonhosted.org/packages/a0/39/acc3d4b15c5207ef7cca823c37eca8c74e3e1a1a63a397798986be3bdef7/websockets-11.0.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:68b977f21ce443d6d378dbd5ca38621755f2063d6fdb3335bda981d552cfff86"},
+    {url = "https://files.pythonhosted.org/packages/a6/1b/5c83c40f8d3efaf0bb2fdf05af94fb920f74842b7aaf31d7598e3ee44d58/websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dcacf2c7a6c3a84e720d1bb2b543c675bf6c40e460300b628bab1b1efc7c034c"},
+    {url = "https://files.pythonhosted.org/packages/a6/9c/2356ecb952fd3992b73f7a897d65e57d784a69b94bb8d8fd5f97531e5c02/websockets-11.0.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:279e5de4671e79a9ac877427f4ac4ce93751b8823f276b681d04b2156713b9dd"},
+    {url = "https://files.pythonhosted.org/packages/a7/8c/7100e9cf310fe1d83d1ae1322203f4eb2b767a7c2b301c1e70db6270306f/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:de36fe9c02995c7e6ae6efe2e205816f5f00c22fd1fbf343d4d18c3d5ceac2f5"},
+    {url = "https://files.pythonhosted.org/packages/a7/f7/1e852351e8073c32885172a6bef64c95d14c13ff3634b01d4a1086321491/websockets-11.0.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:9d9acd80072abcc98bd2c86c3c9cd4ac2347b5a5a0cae7ed5c0ee5675f86d9af"},
+    {url = "https://files.pythonhosted.org/packages/a9/5e/b25c60067d700e811dccb4e3c318eeadd3a19d8b3620de9f97434af777a7/websockets-11.0.3-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:def07915168ac8f7853812cc593c71185a16216e9e4fa886358a17ed0fd9fcf6"},
+    {url = "https://files.pythonhosted.org/packages/b2/ec/56bdd12d847e4fc2d0a7ba2d7f1476f79cda50599d11ffb6080b86f21ef1/websockets-11.0.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ffd7dcaf744f25f82190856bc26ed81721508fc5cbf2a330751e135ff1283564"},
+    {url = "https://files.pythonhosted.org/packages/b5/94/ac47552208583d5dbcce468430c1eb2ae18962f6b3a694a2b7727cc60d4a/websockets-11.0.3-cp311-cp311-win32.whl", hash = "sha256:e1459677e5d12be8bbc7584c35b992eea142911a6236a3278b9b5ce3326f282c"},
+    {url = "https://files.pythonhosted.org/packages/b5/a8/8900184ab0b06b6e620ba7e92cf2faa5caa9ba86e148541b8fff1c7b6646/websockets-11.0.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:9f59a3c656fef341a99e3d63189852be7084c0e54b75734cde571182c087b152"},
+    {url = "https://files.pythonhosted.org/packages/b6/96/0d586c25d043aeab9457dad8e407251e3baf314d871215f91847e7b995c4/websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e063b1865974611313a3849d43f2c3f5368093691349cf3c7c8f8f75ad7cb280"},
+    {url = "https://files.pythonhosted.org/packages/b9/6b/26b28115b46e23e74ede76d95792eedfe8c58b21f4daabfff1e9f159c8fe/websockets-11.0.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d67ac60a307f760c6e65dad586f556dde58e683fab03323221a4e530ead6f74d"},
+    {url = "https://files.pythonhosted.org/packages/ba/6c/5c0322b2875e8395e6bf0eff11f43f3e25da7ef5b12f4d908cd3a19ea841/websockets-11.0.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:54c6e5b3d3a8936a4ab6870d46bdd6ec500ad62bde9e44462c32d18f1e9a8e54"},
+    {url = "https://files.pythonhosted.org/packages/c0/21/cb9dfbbea8dc0ad89ced52630e7e61edb425fb9fdc6002f8d0c5dd26b94b/websockets-11.0.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:777354ee16f02f643a4c7f2b3eff8027a33c9861edc691a2003531f5da4f6bc8"},
+    {url = "https://files.pythonhosted.org/packages/c0/a8/a8a582ebeeecc8b5f332997d44c57e241748f8a9856e06a38a5a13b30796/websockets-11.0.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c1f0524f203e3bd35149f12157438f406eff2e4fb30f71221c8a5eceb3617b6b"},
+    {url = "https://files.pythonhosted.org/packages/c4/5b/60eccd7e9703bbe93fc4167d1e7ada7e8e8e51544122198d63fd8e3460b7/websockets-11.0.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:fb06eea71a00a7af0ae6aefbb932fb8a7df3cb390cc217d51a9ad7343de1b8d0"},
+    {url = "https://files.pythonhosted.org/packages/c4/f5/15998b164c183af0513bba744b51ecb08d396ff86c0db3b55d62624d1f15/websockets-11.0.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:1fdf26fa8a6a592f8f9235285b8affa72748dc12e964a5518c6c5e8f916716f7"},
+    {url = "https://files.pythonhosted.org/packages/c6/91/f36454b87edf10a95be9c7212d2dcb8c606ddbf7a183afdc498933acdd19/websockets-11.0.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:1553cb82942b2a74dd9b15a018dce645d4e68674de2ca31ff13ebc2d9f283788"},
+    {url = "https://files.pythonhosted.org/packages/c9/fb/ae5ed4be3514287cf8f6c348c87e1392a6e3f4d6eadae75c18847a2f84b6/websockets-11.0.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7622a89d696fc87af8e8d280d9b421db5133ef5b29d3f7a1ce9f1a7bf7fcfa11"},
+    {url = "https://files.pythonhosted.org/packages/ca/20/25211be61d50189650fb0ec6084b6d6339f5c7c6436a6c217608dcb553e4/websockets-11.0.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:4b253869ea05a5a073ebfdcb5cb3b0266a57c3764cf6fe114e4cd90f4bfa5f5e"},
+    {url = "https://files.pythonhosted.org/packages/d1/ec/7e2b9bebc2e9b4a48404144106bbc6a7ace781feeb0e6a3829551e725fa5/websockets-11.0.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8a34e13a62a59c871064dfd8ffb150867e54291e46d4a7cf11d02c94a5275bae"},
+    {url = "https://files.pythonhosted.org/packages/d8/3b/2ed38e52eed4cf277f9df5f0463a99199a04d9e29c9e227cfafa57bd3993/websockets-11.0.3.tar.gz", hash = "sha256:88fc51d9a26b10fc331be344f1781224a375b78488fc343620184e95a4b27016"},
+    {url = "https://files.pythonhosted.org/packages/d9/36/5741e62ccf629c8e38cc20f930491f8a33ce7dba972cae93dba3d6f02552/websockets-11.0.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6f1a3f10f836fab6ca6efa97bb952300b20ae56b409414ca85bff2ad241d2a61"},
+    {url = "https://files.pythonhosted.org/packages/de/0e/d7274e4d41d7b34f204744c27a23707be2ecefaf6f7df2145655f086ecd7/websockets-11.0.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:41f696ba95cd92dc047e46b41b26dd24518384749ed0d99bea0a941ca87404c4"},
+    {url = "https://files.pythonhosted.org/packages/e1/76/88640f8aeac7eb0d058b913e7bb72682f8d569db44c7d30e576ec4777ce1/websockets-11.0.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:3ccc8a0c387629aec40f2fc9fdcb4b9d5431954f934da3eaf16cdc94f67dbfac"},
+    {url = "https://files.pythonhosted.org/packages/e1/7c/0ad6e7ef0a054d73092f616d20d3d9bd3e1b837554cb20a52d8dd9f5b049/websockets-11.0.3-cp311-cp311-win_amd64.whl", hash = "sha256:e7837cb169eca3b3ae94cc5787c4fed99eef74c0ab9506756eea335e0d6f3ed8"},
+    {url = "https://files.pythonhosted.org/packages/e2/2f/3ad8ac4a9dc9d685e098e534180a36ed68fe2e85e82e225e00daec86bb94/websockets-11.0.3-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:f2e58f2c36cc52d41f2659e4c0cbf7353e28c8c9e63e30d8c6d3494dc9fdedcf"},
+    {url = "https://files.pythonhosted.org/packages/e9/26/1dfaa81788f61c485b4d65f1b28a19615e39f9c45100dce5e2cbf5ad1352/websockets-11.0.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:f467ba0050b7de85016b43f5a22b46383ef004c4f672148a8abf32bc999a87f0"},
+    {url = "https://files.pythonhosted.org/packages/eb/fb/2af7fc3ce2c3f1378d48a15802b4ff2caf6c0dfac13291e73c557caf04f7/websockets-11.0.3-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:42cc5452a54a8e46a032521d7365da775823e21bfba2895fb7b77633cce031bb"},
+    {url = "https://files.pythonhosted.org/packages/ec/3f/0c5cae14e9e86401105833383405787ae4caddd476a8fc5561259253dab7/websockets-11.0.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1a073fc9ab1c8aff37c99f11f1641e16da517770e31a37265d2755282a5d28aa"},
+    {url = "https://files.pythonhosted.org/packages/ed/45/466944e00b324ae3a1fddb305b4abf641f582e131548f07bcd970971b154/websockets-11.0.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:ed058398f55163a79bb9f06a90ef9ccc063b204bb346c4de78efc5d15abfe602"},
+    {url = "https://files.pythonhosted.org/packages/f3/82/2d1f3395d47fab65fa8b801e2251b324300ed8db54753b6fb7919cef0c11/websockets-11.0.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:84d27a4832cc1a0ee07cdcf2b0629a8a72db73f4cf6de6f0904f6661227f256f"},
+    {url = "https://files.pythonhosted.org/packages/f4/3f/65dfa50084a06ab0a05f3ca74195c2c17a1c075b8361327d831ccce0a483/websockets-11.0.3-cp39-cp39-win_amd64.whl", hash = "sha256:c792ea4eabc0159535608fc5658a74d1a81020eb35195dd63214dcf07556f67e"},
+]
+"werkzeug 2.3.4" = [
+    {url = "https://files.pythonhosted.org/packages/2d/bf/5a00bb4a70028f7c6000bc9394492154fa9ae3f5226187e3ddcd0aa5eca1/Werkzeug-2.3.4.tar.gz", hash = "sha256:1d5a58e0377d1fe39d061a5de4469e414e78ccb1e1e59c0f5ad6fa1c36c52b76"},
+    {url = "https://files.pythonhosted.org/packages/c2/2f/f0dc628295bd23571c962d5a349307d9c8796a05bfca6571659eaded38e2/Werkzeug-2.3.4-py3-none-any.whl", hash = "sha256:48e5e61472fee0ddee27ebad085614ebedb7af41e88f687aaf881afb723a162f"},
 ]
 "wheel 0.40.0" = [
     {url = "https://files.pythonhosted.org/packages/61/86/cc8d1ff2ca31a312a25a708c891cf9facbad4eae493b3872638db6785eb5/wheel-0.40.0-py3-none-any.whl", hash = "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"},
     {url = "https://files.pythonhosted.org/packages/fc/ef/0335f7217dd1e8096a9e8383e1d472aa14717878ffe07c4772e68b6e8735/wheel-0.40.0.tar.gz", hash = "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873"},
 ]
 "xlrd 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/aa/05/ec9d4fcbbb74bbf4da9f622b3b61aec541e4eccf31d3c60c5422ec027ce2/xlrd-1.2.0.tar.gz", hash = "sha256:546eb36cee8db40c3eaa46c351e67ffee6eeb5fa2650b71bc4c758a29a1b29b2"},
```

### Comparing `xklb-1.26.27/readme.py` & `xklb-1.26.28/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.28/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.28/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/.github/workflows/push.yaml` & `xklb-1.26.28/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/sql/transfer.sql` & `xklb-1.26.28/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/av.py` & `xklb-1.26.28/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/books.py` & `xklb-1.26.28/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/consts.py` & `xklb-1.26.28/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/db.py` & `xklb-1.26.28/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/dl_config.py` & `xklb-1.26.28/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/dl_extract.py` & `xklb-1.26.28/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/fs_extract.py` & `xklb-1.26.28/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/gui.py` & `xklb-1.26.28/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/hn_extract.py` & `xklb-1.26.28/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/lb.py` & `xklb-1.26.28/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/play_actions.py` & `xklb-1.26.28/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/playback.py` & `xklb-1.26.28/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/player.py` & `xklb-1.26.28/xklb/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,19 +284,19 @@
     local_media = [p.rstrip(os.sep) for p in playlists if not p.startswith("http")]
     for folder in local_media:
         with args.db.conn:
             args.db.conn.execute("delete from media where path like ?", (folder + "%",))
 
 
 class Action:
-    KEEP = "keep"
-    DELETE = "delete"
-    DELETE_IF_AUDIOBOOK = "delete_if_audiobook"
-    SOFTDELETE = "softdelete"
-    MOVE = "move"
+    KEEP = "KEEP"
+    DELETE = "DELETE"
+    DELETE_IF_AUDIOBOOK = "DELETE_IF_AUDIOBOOK"
+    SOFTDELETE = "SOFTDELETE"
+    MOVE = "MOVE"
 
 
 class AskAction:
     ASK_KEEP = (Action.KEEP, Action.DELETE)
     ASK_MOVE = (Action.MOVE, Action.KEEP)
     ASK_DELETE = (Action.DELETE, Action.KEEP)
     ASK_SOFTDELETE = (Action.SOFTDELETE, Action.KEEP)
@@ -330,27 +330,28 @@
                 false_action=false_action,
             )
         else:
             response = utils.confirm(true_action.title() + "?")
         post_act(args, media_file, action=true_action if response else false_action)
 
     action = action or args.post_action
+    action = action.upper()
 
     if action == Action.KEEP:
         pass
     elif action == Action.DELETE:
         handle_delete_action()
     elif action == Action.DELETE_IF_AUDIOBOOK:
         if "audiobook" in media_file.lower():
             handle_delete_action()
     elif action == Action.SOFTDELETE:
         handle_soft_delete_action()
     elif action == Action.MOVE:
         handle_move_action()
-    elif action.startswith("ask_"):
+    elif action.startswith("ASK_"):
         handle_ask_action(action)
     else:
         raise ValueError("Unrecognized action:", action)
 
 
 def override_sort(sort_expression: str) -> str:
     def year_month_sql(var):
```

### Comparing `xklb-1.26.27/xklb/praw_extract.py` & `xklb-1.26.28/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/stats.py` & `xklb-1.26.28/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/subtitle.py` & `xklb-1.26.28/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/tabs_actions.py` & `xklb-1.26.28/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/tabs_extract.py` & `xklb-1.26.28/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/tube_backend.py` & `xklb-1.26.28/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/tube_extract.py` & `xklb-1.26.28/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/utils.py` & `xklb-1.26.28/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/__init__.py` & `xklb-1.26.28/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/bigdirs.py` & `xklb-1.26.28/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/christen.py` & `xklb-1.26.28/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/copy_play_counts.py` & `xklb-1.26.28/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/dedupe.py` & `xklb-1.26.28/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/merge_dbs.py` & `xklb-1.26.28/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/merge_online_local.py` & `xklb-1.26.28/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/move_list.py` & `xklb-1.26.28/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/optimize_db.py` & `xklb-1.26.28/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/redownload.py` & `xklb-1.26.28/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/relmv.py` & `xklb-1.26.28/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/scatter.py` & `xklb-1.26.28/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.28/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/mining/nfb_ca.py` & `xklb-1.26.28/xklb/scripts/mining/nfb_ca.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/mining/nouns.py` & `xklb-1.26.28/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/mining/pushshift.py` & `xklb-1.26.28/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.26.28/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/xklb/scripts/mining/words.py` & `xklb-1.26.28/xklb/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/assets/kotobago.png` & `xklb-1.26.28/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/.gitignore` & `xklb-1.26.28/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/LICENSE` & `xklb-1.26.28/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/README.md` & `xklb-1.26.28/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.027)
+    xk media library subcommands (v1.26.028)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.26.27/pyproject.toml` & `xklb-1.26.28/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.27/PKG-INFO` & `xklb-1.26.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.27
+Version: 1.26.28
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.027)
+    xk media library subcommands (v1.26.028)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

