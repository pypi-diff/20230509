# Comparing `tmp/pdfalyzer-1.8.3.tar.gz` & `tmp/pdfalyzer-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfalyzer-1.8.3.tar", max compression
+gzip compressed data, was "pdfalyzer-1.9.0.tar", max compression
```

## Comparing `pdfalyzer-1.8.3.tar` & `pdfalyzer-1.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     6505 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2022-09-10 17:07:17.000000 pdfalyzer-1.8.3/LICENSE
--rw-r--r--   0        0        0    19194 2022-10-06 02:08:45.000000 pdfalyzer-1.8.3/README.md
--rw-r--r--   0        0        0     3025 2022-10-06 04:24:21.000000 pdfalyzer-1.8.3/pdfalyzer/__init__.py
--rw-r--r--   0        0        0    14167 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/pdfalyzer/binary/binary_scanner.py
--rw-r--r--   0        0        0     7058 2022-10-03 02:07:05.000000 pdfalyzer-1.8.3/pdfalyzer/binary/bytes_decoder.py
--rw-r--r--   0        0        0     5183 2022-10-03 02:07:05.000000 pdfalyzer-1.8.3/pdfalyzer/binary/bytes_match.py
--rw-r--r--   0        0        0     7533 2022-10-03 02:07:05.000000 pdfalyzer-1.8.3/pdfalyzer/binary/decoding_attempt.py
--rw-r--r--   0        0        0     1340 2022-10-05 06:26:22.000000 pdfalyzer-1.8.3/pdfalyzer/config.py
--rw-r--r--   0        0        0     2596 2022-10-01 20:34:09.000000 pdfalyzer-1.8.3/pdfalyzer/decorators/document_model_printer.py
--rw-r--r--   0        0        0    16255 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/pdfalyzer/decorators/pdf_tree_node.py
--rw-r--r--   0        0        0     2069 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/pdfalyzer/detection/constants/binary_regexes.py
--rw-r--r--   0        0        0     4414 2022-10-03 02:06:31.000000 pdfalyzer-1.8.3/pdfalyzer/detection/constants/character_encodings.py
--rw-r--r--   0        0        0      991 2022-10-06 02:08:45.000000 pdfalyzer-1.8.3/pdfalyzer/detection/constants/javascript_reserved_keywords.py
--rw-r--r--   0        0        0     2317 2022-10-03 02:07:05.000000 pdfalyzer-1.8.3/pdfalyzer/detection/encoding_assessment.py
--rw-r--r--   0        0        0     4676 2022-10-03 02:06:31.000000 pdfalyzer-1.8.3/pdfalyzer/detection/encoding_detector.py
--rw-r--r--   0        0        0      775 2022-10-06 02:08:45.000000 pdfalyzer-1.8.3/pdfalyzer/detection/javascript_hunter.py
--rw-r--r--   0        0        0     1673 2022-10-03 02:06:31.000000 pdfalyzer-1.8.3/pdfalyzer/detection/regex_match_metrics.py
--rw-r--r--   0        0        0     5867 2022-10-03 02:07:05.000000 pdfalyzer-1.8.3/pdfalyzer/detection/yara_scanner.py
--rw-r--r--   0        0        0      625 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/pdfalyzer/detection/yaralyzer_helper.py
--rw-r--r--   0        0        0    11645 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/pdfalyzer/font_info.py
--rw-r--r--   0        0        0     5247 2022-10-03 02:07:05.000000 pdfalyzer-1.8.3/pdfalyzer/helpers/bytes_helper.py
--rw-r--r--   0        0        0      303 2022-10-05 06:26:22.000000 pdfalyzer-1.8.3/pdfalyzer/helpers/dict_helper.py
--rw-r--r--   0        0        0      492 2022-10-03 02:07:05.000000 pdfalyzer-1.8.3/pdfalyzer/helpers/file_helper.py
--rw-r--r--   0        0        0      807 2022-10-06 03:24:21.000000 pdfalyzer-1.8.3/pdfalyzer/helpers/number_helper.py
--rw-r--r--   0        0        0     3370 2022-10-05 06:26:22.000000 pdfalyzer-1.8.3/pdfalyzer/helpers/pdf_object_helper.py
--rw-r--r--   0        0        0     7017 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/pdfalyzer/helpers/rich_text_helper.py
--rw-r--r--   0        0        0     1459 2022-10-06 04:24:21.000000 pdfalyzer-1.8.3/pdfalyzer/helpers/string_helper.py
--rw-r--r--   0        0        0     3005 2022-09-30 05:28:10.431358 pdfalyzer-1.8.3/pdfalyzer/output/decoding_attempts_table.py
--rw-r--r--   0        0        0      549 2022-10-06 04:24:21.000000 pdfalyzer-1.8.3/pdfalyzer/output/layout.py
--rw-r--r--   0        0        0    23548 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/pdfalyzer/pdfalyzer.py
--rw-r--r--   0        0        0      223 2022-10-04 03:02:12.000000 pdfalyzer-1.8.3/pdfalyzer/stream_ids_for_doc_pdf.py
--rw-r--r--   0        0        0     2606 2022-10-01 20:34:09.000000 pdfalyzer-1.8.3/pdfalyzer/util/adobe_strings.py
--rw-r--r--   0        0        0     6440 2022-10-06 02:08:45.000000 pdfalyzer-1.8.3/pdfalyzer/util/argument_parser.py
--rw-r--r--   0        0        0      156 2022-10-05 06:26:22.000000 pdfalyzer-1.8.3/pdfalyzer/util/debugging.py
--rw-r--r--   0        0        0       98 2022-10-01 20:34:09.000000 pdfalyzer-1.8.3/pdfalyzer/util/exceptions.py
--rw-r--r--   0        0        0      445 2022-10-05 06:26:22.000000 pdfalyzer-1.8.3/pdfalyzer/util/filesystem_awareness.py
--rw-r--r--   0        0        0     3389 2022-10-03 02:07:05.000000 pdfalyzer-1.8.3/pdfalyzer/util/logging.py
--rw-r--r--   0        0        0     3169 2022-10-05 06:26:22.000000 pdfalyzer-1.8.3/pdfalyzer/util/pdf_parser_manager.py
--rw-r--r--   0        0        0     1522 2022-10-06 22:29:33.000000 pdfalyzer-1.8.3/pyproject.toml
--rw-r--r--   0        0        0    31147 2022-10-06 02:08:45.000000 pdfalyzer-1.8.3/yara/PDF.yara
--rw-r--r--   0        0        0      804 2022-10-06 02:08:45.000000 pdfalyzer-1.8.3/yara/PDF_binary_stream.yara
--rw-r--r--   0        0        0    20911 1970-01-01 00:00:00.000000 pdfalyzer-1.8.3/setup.py
--rw-r--r--   0        0        0    20601 1970-01-01 00:00:00.000000 pdfalyzer-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     6716 2022-10-07 03:59:53.000000 pdfalyzer-1.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2022-09-10 17:07:17.000000 pdfalyzer-1.9.0/LICENSE
+-rw-r--r--   0        0        0    19194 2022-10-06 02:08:45.000000 pdfalyzer-1.9.0/README.md
+-rw-r--r--   0        0        0     3025 2022-10-06 04:24:21.000000 pdfalyzer-1.9.0/pdfalyzer/__init__.py
+-rw-r--r--   0        0        0    14165 2022-10-07 03:59:46.000000 pdfalyzer-1.9.0/pdfalyzer/binary/binary_scanner.py
+-rw-r--r--   0        0        0     7058 2022-10-03 02:07:05.000000 pdfalyzer-1.9.0/pdfalyzer/binary/bytes_decoder.py
+-rw-r--r--   0        0        0     5183 2022-10-03 02:07:05.000000 pdfalyzer-1.9.0/pdfalyzer/binary/bytes_match.py
+-rw-r--r--   0        0        0     7533 2022-10-03 02:07:05.000000 pdfalyzer-1.9.0/pdfalyzer/binary/decoding_attempt.py
+-rw-r--r--   0        0        0     1340 2022-10-05 06:26:22.000000 pdfalyzer-1.9.0/pdfalyzer/config.py
+-rw-r--r--   0        0        0     2596 2022-10-01 20:34:09.000000 pdfalyzer-1.9.0/pdfalyzer/decorators/document_model_printer.py
+-rw-r--r--   0        0        0    16254 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/decorators/pdf_tree_node.py
+-rw-r--r--   0        0        0     2069 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/detection/constants/binary_regexes.py
+-rw-r--r--   0        0        0     4414 2022-10-03 02:06:31.000000 pdfalyzer-1.9.0/pdfalyzer/detection/constants/character_encodings.py
+-rw-r--r--   0        0        0      991 2022-10-06 02:08:45.000000 pdfalyzer-1.9.0/pdfalyzer/detection/constants/javascript_reserved_keywords.py
+-rw-r--r--   0        0        0     2317 2022-10-03 02:07:05.000000 pdfalyzer-1.9.0/pdfalyzer/detection/encoding_assessment.py
+-rw-r--r--   0        0        0     4676 2022-10-03 02:06:31.000000 pdfalyzer-1.9.0/pdfalyzer/detection/encoding_detector.py
+-rw-r--r--   0        0        0      775 2022-10-06 02:08:45.000000 pdfalyzer-1.9.0/pdfalyzer/detection/javascript_hunter.py
+-rw-r--r--   0        0        0     1673 2022-10-03 02:06:31.000000 pdfalyzer-1.9.0/pdfalyzer/detection/regex_match_metrics.py
+-rw-r--r--   0        0        0     5867 2022-10-03 02:07:05.000000 pdfalyzer-1.9.0/pdfalyzer/detection/yara_scanner.py
+-rw-r--r--   0        0        0      625 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/detection/yaralyzer_helper.py
+-rw-r--r--   0        0        0    11284 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/font_info.py
+-rw-r--r--   0        0        0     5247 2022-10-03 02:07:05.000000 pdfalyzer-1.9.0/pdfalyzer/helpers/bytes_helper.py
+-rw-r--r--   0        0        0      303 2022-10-05 06:26:22.000000 pdfalyzer-1.9.0/pdfalyzer/helpers/dict_helper.py
+-rw-r--r--   0        0        0      492 2022-10-03 02:07:05.000000 pdfalyzer-1.9.0/pdfalyzer/helpers/file_helper.py
+-rw-r--r--   0        0        0      310 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/helpers/number_helper.py
+-rw-r--r--   0        0        0     3370 2022-10-05 06:26:22.000000 pdfalyzer-1.9.0/pdfalyzer/helpers/pdf_object_helper.py
+-rw-r--r--   0        0        0     7044 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/helpers/rich_text_helper.py
+-rw-r--r--   0        0        0     1459 2022-10-06 04:24:21.000000 pdfalyzer-1.9.0/pdfalyzer/helpers/string_helper.py
+-rw-r--r--   0        0        0     3005 2022-09-30 05:28:10.431358 pdfalyzer-1.9.0/pdfalyzer/output/decoding_attempts_table.py
+-rw-r--r--   0        0        0      812 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/output/layout.py
+-rw-r--r--   0        0        0    24763 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/pdfalyzer.py
+-rw-r--r--   0        0        0      223 2022-10-04 03:02:12.000000 pdfalyzer-1.9.0/pdfalyzer/stream_ids_for_doc_pdf.py
+-rw-r--r--   0        0        0     2606 2022-10-01 20:34:09.000000 pdfalyzer-1.9.0/pdfalyzer/util/adobe_strings.py
+-rw-r--r--   0        0        0     6716 2022-10-07 03:49:29.000000 pdfalyzer-1.9.0/pdfalyzer/util/argument_parser.py
+-rw-r--r--   0        0        0      156 2022-10-05 06:26:22.000000 pdfalyzer-1.9.0/pdfalyzer/util/debugging.py
+-rw-r--r--   0        0        0       98 2022-10-01 20:34:09.000000 pdfalyzer-1.9.0/pdfalyzer/util/exceptions.py
+-rw-r--r--   0        0        0      445 2022-10-05 06:26:22.000000 pdfalyzer-1.9.0/pdfalyzer/util/filesystem_awareness.py
+-rw-r--r--   0        0        0     3389 2022-10-03 02:07:05.000000 pdfalyzer-1.9.0/pdfalyzer/util/logging.py
+-rw-r--r--   0        0        0     3169 2022-10-05 06:26:22.000000 pdfalyzer-1.9.0/pdfalyzer/util/pdf_parser_manager.py
+-rw-r--r--   0        0        0     1523 2022-10-07 03:59:46.000000 pdfalyzer-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    31147 2022-10-06 02:08:45.000000 pdfalyzer-1.9.0/yara/PDF.yara
+-rw-r--r--   0        0        0      804 2022-10-06 02:08:45.000000 pdfalyzer-1.9.0/yara/PDF_binary_stream.yara
+-rw-r--r--   0        0        0    20911 1970-01-01 00:00:00.000000 pdfalyzer-1.9.0/setup.py
+-rw-r--r--   0        0        0    20601 1970-01-01 00:00:00.000000 pdfalyzer-1.9.0/PKG-INFO
```

### Comparing `pdfalyzer-1.8.3/CHANGELOG.md` & `pdfalyzer-1.9.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # NEXT RELEASE
 
