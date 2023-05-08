# Comparing `tmp/video-subtitles-1.0.0.tar.gz` & `tmp/video-subtitles-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-subtitles-1.0.0.tar", last modified: Mon May  8 22:38:18 2023, max compression
+gzip compressed data, was "video-subtitles-1.0.1.tar", last modified: Mon May  8 23:54:02 2023, max compression
```

## Comparing `video-subtitles-1.0.0.tar` & `video-subtitles-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.615620 video-subtitles-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.538620 video-subtitles-1.0.0/.github/
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.564621 video-subtitles-1.0.0/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      801 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      803 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      800 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     2059 2023-05-08 22:03:27.000000 video-subtitles-1.0.0/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.568620 video-subtitles-1.0.0/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/.vscode/launch.json
--rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1385 2023-05-08 22:38:18.614620 video-subtitles-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      687 2023-05-08 03:53:14.000000 video-subtitles-1.0.0/README.md
--rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.0/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/make_venv.py
--rw-rw-rw-   0        0        0      723 2023-05-08 20:43:38.000000 video-subtitles-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       47 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 22:38:18.615620 video-subtitles-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.541622 video-subtitles-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.575620 video-subtitles-1.0.0/src/video_subtitles/
--rw-rw-rw-   0        0        0       34 2023-05-08 10:03:48.000000 video-subtitles-1.0.0/src/video_subtitles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.606620 video-subtitles-1.0.0/src/video_subtitles/assets/
--rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/src/video_subtitles/assets/example.txt
--rw-rw-rw-   0        0        0     3960 2023-05-08 22:35:30.000000 video-subtitles-1.0.0/src/video_subtitles/cli.py
--rw-rw-rw-   0        0        0     2344 2023-05-08 22:35:30.000000 video-subtitles-1.0.0/src/video_subtitles/run.py
--rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.0/src/video_subtitles/translate.py
--rw-rw-rw-   0        0        0     2373 2023-05-08 10:07:09.000000 video-subtitles-1.0.0/src/video_subtitles/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.604620 video-subtitles-1.0.0/src/video_subtitles.egg-info/
--rw-rw-rw-   0        0        0     1385 2023-05-08 22:38:18.000000 video-subtitles-1.0.0/src/video_subtitles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      862 2023-05-08 22:38:18.000000 video-subtitles-1.0.0/src/video_subtitles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 22:38:18.000000 video-subtitles-1.0.0/src/video_subtitles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-08 22:38:18.000000 video-subtitles-1.0.0/src/video_subtitles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-05-08 22:38:18.000000 video-subtitles-1.0.0/src/video_subtitles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-08 22:38:18.000000 video-subtitles-1.0.0/src/video_subtitles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 22:38:18.612622 video-subtitles-1.0.0/tests/
--rw-rw-rw-   0        0        0      496 2023-05-08 22:35:30.000000 video-subtitles-1.0.0/tests/test_cli.py
--rw-rw-rw-   0        0        0      951 2023-05-08 22:35:30.000000 video-subtitles-1.0.0/tests/test_full.py
--rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.0/tests/test_srt_translator.py
--rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.0/tests/video.mp4
--rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/tox.ini
--rw-rw-rw-   0        0        0      291 2023-05-08 03:14:30.000000 video-subtitles-1.0.0/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.527949 video-subtitles-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.449946 video-subtitles-1.0.1/.github/
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.485947 video-subtitles-1.0.1/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.1/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.1/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.1/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     2059 2023-05-08 22:03:27.000000 video-subtitles-1.0.1/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.489945 video-subtitles-1.0.1/.vscode/
+-rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/.vscode/launch.json
+-rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5450 2023-05-08 23:54:02.527949 video-subtitles-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4660 2023-05-08 23:48:34.000000 video-subtitles-1.0.1/README.md
+-rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.1/activate.sh
+-rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/lint.sh
+-rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/make_venv.py
+-rw-rw-rw-   0        0        0      755 2023-05-08 23:34:23.000000 video-subtitles-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       66 2023-05-08 22:45:19.000000 video-subtitles-1.0.1/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 23:54:02.528947 video-subtitles-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.451947 video-subtitles-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.495946 video-subtitles-1.0.1/src/video_subtitles/
+-rw-rw-rw-   0        0        0       34 2023-05-08 23:47:55.000000 video-subtitles-1.0.1/src/video_subtitles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.519946 video-subtitles-1.0.1/src/video_subtitles/assets/
+-rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/src/video_subtitles/assets/example.txt
+-rw-rw-rw-   0        0        0     4199 2023-05-08 23:46:45.000000 video-subtitles-1.0.1/src/video_subtitles/cli.py
+-rw-rw-rw-   0        0        0     3071 2023-05-08 23:47:31.000000 video-subtitles-1.0.1/src/video_subtitles/run.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.1/src/video_subtitles/say.py
+-rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.1/src/video_subtitles/translate.py
+-rw-rw-rw-   0        0        0     2373 2023-05-08 10:07:09.000000 video-subtitles-1.0.1/src/video_subtitles/util.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.518947 video-subtitles-1.0.1/src/video_subtitles.egg-info/
+-rw-rw-rw-   0        0        0     5450 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.525947 video-subtitles-1.0.1/tests/
+-rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.1/tests/test_cli.py
+-rw-rw-rw-   0        0        0      951 2023-05-08 23:21:31.000000 video-subtitles-1.0.1/tests/test_full.py
+-rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.1/tests/test_srt_translator.py
+-rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.1/tests/video.mp4
+-rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/tox.ini
+-rw-rw-rw-   0        0        0      291 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/upload_package.sh
```

### Comparing `video-subtitles-1.0.0/.github/workflows/lint.yml` & `video-subtitles-1.0.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/.github/workflows/push_macos.yml` & `video-subtitles-1.0.1/.github/workflows/push_win.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-name: MacOS_Tests
+name: Win_Tests
 
 on: [push]
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python-version: [3.10.4]
-        os: [macos-latest]
+        os: [windows-latest]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - uses: actions/cache@v3
@@ -23,10 +23,11 @@
         restore-keys: |
           ${{ runner.os }}-pip-
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install .
         python -m pip install pytest
