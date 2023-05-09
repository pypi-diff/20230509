# Comparing `tmp/clown_sort-1.3.3.tar.gz` & `tmp/clown_sort-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.3.3.tar", max compression
+gzip compressed data, was "clown_sort-1.4.0.tar", max compression
```

## Comparing `clown_sort-1.3.3.tar` & `clown_sort-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1999 2023-04-24 00:48:38.955951 clown_sort-1.3.3/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.3.3/LICENSE
--rw-r--r--   0        0        0     7617 2023-04-16 21:33:01.097803 clown_sort-1.3.3/README.md
--rw-r--r--   0        0        0     3294 2023-04-16 21:18:44.118253 clown_sort-1.3.3/clown_sort/__init__.py
--rw-r--r--   0        0        0     6991 2023-04-14 22:38:02.184270 clown_sort-1.3.3/clown_sort/config.py
--rw-r--r--   0        0        0     7530 2023-04-16 21:19:30.844002 clown_sort-1.3.3/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4260 2023-04-16 21:12:34.135691 clown_sort-1.3.3/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     1330 2023-04-24 00:42:15.932759 clown_sort-1.3.3/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0     9805 2023-04-16 21:08:33.938145 clown_sort-1.3.3/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3109 2023-04-14 22:23:25.165083 clown_sort-1.3.3/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     7489 2023-04-24 00:44:38.181699 clown_sort-1.3.3/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3298 2023-04-14 23:18:26.928346 clown_sort-1.3.3/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1455 2023-02-27 03:16:08.096928 clown_sort-1.3.3/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.3.3/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-02-27 01:29:17.019569 clown_sort-1.3.3/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.3.3/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.3.3/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      345 2023-04-16 20:51:08.331725 clown_sort-1.3.3/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1558 2023-04-24 00:48:38.962489 clown_sort-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     9177 1970-01-01 00:00:00.000000 clown_sort-1.3.3/setup.py
--rw-r--r--   0        0        0     8981 1970-01-01 00:00:00.000000 clown_sort-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2223 2023-05-09 18:21:24.058982 clown_sort-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.4.0/LICENSE
+-rw-r--r--   0        0        0     7617 2023-04-16 21:33:01.097803 clown_sort-1.4.0/README.md
+-rw-r--r--   0        0        0     3316 2023-04-24 00:56:40.931125 clown_sort-1.4.0/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7429 2023-05-09 18:20:37.529588 clown_sort-1.4.0/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-05-09 18:20:37.530028 clown_sort-1.4.0/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4745 2023-05-09 18:20:37.530359 clown_sort-1.4.0/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     1330 2023-04-24 00:42:15.932759 clown_sort-1.4.0/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    10796 2023-05-09 18:20:37.530660 clown_sort-1.4.0/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3139 2023-05-09 18:20:37.531050 clown_sort-1.4.0/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     8483 2023-05-09 18:20:37.531375 clown_sort-1.4.0/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.4.0/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.4.0/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.4.0/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-04-30 19:27:53.085722 clown_sort-1.4.0/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.4.0/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3354 2023-04-16 21:09:14.093347 clown_sort-1.4.0/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      520 2023-05-09 18:20:37.532239 clown_sort-1.4.0/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1558 2023-05-09 18:21:17.194294 clown_sort-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8981 1970-01-01 00:00:00.000000 clown_sort-1.4.0/PKG-INFO
```

### Comparing `clown_sort-1.3.3/CHANGELOG.md` & `clown_sort-1.4.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # NEXT RELEASE
 
+## 1.4.0
+* Add `--manual-fallback` option
+* Handle truncated image file binary errors
+* Display the string that matched the rule when copying
+* Better handling of re-scanning already sorted files
+* New crypto sorting rules
+
 ### 1.3.3
 * Handle more unparseable PDF issues more gracefully
 * New crypto sort rules
 
 ### 1.3.2
 * Make `--rescan-sorted` respect `--all` flag
 * Don't append empty string to images that no text was extracted from
```

### Comparing `clown_sort-1.3.3/LICENSE` & `clown_sort-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.3/README.md` & `clown_sort-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.3/clown_sort/__init__.py` & `clown_sort-1.4.0/clown_sort/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             load_dotenv(dotenv_path=dotenv_file)
             break
 
 from clown_sort.config import Config
 from clown_sort.files.image_file import ImageFile
 from clown_sort.files.pdf_file import PdfFile
 from clown_sort.files.sortable_file import SortableFile
-from clown_sort.sort_selector import process_file
+from clown_sort.sort_selector import process_file_with_popup
 from clown_sort.util.filesystem_helper import (IMAGE_FILE_EXTENSIONS, files_in_dir, is_image, is_pdf,
      set_timestamp_based_on_screenshot_filename)
 from clown_sort.util.logging import log
 from clown_sort.util.rich_helper import console
 
 
 def sort_screenshots():
@@ -32,15 +32,15 @@
 
     for image in screenshot_paths(Config.screenshots_dir):
         if Config.manual_sort:
             if not isinstance(image, ImageFile):
                 print(f"'{image.file_path}' is not suitable for manual sort, skipping...")
                 continue
 
-            process_file(image)
+            process_file_with_popup(image)
         else:
             image.sort_file()
 
 
 def set_screenshot_timestamps():
     Config.configure()
```

### Comparing `clown_sort-1.3.3/clown_sort/config.py` & `clown_sort-1.4.0/clown_sort/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     DEFAULT_RULES_CSV_PATHS = [CRYPTO_RULES_CSV_PATH]
 
 
 class Config:
     debug: bool = False
     dry_run: bool = True
     manual_sort: bool = False
+    manual_fallback: bool = False
     only_if_match: bool = False
     leave_in_place: bool = False
     screenshots_only: bool = True
     delete_originals: bool = False
     rescan_sorted: bool = False
     yes_overwrite: bool = False
     sort_rules: List[SortRule] = []
@@ -85,17 +86,21 @@
         else:
             print("Dry run...")
 
         if args.all:
             print("Processing all files in directory, not just 'Screenshot' files....")
             Config.screenshots_only = False
 
-        if args.manual_sort:
+        if args.manual_sort or args.manual_fallback:
             _check_for_pysimplegui()