+# 1.9.0
+* Scan all binary streams, not just fonts.  Separate `--streams` option is provided. (`--font` option has much less output)
+* Display MD5, SHA1, and SHA256 for all binary streams as well as overall file
 
 # 1.8.3
 * Highlight suspicious instructions in red, BOMs in green
 * Reenable guillemet quote matching
 * Clearer labeling of binary scan results
 * Sync with `yaralyzer` v0.4.0
```

### Comparing `pdfalyzer-1.8.3/LICENSE` & `pdfalyzer-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/README.md` & `pdfalyzer-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/__init__.py` & `pdfalyzer-1.9.0/pdfalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/binary/binary_scanner.py` & `pdfalyzer-1.9.0/pdfalyzer/binary/binary_scanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from yaralyzer.util.logging import log
 
 from pdfalyzer.config import PdfalyzerConfig
 from pdfalyzer.detection.constants.binary_regexes import BACKTICK, DANGEROUS_STRINGS, FRONTSLASH, GUILLEMET, QUOTE_PATTERNS
 from pdfalyzer.helpers.rich_text_helper import (DANGER_HEADER, NOT_FOUND_MSG,
      generate_subtable, get_label_style, pad_header)
 from pdfalyzer.helpers.string_helper import generate_hyphen_line
-from pdfalyzer.output.layout import print_section_header, print_section_subheader, subheading_width
+from pdfalyzer.output.layout import half_width, print_section_header, print_section_subheader, subheading_width
 from pdfalyzer.util.adobe_strings import CURRENTFILE_EEXEC
 
 # For rainbow colors
 CHAR_ENCODING_1ST_COLOR_NUMBER = 203
 
 
 class BinaryScanner:
@@ -48,36 +48,36 @@
 
         self.stream_length = len(_bytes)
         self.regex_extraction_stats = defaultdict(lambda: RegexMatchMetrics())
         self.suppression_notice_queue = []
 
     def check_for_dangerous_instructions(self) -> None:
         """Scan for all the strings in DANGEROUS_INSTRUCTIONS list and decode bytes around them"""
-        print_section_header("Scanning Binary For Anything 'Mad Sus'...", style=DANGER_HEADER)
+        print_section_subheader("Scanning Binary For Anything 'Mad Sus'...", style=f"{DANGER_HEADER} reverse")
 
         for instruction in DANGEROUS_STRINGS:
             yaralyzer = self._pattern_yaralyzer(instruction, REGEX)
             yaralyzer.highlight_style = 'bright_red bold'
             self.process_yara_matches(yaralyzer, instruction, force=True)
 
     def check_for_boms(self) -> None:
