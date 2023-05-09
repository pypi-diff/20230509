# Comparing `tmp/tldr-3.1.0.tar.gz` & `tmp/tldr-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp4l4pzol5/tmpen47egw7/tldr-3.1.0.tar", last modified: Mon Feb 21 19:16:54 2022, max compression
+gzip compressed data, was "/tmp/tmp3dtpnmg_/.tmp-gvdga5lv/tldr-3.2.0.tar", last modified: Tue May  9 16:13:07 2023, max compression
```

## Comparing `tldr-3.1.0.tar` & `tldr-3.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 19:16:54.000000 tldr-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-02-21 19:16:42.000000 tldr-3.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     8141 2022-02-21 19:16:54.000000 tldr-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7072 2022-02-21 19:16:42.000000 tldr-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 19:16:54.000000 tldr-3.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 19:16:54.000000 tldr-3.1.0/docs/man/
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-02-21 19:16:50.000000 tldr-3.1.0/docs/man/tldr.1
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-02-21 19:16:42.000000 tldr-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-21 19:16:54.000000 tldr-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-02-21 19:16:42.000000 tldr-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 19:16:54.000000 tldr-3.1.0/tldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8141 2022-02-21 19:16:54.000000 tldr-3.1.0/tldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-21 19:16:54.000000 tldr-3.1.0/tldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-21 19:16:54.000000 tldr-3.1.0/tldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-02-21 19:16:54.000000 tldr-3.1.0/tldr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-02-21 19:16:54.000000 tldr-3.1.0/tldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-02-21 19:16:54.000000 tldr-3.1.0/tldr.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    18303 2022-02-21 19:16:42.000000 tldr-3.1.0/tldr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:13:07.000000 tldr-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-05-09 16:12:49.000000 tldr-3.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     8166 2023-05-09 16:13:07.000000 tldr-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7066 2023-05-09 16:12:49.000000 tldr-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:13:07.000000 tldr-3.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:13:07.000000 tldr-3.2.0/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-05-09 16:13:03.000000 tldr-3.2.0/docs/man/tldr.1
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-09 16:12:49.000000 tldr-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 16:13:07.000000 tldr-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-05-09 16:12:49.000000 tldr-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:13:07.000000 tldr-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-05-09 16:12:49.000000 tldr-3.2.0/tests/test_tldr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:13:07.000000 tldr-3.2.0/tldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8166 2023-05-09 16:13:06.000000 tldr-3.2.0/tldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-09 16:13:06.000000 tldr-3.2.0/tldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 16:13:06.000000 tldr-3.2.0/tldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-09 16:13:06.000000 tldr-3.2.0/tldr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-09 16:13:06.000000 tldr-3.2.0/tldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-09 16:13:06.000000 tldr-3.2.0/tldr.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)    18425 2023-05-09 16:12:49.000000 tldr-3.2.0/tldr.py
```

### Comparing `tldr-3.1.0/LICENSE.md` & `tldr-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tldr-3.1.0/PKG-INFO` & `tldr-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: tldr
-Version: 3.1.0
+Version: 3.2.0
 Summary: command line client for tldr
 Home-page: https://github.com/tldr-pages/tldr-python-client
 Author: Felix Yan
 Author-email: felixonmars@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: SunOS/Solaris
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: System
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # tldr-python-client
@@ -91,21 +91,21 @@
 export TLDR_COLOR_DESCRIPTION="white"
 export TLDR_COLOR_EXAMPLE="green"
 export TLDR_COLOR_COMMAND="red"
 export TLDR_COLOR_PARAMETER="white"
 export TLDR_LANGUAGE="es"
 export TLDR_CACHE_ENABLED=1
 export TLDR_CACHE_MAX_AGE=720
