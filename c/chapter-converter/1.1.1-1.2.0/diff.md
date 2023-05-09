# Comparing `tmp/chapter_converter-1.1.1.tar.gz` & `tmp/chapter_converter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chapter_converter-1.1.1.tar", last modified: Wed Apr  5 16:24:31 2023, max compression
+gzip compressed data, was "chapter_converter-1.2.0.tar", last modified: Tue May  9 12:44:07 2023, max compression
```

## Comparing `chapter_converter-1.1.1.tar` & `chapter_converter-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 16:24:31.890939 chapter_converter-1.1.1/
--rw-rw-rw-   0        0        0     1088 2018-07-04 07:26:08.000000 chapter_converter-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     5389 2023-04-05 16:24:31.890939 chapter_converter-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4880 2023-04-05 16:20:22.000000 chapter_converter-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 16:24:31.879939 chapter_converter-1.1.1/chapter_converter/
--rw-rw-rw-   0        0        0        0 2023-04-05 14:35:45.000000 chapter_converter-1.1.1/chapter_converter/__init__.py
--rw-rw-rw-   0        0        0       77 2023-04-05 15:50:11.000000 chapter_converter-1.1.1/chapter_converter/__main__.py
--rw-rw-rw-   0        0        0     8209 2023-04-05 15:56:16.000000 chapter_converter-1.1.1/chapter_converter/chapter_converter.py
--rw-rw-rw-   0        0        0      149 2023-04-05 15:41:44.000000 chapter_converter-1.1.1/chapter_converter/gui.py
-drwxrwxrwx   0        0        0        0 2023-04-05 16:24:31.889941 chapter_converter-1.1.1/chapter_converter.egg-info/
--rw-rw-rw-   0        0        0     5389 2023-04-05 16:24:31.000000 chapter_converter-1.1.1/chapter_converter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-05 16:24:31.000000 chapter_converter-1.1.1/chapter_converter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 16:24:31.000000 chapter_converter-1.1.1/chapter_converter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-04-05 16:24:31.000000 chapter_converter-1.1.1/chapter_converter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-04-05 16:24:31.000000 chapter_converter-1.1.1/chapter_converter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-05 14:42:39.000000 chapter_converter-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      800 2023-04-05 16:24:31.894938 chapter_converter-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-05 14:42:52.000000 chapter_converter-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:44:07.533189 chapter_converter-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 12:43:47.000000 chapter_converter-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-09 12:44:07.533189 chapter_converter-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-09 12:43:47.000000 chapter_converter-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:44:07.533189 chapter_converter-1.2.0/chapter_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:43:47.000000 chapter_converter-1.2.0/chapter_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 12:43:47.000000 chapter_converter-1.2.0/chapter_converter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-05-09 12:43:47.000000 chapter_converter-1.2.0/chapter_converter/chapter_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-09 12:43:47.000000 chapter_converter-1.2.0/chapter_converter/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:44:07.533189 chapter_converter-1.2.0/chapter_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-09 12:44:07.000000 chapter_converter-1.2.0/chapter_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-09 12:44:07.000000 chapter_converter-1.2.0/chapter_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:44:07.000000 chapter_converter-1.2.0/chapter_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 12:44:07.000000 chapter_converter-1.2.0/chapter_converter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 12:44:07.000000 chapter_converter-1.2.0/chapter_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 12:43:47.000000 chapter_converter-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-09 12:44:07.533189 chapter_converter-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:43:47.000000 chapter_converter-1.2.0/setup.py
```

### Comparing `chapter_converter-1.1.1/PKG-INFO` & `chapter_converter-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,182 +1,168 @@
-Metadata-Version: 2.1
-Name: chapter_converter
-Version: 1.1.1
-Summary: Convert between several different video chapter file formats with ease.
-Home-page: https://github.com/fireattack/chapter_converter
-Author: fireattack
-Author-email: 
-License: MIT
-Project-URL: Source, https://github.com/fireattack/chapter_converter
-Project-URL: Tracker, https://github.com/fireattack/chapter_converter/issues
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
-
-[![PyPI Version](https://img.shields.io/pypi/v/chapter-converter.svg)](https://pypi.python.org/pypi/chapter-converter)
-
-# chapter_converter
-Convert between several different video chapter file formats with ease.
-
-## Features
-
-* Auto input format detection: including chapter files and video files with chapters (`.mkv` and `.mp4`. Requires `mkvtoolnix` binaries in path).
-* Auto input encoding detection
-* Can specify output format and filename
-* Clipboard support (input and output) for editing purposes
-
-## Install
-
-```
-pip install -U chapter_converter
-```
-or from source:
-```
-pip install -U git+https://github.com/fireattack/chapter_converter
-```
-
-## Usage
-
-CLI script is named `chap`. Or you can use `python -m chapter_converter`.
-
-```
-usage: chap [-h] [-f {simple,pot,ogm,tab,xml}] [--mp4-charset MP4_CHARSET] [--charset CHARSET] [-o OUTPUT] [-c] [filename]
-
-positional arguments:
-  filename              input filename
-
-options:
-  -h, --help            show this help message and exit
-  -f {simple,pot,ogm,tab,xml}, --format {simple,pot,ogm,tab,xml}
-                        output format (default: pot)
-  --mp4-charset MP4_CHARSET
-                        input chapter charset for mp4 file, since it can't be auto detected (default: utf-8)
-  --charset CHARSET     output file charset (default: utf-8-sig)
-  -o OUTPUT, --output OUTPUT
-                        output filename (default: original_filename.format[.txt])
-  -c, --clipboard       automatically process text in clipboard and save it back.
-```
-
-If you prefer a single file than a package, you can just download `chapter_converter.py` in `chapter_converter/` and use it directly (`chapter_converter.py -h`).
-
-A simple GUI is also provided as-is by running `chapgui`. You need to install module `gooey` in `pip` manually to make it work. See [my comments](https://github.com/fireattack/chapter_converter/pull/4#issuecomment-1359129224) for some caveats.
-
-As a Python module:
-
-```python
-from chapter_converter import chapter_converter
-
-chapter_converter.main('input.pbf', '-o', 'output.xml')
-```
-
-### Note
-
-* Output by default saved as UTF-8-BOM for max compatibility on Windows. You can change it by passing in `--charset` argument.
-* When `-c` is used, you can still pass in a file as input instead.
-* When `-c` is used, you can still pass in an output filename (using `-o` and/or `-f`) as output instead.
-
-## Supported formats
-
-See also: example files in `examples/`.
-
-### MKV and MP4 video containers (inputs only)
-
-Guessed by suffix. Not idiot-proof, please only feed in file with chapters.
-
-### Simple format (`simple`)
-
-I made it up.
-
-Format:
-* Each line: `{timestamp},{title}`
-
-Example:
-
-```
-0:17:02.148,Title1
-0:42:19.976,Title2
-0:58:10.114,Title3
-...
-```
-
-### Tab format (`tab`)
-
-Similar to Simple, but separated by tab instead of comma.
-
-Format:
-* Each line: `{timestamp}	{title}`
-
-Example:
-
-```
-0:17:02.148	Title1
-0:42:19.976	Title2
-0:58:10.114	Title3
-...
-```
-
-### OGM format (`ogm`)
-
-Can be recognized by common video tools, such as [MKVToolNix](https://mkvtoolnix.download/).
-
-Format:
-* Odd lines: `CHAPTER{i:02}={timestamp}`
-* Even lines: `CHAPTER{i:02}NAME={tilte}`
-
-`i` starts at 1.
-
-Example:
-
-```
-CHAPTER01=0:17:02.148
-CHAPTER01NAME=Title1
-CHAPTER02=0:42:19.976
-CHAPTER02NAME=Title2
-CHAPTER03=0:58:10.114
-...
-```
-
-### MediaInfo format (`mediainfo`)
-
-The way [MediaInfo](https://mediaarea.net/en/MediaInfo) presents chapter information in text form. Input only. Supports both with or without the "Menu" line.
-
-Format:
-* Each line: `{timestamp}\s+: ({two_letter_lang_code})?:{title}`
-
-Example:
-
-```
-Menu
-00:00:00.000                : en:Contours
-00:02:49.624                : en:From the Sea
-00:08:41.374                : en:Bread and Wine
-00:12:18.041                : en:Faceless
-...
-```
-
-### XML format (`xml`)
-
-XML chapter format defined by [Matroska specification](https://matroska.org/technical/specs/chapters/index.html).
-
-###  [PotPlayer](https://potplayer.daum.net/) Bookmark format (.pbf) (`pot`)
-
-A format PotPlayer uses for its bookmarks. If you put the file together with the video file (same name except extension, just like any external resources), it will be recognized by PotPlayer just like internal chapters - you can use "H" to view and select, and they will show up as markers on navigation bar too:
-
-![Pot Bookmark Example](https://raw.githubusercontent.com/fireattack/chapter_converter/master/img/pot.png)
-
-It is not ideal, but it's the closest thing to "external chapter file" to my knowledge.
-
-Format:
-
-* First line: `[Bookmark]`
-* Other lines: `{i}={timestamp_in_ms}*{title}*{some_optional_hash_for_pot_internal_usage}`
-
-`i` starts at 0.
-
-Example:
-
-```
-[Bookmark]
-0=1022148*Title1*
-1=2539976*Titile2*
-...
-```
+[![PyPI Version](https://img.shields.io/pypi/v/chapter-converter.svg)](https://pypi.python.org/pypi/chapter-converter)
+
+# chapter_converter
+Convert between several different video chapter file formats with ease.
+
+## Features
+
+* Auto input format detection: including chapter files and video files with chapters (`.mkv` and `.mp4`. Requires `mkvtoolnix` binaries in path).
+* Auto input encoding detection
+* Can specify output format and filename
+* Clipboard support (input and output) for editing purposes
+
+## Install
+
+```
+pip install -U chapter_converter
+```
+or from source:
+```
+pip install -U git+https://github.com/fireattack/chapter_converter
+```
+
+## Usage
+
+CLI script is named `chap`. Or you can use `python -m chapter_converter`.
+
+```
+usage: chap [-h] [-f {simple,pot,ogm,tab,xml}] [--mp4-charset MP4_CHARSET] [--charset CHARSET] [-o OUTPUT] [-c] [filename]
+
+positional arguments:
+  filename              input filename
+
+options:
+  -h, --help            show this help message and exit
+  -f {simple,pot,ogm,tab,xml}, --format {simple,pot,ogm,tab,xml}
+                        output format (default: pot)
+  --mp4-charset MP4_CHARSET
+                        input chapter charset for mp4 file, since it can't be auto detected (default: utf-8)
+  --charset CHARSET     output file charset (default: utf-8-sig)
+  -o OUTPUT, --output OUTPUT
+                        output filename (default: original_filename.format[.txt])
+  -c, --clipboard       automatically process text in clipboard and save it back.
+```
+
+If you prefer a single file than a package, you can just download `chapter_converter.py` in `chapter_converter/` and use it directly (`chapter_converter.py -h`).
+
+A simple GUI is also provided as-is by running `chapgui`. You need to install module `gooey` in `pip` manually to make it work. See [my comments](https://github.com/fireattack/chapter_converter/pull/4#issuecomment-1359129224) for some caveats.
+
+As a Python module:
+
+```python
+from chapter_converter import chapter_converter
+
+chapter_converter.main('input.pbf', '-o', 'output.xml')
+```
+
+### Note
+
+* Output by default saved as UTF-8-BOM for max compatibility on Windows. You can change it by passing in `--charset` argument.
+* When `-c` is used, you can still pass in a file as input instead.
+* When `-c` is used, you can still pass in an output filename (using `-o` and/or `-f`) as output instead.
+
+## Supported formats
+
+See also: example files in `examples/`.
+
+### MKV and MP4 video containers (inputs only)
+
+Guessed by suffix. Not idiot-proof, please only feed in file with chapters.
+
+### Simple format (`simple`)
+
+I made it up.
+
+Format:
+* Each line: `{timestamp},{title}`
+
+Example:
+
+```
+0:17:02.148,Title1
+0:42:19.976,Title2
+0:58:10.114,Title3
+...
+```
+
+### Tab format (`tab`)
+
+Similar to Simple, but separated by tab instead of comma.
+
+Format:
+* Each line: `{timestamp}	{title}`
+
+Example:
+
+```
+0:17:02.148	Title1
+0:42:19.976	Title2
+0:58:10.114	Title3
+...
+```
+
+### OGM format (`ogm`)
+
+Can be recognized by common video tools, such as [MKVToolNix](https://mkvtoolnix.download/).
+
+Format:
+* Odd lines: `CHAPTER{i:02}={timestamp}`
+* Even lines: `CHAPTER{i:02}NAME={tilte}`
+
+`i` starts at 1.
+
+Example:
+
+```
+CHAPTER01=0:17:02.148
+CHAPTER01NAME=Title1
+CHAPTER02=0:42:19.976
+CHAPTER02NAME=Title2
+CHAPTER03=0:58:10.114
+...
+```
+
+### MediaInfo format (`mediainfo`)
+
+The way [MediaInfo](https://mediaarea.net/en/MediaInfo) presents chapter information in text form. Input only. Supports both with or without the "Menu" line.
+
+Format:
+* Each line: `{timestamp}\s+: ({two_letter_lang_code})?:{title}`
+
+Example:
+
+```
+Menu
+00:00:00.000                : en:Contours
+00:02:49.624                : en:From the Sea
+00:08:41.374                : en:Bread and Wine
+00:12:18.041                : en:Faceless
+...
+```
+
+### XML format (`xml`)
+
+XML chapter format defined by [Matroska specification](https://matroska.org/technical/specs/chapters/index.html).
+
+###  [PotPlayer](https://potplayer.daum.net/) Bookmark format (.pbf) (`pot`)
+
+A format PotPlayer uses for its bookmarks. If you put the file together with the video file (same name except extension, just like any external resources), it will be recognized by PotPlayer just like internal chapters - you can use "H" to view and select, and they will show up as markers on navigation bar too:
+
+![Pot Bookmark Example](https://raw.githubusercontent.com/fireattack/chapter_converter/master/img/pot.png)
+
+It is not ideal, but it's the closest thing to "external chapter file" to my knowledge.
+
+Format:
+
+* First line: `[Bookmark]`
+* Other lines: `{i}={timestamp_in_ms}*{title}*{some_optional_hash_for_pot_internal_usage}`
+
+`i` starts at 0.
+
+Example:
+
+```
+[Bookmark]
+0=1022148*Title1*
+1=2539976*Titile2*
+...
+```
```

### Comparing `chapter_converter-1.1.1/README.md` & `chapter_converter-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,182 @@
-[![PyPI Version](https://img.shields.io/pypi/v/chapter-converter.svg)](https://pypi.python.org/pypi/chapter-converter)
-
-# chapter_converter
-Convert between several different video chapter file formats with ease.
-
-## Features
-
-* Auto input format detection: including chapter files and video files with chapters (`.mkv` and `.mp4`. Requires `mkvtoolnix` binaries in path).
-* Auto input encoding detection
-* Can specify output format and filename
-* Clipboard support (input and output) for editing purposes
-
-## Install
-
-```
-pip install -U chapter_converter
-```
-or from source:
-```
-pip install -U git+https://github.com/fireattack/chapter_converter
-```
-
-## Usage
-
-CLI script is named `chap`. Or you can use `python -m chapter_converter`.
-
-```
-usage: chap [-h] [-f {simple,pot,ogm,tab,xml}] [--mp4-charset MP4_CHARSET] [--charset CHARSET] [-o OUTPUT] [-c] [filename]
-
-positional arguments:
-  filename              input filename
-
-options:
-  -h, --help            show this help message and exit
-  -f {simple,pot,ogm,tab,xml}, --format {simple,pot,ogm,tab,xml}
-                        output format (default: pot)
-  --mp4-charset MP4_CHARSET
-                        input chapter charset for mp4 file, since it can't be auto detected (default: utf-8)
-  --charset CHARSET     output file charset (default: utf-8-sig)
-  -o OUTPUT, --output OUTPUT
-                        output filename (default: original_filename.format[.txt])
-  -c, --clipboard       automatically process text in clipboard and save it back.
-```
-
-If you prefer a single file than a package, you can just download `chapter_converter.py` in `chapter_converter/` and use it directly (`chapter_converter.py -h`).
-
-A simple GUI is also provided as-is by running `chapgui`. You need to install module `gooey` in `pip` manually to make it work. See [my comments](https://github.com/fireattack/chapter_converter/pull/4#issuecomment-1359129224) for some caveats.
-
-As a Python module:
-
-```python
-from chapter_converter import chapter_converter
-
-chapter_converter.main('input.pbf', '-o', 'output.xml')
-```
-
-### Note
-
-* Output by default saved as UTF-8-BOM for max compatibility on Windows. You can change it by passing in `--charset` argument.
-* When `-c` is used, you can still pass in a file as input instead.
-* When `-c` is used, you can still pass in an output filename (using `-o` and/or `-f`) as output instead.
-
-## Supported formats
-
-See also: example files in `examples/`.
-
-### MKV and MP4 video containers (inputs only)
-
-Guessed by suffix. Not idiot-proof, please only feed in file with chapters.
-
-### Simple format (`simple`)
-
-I made it up.
-
-Format:
-* Each line: `{timestamp},{title}`
-
-Example:
-
-```
-0:17:02.148,Title1
-0:42:19.976,Title2
-0:58:10.114,Title3
-...
-```
-
-### Tab format (`tab`)
-
-Similar to Simple, but separated by tab instead of comma.
-
-Format:
-* Each line: `{timestamp}	{title}`
-
-Example:
-
-```
-0:17:02.148	Title1
-0:42:19.976	Title2
-0:58:10.114	Title3
-...
-```
-
-### OGM format (`ogm`)
-
-Can be recognized by common video tools, such as [MKVToolNix](https://mkvtoolnix.download/).
-
-Format:
-* Odd lines: `CHAPTER{i:02}={timestamp}`
-* Even lines: `CHAPTER{i:02}NAME={tilte}`
-
-`i` starts at 1.
-
-Example:
-
-```
-CHAPTER01=0:17:02.148
-CHAPTER01NAME=Title1
-CHAPTER02=0:42:19.976
-CHAPTER02NAME=Title2
-CHAPTER03=0:58:10.114
-...
-```
-
-### MediaInfo format (`mediainfo`)
-
-The way [MediaInfo](https://mediaarea.net/en/MediaInfo) presents chapter information in text form. Input only. Supports both with or without the "Menu" line.
-
-Format:
-* Each line: `{timestamp}\s+: ({two_letter_lang_code})?:{title}`
-
-Example:
-
-```
-Menu
-00:00:00.000                : en:Contours
-00:02:49.624                : en:From the Sea
-00:08:41.374                : en:Bread and Wine
-00:12:18.041                : en:Faceless
-...
-```
-
-### XML format (`xml`)
-
-XML chapter format defined by [Matroska specification](https://matroska.org/technical/specs/chapters/index.html).
-
-###  [PotPlayer](https://potplayer.daum.net/) Bookmark format (.pbf) (`pot`)
-
-A format PotPlayer uses for its bookmarks. If you put the file together with the video file (same name except extension, just like any external resources), it will be recognized by PotPlayer just like internal chapters - you can use "H" to view and select, and they will show up as markers on navigation bar too:
-
-![Pot Bookmark Example](https://raw.githubusercontent.com/fireattack/chapter_converter/master/img/pot.png)
-
-It is not ideal, but it's the closest thing to "external chapter file" to my knowledge.
-
-Format:
-
-* First line: `[Bookmark]`
-* Other lines: `{i}={timestamp_in_ms}*{title}*{some_optional_hash_for_pot_internal_usage}`
-
-`i` starts at 0.
-
-Example:
-
-```
-[Bookmark]
-0=1022148*Title1*
-1=2539976*Titile2*
-...
-```
+Metadata-Version: 2.1
+Name: chapter_converter
+Version: 1.2.0
+Summary: Convert between several different video chapter file formats with ease.
+Home-page: https://github.com/fireattack/chapter_converter
+Author: fireattack
+Author-email: 
+License: MIT
+Project-URL: Source, https://github.com/fireattack/chapter_converter
+Project-URL: Tracker, https://github.com/fireattack/chapter_converter/issues
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+[![PyPI Version](https://img.shields.io/pypi/v/chapter-converter.svg)](https://pypi.python.org/pypi/chapter-converter)
+
+# chapter_converter
+Convert between several different video chapter file formats with ease.
+
+## Features
+
+* Auto input format detection: including chapter files and video files with chapters (`.mkv` and `.mp4`. Requires `mkvtoolnix` binaries in path).
+* Auto input encoding detection
+* Can specify output format and filename
+* Clipboard support (input and output) for editing purposes
+
+## Install
+
+```
+pip install -U chapter_converter
+```
+or from source:
+```
+pip install -U git+https://github.com/fireattack/chapter_converter
+```
+
+## Usage
+
+CLI script is named `chap`. Or you can use `python -m chapter_converter`.
+
+```
+usage: chap [-h] [-f {simple,pot,ogm,tab,xml}] [--mp4-charset MP4_CHARSET] [--charset CHARSET] [-o OUTPUT] [-c] [filename]
+
+positional arguments:
+  filename              input filename
+
+options:
+  -h, --help            show this help message and exit
+  -f {simple,pot,ogm,tab,xml}, --format {simple,pot,ogm,tab,xml}
+                        output format (default: pot)
+  --mp4-charset MP4_CHARSET
+                        input chapter charset for mp4 file, since it can't be auto detected (default: utf-8)
+  --charset CHARSET     output file charset (default: utf-8-sig)
+  -o OUTPUT, --output OUTPUT
+                        output filename (default: original_filename.format[.txt])
+  -c, --clipboard       automatically process text in clipboard and save it back.
+```
+
+If you prefer a single file than a package, you can just download `chapter_converter.py` in `chapter_converter/` and use it directly (`chapter_converter.py -h`).
+
+A simple GUI is also provided as-is by running `chapgui`. You need to install module `gooey` in `pip` manually to make it work. See [my comments](https://github.com/fireattack/chapter_converter/pull/4#issuecomment-1359129224) for some caveats.
+
+As a Python module:
+
+```python
+from chapter_converter import chapter_converter
+
+chapter_converter.main('input.pbf', '-o', 'output.xml')
+```
+
+### Note
+
+* Output by default saved as UTF-8-BOM for max compatibility on Windows. You can change it by passing in `--charset` argument.
+* When `-c` is used, you can still pass in a file as input instead.
+* When `-c` is used, you can still pass in an output filename (using `-o` and/or `-f`) as output instead.
+
+## Supported formats
+
+See also: example files in `examples/`.
+
+### MKV and MP4 video containers (inputs only)
+
+Guessed by suffix. Not idiot-proof, please only feed in file with chapters.
+
+### Simple format (`simple`)
+
+I made it up.
+
+Format:
+* Each line: `{timestamp},{title}`
+
+Example:
+
+```
+0:17:02.148,Title1
+0:42:19.976,Title2
+0:58:10.114,Title3
+...
+```
+
+### Tab format (`tab`)
+
+Similar to Simple, but separated by tab instead of comma.
+
+Format:
+* Each line: `{timestamp}	{title}`
+
+Example:
+
+```
+0:17:02.148	Title1
+0:42:19.976	Title2
+0:58:10.114	Title3
+...
+```
+
+### OGM format (`ogm`)
+
+Can be recognized by common video tools, such as [MKVToolNix](https://mkvtoolnix.download/).
+
+Format:
+* Odd lines: `CHAPTER{i:02}={timestamp}`
+* Even lines: `CHAPTER{i:02}NAME={tilte}`
+
+`i` starts at 1.
+
+Example:
+
+```
+CHAPTER01=0:17:02.148
+CHAPTER01NAME=Title1
+CHAPTER02=0:42:19.976
+CHAPTER02NAME=Title2
+CHAPTER03=0:58:10.114
+...
+```
+
+### MediaInfo format (`mediainfo`)
+
+The way [MediaInfo](https://mediaarea.net/en/MediaInfo) presents chapter information in text form. Input only. Supports both with or without the "Menu" line.
+
+Format:
+* Each line: `{timestamp}\s+: ({two_letter_lang_code})?:{title}`
+
+Example:
+
+```
+Menu
+00:00:00.000                : en:Contours
+00:02:49.624                : en:From the Sea
+00:08:41.374                : en:Bread and Wine
+00:12:18.041                : en:Faceless
+...
+```
+
+### XML format (`xml`)
+
+XML chapter format defined by [Matroska specification](https://matroska.org/technical/specs/chapters/index.html).
+
+###  [PotPlayer](https://potplayer.daum.net/) Bookmark format (.pbf) (`pot`)
+
+A format PotPlayer uses for its bookmarks. If you put the file together with the video file (same name except extension, just like any external resources), it will be recognized by PotPlayer just like internal chapters - you can use "H" to view and select, and they will show up as markers on navigation bar too:
+
+![Pot Bookmark Example](https://raw.githubusercontent.com/fireattack/chapter_converter/master/img/pot.png)
+
+It is not ideal, but it's the closest thing to "external chapter file" to my knowledge.
+
+Format:
+
+* First line: `[Bookmark]`
+* Other lines: `{i}={timestamp_in_ms}*{title}*{some_optional_hash_for_pot_internal_usage}`
+
+`i` starts at 0.
+
+Example:
+
+```
+[Bookmark]
+0=1022148*Title1*
+1=2539976*Titile2*
+...
+```
```

### Comparing `chapter_converter-1.1.1/chapter_converter/chapter_converter.py` & `chapter_converter-1.2.0/chapter_converter/chapter_converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,221 +1,215 @@
-import argparse
-import datetime
-import re
-from os import remove
-from os.path import exists, splitext
-from subprocess import run
-
-import chardet
-import win32clipboard
-
-
-def get_clipboard_data():
-    win32clipboard.OpenClipboard()
-    data = win32clipboard.GetClipboardData(win32clipboard.CF_UNICODETEXT)
-    win32clipboard.CloseClipboard()
-    return data
-
-
-def set_clipboard_data(data: str):
-    win32clipboard.OpenClipboard()
-    win32clipboard.EmptyClipboard()
-    win32clipboard.SetClipboardText(data, win32clipboard.CF_UNICODETEXT)
-    win32clipboard.CloseClipboard()
-
-
-def ms_to_timestamp(ms_str: str):
-    ms = int(ms_str)
-    return f'{datetime.timedelta(seconds=ms//1000)}.{ms % 1000:03d}'
-
-
-def timestamp_to_ms(timestamp: str):
-    '''acceptable timestamp format: [00:]00:00[.000]'''
-    if timestamp.count(':') == 1:
-        timestamp = f'00:{timestamp}'
-    if '.' not in timestamp:
-        timestamp += '.000'
-    h, m, s, ms = re.split('[:.]', timestamp)
-    ms = ms.ljust(3, '0')[:3]
-    return str(1000 * (int(h) * 3600 + int(m) * 60 + int(s)) + int(ms))
-
-
-def load_file_content(filename: str):
-    # Detect file encoding
-    with open(filename, 'rb') as file:
-        raw = file.read()
-        encoding = chardet.detect(raw)['encoding']
-    # Detect format of input file
-    with open(filename, encoding=encoding) as f:
-        return f.readlines()
-
-
-def extract_and_read_chapters():
-    run(['mkvextract', 'temp.mks', 'chapters', '-s', 'temp.ogm.txt'])
-    result = load_file_content('temp.ogm.txt')
-    remove('temp.mks')
-    remove('temp.ogm.txt')
-    return result
-
-
-def get_output_filename(args: argparse.Namespace):
-    if args.output:
-        new_filename = args.output
-        assert isinstance(new_filename, str) # For type checking
-    elif args.format == 'pot':
-        new_filename = f'{splitext(args.filename)[0]}.pbf'
-    elif args.format == 'xml':
-        new_filename = f'{splitext(args.filename)[0]}.xml'
-    else:
-        new_filename = f'{splitext(args.filename)[0]}.{args.format}.txt'
-    # Ensure to not override existing file(s)
-    i = 2
-    stem = splitext(new_filename)[0]
-    ext = splitext(new_filename)[1]
-    while exists(new_filename):
-        new_filename = f'{stem} ({i}){ext}'
-        i += 1
-    return new_filename
-
-
-def args_parser():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("filename", nargs='?', help="input filename")
-    parser.add_argument("-f", "--format", choices=['simple', 'pot', 'ogm', 'tab', 'xml'], help="output format (default: pot)")
-    parser.add_argument("--mp4-charset", default='utf-8', help="input chapter charset for mp4 file, since it can't be auto detected (default: utf-8)")
-    parser.add_argument("--charset", default='utf-8-sig', help="output file charset (default: utf-8-sig)")
-    parser.add_argument("-o", "--output", help="output filename (default: original_filename.format[.txt])")
-    parser.add_argument('-c', '--clipboard', action='store_true', help='automatically process text in clipboard and save it back.')
-    return parser
-
-
-def main(*paras):
-    parser = args_parser()
-    if paras:
-        paras = list(map(str, paras))
-        args = parser.parse_args(paras)
-    else:
-        args = parser.parse_args()
-
-    # Input handling, get lines
-    if args.filename and exists(args.filename):
-        lower_ext = splitext(args.filename)[1].lower()
-        if lower_ext == '.xml':
-            run(['mkvmerge', '-o', 'temp.mks', '--chapters', args.filename])
-            lines = extract_and_read_chapters()
-        elif lower_ext in ['.mp4', '.mkv']:
-            run(['mkvmerge', '-o', 'temp.mks', '-A', '-D', '--chapter-charset', args.mp4_charset, args.filename])
-            lines = extract_and_read_chapters()
-        else:
-            lines = load_file_content(args.filename)
-    elif args.clipboard:
-        f = get_clipboard_data()
-        if f:
-            print('Get data from clipboard:')
-            print(f)
-            lines = f.splitlines()
-        else:
-            print('No valid input data in clipboard!')
-            return 0
-    else:
-        print('Input file missing or invalid!')
-        return 0
-    # Strip every line and remove empty lines
-    lines = [line.strip() for line in lines if line.strip()]
-
-    # Detect input format
-    input_format = ''
-    MEDIAINFO_RE = r"([0-9:.]+?)\s+:\s[a-z]{0,2}:(.+)"
-    HUMAN_RE = r"(?P<time>\d+:\d{1,2}[0-9:.]*)(,?\s*)(?P<name>.+)"
-    if re.match(HUMAN_RE, lines[0]):
-        input_format = 'human'
-    elif re.match(r"CHAPTER\d", lines[0]):
-        input_format = 'ogm'
-    elif lines[0].startswith('[Bookmark]'):
-        input_format = 'pot'
-    elif lines[0].startswith('Menu') and re.match(MEDIAINFO_RE, lines[1]):
-        lines = lines[1:]
-        input_format = 'mediainfo'
-    elif re.match(MEDIAINFO_RE, lines[0]):
-        input_format = 'mediainfo'
-    if not input_format:
-        print("Can't guess file format!")
-        return 0
-
-    # Input text parsing
-    chapters = []
-    if input_format == 'human':
-        for line in lines:
-            m = re.match(HUMAN_RE, line)
-            if m:
-                timestamp = ms_to_timestamp(timestamp_to_ms(m['time'])) # normalize timestamp
-                name = m['name']
-                chapters.append((timestamp, name))
-    elif input_format == 'ogm':
-        chapters = [(lines[i].split('=')[1], lines[i + 1].split('=')[1])
-                    for i in range(0, len(lines), 2)]
-    elif input_format == 'pot':
-        for line in lines[1:]:
-            m = re.match(r'\d+=(\d+)\*([^*]+)', line)
-            if m:
-                timestamp = ms_to_timestamp(m[1])
-                chapters.append((timestamp, m[2]))
-    elif input_format == 'mediainfo':
-        for line in lines:
-            m = re.match(MEDIAINFO_RE, line)
-            if m:
-                chapters.append((m[1], m[2]))
-
-    # Set default output format if not specified.
-    if not args.format:
-        args.format = 'pot' # Default to pot
-        if args.clipboard:
-            args.format = 'tab' # Default to "tab" if getting from clipboard for spreadsheet editing.
-        if args.output: # Get output format from output filename, if specified.
-            lower_ext = splitext(args.output)[-1].lower()
-            if lower_ext == '.pbf':
-                args.format = 'pot'
-            elif lower_ext == '.xml':
-                args.format = 'xml'
-            elif lower_ext == '.txt':
-                args.format = 'ogm'
-
-    # Generate output text
-    output = ''
-    if args.format == 'tab':
-        for time, title in chapters:
-            output += f'{time}\t{title}\n'
-    elif args.format == 'simple':
-        for time, title in chapters:
-            output += f'{time},{title}\n'
-    elif args.format in ['ogm', 'xml']:
-        for i, (time, title) in enumerate(chapters, start=1):
-            output += f'CHAPTER{i:02}={time}\n'
-            output += f'CHAPTER{i:02}NAME={title}\n'
-    elif args.format == 'pot':
-        output += '[Bookmark]\n'
-        for i, (time, title) in enumerate(chapters):
-            output += f'{i}={timestamp_to_ms(time)}*{title}*\n'
-
-    # Output to clipboard if no output is specified
-    if args.clipboard and not args.output:
-        print('Set data to clipboard:')
-        print(output)
-        set_clipboard_data(output.replace('\n', '\r\n'))
-    # Output to file iff output filename is specified or not clipboard mode.
-    else:
-        new_filename = get_output_filename(args)
-        print(f'Write to file: {new_filename}')
-        if args.format == 'xml':
-            with open('temp.ogm.txt', 'w', encoding=args.charset) as f:
-                f.write(output)
-            run(['mkvmerge', '-o', 'temp.mks', '--chapters', 'temp.ogm.txt'])
-            run(['mkvextract', 'temp.mks', 'chapters', new_filename])
-            remove('temp.mks')
-            remove('temp.ogm.txt')
-        else:
-            with open(new_filename, 'w', encoding=args.charset) as f:
-                f.write(output)
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import datetime
+import re
+from os import remove
+from os.path import exists, splitext
+from subprocess import run
+
+import chardet
+import pyperclip
+
+
+def get_clipboard_data():
+    return pyperclip.paste()
+
+
+def set_clipboard_data(data: str):
+    pyperclip.copy(data)
+
+
+def ms_to_timestamp(ms_str: str):
+    ms = int(ms_str)
+    return f'{datetime.timedelta(seconds=ms//1000)}.{ms % 1000:03d}'
+
+
+def timestamp_to_ms(timestamp: str):
+    '''acceptable timestamp format: [00:]00:00[.000]'''
+    if timestamp.count(':') == 1:
+        timestamp = f'00:{timestamp}'
+    if '.' not in timestamp:
+        timestamp += '.000'
+    h, m, s, ms = re.split('[:.]', timestamp)
+    ms = ms.ljust(3, '0')[:3]
+    return str(1000 * (int(h) * 3600 + int(m) * 60 + int(s)) + int(ms))
+
+
+def load_file_content(filename: str):
+    # Detect file encoding
+    with open(filename, 'rb') as file:
+        raw = file.read()
+        encoding = chardet.detect(raw)['encoding']
+    # Detect format of input file
+    with open(filename, encoding=encoding) as f:
+        return f.readlines()
+
+
+def extract_and_read_chapters():
+    run(['mkvextract', 'temp.mks', 'chapters', '-s', 'temp.ogm.txt'])
+    result = load_file_content('temp.ogm.txt')
+    remove('temp.mks')
+    remove('temp.ogm.txt')
+    return result
+
+
+def get_output_filename(args: argparse.Namespace):
+    if args.output:
+        new_filename = args.output
+        assert isinstance(new_filename, str) # For type checking
+    elif args.format == 'pot':
+        new_filename = f'{splitext(args.filename)[0]}.pbf'
+    elif args.format == 'xml':
+        new_filename = f'{splitext(args.filename)[0]}.xml'
+    else:
+        new_filename = f'{splitext(args.filename)[0]}.{args.format}.txt'
+    # Ensure to not override existing file(s)
+    i = 2
+    stem = splitext(new_filename)[0]
+    ext = splitext(new_filename)[1]
+    while exists(new_filename):
+        new_filename = f'{stem} ({i}){ext}'
+        i += 1
+    return new_filename
+
+
+def args_parser():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("filename", nargs='?', help="input filename")
+    parser.add_argument("-f", "--format", choices=['simple', 'pot', 'ogm', 'tab', 'xml'], help="output format (default: pot)")
+    parser.add_argument("--mp4-charset", default='utf-8', help="input chapter charset for mp4 file, since it can't be auto detected (default: utf-8)")
+    parser.add_argument("--charset", default='utf-8-sig', help="output file charset (default: utf-8-sig)")
+    parser.add_argument("-o", "--output", help="output filename (default: original_filename.format[.txt])")
+    parser.add_argument('-c', '--clipboard', action='store_true', help='automatically process text in clipboard and save it back.')
+    return parser
+
+
+def main(*paras):
+    parser = args_parser()
+    if paras:
+        paras = list(map(str, paras))
+        args = parser.parse_args(paras)
+    else:
+        args = parser.parse_args()
+
+    # Input handling, get lines
+    if args.filename and exists(args.filename):
+        lower_ext = splitext(args.filename)[1].lower()
+        if lower_ext == '.xml':
+            run(['mkvmerge', '-o', 'temp.mks', '--chapters', args.filename])
+            lines = extract_and_read_chapters()
+        elif lower_ext in ['.mp4', '.mkv']:
+            run(['mkvmerge', '-o', 'temp.mks', '-A', '-D', '--chapter-charset', args.mp4_charset, args.filename])
+            lines = extract_and_read_chapters()
+        else:
+            lines = load_file_content(args.filename)
+    elif args.clipboard:
+        f = get_clipboard_data()
+        if f:
+            print('Get data from clipboard:')
+            print(f)
+            lines = f.splitlines()
+        else:
+            print('No valid input data in clipboard!')
+            return 0
+    else:
+        print('Input file missing or invalid!')
+        return 0
+    # Strip every line and remove empty lines
+    lines = [line.strip() for line in lines if line.strip()]
+
+    # Detect input format
+    input_format = ''
+    MEDIAINFO_RE = r"([0-9:.]+?)\s+:\s[a-z]{0,2}:(.+)"
+    HUMAN_RE = r"(?P<time>\d+:\d{1,2}[0-9:.]*)(,?\s*)(?P<name>.+)"
+    if re.match(HUMAN_RE, lines[0]):
+        input_format = 'human'
+    elif re.match(r"CHAPTER\d", lines[0]):
+        input_format = 'ogm'
+    elif lines[0].startswith('[Bookmark]'):
+        input_format = 'pot'
+    elif lines[0].startswith('Menu') and re.match(MEDIAINFO_RE, lines[1]):
+        lines = lines[1:]
+        input_format = 'mediainfo'
+    elif re.match(MEDIAINFO_RE, lines[0]):
+        input_format = 'mediainfo'
+    if not input_format:
+        print("Can't guess file format!")
+        return 0
+
+    # Input text parsing
+    chapters = []
+    if input_format == 'human':
+        for line in lines:
+            m = re.match(HUMAN_RE, line)
+            if m:
+                timestamp = ms_to_timestamp(timestamp_to_ms(m['time'])) # normalize timestamp
+                name = m['name']
+                chapters.append((timestamp, name))
+    elif input_format == 'ogm':
+        chapters = [(lines[i].split('=')[1], lines[i + 1].split('=')[1])
+                    for i in range(0, len(lines), 2)]
+    elif input_format == 'pot':
+        for line in lines[1:]:
+            m = re.match(r'\d+=(\d+)\*([^*]+)', line)
+            if m:
+                timestamp = ms_to_timestamp(m[1])
+                chapters.append((timestamp, m[2]))
+    elif input_format == 'mediainfo':
+        for line in lines:
+            m = re.match(MEDIAINFO_RE, line)
+            if m:
+                chapters.append((m[1], m[2]))
+
+    # Set default output format if not specified.
+    if not args.format:
+        args.format = 'pot' # Default to pot
+        if args.clipboard:
+            args.format = 'tab' # Default to "tab" if getting from clipboard for spreadsheet editing.
+        if args.output: # Get output format from output filename, if specified.
+            lower_ext = splitext(args.output)[-1].lower()
+            if lower_ext == '.pbf':
+                args.format = 'pot'
+            elif lower_ext == '.xml':
+                args.format = 'xml'
+            elif lower_ext == '.txt':
+                args.format = 'ogm'
+
+    # Generate output text
+    output = ''
+    if args.format == 'tab':
+        for time, title in chapters:
+            output += f'{time}\t{title}\n'
+    elif args.format == 'simple':
+        for time, title in chapters:
+            output += f'{time},{title}\n'
+    elif args.format in ['ogm', 'xml']:
+        for i, (time, title) in enumerate(chapters, start=1):
+            output += f'CHAPTER{i:02}={time}\n'
+            output += f'CHAPTER{i:02}NAME={title}\n'
+    elif args.format == 'pot':
+        output += '[Bookmark]\n'
+        for i, (time, title) in enumerate(chapters):
+            output += f'{i}={timestamp_to_ms(time)}*{title}*\n'
+
+    # Output to clipboard if no output is specified
+    if args.clipboard and not args.output:
+        print('Set data to clipboard:')
+        print(output)
+        set_clipboard_data(output.replace('\n', '\r\n'))
+    # Output to file iff output filename is specified or not clipboard mode.
+    else:
+        new_filename = get_output_filename(args)
+        print(f'Write to file: {new_filename}')
+        if args.format == 'xml':
+            with open('temp.ogm.txt', 'w', encoding=args.charset) as f:
+                f.write(output)
+            run(['mkvmerge', '-o', 'temp.mks', '--chapters', 'temp.ogm.txt'])
+            run(['mkvextract', 'temp.mks', 'chapters', new_filename])
+            remove('temp.mks')
+            remove('temp.ogm.txt')
+        else:
+            with open(new_filename, 'w', encoding=args.charset) as f:
+                f.write(output)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `chapter_converter-1.1.1/chapter_converter.egg-info/PKG-INFO` & `chapter_converter-1.2.0/chapter_converter.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-Metadata-Version: 2.1
-Name: chapter-converter
-Version: 1.1.1
-Summary: Convert between several different video chapter file formats with ease.
-Home-page: https://github.com/fireattack/chapter_converter
-Author: fireattack
-Author-email: 
-License: MIT
-Project-URL: Source, https://github.com/fireattack/chapter_converter
-Project-URL: Tracker, https://github.com/fireattack/chapter_converter/issues
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
-
-[![PyPI Version](https://img.shields.io/pypi/v/chapter-converter.svg)](https://pypi.python.org/pypi/chapter-converter)
-
-# chapter_converter
-Convert between several different video chapter file formats with ease.
-
-## Features
-
-* Auto input format detection: including chapter files and video files with chapters (`.mkv` and `.mp4`. Requires `mkvtoolnix` binaries in path).
-* Auto input encoding detection
-* Can specify output format and filename
-* Clipboard support (input and output) for editing purposes
-
-## Install
-
-```
-pip install -U chapter_converter
-```
-or from source:
-```
-pip install -U git+https://github.com/fireattack/chapter_converter
-```
-
-## Usage
-
-CLI script is named `chap`. Or you can use `python -m chapter_converter`.
-
-```
-usage: chap [-h] [-f {simple,pot,ogm,tab,xml}] [--mp4-charset MP4_CHARSET] [--charset CHARSET] [-o OUTPUT] [-c] [filename]
-
-positional arguments:
-  filename              input filename
-
-options:
-  -h, --help            show this help message and exit
-  -f {simple,pot,ogm,tab,xml}, --format {simple,pot,ogm,tab,xml}
-                        output format (default: pot)
-  --mp4-charset MP4_CHARSET
-                        input chapter charset for mp4 file, since it can't be auto detected (default: utf-8)
-  --charset CHARSET     output file charset (default: utf-8-sig)
-  -o OUTPUT, --output OUTPUT
-                        output filename (default: original_filename.format[.txt])
-  -c, --clipboard       automatically process text in clipboard and save it back.
-```
-
-If you prefer a single file than a package, you can just download `chapter_converter.py` in `chapter_converter/` and use it directly (`chapter_converter.py -h`).
-
-A simple GUI is also provided as-is by running `chapgui`. You need to install module `gooey` in `pip` manually to make it work. See [my comments](https://github.com/fireattack/chapter_converter/pull/4#issuecomment-1359129224) for some caveats.
-
-As a Python module:
-
-```python
-from chapter_converter import chapter_converter
-
-chapter_converter.main('input.pbf', '-o', 'output.xml')
-```
-
-### Note
-
-* Output by default saved as UTF-8-BOM for max compatibility on Windows. You can change it by passing in `--charset` argument.
-* When `-c` is used, you can still pass in a file as input instead.
-* When `-c` is used, you can still pass in an output filename (using `-o` and/or `-f`) as output instead.
-
-## Supported formats
-
-See also: example files in `examples/`.
-
-### MKV and MP4 video containers (inputs only)
-
-Guessed by suffix. Not idiot-proof, please only feed in file with chapters.
-
-### Simple format (`simple`)
-
-I made it up.
-
-Format:
-* Each line: `{timestamp},{title}`
-
-Example:
-
-```
-0:17:02.148,Title1
-0:42:19.976,Title2
-0:58:10.114,Title3
-...
-```
-
-### Tab format (`tab`)
-
-Similar to Simple, but separated by tab instead of comma.
-
-Format:
-* Each line: `{timestamp}	{title}`
-
-Example:
-
-```
-0:17:02.148	Title1
-0:42:19.976	Title2
-0:58:10.114	Title3
-...
-```
-
-### OGM format (`ogm`)
-
-Can be recognized by common video tools, such as [MKVToolNix](https://mkvtoolnix.download/).
-
-Format:
-* Odd lines: `CHAPTER{i:02}={timestamp}`
-* Even lines: `CHAPTER{i:02}NAME={tilte}`
-
-`i` starts at 1.
-
-Example:
-
-```
-CHAPTER01=0:17:02.148
-CHAPTER01NAME=Title1
-CHAPTER02=0:42:19.976
-CHAPTER02NAME=Title2
-CHAPTER03=0:58:10.114
-...
-```
-
-### MediaInfo format (`mediainfo`)
-
-The way [MediaInfo](https://mediaarea.net/en/MediaInfo) presents chapter information in text form. Input only. Supports both with or without the "Menu" line.
-
-Format:
-* Each line: `{timestamp}\s+: ({two_letter_lang_code})?:{title}`
-
-Example:
-
-```
-Menu
-00:00:00.000                : en:Contours
-00:02:49.624                : en:From the Sea
-00:08:41.374                : en:Bread and Wine
-00:12:18.041                : en:Faceless
-...
-```
-
-### XML format (`xml`)
-
-XML chapter format defined by [Matroska specification](https://matroska.org/technical/specs/chapters/index.html).
-
-###  [PotPlayer](https://potplayer.daum.net/) Bookmark format (.pbf) (`pot`)
-
-A format PotPlayer uses for its bookmarks. If you put the file together with the video file (same name except extension, just like any external resources), it will be recognized by PotPlayer just like internal chapters - you can use "H" to view and select, and they will show up as markers on navigation bar too:
-
-![Pot Bookmark Example](https://raw.githubusercontent.com/fireattack/chapter_converter/master/img/pot.png)
-
-It is not ideal, but it's the closest thing to "external chapter file" to my knowledge.
-
-Format:
-
-* First line: `[Bookmark]`
-* Other lines: `{i}={timestamp_in_ms}*{title}*{some_optional_hash_for_pot_internal_usage}`
-
-`i` starts at 0.
-
-Example:
-
-```
-[Bookmark]
-0=1022148*Title1*
-1=2539976*Titile2*
-...
-```
+Metadata-Version: 2.1
+Name: chapter-converter
+Version: 1.2.0
+Summary: Convert between several different video chapter file formats with ease.
+Home-page: https://github.com/fireattack/chapter_converter
+Author: fireattack
+Author-email: 
+License: MIT
+Project-URL: Source, https://github.com/fireattack/chapter_converter
+Project-URL: Tracker, https://github.com/fireattack/chapter_converter/issues
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+[![PyPI Version](https://img.shields.io/pypi/v/chapter-converter.svg)](https://pypi.python.org/pypi/chapter-converter)
+
+# chapter_converter
+Convert between several different video chapter file formats with ease.
+
+## Features
+
+* Auto input format detection: including chapter files and video files with chapters (`.mkv` and `.mp4`. Requires `mkvtoolnix` binaries in path).
+* Auto input encoding detection
+* Can specify output format and filename
+* Clipboard support (input and output) for editing purposes
+
+## Install
+
+```
+pip install -U chapter_converter
+```
+or from source:
+```
+pip install -U git+https://github.com/fireattack/chapter_converter
+```
+
+## Usage
+
+CLI script is named `chap`. Or you can use `python -m chapter_converter`.
+
+```
+usage: chap [-h] [-f {simple,pot,ogm,tab,xml}] [--mp4-charset MP4_CHARSET] [--charset CHARSET] [-o OUTPUT] [-c] [filename]
+
+positional arguments:
+  filename              input filename
+
+options:
+  -h, --help            show this help message and exit
+  -f {simple,pot,ogm,tab,xml}, --format {simple,pot,ogm,tab,xml}
+                        output format (default: pot)
+  --mp4-charset MP4_CHARSET
+                        input chapter charset for mp4 file, since it can't be auto detected (default: utf-8)
+  --charset CHARSET     output file charset (default: utf-8-sig)
+  -o OUTPUT, --output OUTPUT
+                        output filename (default: original_filename.format[.txt])
+  -c, --clipboard       automatically process text in clipboard and save it back.
+```
+
+If you prefer a single file than a package, you can just download `chapter_converter.py` in `chapter_converter/` and use it directly (`chapter_converter.py -h`).
+
+A simple GUI is also provided as-is by running `chapgui`. You need to install module `gooey` in `pip` manually to make it work. See [my comments](https://github.com/fireattack/chapter_converter/pull/4#issuecomment-1359129224) for some caveats.
+
+As a Python module:
+
+```python
+from chapter_converter import chapter_converter
+
+chapter_converter.main('input.pbf', '-o', 'output.xml')
+```
+
+### Note
+
+* Output by default saved as UTF-8-BOM for max compatibility on Windows. You can change it by passing in `--charset` argument.
+* When `-c` is used, you can still pass in a file as input instead.
+* When `-c` is used, you can still pass in an output filename (using `-o` and/or `-f`) as output instead.
+
+## Supported formats
+
+See also: example files in `examples/`.
+
+### MKV and MP4 video containers (inputs only)
+
+Guessed by suffix. Not idiot-proof, please only feed in file with chapters.
+
+### Simple format (`simple`)
+
+I made it up.
+
+Format:
+* Each line: `{timestamp},{title}`
+
+Example:
+
+```
+0:17:02.148,Title1
+0:42:19.976,Title2
+0:58:10.114,Title3
+...
+```
+
+### Tab format (`tab`)
+
+Similar to Simple, but separated by tab instead of comma.
+
+Format:
+* Each line: `{timestamp}	{title}`
+
+Example:
+
+```
+0:17:02.148	Title1
+0:42:19.976	Title2
+0:58:10.114	Title3
+...
+```
+
+### OGM format (`ogm`)
+
+Can be recognized by common video tools, such as [MKVToolNix](https://mkvtoolnix.download/).
+
+Format:
+* Odd lines: `CHAPTER{i:02}={timestamp}`
+* Even lines: `CHAPTER{i:02}NAME={tilte}`
+
+`i` starts at 1.
+
+Example:
+
+```
+CHAPTER01=0:17:02.148
+CHAPTER01NAME=Title1
+CHAPTER02=0:42:19.976
+CHAPTER02NAME=Title2
+CHAPTER03=0:58:10.114
+...
+```
+
+### MediaInfo format (`mediainfo`)
+
+The way [MediaInfo](https://mediaarea.net/en/MediaInfo) presents chapter information in text form. Input only. Supports both with or without the "Menu" line.
+
+Format:
+* Each line: `{timestamp}\s+: ({two_letter_lang_code})?:{title}`
+
+Example:
+
+```
+Menu
+00:00:00.000                : en:Contours
+00:02:49.624                : en:From the Sea
+00:08:41.374                : en:Bread and Wine
+00:12:18.041                : en:Faceless
+...
+```
+
+### XML format (`xml`)
+
+XML chapter format defined by [Matroska specification](https://matroska.org/technical/specs/chapters/index.html).
+
+###  [PotPlayer](https://potplayer.daum.net/) Bookmark format (.pbf) (`pot`)
+
+A format PotPlayer uses for its bookmarks. If you put the file together with the video file (same name except extension, just like any external resources), it will be recognized by PotPlayer just like internal chapters - you can use "H" to view and select, and they will show up as markers on navigation bar too:
+
+![Pot Bookmark Example](https://raw.githubusercontent.com/fireattack/chapter_converter/master/img/pot.png)
+
+It is not ideal, but it's the closest thing to "external chapter file" to my knowledge.
+
+Format:
+
+* First line: `[Bookmark]`
+* Other lines: `{i}={timestamp_in_ms}*{title}*{some_optional_hash_for_pot_internal_usage}`
+
+`i` starts at 0.
+
+Example:
+
+```
+[Bookmark]
+0=1022148*Title1*
+1=2539976*Titile2*
+...
+```
```