-        print_section_subheader("Scanning Binary for any BOMs...")
+        print_section_subheader("Scanning Binary for any BOMs...", style='BOM')
 
         for bom_bytes, bom_name in BOMS.items():
             yaralyzer = self._pattern_yaralyzer(hex_string(bom_bytes), HEX, bom_name)
-            yaralyzer.highlight_style = 'bright_green bold'
+            yaralyzer.highlight_style = 'BOM'
             self.process_yara_matches(yaralyzer, bom_name, force=True)
 
     def force_decode_all_quoted_bytes(self) -> None:
         """Find all strings matching QUOTE_PATTERNS (AKA between quote chars) and decode them with various encodings"""
         quote_types = QUOTE_PATTERNS.keys() if PdfalyzerConfig.QUOTE_TYPE is None else [PdfalyzerConfig.QUOTE_TYPE]
 
         for quote_type in quote_types:
             quote_pattern = QUOTE_PATTERNS[quote_type]
-            print_section_header(f"Forcing Decode of {quote_type.capitalize()} Quoted Strings", style=BYTES_NO_DIM)
+            print_section_subheader(f"Forcing Decode of {quote_type.capitalize()} Quoted Strings", style=BYTES_NO_DIM)
             yaralyzer = self._quote_yaralyzer(quote_pattern, quote_type)
             self.process_yara_matches(yaralyzer, f"{quote_type}_quoted")
 
     # -------------------------------------------------------------------------------
     # These extraction iterators will iterate over all matches for a specific pattern.
     # extract_regex_capture_bytes() is the generalized method that acccepts any regex.
     # -------------------------------------------------------------------------------
@@ -96,30 +96,30 @@
     def print_stream_preview(self, num_bytes=None, title_suffix=None) -> None:
         """Print a preview showing the beginning and end of the stream data"""
         num_bytes = num_bytes or console_width()
         snipped_byte_count = self.stream_length - (num_bytes * 2)
         console.line()
 
         if snipped_byte_count < 0:
-            title = f"All {self.stream_length} bytes in stream"
+            title = f"ALL {self.stream_length} BYTES IN STREAM"
         else:
-            title = f"First and last {num_bytes} bytes of {self.stream_length} byte stream"
+            title = f"FIRST AND LAST {num_bytes} BYTES OF {self.stream_length} BYTE STREAM"
 
         title += title_suffix if title_suffix is not None else ''
-        console.print(Panel(title, style='bytes.title', expand=False))
-        console.print(generate_hyphen_line(title='BEGIN BYTES'), style='dim')
+        title = f"BEGIN {title}".upper()
+        console.print(generate_hyphen_line(title=title), style='dim')
 
         if snipped_byte_count < 0:
             print_bytes(self.bytes)
         else:
             print_bytes(self.bytes[:num_bytes])
             console.print(f"\n    <...skip {snipped_byte_count} bytes...>\n", style='dim')
             print_bytes(self.bytes[-num_bytes:])
 
-        console.print(generate_hyphen_line(title='END BYTES'), style='dim')
+        console.print(generate_hyphen_line(title=title), style='dim')
         console.line()
 
     def print_decoding_stats_table(self) -> None:
         """Diplay aggregate results on the decoding attempts we made on subsets of self.bytes"""
         stats_table = new_decoding_stats_table(self.label.plain if self.label else '')
         regexes_not_found_in_stream = []
 
@@ -146,15 +146,15 @@
             stats_table.add_row(str(matcher), regex_subtable, decodes_subtable)
 
         for row in regexes_not_found_in_stream:
             row[0] = Text(row[0], style='color(235)')
             stats_table.add_row(*row, style='color(232)')
 
         console.line(2)
-        console.print(stats_table)
+        console.print(stats_table, justify='center')
 
     def process_yara_matches(self, yaralyzer: Yaralyzer, pattern: str, force: bool = False) -> None:
         """Decide whether to attempt to decode the matched bytes, track stats. force param ignores min/max length"""
         for bytes_match, bytes_decoder in yaralyzer.match_iterator():
             self.regex_extraction_stats[pattern].match_count += 1
             self.regex_extraction_stats[pattern].bytes_matched += bytes_match.match_length
             self.regex_extraction_stats[pattern].bytes_match_objs.append(bytes_match)
@@ -257,15 +257,15 @@
 def new_decoding_stats_table(title) -> Table:
     """Build an empty table for displaying decoding stats"""
     title = prefix_with_plain_text_obj(title, style='blue underline')
     title.append(": Decoding Attempts Summary Statistics", style='bright_white bold')
 
     table = Table(
         title=title,
-        min_width=subheading_width(),
+        min_width=half_width(),
         show_lines=True,
         padding=(0, 1),
         style='color(18)',
         border_style='color(111) dim',
         header_style='color(235) on color(249) reverse',
         title_style='color(249) bold')
```

### Comparing `pdfalyzer-1.8.3/pdfalyzer/binary/bytes_decoder.py` & `pdfalyzer-1.9.0/pdfalyzer/binary/bytes_decoder.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/binary/bytes_match.py` & `pdfalyzer-1.9.0/pdfalyzer/binary/bytes_match.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/binary/decoding_attempt.py` & `pdfalyzer-1.9.0/pdfalyzer/binary/decoding_attempt.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/config.py` & `pdfalyzer-1.9.0/pdfalyzer/config.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/decorators/document_model_printer.py` & `pdfalyzer-1.9.0/pdfalyzer/decorators/document_model_printer.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/decorators/pdf_tree_node.py` & `pdfalyzer-1.9.0/pdfalyzer/decorators/pdf_tree_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
      StreamObject)
 from rich.markup import escape
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 from rich.tree import Tree
 from yaralyzer.helpers.bytes_helper import clean_byte_string, hex_text
+from yaralyzer.helpers.rich_text_helper import size_text
 from yaralyzer.output.rich_console import BYTES_NO_DIM, YARALYZER_THEME, console
 from yaralyzer.util.logging import log
 
 from yaralyzer.encoding_detection.character_encodings import NEWLINE_BYTE
-from pdfalyzer.helpers.number_helper import size_string
 from pdfalyzer.helpers.pdf_object_helper import get_references, get_symlink_representation
 from pdfalyzer.helpers.rich_text_helper import (PDF_ARRAY, TYPE_STYLES, get_label_style,
      get_type_style, get_type_string_style)
 from pdfalyzer.helpers.string_helper import pypdf_class_name
 from pdfalyzer.util.adobe_strings import (DANGEROUS_PDF_KEYS, FIRST, FONT, LAST, NEXT, TYPE1_FONT, S,
      SUBTYPE, TRAILER, TYPE, UNLABELED, XREF, XREF_STREAM)
 from pdfalyzer.util.exceptions import PdfWalkError
@@ -281,15 +281,15 @@
 
             style = PREVIEW_STYLES[hex_or_stream]
             row_label = f"{hex_or_stream}{row_label}\n  ({stream_preview_length} bytes)"
             return_rows.append([Text(row_label, 'grey'), Text(stream_string, style)])
 
         add_preview_row(STREAM, stream_preview_string)
         add_preview_row(HEX, stream_preview_hex)
-        return_rows.append([Text('StreamLength', style='grey'), size_string(len(self.stream_data))])
+        return_rows.append([Text('StreamLength', style='grey'), size_text(len(self.stream_data))])
         return return_rows
 
     def generate_rich_tree(self, tree=None, depth=0):
         """Recursively generates a rich.tree.Tree object from this node"""
         tree = tree or Tree(self.generate_rich_table())
 
         for child in self.children:
```

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/constants/binary_regexes.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/constants/binary_regexes.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/constants/character_encodings.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/constants/character_encodings.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/constants/javascript_reserved_keywords.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/constants/javascript_reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/encoding_assessment.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/encoding_assessment.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/encoding_detector.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/encoding_detector.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/javascript_hunter.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/javascript_hunter.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/regex_match_metrics.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/regex_match_metrics.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/yara_scanner.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/yara_scanner.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/detection/yaralyzer_helper.py` & `pdfalyzer-1.9.0/pdfalyzer/detection/yaralyzer_helper.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/font_info.py` & `pdfalyzer-1.9.0/pdfalyzer/font_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 from rich.panel import Panel
 from rich.padding import Padding
 from rich.table import Table
 from rich.text import Text
 from yaralyzer.config import YaralyzerConfig
 from yaralyzer.helpers.bytes_helper import print_bytes
 from yaralyzer.output.rich_console import console
+from yaralyzer.output.rich_layout_elements import bytes_hashes_table
 from yaralyzer.util.logging import log
 
 from pdfalyzer.binary.binary_scanner import BinaryScanner
 from pdfalyzer.config import PdfalyzerConfig
 from pdfalyzer.detection.yaralyzer_helper import get_bytes_yaralyzer
 from pdfalyzer.helpers.rich_text_helper import get_label_style, get_type_style
 from pdfalyzer.helpers.string_helper import pp
-from pdfalyzer.output.layout import subheading_width
+from pdfalyzer.output.layout import print_section_subheader, subheading_width
 from pdfalyzer.util.adobe_strings import (FONT, FONT_DESCRIPTOR, FONT_FILE, FONT_LENGTHS, RESOURCES, SUBTYPE,
      TO_UNICODE, TYPE, W, WIDTHS)
 
 
 CHARMAP_TITLE_PADDING = (1, 0, 0, 2)
 CHARMAP_PADDING = (0, 2, 0, 10)
 CHARMAP_TITLE = 'Character Mapping (As Extracted By PyPDF2)'
@@ -161,25 +162,14 @@
 
     def print_summary(self):
         """Prints a table of info about the font drawn from the various PDF objects. quote_type of None means all."""
         self.print_header_panel()
         console.print(self._summary_table())
         self.print_character_mapping()
         self.print_prepared_charmap()
-
-        if self.binary_scanner is not None:
-            self.binary_scanner.print_stream_preview(title_suffix=f" of /FontFile for {self.display_title}")
-            self.binary_scanner.check_for_dangerous_instructions()
-            self.binary_scanner.check_for_boms()
-
-            if not YaralyzerConfig.SUPPRESS_DECODES:
-                self.binary_scanner.force_decode_all_quoted_bytes()
-
-            self.binary_scanner.print_decoding_stats_table()
-
         console.line(2)
 
     def print_character_mapping(self):
         """Prints the character mapping extracted by PyPDF2._charmap in tidy columns"""
         if self.character_mapping is None or len(self.character_mapping) == 0:
             log.info(f"No character map found in {self}")
             return
```