-            Config.manual_sort = True
+
+            if args.manual_sort:
+                Config.manual_sort = True
+            if args.manual_fallback:
+                Config.manual_fallback = True
 
     @classmethod
     def set_directories(
             cls,
             screenshots_dir: StringOrPath,
             destination_dir: StringOrPath,
             rules_csv_paths: List[StringOrPath]
@@ -184,13 +189,16 @@
     if msg is None:
         msg = Text('WARNING: ', style='bright_red').append(
             f"Optional package '{module_name}' not installed. . Try running:",
             style='bright_white'
         )
 
     console = Console()
-    console.line(2)
+    console.line()
     console.print(msg)
-    console.line(2)
+    console.line()
     console.print(f"     pipx install clown_sort[{module_name}]", style='bright_cyan')
-    console.line(2)
-
+    console.line()
+    console.print(f"(or 'poetry install --all-extras' if you're in a development environment)")
+    console.line()
+    console.print(f"You make also need to install 'python-tk'.")
+    console.print("In macOS this can be installed with 'brew install python-tk'.")
```

### Comparing `clown_sort-1.3.3/clown_sort/filename_extractor.py` & `clown_sort-1.4.0/clown_sort/filename_extractor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Decide on a filename string based on some OCR text.
 """
 import re
+from difflib import SequenceMatcher
 from typing import Optional
 
 from rich.text import Text
 
 from clown_sort.util.logging import log
 from clown_sort.util.rich_helper import console
-from clown_sort.util.string_helper import strip_bad_chars
-
-MAX_FILENAME_LENGTH = 225
+from clown_sort.util.string_helper import strip_bad_chars, strip_mac_screenshot
 
 TWEET_REPLY_REGEX = re.compile(
     'Replying to (@\\w{3,15}).*?\\n(?P<body>.*)',
     re.DOTALL | re.MULTILINE
 )
 
 TWEET_REGEX = re.compile(
@@ -32,15 +31,19 @@
     re.DOTALL | re.MULTILINE | re.IGNORECASE
 )
 
 REVEDDIT_REGEX = re.compile('Reveddit Real.?Time')
 SUBREDDIT_REGEX = re.compile('/r/(?P<subreddit>\\w+)|\\sse(lf|ir)\\.(?P<subreddit2>\\w+)')
 DUNE_ANALYTICS_REGEX = re.compile('Query results (.*) @\\w+')
 RETWEETED_REGEX = re.compile('(.*) Retweeted')
+
+MAX_FILENAME_LENGTH = 225
 MIN_LENGTH_FOR_DUPE_CHECK = 9
+DEFAULT_LENGTH_FOR_LONG_FILENAMES = 150
+MIN_SIMILARITY_RATIO_TO_BE_SAME = 0.80
 
 
 class FilenameExtractor:
     def __init__(self, image_file: 'ImageFile') -> None:
         self.image_file = image_file
         self.text: Optional[str] = image_file.extracted_text()
         self.basename_length: int = len(image_file.basename)
@@ -60,37 +63,41 @@
             new_filename = filename_str + self.image_file.basename
         elif self._is_tweet() or self._is_reddit():
             if self._is_tweet():
                 filename_str = self._filename_str_for_tweet()
             else:
                 filename_str = self._filename_str_for_reddit()
 
+            filename_str = filename_str[0:-1] if filename_str.endswith('.') else filename_str
             filename = f"{filename_str} {self.image_file.basename_without_ext}"
-            filename = filename[0:-1] if filename.endswith('.') else filename
             new_filename = filename + self.image_file.extname
         elif self._is_reveddit():
             filename_str = 'Reveddit '
             subreddit_match = SUBREDDIT_REGEX.search(self.text)
 
             if subreddit_match is not None:
-                filename_str += 'r_' + (subreddit_match.group('subreddit') or subreddit_match.group('subreddit2')) + ' '
+                filename_str += 'r_' + (subreddit_match.group('subreddit') or subreddit_match.group('subreddit2'))
 
-            new_filename = filename_str + self.image_file.basename
+            new_filename = filename_str[0:self.available_char_count]  + ' ' + self.image_file.basename
         else:
-            filename_str = self.text[0:self.available_char_count]
-            new_filename = self._build_filename(self.image_file.basename_without_ext, filename_str)
-            new_filename += self.image_file.extname
+            filename_str = self.text[0:max(100, self.available_char_count)]
+            new_filename = self._build_filename(self.image_file.basename_without_ext, self.text)
+            new_filename = new_filename[0:MAX_FILENAME_LENGTH] + self.image_file.extname
 
         if self._is_text_already_in_filename(filename_str):
             return self.image_file.basename
 
+        if len(new_filename) > 255:
+            raise ValueError(f"'{new_filename}' is {len(new_filename)} chars")
+
         return new_filename
 
     def _is_tweet(self) -> bool:
         """Return true if the text looks like a tweet."""
+        # TODO: the check for @crypto_oracle is a hack
         return TWEET_REGEX.search(self.text) is not None and '@crypto_oracle' not in self.text
 
     def _is_retweet(self) -> bool:
         """Return true if the text looks like a retweet."""
         return self._is_tweet() and RETWEETED_REGEX.search(self._first_line()) is not None
 
     def _retweeter(self) -> Optional[str]:
@@ -159,22 +166,48 @@
             filename_text: str = f"Reddit post by {self.author}"
 
         return self._build_filename(filename_text, body)
 
     def _build_filename(self, filename_text: str, body: str) -> str:
         """Construct a workable filename."""
         body = strip_bad_chars(body)
-        body = body[0:self.available_char_count - len(filename_text) - 2].strip()
+        end_position = self.available_char_count - len(filename_text) - 2
+
+        if end_position < 0:
+            end_position = DEFAULT_LENGTH_FOR_LONG_FILENAMES
+
+        body = body[0:end_position].strip()
+
+        if len(body) == 0:
+            return filename_text
+
         return f'{filename_text} - "{body}"'.replace('  ', ' ')
 
     def _is_text_already_in_filename(self, filename_str: str) -> bool:
         """Check if the extracted text is already in the filename"""
-        clean_filename_str = strip_bad_chars(filename_str)
 
-        if filename_str[0:100] in self.image_file.basename and len(filename_str) > MIN_LENGTH_FOR_DUPE_CHECK:
+        # Subtract 25 to account for the 'Screenshot at 2020-05-05' etc part of filename
+        chars_to_compare = min(len(filename_str), len(self.image_file.basename) - 25)
+        # In case it's < 0 or v. small
+        chars_to_compare = max(chars_to_compare, MIN_LENGTH_FOR_DUPE_CHECK)
+
+        # Cleanup strings before comparing
+        clean_filename_str = strip_mac_screenshot(strip_bad_chars(filename_str))[0:chars_to_compare]
+        clean_basename = strip_mac_screenshot(self.image_file.basename)[0:len(clean_filename_str)]
+        matcher = SequenceMatcher(None, clean_filename_str, clean_basename)
+        similarity = matcher.ratio()
+
+        is_duplicate_text = (matcher.ratio() > MIN_SIMILARITY_RATIO_TO_BE_SAME) \
+                         or (clean_filename_str in self.image_file.basename)
+
+        msg = f"Similarity of '{clean_filename_str}'\n  and '{clean_basename}'\n" \
+              f"  is {similarity} (is_duplicate_text: {is_duplicate_text})"
+        log.debug(msg)
+
+        if is_duplicate_text and len(filename_str) > MIN_LENGTH_FOR_DUPE_CHECK:
             log.debug(f"'{clean_filename_str}' already appears in filename, not renaming.")
             log.debug(f"Extracted text: '{self.text}'")
             return True
         else:
             log.debug(f"\n'{clean_filename_str}'\nis not in\n'{self.image_file.basename}'\n")
             return False
```

### Comparing `clown_sort-1.3.3/clown_sort/files/image_file.py` & `clown_sort-1.4.0/clown_sort/files/image_file.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,47 +2,48 @@
 Wrapper for image files.
 
 OCR:  https://pypi.org/project/pytesseract/
 EXIF: https://blog.matthewgove.com/2022/05/13/how-to-bulk-edit-your-photos-exif-data-with-10-lines-of-python/
 Tags: https://exiftool.org/TagNames/EXIF.html
 """
 import io
+import re
 from pathlib import Path
 from typing import Optional
 
 import pytesseract
 from PIL import Image
 from PIL.ExifTags import TAGS
 
 from clown_sort.config import Config
 from clown_sort.filename_extractor import FilenameExtractor
-from clown_sort.files.sortable_file import SortableFile
+from clown_sort.files.sortable_file import RuleMatch, SortableFile
 from clown_sort.util.filesystem_helper import copy_file_creation_time
 from clown_sort.util.logging import log
-from clown_sort.util.rich_helper import console
+from clown_sort.util.rich_helper import console, warning_text
 
 THUMBNAIL_DIMENSIONS = (400, 400)
 IMAGE_DESCRIPTION = 'ImageDescription'
 FILENAME_LENGTH_TO_CONSIDER_SORTED = 80
 
 EXIF_CODES = {
     IMAGE_DESCRIPTION: 270,
 }
 
 
 class ImageFile(SortableFile):
-    def copy_file_to_sorted_dir(self, destination_path: Path) -> Path:
+    def copy_file_to_sorted_dir(self, destination_path: Path, match: Optional[re.Match] = None) -> Path:
         """
         Copies to a new file and injects the ImageDescription exif tag.
         If :destination_subdir is given new file will be in :destination_subdir off
         of the configured :destination_dir. Returns new file path.
         """
         exif_data = self.raw_exif_dict()
         exif_data.update([(EXIF_CODES[IMAGE_DESCRIPTION], self.extracted_text())])
-        self._log_copy_file(destination_path)
+        self._log_copy_file(destination_path, match)
 
         if Config.dry_run:
             return destination_path
 
         try:
             self.pillow_image_obj().save(destination_path, exif=exif_data)
             copy_file_creation_time(self.file_path, destination_path)
@@ -80,14 +81,21 @@
     def extracted_text(self) -> Optional[str]:
         """Use Tesseract to OCR the text in the image, which is returned as a string."""
         if self.text_extraction_attempted:
             return self._extracted_text
 
         try:
             self._extracted_text = pytesseract.image_to_string(self.pillow_image_obj())
+        except OSError as e:
+            if 'truncated' in str(e):
+                console.print(warning_text(f"Truncated image file! '{self.file_path}'!"))
+            else:
+                console.print_exception()
+                console.print(f"Error while extracting '{self.file_path}'!", style='bright_red')
+                raise e
         except Exception as e:
             console.print_exception()
             console.print(f"Error while extracting '{self.file_path}'!", style='bright_red')
             raise e
 
         if self._extracted_text is not None:
             self._extracted_text = self._extracted_text.strip()
@@ -104,13 +112,16 @@
         """Return a key/value list of exif tags where keys are integers."""
         return self.pillow_image_obj().getexif()
 
     def pillow_image_obj(self) -> Image.Image:
         """Return the file as Pillow Image object."""
         return Image.open(self.file_path)
 
+    def _can_be_presented_in_popup(self) -> bool:
+        return True
+
     def __repr__(self) -> str:
         return f"ImageFile('{self.file_path}')"
 
     # def __rich_console__(self, console: Console, options: ConsoleOptions) -> RenderResult:
     #     super().__rich_console__(console, options)
     #     log.debug(f"RAW EXIF: {self.raw_exif_dict()}")
```

### Comparing `clown_sort-1.3.3/clown_sort/files/pdf_file.py` & `clown_sort-1.4.0/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.3/clown_sort/files/sortable_file.py` & `clown_sort-1.4.0/clown_sort/files/sortable_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """
 Base class for sortable files of any type.
 """
+import re
 import shutil
+from collections import namedtuple
 from os import path, remove
 from pathlib import Path
 from typing import List, Optional, Union
 
 from exiftool import ExifToolHelper
 from rich.console import Console, ConsoleOptions, RenderResult
 from rich.panel import Panel
 from rich.prompt import Confirm
 from rich.text import Text
 
 from clown_sort.config import Config
 from clown_sort.filename_extractor import FilenameExtractor
+from clown_sort.sort_selector import process_file_with_popup
 from clown_sort.util.filesystem_helper import copy_file_creation_time
 from clown_sort.util.logging import log
 from clown_sort.util.rich_helper import (bullet_text, comma_join, console, copying_file_log_message,
      indented_bullet, mild_warning, moving_file_log_message, print_dim_bullet)
 
+RuleMatch = namedtuple('RuleMatch', ['folder', 'match'])
+
 MAX_EXTRACTION_LENGTH = 4096
 NOT_MOVING_FILE = "Not moving file to processed dir because it's"
 NO_SORT_FOLDERS_MSG = bullet_text('No sort folders matched so copying to base sorted dir...', style='color(209)')
 
 
 class SortableFile:
     def __init__(self, file_path: Union[str, Path]) -> None:
@@ -33,45 +38,58 @@
         self.text_extraction_attempted: bool = False
         self._extracted_text: Optional[str] = None
         self._new_basename: Optional[str] = None
         self._filename_extractor: Optional[FilenameExtractor] = None
         self._paths_of_sorted_copies: List[Path] = []
 
     @classmethod
-    def get_sort_folders(cls, search_text: Optional[str]) -> List[str]:
+    def get_sort_folders(cls, search_text: Optional[str]) -> List[RuleMatch]:
         """Find any folders that could be relevant."""
         if search_text is None:
             return []
 
-        return [sr.folder for sr in Config.sort_rules if sr.regex.search(search_text)]
+        return [
+            RuleMatch(sr.folder, sr.regex.search(search_text))
+            for sr in Config.sort_rules if sr.regex.search(search_text)
+        ]
 
     def sort_file(self) -> None:
         """Sort the file to destination_dir subdir."""
         console.print(self)
         search_text = self.basename_without_ext + ' ' + (self.extracted_text() or '')
-        sort_folders = type(self).get_sort_folders(search_text)
+        rule_matches = type(self).get_sort_folders(search_text)
+        sort_folders = [rm.folder for rm in rule_matches]
 
         # Handle the case where there are no matches to any configured folders.
-        if len(sort_folders) == 0:
-            if Config.only_if_match:
+        if len(rule_matches) == 0:
+            if Config.manual_fallback and self._can_be_presented_in_popup():
+                process_file_with_popup(self)
+                return
+            elif Config.only_if_match:
                 print_dim_bullet('No folder match and --only-if-match option selected. Skipping...')
                 return
             elif Config.sorted_screenshots_dir in self.file_path.parents:
                 print_dim_bullet("Not moving because no folder match and file already in a sorted folder...")
                 return
 
             console.print(NO_SORT_FOLDERS_MSG)
             sort_folders = [None]
+            rule_matches = [None]
         else:
             console.print(bullet_text(Text('Sort folders: ') + comma_join(sort_folders, 'sort_folder')))
 
         # Copy the renamed file to all the folders whose sorting rules were matched.
-        for folder in sort_folders:
+        for rule_match in rule_matches:
             # Create the subdir if it doesn't exist.
-            if folder is not None:
+            folder = None
+            match = None
+
+            if rule_match is not None:
+                folder = rule_match.folder
+                match = rule_match.match
                 destination_dir = Config.sorted_screenshots_dir.joinpath(folder)
 
                 if not destination_dir.is_dir() and not Config.dry_run:
                     log.info(f"Creating subdirectory '{destination_dir}'...")
                     destination_dir.mkdir()
 
             destination_path = self.sort_destination_path(folder)
@@ -91,15 +109,15 @@
                 console.print(msg)
 
                 if not (Config.yes_overwrite or Confirm.ask(f"Overwrite?")):
                     console.print("Skipping...", style='dim')
                     continue
 
             self._paths_of_sorted_copies.append(destination_path)
-            self.copy_file_to_sorted_dir(destination_path)
+            self.copy_file_to_sorted_dir(destination_path, match)
 
         if Config.leave_in_place:
             console.print(bullet_text(Text('Leaving in place...', style='dim')))
             return
 
         # Don't move the file to the processed_dir if it started in a sorted location
         if self.file_path in self._paths_of_sorted_copies:
@@ -125,21 +143,21 @@
         try:
             with ExifToolHelper() as exiftool:
                 return exiftool.get_metadata(self.file_path)[0]
         except:
             log.warning("ExifTool not found; EXIF data ignored. 'brew install exiftool' may solve this.")
             return {}
 
-    def copy_file_to_sorted_dir(self, destination_path: Path):
+    def copy_file_to_sorted_dir(self, destination_path: Path, match: Optional[re.Match] = None):
         """Move or copy the file to destination_subdir."""
         if self.file_path == destination_path:
             console.print(indented_bullet("Source and destination are the same..."))
             return
 
-        self._log_copy_file(destination_path)
+        self._log_copy_file(destination_path, match)
 
         if Config.dry_run:
             console.print(indented_bullet("Dry run so not actually copying...", style='dim'))
         else:
             shutil.copy2(self.file_path, destination_path)
             copy_file_creation_time(self.file_path, destination_path)
 
@@ -148,27 +166,33 @@
         destination_path = Config.sorted_screenshots_dir
 
         if subdir is not None:
             destination_path = destination_path.joinpath(subdir)
 
         return destination_path.joinpath(self.new_basename())
 
-    def _log_copy_file(self, destination_path: Path) -> None:
+    def _log_copy_file(self, destination_path: Path, match: Optional[re.Match] = None) -> None:
         """Log info about a file copy."""
         if Config.debug:
             console.print(copying_file_log_message(self.basename, destination_path))
             return
 
         log_msg = Text('').append('Copying to ', style='dim')
 
         if destination_path.parent == Config.destination_dir:
             console.print(indented_bullet(log_msg.append('root sorted dir...')))
         else:
             log_msg.append(str(destination_path.parent), style='sort_destination')
-            console.print(indented_bullet(log_msg.append('...')))
+
+            if match is not None:
+                log_msg.append(f" (matched '", style='dim')
+                log_msg.append(match.group(0).strip(), style='magenta dim')
+                log_msg.append("')", style='dim')
+
+            console.print(indented_bullet(log_msg))
 
     def _move_to_processed_dir(self) -> None:
         """Relocate the original file to the [SCREENSHOTS_DIR]/Processed/ folder."""
         processed_file_path = Config.processed_screenshots_dir.joinpath(self.file_path.name)
 
         if Config.debug:
             console.print(moving_file_log_message(str(self.file_path), processed_file_path))
@@ -190,14 +214,17 @@
 
         if Config.dry_run:
             console.print(indented_bullet(Text('Skipping delete because this is a dry run...', style='dim')))
             return
 
         remove(self.file_path)
 
+    def _can_be_presented_in_popup(self) -> bool:
+        return False
+
     def __str__(self) -> str:
         return str(self.file_path)
 
     def __repr__(self) -> str:
         return f"SortableFile('{self.file_path}')"
 
     def __rich_console__(self, console: Console, options: ConsoleOptions) -> RenderResult:
```

### Comparing `clown_sort-1.3.3/clown_sort/sort_selector.py` & `clown_sort-1.4.0/clown_sort/sort_selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
 Open a GUI window to allow manual name / select.
+TODO: rename to something more appropriate
 """
 import shutil
 import sys
 from os import path, remove
 from subprocess import run
 
 from rich.panel import Panel
 from rich.text import Text
 
 from clown_sort.config import Config
 from clown_sort.filename_extractor import FilenameExtractor
-from clown_sort.files.image_file import ImageFile
 from clown_sort.util.dict_helper import get_dict_key_by_value
 from clown_sort.util.logging import log
 from clown_sort.util.rich_helper import bullet_text, console, indented_bullet
 
-RADIO_COLS = 10
+RADIO_COLS = 11
 DELETE = 'Delete'
 OK = 'Move'
 OPEN = 'Preview Image'
 SKIP = 'Skip'
 EXIT = 'Exit'
 
 
-def process_file(image: ImageFile) -> None:
+def process_file_with_popup(image: 'ImageFile') -> None:
     import PySimpleGUI as sg
-    console.print(Panel(Text("Processing: '").append(str(image.file_path), style='cyan reverse').append("'..."), expand=False))
+    file_msg = Text("Processing: '").append(str(image.file_path), style='cyan reverse').append("'...")
+    console.print(Panel(file_msg, expand=False))
     extracted_text = ' '.join((image.extracted_text() or '').splitlines())
     log.info(f"OCR Text: {extracted_text} ({len(extracted_text)} chars)")
     suggested_filename = FilenameExtractor(image).filename()
     input = sg.Input(suggested_filename, size=(len(suggested_filename), 1))
 
     layout = [
         [sg.Image(data=image.image_bytes(), key="-IMAGE-")],
```

### Comparing `clown_sort-1.3.3/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.4.0/clown_sort/sorting_rules/crypto.csv`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 folder,regex
 1mdb,1mdb|jho[-_\s]*low|Victor[-_\s]*Hoo
 3ac,3ac|Three[-_\s]*Arrows[-_\s]*Capital|su[-_\s]*zhu|zhu[-_\s]*su|kyle[-_\s]*davies|OPNX
 A16Z,a16z|andreessen|packym|arianna[-_\s1]*simpson
 Aave,aave
 AAX,\baax
+Algorand,\bAlgorand|\b[$#]ALGO\b
 Arbitrum,Arbitrum|[$#]ARB\b
 Amber Group,Amber[-_\s]*Group|\btiantian\b|\bkullander\b|\btony[-_\s]*he\b|\bbo[-_\s]*shen\b
 Aptos,\bAptos\b
 Art,occult
 Avalanche,\bAvax|AVAX\b|avalanche
-Banks,SEBA[^a-z]|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group|\$FRC|Commercium[-_\s]*Financial
-Bankless,Bankless
-Biconomy,Biconomy|Omchain
+Banks,SEBA[^a-z]|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group|\$FRC|Commercium[-_\s]*Financial|\bmetabank|\bHBAN\b|Huntington[-_\s]*Bancshares|United[-_\s]*Texas|\bUTB\b
+Bankless,Bankless|David[-_\s]*Hoffman
+Biconomy,\bBiconomy|Omchain
 Binary Options,binary[-_\s]*options
-Binance,binance|biconomy|\bbnb|bsc|cz|bifinity|binaryx|billance|changpeng|joselito|paysafe|SwipeIO|Swipe\s*Wallet|keyway|\bkey[-_\s]*vision|TrustWallet|BUSD|\boztures|Kaiser[-_\s]*Ng|InvestByBit
+Binance,binance|biconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|joselito|paysafe|\bSwipe[-_\s]*(IO|Wallet)|\bkeyway|\bkey[-_\s]*vision|\bTrustWallet\b|BUSD|\boztures|Kaiser[-_\s]*Ng|InvestByBit
 Bitdeer,Bitdeer
 BitGet,Bitget
+Bithumb,\bbithumb
 Bitmain,Bitmain
 Bitstamp,Bitstamp
 Bittrex,Bittrex|Ritchie[-_\s]*Lai|Kiran[-_\s]*Raj|John[-_\s]*Roth
 Bitzlato,Bitzlato
 Blockchain8,Blockchain8|tom[-_\s]*emmer|ritchie[-_\s]*torres|repritchie|Warren[-_\s]*Davidson|Byron[-_\s]*Donalds|Ted[-_\s]*Budd|Josh[-_\s]*Gotheimer|Jake[-_\s]*Auchincloss|Darren[-_\s]*Soto|ro[-_\s]*khanna|KMSmithDC|Kristin[-_\s]*Smith\b|Warren[-_\s]*Davidson
 Blockchain Capital,Blockchain[-_\s]*Capital|\bbrock\b|brockpierce
-BlockFi,BlockFi
+BlockFi,BlockFi|Zac[-_\s]*Prince|Brian[-_\s]*Oliver
 Blockstream,Blockstream
 Bored Ape Yacht Club,BAYC|Bored[-_\s]*Ape|yuga[-_\s]*labs
-Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi|Max[-_\s]*Keiser|Cowboy[-_\s]*Crypto|minimalcsgo
-Broettes,Nicole[-_\s]*Behnam
-Bybit,\bBybit\b|Ben[-_\s]*Zhou|InvestByBit
+Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi|Max[-_\s]*Keiser|Cowboy[-_\s]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s]*Paul\b|raoul(gmi|[-_\s]*pal)
+Broettes,Nicole[-_\s]*Behnam|natbrunell
+Bybit,\bBybit\b|Ben[-_\s]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
-Cathie Wood,Cathie\s*Wood|\bARK(F|G|K|\s*Innovation|\s*Invest)
+Cathie Wood,Cathie\s*Wood|\bARK(F|G|K|\s*Innovation|\s*Invest)|\bIZRL
 Celsius,celsius|mashinsky|levity[-_\s]*and[-_\s]*love|celsian
 Circle,[@#]circle|usdc|circle[-_\s]*internet|disparte|\ballaire|jerallaire
 CMCC Global,CMCC[-_\s]*Global
-Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b|Asiff[-_\s]*Hirji|\bbalaji|Fred[-_\s]*Ehrsam
+Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b|Asiff[-_\s]*Hirji|\bbalaji|Fred[-_\s]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk|OPNX|flexusd|Leslie[-_\s]*Lamb|dougpolkvids
+CoinLoan,coinloan|Faliushin
 CompoundFi,compoundfi|leshner|\bgonen\b
-Cross River Bank,CRB|Cross[-_\s]*River|Prestige[-_\s]*Capital|bae[-_\s]*communications|Zenfi|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim
+Cross River Bank,CRB|Cross[-_\s]*River|Prestige[-_\s]*Capital|bae[-_\s]*communications|Zenfi|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv
 Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s
 CUBI,\bCUBI\b|Customers[-_\s]*Ban(k|corp)
-Custodia,custodia|caitlin[-_\s]*long
-dalle,craiyon
+Custodia,custodia\b|caitlin[-_\s]*long
+dalle,craiyon|midjourney|\bdall[-_\s]*e\b
 DCG,DCG|digital\s*currency\s*group|sh?ill?bert|Grayscale|GBTC
+DeFi,\bdefi\b|decentralized[-_\s]*finance
+Dragonfly Capital,Dragonfly[-_\s]*Capital
 DWF,DWF|Andrey[-_\s]*Grachev|\bgrachev\b
-Effective Altruism,\bEA\b|effective[-_\s]*altruism
+Effective Altruism,\bE\.?A\.?\b|effective[-_\s]*altruism
 El Salvador,El[-_\s]*Salvador|Bukele|Max[-_\s]*Keiser
+Elon Musk,\bTesla\b|\bTSLA\b|\bElon\b|\bElmo\b
 EOS,\bEOS\b|\bBlumer\b|\bLarimer\b|@B1\b|Block[-_\.\s]One
 Euler Finance,\beuler\b
 FalconX,falconx
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
 Friedlander Group,Friedlander|Agro[-_\s]*Bank|all\s*year\*m|\bbrock\b|brockpierce|litvishhocker
 FTX,FTX|FTT|SBF|Trabucco|Bankman|Ellison|Nishad|Alameda|Moonstone|friedberg|autism\s*capital
 Galaxy Digital,novogratz|Alex[-_\s]*Thorn
 Gelato Network,Gelato[-_\s]*Network|\bSorbet[-_\s]*Finance|@gitpusha|hilmar[-_\s]*x|\bmistx\b|@_alchemistcoin|@ChaosLabs_NFT|Arrakis[-_\s]*Finance|Dave[-_\s]*Leibowitz|Hilmar[-_\s]*Orth|joehquak
 Gemini,Gemini|winklev|@cameron
 Genesis,Genesis|Michael\s?Moro
 Goldfinch,goldfinch
+Hamas,\bHamas\b|Al[-_\s]*Qassam
 Hex,\bHex\b|[#$]Hex|Pulsechain|Richard\s*Heart|Hexican
 Hoo,Hoo[-_\s]*(Research|Exchange)|[#$]Hoo\b|Rexy\s*(Hoo|Wang)|\bhoo\b
 Huobi,huobi|jiao_newlife|jiaojiao|Leon[-_\s]*Li
+Iran,\bIran\b|\bIranian\b|Nobitex|\bCoinNik|\bWallex\b|Sarmayex|\bRabex\b
 Jump Trading,Jump[-_\s]*Trading|@jump_
 Justin Sun,justin[-_\s]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina
-Kazakhstan,kazakhstan|Freedom[-_\s]*Holding|\balmaty|Timor[-_\s]*Turlov|\bFFIN[-_\s]*brokerage
+Kazakhstan,\bkazakh|Freedom[-_\s]*Holding|\balmaty|Timor[-_\s]*Turlov|\bFFIN[-_\s]*brokerage
 Kinesis,kinesis|\bKVT\b|\bABX\b|\bKAG\b
 Kraken,kraken|payward
 KuCoin,kucoin
 LBRY,LBRY|\bLBC\b
 Lexpunk Army,lexpunk|gabriel[-_\s]*shapiro|_gabrielShapir0|\blex_node\b
 Lifeboat Foundation,Lifeboat[-_\s]*Foundation
-North Korea,lazarus|North\s*Korea|pyongyang
+North Korea,lazarus|North\s*Korea|pyongyang|\bDPRK|puuurtbubv|@fast4release
 Paul LeRoux,leroux
 Polygon Labs,polygon[-_\s]*labs|ryan[-_\s]*watt\b|@Fwiz|Rebecca[-_\s]*Rettig|[#$]DOT\b
 MakerDAO,makerdao|[$#\s]DAI[^\w]
 Marathon,\$MARA|marathon
 Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s]*Cheng
 Mario Nawfal,mario[-_\s]*nawfal
 Messari,Ryan\s*Selkis|twobitidiot|messari|@robustus|Dan[-_\s]*McArdle
@@ -84,58 +92,60 @@
 Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*(Bank|Commercial)
 Founders Bank,Michael[-_\s]*Bianchi|Founders[-_\s]*Bank
 Miles Guo,\bguo\b|hcoin|himalaya[-_\s]*exchange|bannon|fjb|miles[-_\s]*kwok|brother[-_\s]*seven|kin[-_\s]*ming[-_\s]*je|william[-_\s]*je\b|\bHaoyun\b
 Miners,bitcoin[-_\s]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s]*Scientific|Iris[-_\s]*Energy|Blockstream
 Moonpay,moonpay
 MSTR,Saylor|MSTR
 Near Protocol,NEAR[-_\s]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s]*Rettig
-Nexo,Nexo
+Nexo,\bNexo\b|Antoni[-_\s]*Trenchev|Georgi[-_\s]*Shulev|Lydia[-_\s]*Shuleva
 NFTs,crypto[-_\s]*punk|pudgy[-_\s]*penguin
 OKX,oke?[cx]|star[-_\s]*xu
 Olympus DAO,\bOlympus\b|\bOHM\b
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea
-PAG,\bpag\b
+PAG,\bpag\b|Weijian[-_\s]*Shan
 Paradigm,Fred[-_\s]*Ehrsam|paradigm\b
 Paxful,paxful|Ray[-_\s]*(Youssef|Savant)|Artur[-_\s]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
 Payrnet,payrnet|railsr|railsbank
 Pi,\$PI[^\w]|Pi[-_\s]*Network
 Prime Trust,Prime[-\s_]?Trust
 PVBC,PVBC|BankProv
 Quadriga,Quadriga|Gerald[-_\s]*Cotten
 Revolut,revolut[^\w]
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,[$#]RIOT\b|Riot[-\s_]*(Block|Platform)|Bioptix
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
 SEC,\bSEC(\b|Gov)|Gensler|Securities.{0,6}Exchange.{0,6}Commission
-Signature Bank,SBNY|Signature[-_\s]*Bank|Signet
+Signature Bank,SBNY|Signature[-_\s]*Bank|Signet|Scott[-_\s]*Shay\b|(Joseph|Joe)[-_\s]*DePaolo
 Silicon Valley Bank,si?vb|Silicon[-_\s]*Valley[-_\s]*Bank
 Silk Road,Silk[-_\s]*Road|\bulbricht|\bDPR\b
 Silvergate,\$SI|Silvergate|Alan\s*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s]*Rettig
+Skrill,\bskrill
 Solana,Solana|Serum
 Symbolic Capital,Symbolic[-_\s]*Capital|Lev[-_\s]Livnev
 TerraLuna,luna\b|do[-_\s]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s]*Foundation\b
-Tether,tether|usdt|paolo|friedberg|hoegner|Noble\s?Bank|Deltec[^\']|b(e|i)tfinex[^e]|\bbrock\b|brockpierce|Capital[-_\s]*Union|Noblex|SJMBT|Global[-_\s]*Trad(ing|e)[-_\s]*Solutions|ifinex|BFXNA|BFXWW|[$#]Leo\b
+Tether,tether|usdt|paolo|friedberg|hoegner|Noble\s?Bank|Deltec[^\']|b(e|i)tfinex[^e]|\bbrock\b|brockpierce|Capital[-_\s]*Union|Noblex|SJMBT|Global[-_\s]*Trad(ing|e)[-_\s]*Solutions|ifinex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s]*Potter|Stablehouse|Samson[-_\s]*Mow|Gabor[-_\s]*Grubacs|XBTO|Paul[-_\s]*Eisma|Philippe[-_\s]*Bekhazi
 Tornado Cash,tornado\s*cash
 Transactive Systems UAB,Transactive
 Tron,\btron\b|tron(block|\s*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
 VCs,venture[-_\s]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s]*sacks|\bthiel\b|sequoia|founders[-_\s]*fund|Valar[-_\s]*Ventures|6th[-_\s]*Man[-_\s]*Ventures|Northzone|Warburg[-_\s]*Serres|Alan[-_\s]*Howard|Tiger[-_\s]*Global
+Vitalik Buterin,\bvitalik\b
 Voyager,voyager
 Wallet Addresses BCH,bitcoincash:q.*\b
-Wallet Addresses Bitcoin,(bc1|[13])[a-zA-HJ-NP-Z0–9]{25,39}\b
-Wallet Addresses Cardano,addr1[a-z0–9]+\b
-Wallet Addresses Cosmos,cosmos[a-zA-Z0–9_.-]{10,}\b
-Wallet Addresses Dash,X[1–9A-HJ-NP-Za-km-z]{33}
-Wallet Addresses Doge,\sD[a-zA-Z0–9_.-]{33}
-Wallet Addresses Ethereum,0x[a-fA-F0–9]{40}
-Wallet Addresses Monero,[48][0–9AB][1–9A-HJ-NP-Za-km-z]{93}
-Wallet Addresses Polkadot,1[0–9a-zA-Z]{47}
-Wallet Addresses Ripple,r[0–9a-zA-Z]{33}
-Wallet Addresses Stellar,G[0–9A-Z]{40,60}\b
+Wallet Addresses Bitcoin,\b(bc1|[13])[a-zA-HJ-NP-Z0–9]{25,39}\b
+Wallet Addresses Cardano,\baddr1[a-z0–9]+\b
+Wallet Addresses Cosmos,\bcosmos[a-zA-Z0–9_.-]{10,}\b
+Wallet Addresses Dash,\bX[1–9A-HJ-NP-Za-km-z]{33}
+Wallet Addresses Doge,\bD[a-zA-Z0–9_.-]{33}
+Wallet Addresses Ethereum,\b0x[a-fA-F0–9]{40}
+Wallet Addresses Monero,\b[48][0–9AB][1–9A-HJ-NP-Za-km-z]{93}
+Wallet Addresses Polkadot,\b1[0–9a-zA-Z]{47}
+Wallet Addresses Ripple,\br[0–9a-zA-Z]{33}
+Wallet Addresses Stellar,\bG[0–9A-Z]{40,60}\b
 Waves,sasha35625|sasha\.waves|\bvires|sasha[-_\s]*ivanov|boris[-_\s]*titov|[$#]waves\b
 Wintermute,wintermute|\bbebop\b
 Wirecard,wirecard|\bmarsalek\b|\bBafin\b
 Wyre,\bwyre|sendwyre
```

### Comparing `clown_sort-1.3.3/clown_sort/util/argument_parser.py` & `clown_sort-1.4.0/clown_sort/util/argument_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,17 @@
                     metavar='DESTINATION_DIR',
                     help='destination folder to place the Sorted/ and Processed/ dirs (default: SCREENSHOTS_DIR)',
                     default=str(DEFAULT_DESTINATION_DIR).replace(str(Path.home()), '~'))
 
 parser.add_argument('-m', '--manual-sort', action='store_true',
                     help='causes a popup to be presented for each file where it can be manually named and a sorting destination selected (experimental)')
 
+parser.add_argument('-mf', '--manual-fallback', action='store_true',
+                    help='causes a popup to be presented for each file only as a fallback when no sort rules are matched (experimental)')
+
 parser.add_argument('-r', '--rules-csv',
                     action='append',
                     metavar='RULES_FILE.CSV',
                     help=f"sorting rules can be supplied more than once (use string '{CRYPTO}' to use the defaults)")
 
 parser.add_argument('-f', '--filename-regex',
                     help='filename regular expression',
```

### Comparing `clown_sort-1.3.3/clown_sort/util/constants.py` & `clown_sort-1.4.0/clown_sort/util/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 # Sorting rules stuff
 SORTING_RULES_DIR = importlib.resources.files(PACKAGE_NAME).joinpath('sorting_rules')
 CRYPTO_RULES_CSV_PATH = str(SORTING_RULES_DIR.joinpath('crypto.csv'))
 
 
 # Filename regex stuff
+SCREENSHOT_REGEX = re.compile('Screen Shot (\\d{4}-\\d{2}-\\d{2} at \\d{1,2}\\.\\d{2}\\.\\d{2} [AP]M)')
 MAC_SCREENSHOT_REGEX = re.compile('Screen Shot (\\d{4}-\\d{2}-\\d{2} at \\d{1,2}\\.\\d{2}\\.\\d{2} [AP]M).(png|jpe?g)')
 ENV_FILENAME_REGEX = environ.get('CLOWN_SORT_FILENAME_REGEX')
 
 if ENV_FILENAME_REGEX is None:
     DEFAULT_FILENAME_REGEX = MAC_SCREENSHOT_REGEX
 else:
     DEFAULT_FILENAME_REGEX = re.compile(ENV_FILENAME_REGEX)
```

### Comparing `clown_sort-1.3.3/clown_sort/util/filesystem_helper.py` & `clown_sort-1.4.0/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.3/clown_sort/util/rich_helper.py` & `clown_sort-1.4.0/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.3/pyproject.toml` & `clown_sort-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.3.3"
+version = "1.4.0"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.3.3/setup.py` & `clown_sort-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,167 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: clown-sort
+Version: 1.4.0
+Summary: Sort screenshots based on rules or through individual review.
+Home-page: https://github.com/michelcrypt4d4mus/clown_sort
+Keywords: ocr,organization,organizer,screenshot,rename,sort
+Author: Michel de Cryptadamus
+Author-email: michel@cryptadamus.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Desktop Environment :: File Managers
+Classifier: Topic :: Multimedia :: Graphics :: Capture
+Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Provides-Extra: gui
+Provides-Extra: pdf
+Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0) ; extra == "gui"
+Requires-Dist: exif (>=1.5.0,<2.0.0)
+Requires-Dist: filedate (>=2.0,<3.0)
+Requires-Dist: piexif (>=1.1.3,<2.0.0)
+Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: pycryptodome (>=3.17,<4.0) ; extra == "pdf"
+Requires-Dist: pyexiftool (>=0.5.5,<0.6.0)
+Requires-Dist: pypdf (>=3.4.1,<4.0.0)
+Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
+Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
+Requires-Dist: rich (>=13.0.1,<14.0.0)
+Requires-Dist: rich-argparse-plus (>=0.3.1.4,<0.4.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['clown_sort', 'clown_sort.files', 'clown_sort.util']
+# CLOWN SORT
+Sometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can't find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.
 
-package_data = \
-{'': ['*'], 'clown_sort': ['sorting_rules/*']}
+Clown Sort[^1] solves this.
 
-install_requires = \
-['exif>=1.5.0,<2.0.0',
- 'filedate>=2.0,<3.0',
- 'piexif>=1.1.3,<2.0.0',
- 'pillow>=9.4.0,<10.0.0',
- 'pyexiftool>=0.5.5,<0.6.0',
- 'pypdf>=3.4.1,<4.0.0',
- 'pytesseract>=0.3.10,<0.4.0',
- 'python-dotenv>=0.21.1,<0.22.0',
- 'rich-argparse-plus>=0.3.1.4,<0.4.0.0',
- 'rich>=13.0.1,<14.0.0']
-
-extras_require = \
-{'gui': ['PySimpleGUI>=4.60.4,<5.0.0'], 'pdf': ['pycryptodome>=3.17,<4.0']}
-
-entry_points = \
-{'console_scripts': ['set_screenshot_timestamps = '
-                     'clown_sort:set_screenshot_timestamps',
-                     'sort_screenshots = clown_sort:sort_screenshots']}
-
-setup_kwargs = {
-    'name': 'clown-sort',
-    'version': '1.3.3',
-    'description': 'Sort screenshots based on rules or through individual review.',
-    'long_description': '# CLOWN SORT\nSometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can\'t find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.\n\nClown Sort[^1] solves this.\n\n\n## What It Do\nIt sorts screenshots, PDFs, etc. based on their name and/or their textual contents into folders based on a list of rules. The contents of the tweet/reddit post/whatever are prepended to the filename and the `ImageDescription` EXIF tag is set to the OCR text. As you can configure your own arbitrary rules and run it against any set of images it works on many things other than screenshots of social media clowns, though the default configuration is for cryptocurrency clowns.\n\nFor example this screenshot of a tweet by a noteworthy cryptocurrency "reporter"[^2] on the eve of FTX\'s implosion:\n\n![](doc/larry_cermak_on_alameda_and_ftx.png)\n\nWould be renamed from `Screen Shot 2023-02-17 at 7.11.37 PM.png` to\n\n```\nTweet by @lawmaster: "I will say though before this thread gets taken over: 1. I do believe Alameda has the size to easily buy Binance\\\'s FIT OTC 2. I think the chance of FTX insolvency is near" Screen Shot 2023-02-17 at 7.11.37 PM.png\n```\n\nOther stuff that happens:\n* The `ImageDescription` EXIF tag will be written (for images).\n* All timestamps will be preserved.\n* Files that match multiple patterns will be copied to multiple destination folders.\n* The original file will be moved into a `Processed/` directory after it has been handled.\n\nNote also that:\n* This works on images that are more substantive than just self-clowning screenshots.\n* So far only Tweets and Reddit screenshots have special handling beyond OCR text extraction.\n* PDFs can be sorted by contents or filename, e.g. a PDF named `Norton Anthology of Crypto Bro Poetry.pdf` containing iambic verse like _["Fuck u justin sun  and fuck ur dick face... u all play with investing and money of the people !!!!"](https://universeodon.com/@cryptadamist/109642431382653023)_ by the noted bard JOKER_OF_CRYPTO will be copied to the `Justin Sun/` folder but not renamed.\n* Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.\n\n## Quick Start\n```sh\n# Installation with pipx is preferred if you have it but you can also use pip which comes standard\n# on almost all systems. pipx is only a noticeably better answer if you\'re a python programmer who\n# is concerned about side effects of pip upgrading system python packages.\npip install clown_sort\n\n# Get help\nsort_screenshots -h\n\n# Dry run with default cryptocurrency sort rules (dry runs don\'t actually move anything,\n# they just show you what will happen if you run again with the --execute flag)\nsort_screenshots\n\n# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots\nsort_screenshots --execute\n\n# Sort a different directory of screenshots\nsort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute\n\n# Sort with custom rules\nsort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute\n\n# Sort pdfs\nsort_screenshots -f \'.*pdf$\' -e\n```\n\n# Setup\n[pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.\n```\npipx install clown_sort\n```\n\nSome (not many) PDFs require the `pycryptodome` package to be parsed. If you don\'t have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pycryptodome]`.\n\nUpdating to the latest version can be accomplished with `pipx upgrade clown_sort`.\n\n\n### Configuring With `.clown_sort` File\nIf there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:\n\n1. The current directory\n2. Your home directory\n\nSee [the example](.clown_sort.example) for more information on what can be configured this way.\n\n### Optional Components\nIf you want to use the popup window to manually tag you _may_ need to install:\n* Python TK: `brew install python-tk@3.10` (if you don\'t have [homebrew](https://brew.sh/) you need to install it to run `brew install`)\n\nNot required for standard PNG, JPG, etc. images but you may optionally install `exiftool` for other file types if you want excessive debugging.\n* ExifTool: `brew install exiftool` or download from https://exiftool.org\n\n\n# Usage\nThe default is for the tool to run in "dry run" mode, meaning it doesn\'t actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**\n\nWhile every effort has been made to use Python\'s cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.\n\n### Help Screen\n![](doc/sort_screenshots_help.png)\n\n(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)\n\n### Custom Sorting Rules\nThe default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you\'re not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.\n\n### Example Output (Automated Sorting)\n![](doc/output_example.png)\n\n\n## Manually Sorting (Experimental)\n**This is an experimental feature.** It\'s only been tested on macOS.\n\nIf you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.\n\nTo use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:\n```sh\npipx install clown_sort[PySimpleGUI]\n```\n\n![](doc/manual_select_box.png)\n\n\n# Contributing\nFeel free to file issues or open pull requests.\n\nThis package is managed with [Python Poetry](http://python-poetry.org/). To get going:\n1. Install Poetry.\n1. `git clone` this repo.\n1. `cd clown_sort`\n1. `poetry install`\n1. Optional components can be install with `poetry install -E pdf -E gui`\n\nOnly requirement is that tests should pass before you open it, which you can check with\n\n```\npytest\n```\n\n[^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.\n\n[^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried\'s various scams as part of his commitment to "unrivaled transparency".\n',
-    'author': 'Michel de Cryptadamus',
-    'author_email': 'michel@cryptadamus.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/michelcrypt4d4mus/clown_sort',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
 
+## What It Do
+It sorts screenshots, PDFs, etc. based on their name and/or their textual contents into folders based on a list of rules. The contents of the tweet/reddit post/whatever are prepended to the filename and the `ImageDescription` EXIF tag is set to the OCR text. As you can configure your own arbitrary rules and run it against any set of images it works on many things other than screenshots of social media clowns, though the default configuration is for cryptocurrency clowns.
+
+For example this screenshot of a tweet by a noteworthy cryptocurrency "reporter"[^2] on the eve of FTX's implosion:
+
+![](doc/larry_cermak_on_alameda_and_ftx.png)
+
+Would be renamed from `Screen Shot 2023-02-17 at 7.11.37 PM.png` to
+
+```
+Tweet by @lawmaster: "I will say though before this thread gets taken over: 1. I do believe Alameda has the size to easily buy Binance\'s FIT OTC 2. I think the chance of FTX insolvency is near" Screen Shot 2023-02-17 at 7.11.37 PM.png
+```
+
+Other stuff that happens:
+* The `ImageDescription` EXIF tag will be written (for images).
+* All timestamps will be preserved.
+* Files that match multiple patterns will be copied to multiple destination folders.
+* The original file will be moved into a `Processed/` directory after it has been handled.
+
+Note also that:
+* This works on images that are more substantive than just self-clowning screenshots.
+* So far only Tweets and Reddit screenshots have special handling beyond OCR text extraction.
+* PDFs can be sorted by contents or filename, e.g. a PDF named `Norton Anthology of Crypto Bro Poetry.pdf` containing iambic verse like _["Fuck u justin sun  and fuck ur dick face... u all play with investing and money of the people !!!!"](https://universeodon.com/@cryptadamist/109642431382653023)_ by the noted bard JOKER_OF_CRYPTO will be copied to the `Justin Sun/` folder but not renamed.
+* Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.
+
+## Quick Start
+```sh
+# Installation with pipx is preferred if you have it but you can also use pip which comes standard
+# on almost all systems. pipx is only a noticeably better answer if you're a python programmer who
+# is concerned about side effects of pip upgrading system python packages.
+pip install clown_sort
+
+# Get help
+sort_screenshots -h
+
+# Dry run with default cryptocurrency sort rules (dry runs don't actually move anything,
+# they just show you what will happen if you run again with the --execute flag)
+sort_screenshots
+
+# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots
+sort_screenshots --execute
+
+# Sort a different directory of screenshots
+sort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute
+
+# Sort with custom rules
+sort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute
+
+# Sort pdfs
+sort_screenshots -f '.*pdf$' -e
+```
+
+# Setup
+[pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
+```
+pipx install clown_sort
+```
+
+Some (not many) PDFs require the `pycryptodome` package to be parsed. If you don't have it they will just not be parsed; only the filename will be used for sorting. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with `pipx install clown_sort[pycryptodome]`.
+
+Updating to the latest version can be accomplished with `pipx upgrade clown_sort`.
+
+
+### Configuring With `.clown_sort` File
+If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
+
+1. The current directory
+2. Your home directory
+
+See [the example](.clown_sort.example) for more information on what can be configured this way.
+
+### Optional Components
+If you want to use the popup window to manually tag you _may_ need to install:
+* Python TK: `brew install python-tk@3.10` (if you don't have [homebrew](https://brew.sh/) you need to install it to run `brew install`)
+
+Not required for standard PNG, JPG, etc. images but you may optionally install `exiftool` for other file types if you want excessive debugging.
+* ExifTool: `brew install exiftool` or download from https://exiftool.org
+
+
+# Usage
+The default is for the tool to run in "dry run" mode, meaning it doesn't actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**
+
+While every effort has been made to use Python's cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.
+
+### Help Screen
+![](doc/sort_screenshots_help.png)
+
+(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)
+
+### Custom Sorting Rules
+The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
+
+### Example Output (Automated Sorting)
+![](doc/output_example.png)
+
+
+## Manually Sorting (Experimental)
+**This is an experimental feature.** It's only been tested on macOS.
+
+If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
+
+To use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:
+```sh
+pipx install clown_sort[PySimpleGUI]
+```
+
+![](doc/manual_select_box.png)
+
+
+# Contributing
+Feel free to file issues or open pull requests.
+
+This package is managed with [Python Poetry](http://python-poetry.org/). To get going:
+1. Install Poetry.
+1. `git clone` this repo.
+1. `cd clown_sort`
+1. `poetry install`
+1. Optional components can be install with `poetry install -E pdf -E gui`
+
+Only requirement is that tests should pass before you open it, which you can check with
+
+```
+pytest
+```
+
+[^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.
+
+[^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried's various scams as part of his commitment to "unrivaled transparency".
 
-setup(**setup_kwargs)
```