-export TLDR_PAGES_SOURCE_LOCATION="https://raw.githubusercontent.com/tldr-pages/tldr/master/pages"
+export TLDR_PAGES_SOURCE_LOCATION="https://raw.githubusercontent.com/tldr-pages/tldr/main/pages"
 export TLDR_DOWNLOAD_CACHE_LOCATION="https://tldr-pages.github.io/assets/tldr.zip"
 ```
 
 ### Cache
 
-Cache is downloaded from `TLDR_DOWNLOAD_CACHE_LOCATION` (defaults to the one described in [the client specification](https://github.com/tldr-pages/tldr/blob/master/CLIENT-SPECIFICATION.md#caching)), unzipped and extracted into the [local cache directory](#cache-location). Pages are loaded directly from `TLDR_PAGES_SOURCE_LOCATION` if `tldr <command>` is used.
+Cache is downloaded from `TLDR_DOWNLOAD_CACHE_LOCATION` (defaults to the one described in [the client specification](https://github.com/tldr-pages/tldr/blob/main/CLIENT-SPECIFICATION.md#caching)), unzipped and extracted into the [local cache directory](#cache-location). Pages are loaded directly from `TLDR_PAGES_SOURCE_LOCATION` if `tldr <command>` is used.
 
 * `TLDR_CACHE_ENABLED` (default is `1`):
     * If set to `1`, the client will first try to load from cache, and fall back to fetching from the internet if the cache doesn't exist or is too old.
     * If set to `0`, the client will fetch from the internet, and fall back to the cache if the page cannot be fetched from the internet.
 * `TLDR_CACHE_MAX_AGE` (default is `168` hours, which is equivalent to a week): maximum age of the cache in hours to be considered as valid when `TLDR_CACHE_ENABLED` is set to `1`.
 
 #### Cache location
@@ -178,13 +178,11 @@
 
 ### Remote source
 
 If you wish to use your own instance of the tldr pages instead of the default repository, you
 can either use the `--source` flag when using tldr or by specifying the following environment variables:
 
 * `TLDR_PAGES_SOURCE_LOCATION` to control where to get individual pages from
-  * defaults to `https://raw.githubusercontent.com/tldr-pages/tldr/master/pages`
+  * defaults to `https://raw.githubusercontent.com/tldr-pages/tldr/main/pages`
   * it can also point to local directory using `file:///path/to/directory`
 * `TLDR_DOWNLOAD_CACHE_LOCATION` to control where to pull a zip of all pages from
   * defaults to `https://tldr-pages.github.io/assets/tldr.zip`
-
-
```

### Comparing `tldr-3.1.0/README.md` & `tldr-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,21 +62,21 @@
 export TLDR_COLOR_DESCRIPTION="white"
 export TLDR_COLOR_EXAMPLE="green"
 export TLDR_COLOR_COMMAND="red"
 export TLDR_COLOR_PARAMETER="white"
 export TLDR_LANGUAGE="es"
 export TLDR_CACHE_ENABLED=1
 export TLDR_CACHE_MAX_AGE=720
-export TLDR_PAGES_SOURCE_LOCATION="https://raw.githubusercontent.com/tldr-pages/tldr/master/pages"
+export TLDR_PAGES_SOURCE_LOCATION="https://raw.githubusercontent.com/tldr-pages/tldr/main/pages"
 export TLDR_DOWNLOAD_CACHE_LOCATION="https://tldr-pages.github.io/assets/tldr.zip"
 ```
 
 ### Cache
 
-Cache is downloaded from `TLDR_DOWNLOAD_CACHE_LOCATION` (defaults to the one described in [the client specification](https://github.com/tldr-pages/tldr/blob/master/CLIENT-SPECIFICATION.md#caching)), unzipped and extracted into the [local cache directory](#cache-location). Pages are loaded directly from `TLDR_PAGES_SOURCE_LOCATION` if `tldr <command>` is used.
+Cache is downloaded from `TLDR_DOWNLOAD_CACHE_LOCATION` (defaults to the one described in [the client specification](https://github.com/tldr-pages/tldr/blob/main/CLIENT-SPECIFICATION.md#caching)), unzipped and extracted into the [local cache directory](#cache-location). Pages are loaded directly from `TLDR_PAGES_SOURCE_LOCATION` if `tldr <command>` is used.
 
 * `TLDR_CACHE_ENABLED` (default is `1`):
     * If set to `1`, the client will first try to load from cache, and fall back to fetching from the internet if the cache doesn't exist or is too old.
     * If set to `0`, the client will fetch from the internet, and fall back to the cache if the page cannot be fetched from the internet.
 * `TLDR_CACHE_MAX_AGE` (default is `168` hours, which is equivalent to a week): maximum age of the cache in hours to be considered as valid when `TLDR_CACHE_ENABLED` is set to `1`.
 
 #### Cache location
@@ -149,11 +149,11 @@
 
 ### Remote source
 
 If you wish to use your own instance of the tldr pages instead of the default repository, you
 can either use the `--source` flag when using tldr or by specifying the following environment variables:
 
 * `TLDR_PAGES_SOURCE_LOCATION` to control where to get individual pages from
-  * defaults to `https://raw.githubusercontent.com/tldr-pages/tldr/master/pages`
+  * defaults to `https://raw.githubusercontent.com/tldr-pages/tldr/main/pages`
   * it can also point to local directory using `file:///path/to/directory`
 * `TLDR_DOWNLOAD_CACHE_LOCATION` to control where to pull a zip of all pages from
   * defaults to `https://tldr-pages.github.io/assets/tldr.zip`