### Comparing `pdfalyzer-1.8.3/pdfalyzer/helpers/bytes_helper.py` & `pdfalyzer-1.9.0/pdfalyzer/helpers/bytes_helper.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/helpers/pdf_object_helper.py` & `pdfalyzer-1.9.0/pdfalyzer/helpers/pdf_object_helper.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/helpers/rich_text_helper.py` & `pdfalyzer-1.9.0/pdfalyzer/helpers/rich_text_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 # PDF object styles
 PDF_ARRAY = 'color(120)'
 PDF_NON_TREE_REF = 'color(243)'
 
 PDFALYZER_THEME_DICT = YARALYZER_THEME_DICT.copy()
 PDFALYZER_THEME_DICT.update({
     'address': GREY_ADDRESS,
+    'BOM': 'bright_green',
     # PDF objects
     'pdf.array': PDF_ARRAY,
     'pdf.non_tree_ref': PDF_NON_TREE_REF,
     # fonts
     'font.property': 'color(135)',
     'font.title': 'reverse dark_blue on color(253)',
     # charmap
```

### Comparing `pdfalyzer-1.8.3/pdfalyzer/helpers/string_helper.py` & `pdfalyzer-1.9.0/pdfalyzer/helpers/string_helper.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/output/decoding_attempts_table.py` & `pdfalyzer-1.9.0/pdfalyzer/output/decoding_attempts_table.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/output/layout.py` & `pdfalyzer-1.9.0/pdfalyzer/output/layout.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,23 @@
 
 
 
 def subheading_width() -> int:
     return int(console_width() * 0.75)
 
 
+def half_width() -> int:
+    return int(console_width() * 0.5)
+
+
 def print_section_header(headline: str, style: str = '') -> None:
-    print_section_subheader(headline, f"{style} reverse", True)
+    print_section_subheader(headline, f"{style} reverse", True, console_width())
 
 
-def print_section_subheader(headline: str, style: str = '', expand: bool = False) -> None:
+def print_section_subheader(headline: str, style: str = '', expand: bool = True, width = None) -> None:
     console.line(2)
-    console.print(Panel(headline, style=style, expand=expand))
+    console.print(Panel(headline, style=style, expand=expand, width=width or subheading_width()))
     console.line()
+
+
+def print_section_sub_subheader(headline: str, style: str = ''):
+    print_section_subheader(headline, style, False, half_width())
```

### Comparing `pdfalyzer-1.8.3/pdfalyzer/pdfalyzer.py` & `pdfalyzer-1.9.0/pdfalyzer/pdfalyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,30 @@
 from anytree.search import findall_by_attr
 from PyPDF2 import PdfReader
 from PyPDF2.errors import PdfReadError
 from PyPDF2.generic import IndirectObject, NameObject, NumberObject, StreamObject
 from rich.panel import Panel
 from rich.table import Column, Table
 from rich.text import Text
-from pdfalyzer.detection.yaralyzer_helper import get_file_yaralyzer
+from yaralyzer.config import YaralyzerConfig
+from yaralyzer.helpers.bytes_helper import get_bytes_info
 from yaralyzer.helpers.file_helper import load_binary_data
-from yaralyzer.output.rich_console import console, theme_colors_with_prefix
+from yaralyzer.helpers.rich_text_helper import CENTER, LEFT, size_in_bytes_text
+from yaralyzer.output.rich_console import BYTES_HIGHLIGHT, GREY, console, console_width, theme_colors_with_prefix
+from yaralyzer.output.rich_layout_elements import bytes_hashes_table
 from yaralyzer.util.logging import log
 
+from pdfalyzer.binary.binary_scanner import BinaryScanner
 from pdfalyzer.decorators.document_model_printer import print_with_header
 from pdfalyzer.decorators.pdf_tree_node import PdfTreeNode
-from pdfalyzer.helpers.number_helper import size_string, size_in_bytes_string
+from pdfalyzer.detection.yaralyzer_helper import get_file_yaralyzer
 from pdfalyzer.helpers.pdf_object_helper import get_symlink_representation
 from pdfalyzer.helpers.string_helper import pp
 from pdfalyzer.font_info import FontInfo
-from pdfalyzer.output.layout import print_section_header, print_section_subheader
+from pdfalyzer.output.layout import print_section_header, print_section_subheader, print_section_sub_subheader
 from pdfalyzer.util.adobe_strings import (COLOR_SPACE, D, DEST, EXT_G_STATE, FONT, K, KIDS,
      NON_TREE_REFERENCES, NUMS, OBJECT_STREAM, OPEN_ACTION, P, PARENT, PREV, RESOURCES, SIZE,
      STRUCT_ELEM, TRAILER, TYPE, UNLABELED, XOBJECT, XREF, XREF_STREAM)
 from pdfalyzer.util.exceptions import PdfWalkError
 
 TRAILER_FALLBACK_ID = 10000000
 
@@ -56,17 +60,15 @@
 
 
 class Pdfalyzer:
     def __init__(self, pdf_path: str):
         self.pdf_path = pdf_path
         self.pdf_basename = basename(pdf_path)
         self.pdf_bytes = load_binary_data(pdf_path)
-        self.md5 = hashlib.md5(self.pdf_bytes ).hexdigest().upper()
-        self.sha1 = hashlib.sha1(self.pdf_bytes ).hexdigest().upper()
-        self.sha256 = hashlib.sha256(self.pdf_bytes ).hexdigest().upper()
+        self.pdf_bytes_info = get_bytes_info(self.pdf_bytes)
         pdf_file = open(pdf_path, 'rb')  # Filehandle must be left open for PyPDF2 to perform seeks
         self.pdf = PdfReader(pdf_file)
         self.yaralyzer = get_file_yaralyzer(pdf_path)
 
         # Initialize tracking variables
         self.indeterminate_ids = set()  # See INDETERMINATE_REFERENCES comment
         self.traversed_nodes = {}
@@ -135,23 +137,17 @@
         self.print_font_info()
         self.print_other_relationships()
 
     def print_document_info(self) -> None:
         """Print the embedded document info (author, timestamps, version, etc)"""
         print_section_header(f'Document Info for {self.pdf_basename}')
         console.print(pp.pformat(self.pdf.getDocumentInfo()))
-
-        table = Table('File Size', Column(size_string(len(self.pdf_bytes))))
-        table.add_row('MD5', self.md5)
-        table.add_row('SHA1', self.sha1)
-        table.add_row('SHA256', self.sha256)
-        table.columns[1].style = 'orange3'
-        table.columns[1].header_style = 'bright_cyan'
-        console.print(table)
-        self.print_stream_objects()
+        console.line()
+        console.print(bytes_hashes_table(self.pdf_bytes, self.pdf_basename))
+        console.line()
 
     def print_tree(self):
         print_section_header(f'Simple tree view of {self.pdf_basename}')
 
         for pre, _fill, node in RenderTree(self.pdf_tree, style=DoubleStyle):
             if isinstance(node, SymlinkNode):
                 symlink_rep = get_symlink_representation(node.parent, node)
@@ -171,14 +167,43 @@
 
     def print_font_info(self, font_idnum=None) -> None:
         print_section_header(f'{len(self.font_infos)} fonts found in {self.pdf_basename}')
 
         for font_info in [fi for fi in self.font_infos if font_idnum is None or font_idnum == fi.idnum]:
             font_info.print_summary()
 
+    def print_streams_analysis(self) -> None:
+        print_section_header(f'Binary Stream Analysis / Extraction')
+        console.print(self.stream_objects_table())
+
+        for node in self.stream_node_iterator():
+            node_stream_bytes = node.stream_data
+
+            if node_stream_bytes is None or node.stream_length == 0:
+                print_section_sub_subheader(f"{node} stream has length 0", style='dim')
+                continue
+
+            if not isinstance(node_stream_bytes, bytes):
+                msg = f"Stream in {node} is not bytes, it's {type(node.stream_data)}. Will reencode for YARA " + \
+                       "but they may not be the same bytes as the original stream!"
+                log.warning(msg)
+                node_stream_bytes = node_stream_bytes.encode()
+
+            print_section_subheader(f"{node} Analysis", style=BYTES_HIGHLIGHT, width=console_width())
+            binary_scanner = BinaryScanner(node_stream_bytes, node, node.__rich__())
+            console.print(bytes_hashes_table(binary_scanner.bytes))
+            binary_scanner.print_stream_preview()
+            binary_scanner.check_for_dangerous_instructions()
+
+            if not YaralyzerConfig.SUPPRESS_DECODES:
+                binary_scanner.check_for_boms()
+                binary_scanner.force_decode_all_quoted_bytes()
+
+            binary_scanner.print_decoding_stats_table()
+
     def print_yara_results(self, font_idnum=None) -> None:
         print_section_header(f'YARA Scan for {self.pdf_basename}')
         theme_colors = [color[len('yara') + 1:] for color in theme_colors_with_prefix('yara')]
         color_key = Text('Color Code: ') + Text(' ').join(theme_colors) + Text('\n')
         console.print(color_key, justify='center')
         self.yaralyzer.yaralyze()
 
@@ -195,33 +220,27 @@
             if len(node.other_relationships) == 0:
                 continue
 
             console.print("\n")
             console.print(Panel(f"Non tree relationships for {node}", expand=False))
             node.print_other_relationships()
 
-    def print_traversed_nodes(self) -> None:
-        """Debug method that displays which nodes have already been walked"""
-        for i in sorted(self.traversed_nodes.keys()):
-            console.print(f'{i}: {self.traversed_nodes[i]}')
-
-    def print_stream_objects(self) -> None:
-        print_section_subheader(f'Stream Summary for {self.pdf_basename}')
-
+    def stream_objects_table(self) -> Table:
         table = Table('Stream Length', 'Node')
+
         table.columns[0].justify = 'right'
         stream_nodes: List[PdfTreeNode] = []
 
         for node in self.stream_node_iterator():
             stream_nodes.append(node)
 
         for node in sorted(stream_nodes, key=lambda r: r.idnum):
-            table.add_row(size_in_bytes_string(node.stream_length), node.__rich__())
+            table.add_row(size_in_bytes_text(node.stream_length), node.__rich__())
 
-        console.print(table)
+        return table
 
     def stream_node_iterator(self) -> Iterator[PdfTreeNode]:
         for node in LevelOrderIter(self.pdf_tree):
             if isinstance(node.obj, StreamObject):
                 yield node
 
     def _process_reference(self, node: PdfTreeNode, key: str, address: str, reference: IndirectObject) -> [PdfTreeNode]:
@@ -416,14 +435,19 @@
         return {
             'keys_encountered': keys_encountered,
             'node_count': node_count,
             'node_labels': node_labels,
             'pdf_object_types': pdf_object_types,
         }
 
+    def _print_traversed_nodes(self) -> None:
+        """Debug method that displays which nodes have already been walked"""
+        for i in sorted(self.traversed_nodes.keys()):
+            console.print(f'{i}: {self.traversed_nodes[i]}')
+
     def _verify_all_traversed_nodes_are_in_tree(self) -> None:
         """Make sure every node we can see is reachable from the root of the tree"""
         missing_nodes = [node for idnum, node in self.traversed_nodes.items() if self.find_node_by_idnum(idnum) is None]
 
         if len(missing_nodes) > 0:
             msg = f"Nodes were traversed but never placed: {missing_nodes}"
             console.print(msg)
```

### Comparing `pdfalyzer-1.8.3/pdfalyzer/util/adobe_strings.py` & `pdfalyzer-1.9.0/pdfalyzer/util/adobe_strings.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/util/argument_parser.py` & `pdfalyzer-1.9.0/pdfalyzer/util/argument_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,15 +70,18 @@
                          "try '-f -- [the rest]' if you run into an argument position related piccadilly.",
                     nargs='?',
                     const=ALL_FONTS_OPTION,
                     metavar='ID',
                     type=int)
 
 select.add_argument('-y', '--yara', action='store_true',
-                    help="scan the PDF and all its decoded/decrypted binary streams with YARA rules")
+                    help="scan the PDF with YARA rules")
+
+select.add_argument('-s', '--streams', action='store_true',
+                    help="scan all the PDF's decoded/decrypted for suspicious bytes as well as any YARA rule matches")
 
 select.add_argument('--quote-type',
                     help='scan binary data for quoted data of this type only or all types if not set',
                     choices=list(QUOTE_REGEXES.keys()))
 
 # Make sure the selection section is at the top
 parser._action_groups = parser._action_groups[:2] + [parser._action_groups[-1]] + parser._action_groups[2:-1]