-    - name: Run Tests
+        python -m pip install -r requirements.testing.txt
+    - name: Run Test
       run: |
         pytest tests
```

### Comparing `video-subtitles-1.0.0/.github/workflows/push_ubuntu.yml` & `video-subtitles-1.0.1/.github/workflows/push_ubuntu.yml`

 * *Files 9% similar despite different names*

```diff
@@ -23,10 +23,11 @@
         restore-keys: |
           ${{ runner.os }}-pip-
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install .
         python -m pip install pytest
+        python -m pip install -r requirements.testing.txt
     - name: Run Tests
       run: |
         pytest tests
```

### Comparing `video-subtitles-1.0.0/.github/workflows/push_win.yml` & `video-subtitles-1.0.1/.github/workflows/push_macos.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-name: Win_Tests
+name: MacOS_Tests
 
 on: [push]
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python-version: [3.10.4]
-        os: [windows-latest]
+        os: [macos-latest]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - uses: actions/cache@v3
@@ -23,10 +23,11 @@
         restore-keys: |
           ${{ runner.os }}-pip-
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install .
         python -m pip install pytest
-    - name: Run Test
+        python -m pip install -r requirements.testing.txt
+    - name: Run Tests
       run: |
         pytest tests
```

### Comparing `video-subtitles-1.0.0/.gitignore` & `video-subtitles-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/.vscode/launch.json` & `video-subtitles-1.0.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/.vscode/settings.json` & `video-subtitles-1.0.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/.vscode/tasks.json` & `video-subtitles-1.0.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/LICENSE` & `video-subtitles-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/make_venv.py` & `video-subtitles-1.0.1/make_venv.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/pyproject.toml` & `video-subtitles-1.0.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 description = "Creates Video Subtitles"
 requires-python = ">=3.7"
 keywords = ["template-python-cmd"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "download",
-    "srtranslator"
+    "srtranslator",
+    "gTTS",
+    "playaudio",
 ]
 
 dynamic = ["version"]
 
 [tool.ruff]
 line-length = 200
```

### Comparing `video-subtitles-1.0.0/setup.py` & `video-subtitles-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/src/video_subtitles/cli.py` & `video-subtitles-1.0.1/src/video_subtitles/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import argparse
 import os
 import warnings
 
 from video_subtitles import __version__
 from video_subtitles.run import run
+from video_subtitles.say import say
 from video_subtitles.util import (
     LANGUAGE_CODES,
     MODELS,
     GraphicsInfo,
     ensure_transcribe_anything_installed,
     query_cuda_video_cards,
 )
@@ -75,14 +76,19 @@
     parser.add_argument(
         "--model",
         type=str,
         help="Model to use.",
         default="large",
         choices=MODELS.keys(),
     )
+    parser.add_argument(
+        "--quite",
+        action="store_true",
+        help="Don't say anything.",
+    )
     parser.add_argument("--api-key", default=None, help="Transcribe Anything API key.")
     args = parser.parse_args()
     if not args.languages:
         parser.error("You must provide at least one --languages")
     return args
 
 
@@ -122,14 +128,16 @@
             )
         run(
             file=file,
             deepl_api_key=api_key,
             out_languages=args.languages,
             model=args.model,
         )
+        if not args.quite:
+            say(f"Finished generating srt files for {file}")
     except KeyboardInterrupt:
         print("Exiting due to keyboard interrupt.")
         return 1
     return 0
 
 
 if __name__ == "__main__":
```

### Comparing `video-subtitles-1.0.0/src/video_subtitles/run.py` & `video-subtitles-1.0.1/src/video_subtitles/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 import shutil
 
 from transcribe_anything.api import transcribe
 
 from video_subtitles.translate import srt_wrap, translate
 