```

### Comparing `tldr-3.1.0/docs/man/tldr.1` & `tldr-3.2.0/docs/man/tldr.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "TLDR" "1" "Feb 21, 2022" "" "tldr"
+.TH "TLDR" "1" "May 09, 2023" "" "tldr"
 .SH NAME
-tldr \- tldr 3.1.0
+tldr \- tldr 3.2.0
 .sp
 Python command line client for tldr
 
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -72,15 +72,15 @@
 List all available commands for operating system
 .sp
 Default: False
 .TP
 .B \-s, \-\-source
 Override the default page source
 .sp
-Default: "\fI\%https://raw.githubusercontent.com/tldr\-pages/tldr/master/pages\fP"
+Default: \(dq\fI\%https://raw.githubusercontent.com/tldr\-pages/tldr/main/pages\fP\(dq
 .TP
 .B \-c, \-\-color
 Override color stripping
 .TP
 .B \-r, \-\-render
 Render local markdown files
 .sp
```

### Comparing `tldr-3.1.0/setup.py` & `tldr-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,11 +48,12 @@
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
         "Topic :: System"
     ]
 )
```

### Comparing `tldr-3.1.0/tldr.egg-info/PKG-INFO` & `tldr-3.2.0/tldr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: tldr
-Version: 3.1.0
+Version: 3.2.0
 Summary: command line client for tldr
 Home-page: https://github.com/tldr-pages/tldr-python-client
 Author: Felix Yan
 Author-email: felixonmars@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: SunOS/Solaris
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: System
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # tldr-python-client
@@ -91,21 +91,21 @@
 export TLDR_COLOR_DESCRIPTION="white"
 export TLDR_COLOR_EXAMPLE="green"
 export TLDR_COLOR_COMMAND="red"
 export TLDR_COLOR_PARAMETER="white"
 export TLDR_LANGUAGE="es"
 export TLDR_CACHE_ENABLED=1
 export TLDR_CACHE_MAX_AGE=720
-export TLDR_PAGES_SOURCE_LOCATION="https://raw.githubusercontent.com/tldr-pages/tldr/master/pages"
+export TLDR_PAGES_SOURCE_LOCATION="https://raw.githubusercontent.com/tldr-pages/tldr/main/pages"
 export TLDR_DOWNLOAD_CACHE_LOCATION="https://tldr-pages.github.io/assets/tldr.zip"
 ```
 
 ### Cache
 
-Cache is downloaded from `TLDR_DOWNLOAD_CACHE_LOCATION` (defaults to the one described in [the client specification](https://github.com/tldr-pages/tldr/blob/master/CLIENT-SPECIFICATION.md#caching)), unzipped and extracted into the [local cache directory](#cache-location). Pages are loaded directly from `TLDR_PAGES_SOURCE_LOCATION` if `tldr <command>` is used.
+Cache is downloaded from `TLDR_DOWNLOAD_CACHE_LOCATION` (defaults to the one described in [the client specification](https://github.com/tldr-pages/tldr/blob/main/CLIENT-SPECIFICATION.md#caching)), unzipped and extracted into the [local cache directory](#cache-location). Pages are loaded directly from `TLDR_PAGES_SOURCE_LOCATION` if `tldr <command>` is used.
 
 * `TLDR_CACHE_ENABLED` (default is `1`):
     * If set to `1`, the client will first try to load from cache, and fall back to fetching from the internet if the cache doesn't exist or is too old.
     * If set to `0`, the client will fetch from the internet, and fall back to the cache if the page cannot be fetched from the internet.
 * `TLDR_CACHE_MAX_AGE` (default is `168` hours, which is equivalent to a week): maximum age of the cache in hours to be considered as valid when `TLDR_CACHE_ENABLED` is set to `1`.
 
 #### Cache location
@@ -178,13 +178,11 @@
 
 ### Remote source
 
 If you wish to use your own instance of the tldr pages instead of the default repository, you
 can either use the `--source` flag when using tldr or by specifying the following environment variables:
 
 * `TLDR_PAGES_SOURCE_LOCATION` to control where to get individual pages from
-  * defaults to `https://raw.githubusercontent.com/tldr-pages/tldr/master/pages`
+  * defaults to `https://raw.githubusercontent.com/tldr-pages/tldr/main/pages`
   * it can also point to local directory using `file:///path/to/directory`
 * `TLDR_DOWNLOAD_CACHE_LOCATION` to control where to pull a zip of all pages from
   * defaults to `https://tldr-pages.github.io/assets/tldr.zip`