@@ -119,22 +122,24 @@
     """
     # Create a partial for print_font_info() because it's the only one that can take an argument
     # partials have no __name__ so update_wrapper() propagates the 'print_font_info' as this partial's name
     font_id = None if args.font == ALL_FONTS_OPTION else args.font
     font_info = partial(pdfalyzer.print_font_info, font_idnum=font_id)
     update_wrapper(font_info, pdfalyzer.print_font_info)
 
-    # Top to bottom is the default order of output
+    # The first element string matches the argument in 'select' group.
+    # Top to bottom is the default order of output.
     possible_output_sections = [
         OutputSection('docinfo', pdfalyzer.print_document_info),
         OutputSection('tree', pdfalyzer.print_tree),
         OutputSection('rich', pdfalyzer.print_rich_table_tree),
         OutputSection('font', font_info),
         OutputSection('counts', pdfalyzer.print_summary),
-        OutputSection('yara', pdfalyzer.print_yara_results)
+        OutputSection('yara', pdfalyzer.print_yara_results),
+        OutputSection('streams', pdfalyzer.print_streams_analysis),
     ]
 
     output_sections = [section for section in possible_output_sections if vars(args)[section.argument]]
 
     if len(output_sections) == 0:
         log_and_print("No output section specified so outputting all sections...")
         return possible_output_sections
```

### Comparing `pdfalyzer-1.8.3/pdfalyzer/util/logging.py` & `pdfalyzer-1.9.0/pdfalyzer/util/logging.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pdfalyzer/util/pdf_parser_manager.py` & `pdfalyzer-1.9.0/pdfalyzer/util/pdf_parser_manager.py`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/pyproject.toml` & `pdfalyzer-1.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdfalyzer"
-version = "1.8.3"
+version = "1.9.0"
 description = "A PDF analysis toolkit. Scan a PDF with relevant YARA rules, visualize its inner tree-like data structure in living color (lots of colors), force decodes of suspicious font binaries, and more."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/michelcrypt4d4mus/pdfalyzer"
 repository = "https://github.com/michelcrypt4d4mus/pdfalyzer"
 documentation = "https://github.com/michelcrypt4d4mus/pdfalyzer"
@@ -45,15 +45,16 @@
 python = "^3.9"
 anytree = "~=2.8"
 Deprecated = "^1.2.13"
 PyPDF2 = "^2.10"
 python-dotenv = "^0.21.0"
 rich = "^12.5.1"
 rich-argparse = "^0.3.0"
-yaralyzer = "^0.4.0"
+yaralyzer = "^0.5.2"
+
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pdfalyzer-1.8.3/yara/PDF.yara` & `pdfalyzer-1.9.0/yara/PDF.yara`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/yara/PDF_binary_stream.yara` & `pdfalyzer-1.9.0/yara/PDF_binary_stream.yara`

 * *Files identical despite different names*

### Comparing `pdfalyzer-1.8.3/setup.py` & `pdfalyzer-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 install_requires = \
 ['Deprecated>=1.2.13,<2.0.0',
  'PyPDF2>=2.10,<3.0',
  'anytree>=2.8,<3.0',
  'python-dotenv>=0.21.0,<0.22.0',
  'rich-argparse>=0.3.0,<0.4.0',
  'rich>=12.5.1,<13.0.0',
- 'yaralyzer>=0.4.0,<0.5.0']
+ 'yaralyzer>=0.5.2,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['pdfalyze = pdfalyzer:pdfalyze',
                      'pdfalyzer_show_color_theme = '
                      'pdfalyzer.helpers.rich_text_helper:pdfalyzer_show_color_theme']}
 
 setup_kwargs = {
     'name': 'pdfalyzer',
-    'version': '1.8.3',
+    'version': '1.9.0',
     'description': 'A PDF analysis toolkit. Scan a PDF with relevant YARA rules, visualize its inner tree-like data structure in living color (lots of colors), force decodes of suspicious font binaries, and more.',
     'long_description': '# THE PDFALYZER\nA PDF analysis tool geared towards visualizing the inner tree-like data structure[^1] of a PDF in [spectacularly large and colorful diagrams](#example-output) as well as scanning the various kinds of binary data within the PDF for hidden potentially malicious content.\n\nThe Pdfalyzer makes heavy use of YARA (via [The Yaralyzer](https://github.com/michelcrypt4d4mus/yaralyzer)) for matching/extracting byte patterns. [The Yaralyzer](https://github.com/michelcrypt4d4mus/yaralyzer) actually began its life as The Pdfalyzer\'s matching engine.\n\n**PyPi Users:** If you are reading this document [on PyPi](https://pypi.org/project/pdfalyzer/) be aware that it renders a lot better [over on GitHub](https://github.com/michelcrypt4d4mus/pdfalyzer). Lots of pretty pictures, footnotes that work, etc.\n\n#### Quick Start\n```sh\npipx install pdfalyzer\npdfalyze the_heidiggerian_themes_expressed_in_illmatic.pdf\n```\n`pip install pdfalyzer` also works. See [Installation](#installation) and [Usage](#usage) for more details.\n\n### What It Do\n1. **Generate summary format as well as in depth visualizations of a PDF\'s tree structure**[^1] with helpful color themes that conceptually link objects of similar type. See [the examples below](#example-output) to get an idea.\n1. **Display text representations of the PDF\'s embedded binary data**. Adobe calls these "streams" and they hold things like images, fonts, etc.\n1. **Scan for malicious content in the PDF** both with PDF related [YARA](https://github.com/VirusTotal/yara-python) rules collected from around the internet as well as custom in-depth scans of the embedded font binaries where other tools don\'t look. These scans will be done both to the overall finay binary as well as to each of the PDF\'s embedded binary streams _post decode/decrypt_. Most PDFs have many such streams.\n1. **Show the results of attempting to decode suspicious byte patterns with many differente character encodings.** In particular quoted bytes - those between things like front slashes (hint: think regexes) in addition to regular quote characters. Several encodings are configured as defaults to try but [the `chardet` library](https://github.com/chardet/chardet) is also leveraged to attempt to detect if the binary could be in an unconfigured encoding.\n1. **Be used as a library for your own PDF related code.** All[^2] the inner PDF objects are guaranteed to be available in a searchable tree data structure.\n1. **Ease the extraction of all the binary data in a PDF** (fonts, images, etc) to separate files for further analysis. (The heavy lifting is actually done by [Didier Stevens\'s tools](#installing-didier-stevenss-pdf-analysis-tools) - the pdfalyzer automates what would otherwise be a lot of typing into a single command.)\n\nIf you\'re looking for one of these things this may be the tool for you.\n\nAn exception will be raised if there\'s any issue placing a node while parsing or if there are any nodes not reachable from the root of the tree at the end of parsing.\n\n### What It Don\'t Do\nThis tool is mostly about examining a PDF\'s logical structure and assisting with the discovery of malicious content. As such it doesn\'t have much to offer as far as extracting text from PDFs, rendering PDFs[^3], writing new PDFs, or many of the more conventional things one might do with a portable document.\n\n### Did The World Really Need Another PDF Tool?\nThis tool was built to fill a gap in the PDF assessment landscape following my . Didier Stevens\'s [pdfid.py](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pdfid.py) and [pdf-parser.py](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pdf-parser.py) are still the best game in town when it comes to PDF analysis tools but they lack in the visualization department and also don\'t give you much to work with as far as giving you a data model you can write your own code around. [Peepdf](https://github.com/jesparza/peepdf) seemed promising but turned out to be in a buggy, out of date, and more or less unfixable state. And neither of them offered much in the way of tooling for embedded font analysis.\n\nAll those things being the case lead to a situation where I felt the world might be slightly improved if I strung together a couple of more stable/well known/actively maintained open source projects ([AnyTree](https://github.com/c0fec0de/anytree), [PyPDF2](https://github.com/py-pdf/PyPDF2), and [Rich](https://github.com/Textualize/rich)) into this tool.\n\n\n\n# Example Output\nThe Pdfalyzer can export visualizations to HTML, ANSI colored text, and SVG images using the file export functionality that comes with [Rich](https://github.com/Textualize/rich). SVGs can be turned into `png` format images with a tool like `inkscape` or `cairosvg` (Inkscape works a lot better in our experience).\n\n\n### Basic Tree View\nAs you can see the "mad sus" `/OpenAction` relationship is highlighted bright red, as would be a couple of other suspicious PDF instructions like `/JavaScript` that don\'t exist in the PDF but do exist in other documents.\n\nThe dimmer (as in "harder to see") nodes[^4] marked with `Non Child Reference` give you a way to visualize the relationships between PDF objects that exist outside of the tree structure\'s parent/child relationships.\n\n![Basic Tree](doc/svgs/rendered_images/basic_tree.png)\n\nThat\'s a pretty basic document. If you\'d like to see the tree for a more complicated/longer PDF, [here\'s an example showing the `nmap` cheat sheet](doc/svgs/rendered_images/NMAP_Commands_Cheat_Sheet_and_Tutorial.pdf.tree.svg.png).\n\n### Rich Tree View\nThis image shows a more in-depth view of of the PDF tree for the same document shown above. This tree (AKA the "rich" tree) has almost everything - shows all PDF object properties, all relationships between objects. Even includes sizable previews of any binary data streams embedded or encrypted in the document. Note that the `/OpenAction` is highlighted in bright red, as is the Adobe Type1 font binary (Google\'s project zero regards any Adobe Type1 font as "mad sus").\n\n[Here\'s an even bigger example showing the same `nmap` cheat sheet](doc/svgs/rendered_images/NMAP_Commands_Cheat_Sheet_and_Tutorial.pdf.rich_table_tree.png).\n\n![Rich Tree](doc/svgs/rendered_images/rich_table_tree.png)\n\n### Font Analysis (And Lots Of It)\n#### View the Properties of the Fonts in the PDF\nComes with a preview of the beginning and end of the font\'s raw binary data stream (at least if it\'s that kind of font).\n\n![Font Properties](doc/svgs/rendered_images/font_summary_with_byte_preview.png)\n\n#### Extract Character Mappings from Ancient Adobe Font Formats\nIt\'s actually `PyPDF2` doing the lifting here but we\'re happy to take the credit.\n\n![Font Charmap](doc/svgs/rendered_images/font_character_mapping.png)\n\n#### Search Encrypted Binary Font Data for #MadSus Content No Malware Scanner Will Catch[^5]\n\nThings like, say, a hidden binary `/F` (PDF instruction meaning "URL") followed by a `JS` (I\'ll let you guess what "JS" stands for) and then a binary `»` character (AKA "the character the PDF specification uses to close a section of the PDF\'s logical structure"). Put all that together and it says that you\'re looking at a secret JavaScript instruction embedded in the encrypted part of a font binary. A secret instruction that causes the PDF renderer to pop out of its frame prematurely as it renders the font.\n\n![Font with JS](doc/svgs/rendered_images/font29.js.1.png)\n\n#### Extract And Decode Binary Patterns\nLike, say, bytes between common regular expression markers that you might want to force a decode of in a lot of different encodings.\n\n![Font Scan Regex](doc/svgs/rendered_images/font_34_frontslash_scan.png)\n\nWhen all is said and done you can see some stats that may help you figure out what the character encoding may or may not be for the bytes matched by those patterns:\n\n![Font Decode Summary](doc/svgs/rendered_images/font29_summary_stats.png)\n\n\n#### Now There\'s Even A Fancy Table To Tell You What The `chardet` Library Would Rank As The Most Likely Encoding For A Chunk Of Binary Data\nBehold the beauty:\n![Basic Tree](doc/svgs/rendered_images/decoding_and_chardet_table_2.png)\n\n### Compute Summary Statistics About A PDF\'s Inner Structure\nSome simple counts of some properties of the internal PDF objects. Not the most exciting but sometimes helpful. `pdfid.py` also does something much like this. Not exciting enough to show a screenshot.\n\n\n# Installation\n\n```\npipx install pdfalyzer\n```\n\n[pipx](https://pypa.github.io/pipx/) is a tool that basically runs `pip install` for a python package but in such a way that the installed package\'s requirements are isolated from your system\'s python packages. If you  don\'t feel like installing `pipx` then `pip install` should work fine as long as there are no conflicts between The Pdfalyzer\'s required packages and those on your system already. (If you aren\'t using other python based command line tools then your odds of a conflict are basically 0%.)\n\nFor info on how to setup a dev environment, see [Contributing](#contributing) section at the end of this file.\n\n### Troubleshooting The Installation\n1. If you encounter an error building the python `cryptography` package check your `pip` version (`pip --version`). If it\'s less than 22.0, upgrade `pip` with `pip install --upgrade pip`.\n2. On linux if you encounter an error building `wheel` or `cffi` you may need to install some packages like a compiler for the `rust` language or some SSL libraries. `sudo apt-get install build-essential libssl-dev libffi-dev rustc` may help.\n1. While `poetry.lock` is checked into this repo the versions "required" there aren\'t really "required" so feel free to delete or downgrade if you need to.\n\n### 3rd Party Tools\n#### Installing Didier Stevens\'s PDF Analysis Tools\nStevens\'s tools provide comprehensive info about the contents of a PDF, are guaranteed not to trigger the rendering of any malicious content (especially `pdfid.py`), and have been battle tested for well over a decade. It would probably be a good idea to analyze your PDF with his tools before you start working with this one.\n\nIf you\'re lazy and don\'t want to retrieve his tools yourself there\'s [a simple bash script](scripts/install_didier_stevens_pdf_tools.sh) to download them from his github repo and place them in a `tools/` subdirectory off the project root. Just run this:\n\n```sh\nscripts/install_didier_stevens_pdf_tools.sh\n```\n\nIf there is a discrepancy between the output of betweeen his tools and this one you should assume his tool is correct and The Pdfalyzer is wrong until you conclusively prove otherwise.\n\n#### Installing The `t1utils` Font Suite\n`t1utils` is a suite of old but battle tested apps for manipulating old Adobe font formats.  You don\'t need it unless you\'re dealing with an older Type 1 or Type 2 font binary but given that those have been very popular exploit vectors in the past few years it can be extremely helpful. One of the tools in the suite, [`t1disasm`](https://www.lcdf.org/type/t1disasm.1.html), is particularly useful because it decrypts and decompiles Adobe Type 1 font binaries into a more human readable string representation.\n\nThere\'s [a script](scripts/install_t1utils.sh) to help you install the suite if you need it:\n\n```sh\nscripts/install_t1utils.sh\n```\n\n\n\n# Usage\nRun `pdfalyze --help` to see usage instructions. As of right now these are the options:\n\n![argparse_help](doc/svgs/rendered_images/pdfalyzer_help.png)\n\nBeyond that there\'s [a few scripts](scripts/) in the repo that may be of interest.\n\n### Setting Command Line Options Permanently With A `.pdfalyzer` File\nIf you find yourself specificying the same options over and over you may be able to automate that with a [dotenv](https://pypi.org/project/python-dotenv/) setup. When you run `pdfalyze` on some PDF the tool will check for a file called `.pdfalyzer` first in the current directory and then in the home directory. If it finds a file in either such place it will load options from it. Documentation on the options that can be configured with these files lives in [`.pdfalyzer.example`](.pdfalyzer.example) which doubles as an example file you can copy into place and edit to your needs. Even if don\'t configure your own `.pdfalyzer` file you may still glean some insight from reading the descriptions of the various variables in [.pdfalyzer.example](.pdfalyzer.example); there\'s a little more exposition there than in the output of `pdfalyze -h`.\n\n### Colors And Themes\nRun `pdfalyzer_show_color_theme` to see the color theme employed.\n\n### As A Code Library\nAt its core The Pdfalyzer is taking PDF internal objects gathered by [PyPDF2](https://github.com/py-pdf/PyPDF2) and wrapping them in [AnyTree](https://github.com/c0fec0de/anytree)\'s `NodeMixin` class.  Given that things like searching the tree or accessing internal properties will be done through those packages\' code it may be quite helpful to review their documentation.\n\nAs far as The Pdfalyzer\'s unique functionality goes, `Pdfalyzer` is the class at the heart of the operation. It holds both the PDF\'s logical tree as well as a couple of other data structures that have been pre-processed to make them easier to work with. Chief among these is the `FontInfo` class which pulls together various properties of a font strewn across 3 or 4 different PDF objects and the `BinaryScanner1` class which lets you dig through the raw bytes looking for suspicious patterns.\n\nHere\'s a short intro to how to access these objects:\n\n```python\nfrom pdfalyzer.pdfalyzer import Pdfalyzer\n\n# Load a PDF and parse its nodes into the tree.\nwalker = Pdfalyzer("/path/to/the/evil.pdf")\nactual_pdf_tree = walker.pdf_tree\n\n# Find a PDF object by its ID in the PDF\nnode = walker.find_node_by_idnum(44)\npdf_object = node.obj\n\n# Use anytree\'s findall_by_attr to find nodes with a given property\nfrom anytree.search import findall_by_attr\npage_nodes = findall_by_attr(walker.pdf_tree, name=\'type\', value=\'/Page\')\n\n# Get the fonts\nfont1 = walker.font_infos[0]\n\n# Iterate over backtick quoted strings from a font binary and process them\nfor backtick_quoted_string in font1.binary_scanner.extract_backtick_quoted_bytes():\n    process(backtick_quoted_string)\n\n# Try to decode - by force if necessary - everything in the font binary that looks like a quoted string\n# or regex (meaning bytes between single quotes, double quotes, front slashes, backticks, or guillemet quotes)\nfont1.force_decode_all_quoted_bytes()\n```\n\n\n### Troubleshooting\nThis tool is by no means complete. It was built to handle a specific use case which encompassed a small fraction of the many and varied types of information that can show up in a PDF. While it has been tested on a decent number of large and very complicated PDFs (500-5,000 page manuals from Adobe itself) I\'m sure there are a whole bunch of edge cases that will trip up the code.\n\nIf that does happen and you run into an issue using this tool on a particular PDF it will most likely be an issue with relationships between objects within the PDF that are not meant to be parent/child in the tree structure made visible by this tool. There\'s not so many of these kinds of object references in any given file but there\'s a whole galaxy of possibilities and they must each be manually configured to prevent the tool from building an invalid tree.  If you run into that kind of problem take a look at these list constants in the code:\n\n* `NON_TREE_REFERENCES`\n* `INDETERMINATE_REFERENCES`\n\nYou might be able to easily fix your problem by adding the Adobe object\'s reference key to the appropriate list.\n\n\n\n# PDF Resources\n#### Official Adobe Documentation\n* [Official Adobe PDF 1.7 Specification](https://opensource.adobe.com/dc-acrobat-sdk-docs/standards/pdfstandards/pdf/PDF32000_2008.pdf) - Indispensable map when navigating a PDF forest.\n* [Adobe Type 1 Font Format Specification](https://adobe-type-tools.github.io/font-tech-notes/pdfs/T1_SPEC.pdf) - Official spec for Adobe\'s original font description language and file format. Useful if you have suspicions about malicious fonts. Type1 seems to be the attack vector of choice recently which isn\'t so surprising when you consider that it\'s a 30 year old technology and the code that renders these fonts probably hasn\'t been extensively tested in decades because almost no one uses them anymore outside of people who want to use them as attack vectors.\n* [Adobe CMap and CIDFont Files Specification](https://adobe-type-tools.github.io/font-tech-notes/pdfs/5014.CIDFont_Spec.pdf) - Official spec for the character mappings used by Type1 fonts / basically part of the overall Type1 font specification.\n* [Adobe Type 2 Charstring Format](https://adobe-type-tools.github.io/font-tech-notes/pdfs/5177.Type2.pdf) - Describes the newer Type 2 font operators which are also used in some multiple-master Type 1 fonts.\n\n#### Other Stuff\n* [Didier Stevens\'s free book about malicious PDFs](https://blog.didierstevens.com/2010/09/26/free-malicious-pdf-analysis-e-book/) - The master of the malicious PDFs wrote a whole book about how to analyze them. It\'s an old book but the PDF spec was last changed in 2008 so it\'s still relevant.\n* [Analyzing Malicious PDFs Cheat Sheet](https://zeltser.com/media/docs/analyzing-malicious-document-files.pdf) - Like it says on the tin. If that link fails there\'s a copy [here in the repo](doc/analyzing-malicious-document-files.pdf).\n* [T1Utils Github Repo](https://github.com/kohler/t1utils) - Suite of tools for manipulating Type1 fonts.\n* [`t1disasm` Manual](https://www.lcdf.org/type/t1disasm.1.html) - Probably the most useful part of the T1Utils suite because it can decompile encrypted ancient Adobe Type 1 fonts into something human readable.\n\n\n\n# Contributing\nOne easy way of contributing is to run [the script to test against all the PDFs in `~/Documents`](scripts/test_against_all_pdfs_in_Documents_folder.sh) and reporting any issues.\n\nBeyond that see [CONTRIBUTING.md](CONTRIBUTING.md).\n\n# TODO\n* highlight decodes done at `chardet`s behest\n* Highlight decodes with a lot of Javascript keywords\n* deal with repetitive matches\n\n\n\n[^1]: The official Adobe PDF specification calls this tree the PDF\'s "logical structure", which is a good example of nomenclature that does not help those who see it understand anything about what is being described. I can forgive them given that they named this thing back in the 80s, though it\'s a good example of why picking good names for things at the beginning is so important.\n\n[^2]: All internal PDF objects are guaranteed to exist in the tree except in these situations when warnings will be printed:\n  `/ObjStm` (object stream) is a collection of objects in a single stream that will be unrolled into its component objects.\n  `/XRef` Cross-reference stream objects which hold the same references as the `/Trailer` are hacked in as symlinks of the `/Trailer`\n\n[^3]: Given the nature of the PDFs this tool is meant to be scan anything resembling "rendering" the document is pointedly NOT offered.\n\n[^4]: Technically they are `SymlinkNodes`, a really nice feature of [AnyTree](https://github.com/c0fec0de/anytree).\n\n[^5]: At least they weren\'t catching it as of September 2022.\n\n',
     'author': 'Michel de Cryptadamus',
     'author_email': 'michel@cryptadamus.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/michelcrypt4d4mus/pdfalyzer',
```

### Comparing `pdfalyzer-1.8.3/PKG-INFO` & `pdfalyzer-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfalyzer
-Version: 1.8.3
+Version: 1.9.0
 Summary: A PDF analysis toolkit. Scan a PDF with relevant YARA rules, visualize its inner tree-like data structure in living color (lots of colors), force decodes of suspicious font binaries, and more.
 Home-page: https://github.com/michelcrypt4d4mus/pdfalyzer
 License: GPL-3.0-or-later
 Keywords: ascii art,binary,color,font,encoding,malicious pdf,malware,malware analysis,pdf,threat assessment,visualization,yara
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.9,<4.0
@@ -17,15 +17,15 @@
 Classifier: Topic :: Security
 Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: PyPDF2 (>=2.10,<3.0)
 Requires-Dist: anytree (>=2.8,<3.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: rich-argparse (>=0.3.0,<0.4.0)
-Requires-Dist: yaralyzer (>=0.4.0,<0.5.0)
+Requires-Dist: yaralyzer (>=0.5.2,<0.6.0)
 Project-URL: Documentation, https://github.com/michelcrypt4d4mus/pdfalyzer
 Project-URL: Repository, https://github.com/michelcrypt4d4mus/pdfalyzer
 Description-Content-Type: text/markdown
 
 # THE PDFALYZER
 A PDF analysis tool geared towards visualizing the inner tree-like data structure[^1] of a PDF in [spectacularly large and colorful diagrams](#example-output) as well as scanning the various kinds of binary data within the PDF for hidden potentially malicious content.
```