+IS_GITHUB = os.environ.get("GITHUB_ACTIONS", False)
+
 
 def find_srt_files(folder: str) -> list[str]:
     """Find srt files in a folder."""
     files = []
     # os walk
     for root, _, filenames in os.walk(folder):
         for filename in filenames:
@@ -29,40 +31,57 @@
     """Run the program."""
     print("Running transcription")
     out_languages = out_languages.copy()
     print(f"Output languages: {out_languages}")
     print(f"Model: {model}")
     print(f"File: {file}")
     print("Done running transcription")
-    out_en_dir = transcribe(url_or_file=file, device="cuda", model=model, language="en")
+    device = "cpu" if IS_GITHUB else "cuda"
+    out_en_dir = transcribe(url_or_file=file, device=device, model=model, language="en")
     print(f"Output directory: {out_en_dir}")
     if not os.path.exists(out_en_dir):
         raise RuntimeError(f"Error - folder does not exist: {out_en_dir}")
     if "en" in out_languages:
         out_languages.remove("en")
     src_srt_file = os.path.join(out_en_dir, "out.srt")
     assert os.path.exists(src_srt_file), f"Error - file does not exist: {src_srt_file}"
     outdir = os.path.dirname(out_en_dir)
     for language in out_languages:
         print(f"Translating to: {language}")
         out_folder = os.path.join(outdir, language)
         os.makedirs(out_folder, exist_ok=True)
         out_file = os.path.join(out_folder, "out.srt")
-        translate(
-            api_key=deepl_api_key,
-            in_srt=src_srt_file,
-            out_srt=out_file,
-            from_lang="en",
-            to_lang=language,
-        )
+        attempts = 5
+        for i in range(attempts):
+            if i > 0:
+                print("Retrying...")
+            try:
+                if os.path.exists(out_file):
+                    os.remove(out_file)
+                translate(
+                    api_key=deepl_api_key,
+                    in_srt=src_srt_file,
+                    out_srt=out_file,
+                    from_lang="en",
+                    to_lang=language,
+                )
+                assert os.path.exists(
+                    out_file
+                ), f"Error during translation of {language}: file does not exist: {out_file}"
+                break
+            except Exception as err:  # pylint: disable=broad-except
+                print(err)
+                if i == attempts - 1:
+                    raise
         print(f"Translated: {src_srt_file} -> {out_file}")
     srt_wrap(src_srt_file)
     srt_files = find_srt_files(outdir)
     print(f"Found {len(srt_files)} srt files")
     for srt_file in srt_files:
         language_name = os.path.basename(os.path.dirname(srt_file))
         out_file = os.path.join(outdir, f"{language_name}.srt")
         if os.path.exists(out_file):
             os.remove(out_file)
         shutil.move(srt_file, out_file)
         shutil.rmtree(os.path.dirname(srt_file))
+        break
     print("Done translating")
```

### Comparing `video-subtitles-1.0.0/src/video_subtitles/translate.py` & `video-subtitles-1.0.1/src/video_subtitles/translate.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/src/video_subtitles/util.py` & `video-subtitles-1.0.1/src/video_subtitles/util.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/src/video_subtitles.egg-info/SOURCES.txt` & `video-subtitles-1.0.1/src/video_subtitles.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 .github/workflows/push_win.yml
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 src/video_subtitles/__init__.py
 src/video_subtitles/cli.py
 src/video_subtitles/run.py
+src/video_subtitles/say.py
 src/video_subtitles/translate.py
 src/video_subtitles/util.py
 src/video_subtitles.egg-info/PKG-INFO
 src/video_subtitles.egg-info/SOURCES.txt
 src/video_subtitles.egg-info/dependency_links.txt
 src/video_subtitles.egg-info/entry_points.txt
 src/video_subtitles.egg-info/requires.txt
```

### Comparing `video-subtitles-1.0.0/tests/test_full.py` & `video-subtitles-1.0.1/tests/test_full.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def test_imports(self) -> None:
         """Test command line interface (CLI)."""
         shutil.rmtree("text_video", ignore_errors=True)
         run(
             file="video.mp4",
             deepl_api_key=None,
             out_languages=["es", "fr", "zh"],
-            model="large",
+            model="small",
         )
         self.assertTrue(os.path.exists("text_video"))
         self.assertTrue(os.path.exists(os.path.join("text_video", "en.srt")))
         self.assertTrue(os.path.exists(os.path.join("text_video", "es.srt")))
         self.assertTrue(os.path.exists(os.path.join("text_video", "fr.srt")))
         self.assertTrue(os.path.exists(os.path.join("text_video", "zh.srt")))
```

### Comparing `video-subtitles-1.0.0/tests/test_srt_translator.py` & `video-subtitles-1.0.1/tests/test_srt_translator.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.0/tests/video.mp4` & `video-subtitles-1.0.1/tests/video.mp4`

 * *Files identical despite different names*