-
-
```

### Comparing `tldr-3.1.0/tldr.py` & `tldr-3.2.0/tldr.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 from urllib.parse import quote
 from urllib.request import urlopen, Request
 from urllib.error import HTTPError, URLError
 from termcolor import colored
 import colorama  # Required for Windows
 import shtab
 
-__version__ = "3.1.0"
+__version__ = "3.2.0"
 __client_specification__ = "1.5"
 
 REQUEST_HEADERS = {'User-Agent': 'tldr-python-client'}
 PAGES_SOURCE_LOCATION = os.environ.get(
     'TLDR_PAGES_SOURCE_LOCATION',
-    'https://raw.githubusercontent.com/tldr-pages/tldr/master/pages'
+    'https://raw.githubusercontent.com/tldr-pages/tldr/main/pages'
 ).rstrip('/')
 DOWNLOAD_CACHE_LOCATION = os.environ.get(
     'TLDR_DOWNLOAD_CACHE_LOCATION',
     'https://tldr-pages.github.io/assets/tldr.zip'
 )
 
 USE_NETWORK = int(os.environ.get('TLDR_NETWORK_ENABLED', '1')) > 0
@@ -156,14 +156,15 @@
             platform,
         ))
     else:
         page_url = get_page_url(command, platform, remote, language)
         try:
             data = urlopen(
                 Request(page_url, headers=REQUEST_HEADERS),
+                timeout=10,
                 context=URLOPEN_CONTEXT
             ).read()
             data_downloaded = True
         except Exception:
             if not USE_CACHE:
                 raise
             data = load_page_from_cache(command, platform, language)
@@ -473,30 +474,32 @@
 
     parser.add_argument(
         'command', type=str, nargs='*', help="command to lookup", metavar='command'
     ).complete = {"bash": "shtab_tldr_cmd_list", "zsh": "shtab_tldr_cmd_list"}
 
     shtab.add_argument_to(parser, preamble={
         'bash': r'''shtab_tldr_cmd_list(){{
-          compgen -W "$("{py}" -m tldr --list | sed 's/\W/ /g')" -- "$1"
+          compgen -W "$("{py}" -m tldr --list | sed 's/[^[:alnum:]_]/ /g')" -- "$1"
         }}'''.format(py=sys.executable),
         'zsh': r'''shtab_tldr_cmd_list(){{
-          _describe 'command' "($("{py}" -m tldr --list | sed 's/\W/ /g'))"
+          _describe 'command' "($("{py}" -m tldr --list | sed 's/[^[:alnum:]_]/ /g'))"
         }}'''.format(py=sys.executable)
     })
 
     return parser
 
 
 def main() -> None:
     parser = create_parser()
 
     options = parser.parse_args()
 
     colorama.init(strip=options.color)
+    if options.color is False:
+        os.environ["FORCE_COLOR"] = "true"
 
     if options.update_cache:
         update_cache(language=options.language)
         return
     elif len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
```

