# Comparing `tmp/stitchtoon-1.0.0.tar.gz` & `tmp/stitchtoon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stitchtoon-1.0.0.tar", last modified: Sun May  7 16:43:52 2023, max compression
+gzip compressed data, was "stitchtoon-1.1.0.tar", last modified: Tue May  9 08:14:35 2023, max compression
```

## Comparing `stitchtoon-1.0.0.tar` & `stitchtoon-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      431 2023-05-07 16:26:35.828468 stitchtoon-1.0.0/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0      111 2023-04-28 22:49:08.769926 stitchtoon-1.0.0/.gitignore
--rwxr-xr-x   0        0        0     1073 2023-04-26 07:52:39.218719 stitchtoon-1.0.0/LICENSE
--rw-r--r--   0        0        0      603 2023-04-26 07:52:39.218719 stitchtoon-1.0.0/Makefile
--rwxr-xr-x   0        0        0      363 2023-04-28 10:36:15.659901 stitchtoon-1.0.0/Pipfile
--rw-r--r--   0        0        0    36902 2023-04-28 10:37:12.713234 stitchtoon-1.0.0/Pipfile.lock
--rwxr-xr-x   0        0        0     3019 2023-05-05 16:29:36.234698 stitchtoon-1.0.0/README.md
--rwxr-xr-x   0        0        0     1178 2023-05-07 16:42:27.643062 stitchtoon-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      596 2023-05-07 16:33:56.675945 stitchtoon-1.0.0/requirements.txt
--rwxr-xr-x   0        0        0      136 2023-05-05 16:29:36.234698 stitchtoon-1.0.0/scripts/formatter.py
--rwxr-xr-x   0        0        0      768 2023-04-26 07:52:39.232059 stitchtoon-1.0.0/setup.cfg
--rwxr-xr-x   0        0        0      117 2023-04-26 07:52:39.278749 stitchtoon-1.0.0/setup.py
--rwxr-xr-x   0        0        0     1673 2023-05-07 16:42:35.893063 stitchtoon-1.0.0/src/stitchtoon/__init__.py
--rwxr-xr-x   0        0        0     5611 2023-05-07 16:38:40.459716 stitchtoon-1.0.0/src/stitchtoon/__main__.py
--rwxr-xr-x   0        0        0      219 2023-04-26 07:52:39.232059 stitchtoon-1.0.0/src/stitchtoon/detectors/__init__.py
--rwxr-xr-x   0        0        0      687 2023-04-28 09:37:29.983305 stitchtoon-1.0.0/src/stitchtoon/detectors/direct_slicing.py
--rwxr-xr-x   0        0        0     2011 2023-04-26 12:43:33.252489 stitchtoon-1.0.0/src/stitchtoon/detectors/pixel_comparison.py
--rwxr-xr-x   0        0        0      523 2023-04-26 21:46:22.055454 stitchtoon-1.0.0/src/stitchtoon/detectors/selector.py
--rwxr-xr-x   0        0        0      372 2023-05-07 16:28:37.948475 stitchtoon-1.0.0/src/stitchtoon/services/__init__.py
--rwxr-xr-x   0        0        0     1588 2023-05-07 16:32:43.506041 stitchtoon-1.0.0/src/stitchtoon/services/global_logger.py
--rwxr-xr-x   0        0        0     1861 2023-05-07 16:41:04.949725 stitchtoon-1.0.0/src/stitchtoon/services/image_directory.py
--rwxr-xr-x   0        0        0     3464 2023-05-07 16:28:37.951808 stitchtoon-1.0.0/src/stitchtoon/services/image_handler.py
--rwxr-xr-x   0        0        0     3563 2023-05-07 16:28:37.948475 stitchtoon-1.0.0/src/stitchtoon/services/image_manipulator.py
--rwxr-xr-x   0        0        0      756 2023-04-26 07:52:39.255404 stitchtoon-1.0.0/src/stitchtoon/services/postprocess_runner.py
--rwxr-xr-x   0        0        0     7440 2023-05-07 16:40:29.003056 stitchtoon-1.0.0/src/stitchtoon/services/process.py
--rw-r--r--   0        0        0     1009 2023-05-07 16:10:22.120819 stitchtoon-1.0.0/src/stitchtoon/services/progressbar.py
--rwxr-xr-x   0        0        0     3037 2023-04-26 08:30:42.875031 stitchtoon-1.0.0/src/stitchtoon/services/scanner.py
--rwxr-xr-x   0        0        0        0 2023-04-28 21:57:52.553321 stitchtoon-1.0.0/src/stitchtoon/utils/__init__.py
--rwxr-xr-x   0        0        0     1109 2023-04-28 23:16:20.733227 stitchtoon-1.0.0/src/stitchtoon/utils/constants.py
--rwxr-xr-x   0        0        0      134 2023-04-28 09:58:00.606614 stitchtoon-1.0.0/src/stitchtoon/utils/errors.py
--rwxr-xr-x   0        0        0      451 2023-04-26 07:52:39.262074 stitchtoon-1.0.0/src/stitchtoon/utils/funcs.py
--rwxr-xr-x   0        0        0      823 2023-04-28 10:55:05.359879 stitchtoon-1.0.0/stitchtoon.spec
--rw-r--r--   0        0        0        0 2023-04-26 07:52:39.272079 stitchtoon-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0   138180 2023-05-07 16:35:32.471442 stitchtoon-1.0.0/tests/test/data/01.jpeg
--rw-r--r--   0        0        0  1726886 2023-05-07 16:35:32.528109 stitchtoon-1.0.0/tests/test/data/01.webp
--rw-r--r--   0        0        0   141943 2023-05-07 16:35:32.488109 stitchtoon-1.0.0/tests/test/data/02.jpeg
--rw-r--r--   0        0        0   123745 2023-05-07 16:35:32.494776 stitchtoon-1.0.0/tests/test/data/03.jpeg
--rw-r--r--   0        0        0   142053 2023-05-07 16:35:32.498109 stitchtoon-1.0.0/tests/test/data/04.jpeg
--rw-r--r--   0        0        0     1117 2023-05-07 16:35:32.494776 stitchtoon-1.0.0/tests/test/test_manipulator.py
--rw-r--r--   0        0        0     1101 2023-05-07 16:35:32.494776 stitchtoon-1.0.0/tests/test/test_scan.py
--rw-r--r--   0        0        0      284 2023-04-28 22:41:33.483269 stitchtoon-1.0.0/tox.ini
--rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 stitchtoon-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      431 2023-05-07 16:26:35.828468 stitchtoon-1.1.0/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0      111 2023-04-28 22:49:08.769926 stitchtoon-1.1.0/.gitignore
+-rwxr-xr-x   0        0        0     1073 2023-04-26 07:52:39.218719 stitchtoon-1.1.0/LICENSE
+-rw-r--r--   0        0        0      603 2023-04-26 07:52:39.218719 stitchtoon-1.1.0/Makefile
+-rwxr-xr-x   0        0        0      351 2023-05-08 09:18:19.986354 stitchtoon-1.1.0/Pipfile
+-rw-r--r--   0        0        0    36902 2023-04-28 10:37:12.713234 stitchtoon-1.1.0/Pipfile.lock
+-rwxr-xr-x   0        0        0     3019 2023-05-05 16:29:36.234698 stitchtoon-1.1.0/README.md
+-rwxr-xr-x   0        0        0      121 2023-05-08 09:15:41.929690 stitchtoon-1.1.0/pre-commit.sh
+-rwxr-xr-x   0        0        0     1178 2023-05-08 11:58:10.777055 stitchtoon-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0      596 2023-05-07 16:33:56.675945 stitchtoon-1.1.0/requirements.txt
+-rwxr-xr-x   0        0        0      768 2023-04-26 07:52:39.232059 stitchtoon-1.1.0/setup.cfg
+-rwxr-xr-x   0        0        0      117 2023-04-26 07:52:39.278749 stitchtoon-1.1.0/setup.py
+-rwxr-xr-x   0        0        0     1815 2023-05-08 11:57:59.100388 stitchtoon-1.1.0/src/stitchtoon/__init__.py
+-rwxr-xr-x   0        0        0     6145 2023-05-08 11:57:16.073719 stitchtoon-1.1.0/src/stitchtoon/__main__.py
+-rwxr-xr-x   0        0        0      219 2023-04-26 07:52:39.232059 stitchtoon-1.1.0/src/stitchtoon/detectors/__init__.py
+-rwxr-xr-x   0        0        0      811 2023-05-08 11:39:48.371086 stitchtoon-1.1.0/src/stitchtoon/detectors/direct_slicing.py
+-rwxr-xr-x   0        0        0     2136 2023-05-08 11:39:34.821086 stitchtoon-1.1.0/src/stitchtoon/detectors/pixel_comparison.py
+-rwxr-xr-x   0        0        0      523 2023-04-26 21:46:22.055454 stitchtoon-1.1.0/src/stitchtoon/detectors/selector.py
+-rwxr-xr-x   0        0        0      438 2023-05-08 09:17:36.506355 stitchtoon-1.1.0/src/stitchtoon/services/__init__.py
+-rwxr-xr-x   0        0        0     1578 2023-05-08 08:58:56.639710 stitchtoon-1.1.0/src/stitchtoon/services/global_logger.py
+-rwxr-xr-x   0        0        0     1826 2023-05-08 09:17:36.503021 stitchtoon-1.1.0/src/stitchtoon/services/image_directory.py
+-rwxr-xr-x   0        0        0     3428 2023-05-08 08:58:56.629710 stitchtoon-1.1.0/src/stitchtoon/services/image_handler.py
+-rwxr-xr-x   0        0        0     4256 2023-05-08 11:57:41.203721 stitchtoon-1.1.0/src/stitchtoon/services/image_manipulator.py
+-rwxr-xr-x   0        0        0      746 2023-05-08 08:58:56.589710 stitchtoon-1.1.0/src/stitchtoon/services/postprocess_runner.py
+-rwxr-xr-x   0        0        0     8269 2023-05-08 11:57:18.173720 stitchtoon-1.1.0/src/stitchtoon/services/process.py
+-rw-r--r--   0        0        0     1009 2023-05-07 16:10:22.120819 stitchtoon-1.1.0/src/stitchtoon/services/progressbar.py
+-rwxr-xr-x   0        0        0     3026 2023-05-08 09:17:36.483021 stitchtoon-1.1.0/src/stitchtoon/services/scanner.py
+-rwxr-xr-x   0        0        0        0 2023-04-28 21:57:52.553321 stitchtoon-1.1.0/src/stitchtoon/utils/__init__.py
+-rwxr-xr-x   0        0        0     1155 2023-05-08 11:40:02.797754 stitchtoon-1.1.0/src/stitchtoon/utils/constants.py
+-rwxr-xr-x   0        0        0      134 2023-04-28 09:58:00.606614 stitchtoon-1.1.0/src/stitchtoon/utils/errors.py
+-rwxr-xr-x   0        0        0      451 2023-04-26 07:52:39.262074 stitchtoon-1.1.0/src/stitchtoon/utils/funcs.py
+-rwxr-xr-x   0        0        0      823 2023-04-28 10:55:05.359879 stitchtoon-1.1.0/stitchtoon.spec
+-rw-r--r--   0        0        0        0 2023-04-26 07:52:39.272079 stitchtoon-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0   138180 2023-05-07 16:35:32.471442 stitchtoon-1.1.0/tests/test/data/01.jpeg
+-rw-r--r--   0        0        0  1726886 2023-05-07 16:35:32.528109 stitchtoon-1.1.0/tests/test/data/01.webp
+-rw-r--r--   0        0        0   141943 2023-05-07 16:35:32.488109 stitchtoon-1.1.0/tests/test/data/02.jpeg
+-rw-r--r--   0        0        0   123745 2023-05-07 16:35:32.494776 stitchtoon-1.1.0/tests/test/data/03.jpeg
+-rw-r--r--   0        0        0   142053 2023-05-07 16:35:32.498109 stitchtoon-1.1.0/tests/test/data/04.jpeg
+-rw-r--r--   0        0        0     1117 2023-05-07 16:35:32.494776 stitchtoon-1.1.0/tests/test/test_manipulator.py
+-rw-r--r--   0        0        0     1101 2023-05-07 16:35:32.494776 stitchtoon-1.1.0/tests/test/test_scan.py
+-rw-r--r--   0        0        0      284 2023-04-28 22:41:33.483269 stitchtoon-1.1.0/tox.ini
+-rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 stitchtoon-1.1.0/PKG-INFO
```

### Comparing `stitchtoon-1.0.0/LICENSE` & `stitchtoon-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/Makefile` & `stitchtoon-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/Pipfile.lock` & `stitchtoon-1.1.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/README.md` & `stitchtoon-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/pyproject.toml` & `stitchtoon-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stitchtoon"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Beshr Alghalil", email="beshrghalil@protonmail.com" },
 ]
 description = "A powerful program for stitching and cutting webtoons/manhwa/manhua raws."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["manga", "webtoon", "stitch", "slice", "combin"]
```

### Comparing `stitchtoon-1.0.0/requirements.txt` & `stitchtoon-1.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/setup.cfg` & `stitchtoon-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/src/stitchtoon/__init__.py` & `stitchtoon-1.1.0/src/stitchtoon/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # This file is part of stitchtoon.
 # License: MIT, see the file "LICENSE" for details.
 """Stitch Toon"""
 
 import os
-import sys
 from sys import version_info
 
 
 # Version helper
 def version_helper():
     if __release__:
         version_string = "stitchtoon {0}".format(__version__)
@@ -28,32 +27,37 @@
         except (OSError, subprocess.CalledProcessError, AttributeError):
             version_string = version_string.format(__version__)
     return version_string
 
 
 # Information
 __license__ = "MIT"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __release__ = False
 __author__ = __maintainer__ = "Beshr Ghalil"
 __email__ = "beshrghalil@porotonmail.com"
 
 # Constants
 stitchtoon = os.path.dirname(__file__)
 DEFAULT_PAGER = "less"
 USAGE = "%prog [options] [path]"
 VERSION = version_helper()
 PY3 = version_info[0] >= 3
 
 args = None
 
-from .services.image_directory import Image, ImageDirectory
-from .services.process import process, stitch
+from .services.image_directory import Image
+from .services.image_directory import ImageDirectory
+from .services.process import process
+from .services.process import stitch
 from .services.progressbar import ProgressHandler
-from .services.scanner import is_supported_img, scan, scanimgdir, walkimgdir
+from .services.scanner import is_supported_img
+from .services.scanner import scan
+from .services.scanner import scanimgdir
+from .services.scanner import walkimgdir
 
 __all__ = [
     Image,
     ImageDirectory,
     scan,
     scanimgdir,
     walkimgdir,
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/__main__.py` & `stitchtoon-1.1.0/src/stitchtoon/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
-import math
 import sys
 
 from stitchtoon import __version__
-from stitchtoon.services.global_logger import DEFAULT_LOG_LEVEL, Logger, get_logger
+from stitchtoon.services.global_logger import DEFAULT_LOG_LEVEL
+from stitchtoon.services.global_logger import get_logger
 from stitchtoon.services.process import process
 
 
 def positive_int(value):
     if not value.isdigit() or int(value) <= 0:
         raise argparse.ArgumentTypeError("Not a valid integer value")
     return int(value)
@@ -22,23 +22,26 @@
 
 
 def size_format(value):
     value = value.replace("x", "X")
     size = value.split("X")
     if len(size) > 2:
         raise argparse.ArgumentTypeError(
-            "invalid size format. Supported formats `<height>X<width>` or `<height>`. ex: `5000X760`"
+            "invalid size format. Supported formats `<height>X<width>` or `<height>` or `x<width>`. ex: `5000X760`"
         )
 
-    if len(size) == 1:
+    elif len(size) == 1:
         size.append("0")
+    elif len(size) == 0:
+        return (-1, -1)
+
     for idx, s in enumerate(size):
         if not s.isdigit():
             raise argparse.ArgumentTypeError(
-                "invalid size format. Supported formats `<height>X<width>` or `<height>`. ex: `5000X760`"
+                "invalid size format. Supported formats `<height>X<width>` or `<height>` or `x<width>`. ex: `5000X760`"
             )
         else:
             size[idx] = int(s)
     return size
 
 
 def get_args():
@@ -63,15 +66,25 @@
         help="Saves at specified output path",
     )
     parser.add_argument(
         "-s",
         "--size",
         dest="size",
         type=size_format,
-        required=True,
+        required="-n" not in sys.argv and "--images-number" not in sys.argv,
+        help="Sets the value of the Rough Panel Height And Width, hXw",
+        default=(-1, -1),
+    )
+    parser.add_argument(
+        "-n",
+        "--images-number",
+        dest="images_number",
+        type=positive_int,
+        default=0,
+        required="-s" not in sys.argv and "--size" not in sys.argv,
         help="Sets the value of the Rough Panel Height And Width, hXw",
     )
     parser.add_argument(
         "-t",
         "--type",
         dest="output_format",
         type=str,
@@ -92,15 +105,15 @@
     advanced = parser.add_argument_group("Advanced")
     advanced.add_argument(
         "-w",
         "--width-enforcement",
         dest="width_enforcement",
         type=str,
         default="none",
-        choices=("none", "auto"),
+        choices=("none", "auto", "copywrite"),
         help="Width Enforcement Technique, Default=None)",
     )
     advanced.add_argument(
         "-d",
         "--detection-type",
         type=str,
         dest="detection_type",
@@ -182,14 +195,15 @@
     }
 
     try:
         process(
             input=kwargs.input,
             output=kwargs.output,
             split_height=kwargs.size[0],
+            images_number=kwargs.images_number,
             output_format=kwargs.output_format,
             recursive=kwargs.recursive,
             as_archive=kwargs.as_archive,
             lossy_quality=kwargs.lossy_quality,
             show_progress=kwargs.show_progress,
             params=stitch_params,
         )
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/detectors/direct_slicing.py` & `stitchtoon-1.1.0/src/stitchtoon/detectors/direct_slicing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from PIL import Image as pilImage
-
 from ..services.global_logger import logFunc
 from ..services.image_directory import Image
+from ..utils.constants import SMALLER_ALLOWD_HEIGHT
 
 
 class DirectSlicingDetector:
     @logFunc(inclass=True)
     def run(self, combined_img: Image, split_height: int, **kwargs) -> list[int]:
+        if split_height < SMALLER_ALLOWD_HEIGHT:
+            raise Exception("Height very small to slice")
         # Changes from a pil image to an numpy pixel array
         last_row = combined_img.height
         # Initializes some variables
         slice_locations = [0]
         row = split_height
         while row < last_row:
             slice_locations.append(row)
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/detectors/pixel_comparison.py` & `stitchtoon-1.1.0/src/stitchtoon/detectors/pixel_comparison.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import numpy as np
-from PIL import Image as pilImage
 
 from ..services.global_logger import logFunc
 from ..services.image_directory import Image
+from ..utils.constants import SMALLER_ALLOWD_HEIGHT
 
 
 class PixelComparisonDetector:
     @logFunc(inclass=True)
     def run(self, combined_img: Image, split_height: int, **kwargs) -> list[int]:
         """Uses Neighbouring pixels comparison to detect ideal slice locations"""
+        if split_height < SMALLER_ALLOWD_HEIGHT:
+            raise Exception("Height very small to slice")
         # Changes from a pil Image to an numpy pixel array
         combined_img = np.array(combined_img.pil.convert("L"))
         # Setting up rest of Detector Parameters
         scan_step = kwargs.get("scan_step", 5)
         ignorable_pixels = kwargs.get("ignorable_pixels", 0)
         sensitivity = kwargs.get("sensitivity", 90)
         threshold = int(255 * (1 - (sensitivity / 100)))
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/detectors/selector.py` & `stitchtoon-1.1.0/src/stitchtoon/detectors/selector.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/src/stitchtoon/services/global_logger.py` & `stitchtoon-1.1.0/src/stitchtoon/services/global_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import functools
 import logging
-import os
 import sys
 from datetime import datetime
 
 DEFAULT_LOG_LEVEL = logging.ERROR
 
 
 def get_logger(log_level=logging.ERROR, filename=sys.stdout):
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/services/image_directory.py` & `stitchtoon-1.1.0/src/stitchtoon/services/image_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from __future__ import annotations
 
 import os
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from dataclasses import field
 
 from PIL import Image as pilImage
 from psd_tools import PSDImage
 
-from ..utils.constants import (
-    FORMAT_NAME_MAPPER,
-    PHOTOSHOP_FILE_TYPES,
-    SUPPORTED_IMG_TYPES,
-)
+from ..utils.constants import PHOTOSHOP_FILE_TYPES
 from ..utils.errors import ImageNotOpenedError
 
 
 @dataclass
 class Image:
     path: os.PathLike
     name: str
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/services/image_handler.py` & `stitchtoon-1.1.0/src/stitchtoon/services/image_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import io
 import os
 import os.path as osp
 import zipfile
-from datetime import datetime as dt
 
 from PIL import Image as pilImage
 from psd_tools import PSDImage
 
 from ..utils.constants import PHOTOSHOP_FILE_TYPES
 from .global_logger import logFunc
 from .image_directory import Image
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/services/image_manipulator.py` & `stitchtoon-1.1.0/src/stitchtoon/services/image_manipulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 from PIL import Image as pilImage
 
 from ..utils.constants import WIDTH_ENFORCEMENT
+from ..utils.errors import SizeLimitError
 from .global_logger import logFunc
 from .image_directory import Image
 from .progressbar import ProgressHandler
 
 
 class ImageManipulator:
+    @logFunc
+    @staticmethod
+    def _resize_img(img: Image, new_img_width) -> Image:
+        if img.width == new_img_width:
+            return img
+        img_ratio = float(img.height / img.width)
+        new_img_height = int(img_ratio * new_img_width)
+        if new_img_height > 0:
+            img.pil = img.pil.resize(
+                (new_img_width, new_img_height), pilImage.Resampling.LANCZOS
+            )
+        return img
+
     @logFunc(inclass=True)
     @staticmethod
     def resize(
         img_objs: list[Image],
         enforce_setting: WIDTH_ENFORCEMENT,
         custom_width: int = 720,
     ) -> list[Image]:
@@ -25,28 +39,30 @@
             list[Image]
         """
 
         if enforce_setting == WIDTH_ENFORCEMENT.NONE.value and not custom_width:
             return img_objs
 
         new_img_width = 0
-        if enforce_setting == WIDTH_ENFORCEMENT.AUTO.value:
+        if enforce_setting == WIDTH_ENFORCEMENT.COPYWRITE.value:
+            if len(img_objs) >= 2:
+                new_img_width = img_objs[1].width
+                ImageManipulator._resize_img(img_objs[0], new_img_width)
+            return img_objs
+
+        elif enforce_setting == WIDTH_ENFORCEMENT.AUTO.value:
             widths, heights = zip(*(img.size for img in img_objs))
             new_img_width = min(widths)
+
         elif enforce_setting == WIDTH_ENFORCEMENT.FIXED.value or custom_width:
             new_img_width = custom_width
+
         for img in img_objs:
-            if img.width == new_img_width:
-                continue
-            img_ratio = float(img.height / img.width)
-            new_img_height = int(img_ratio * new_img_width)
-            if new_img_height > 0:
-                img.pil = img.pil.resize(
-                    (new_img_width, new_img_height), pilImage.Resampling.LANCZOS
-                )
+            ImageManipulator._resize_img(img, new_img_width)
+
         return img_objs
 
     @logFunc(inclass=True)
     @staticmethod
     def combine(
         img_objs: list[Image], progress: ProgressHandler = None, increament: int = 0
     ) -> Image:
@@ -71,16 +87,19 @@
         images_len = len(img_objs)
         for idx, img in enumerate(img_objs, 1):
             combined_img.paste(img.pil, (0, combine_offset))
             combine_offset += img.height
             img.pil.close()
             progress.update(progress.value + increament, f"Combined {idx}/{images_len}")
 
-        img = img_objs[0].copy()
+        img = Image(
+            path=img_objs[0].path, format=img_objs[0].format, name=img_objs[0].name
+        )
         img.pil = combined_img
+        progress.update(progress.value, "All combined")
         return img
 
     @logFunc(inclass=True)
     @staticmethod
     def slice(combined_img: Image, slice_locations: list[int]) -> list[Image]:
         """Combines given combined img to into multiple img slices given the slice locations.
 
@@ -94,13 +113,16 @@
 
         max_width = combined_img.width
         img_objs = []
         for index in range(1, len(slice_locations)):
             upper_limit = slice_locations[index - 1]
             lower_limit = slice_locations[index]
             slice_boundaries = (0, upper_limit, max_width, lower_limit)
-            img_slice = combined_img.pil.crop(slice_boundaries)
+            try:
+                img_slice = combined_img.pil.crop(slice_boundaries)
+            except ValueError:
+                raise SizeLimitError("Images to small to slice")
             img = combined_img.copy()
             img.pil = img_slice
             img_objs.append(img)
         combined_img.pil.close()
         return img_objs
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/services/postprocess_runner.py` & `stitchtoon-1.1.0/src/stitchtoon/services/postprocess_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import subprocess
 
 from ..services.global_logger import logFunc
 
 
 @logFunc
 def postprocess_run(cmd: str, cmd_args: str = (), console=print):
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/services/process.py` & `stitchtoon-1.1.0/src/stitchtoon/services/process.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import gc
 import os.path as osp
 from os import PathLike
 
 from stitchtoon.detectors import select_detector
-from stitchtoon.services import ImageHandler, ImageManipulator, logFunc, scan
+from stitchtoon.services import ImageHandler
+from stitchtoon.services import ImageManipulator
+from stitchtoon.services import logFunc
+from stitchtoon.services import scan
 from stitchtoon.services.image_directory import Image
-from stitchtoon.services.progressbar import DefaultCliProgress, ProgressHandler
-from stitchtoon.utils.constants import (
-    FORMAT_NAME_MAPPER,
-    FORMAT_SIZE_MAPPER,
-    SIZE_LIMITS,
-    WIDTH_ENFORCEMENT,
-    ProcessDefaults,
-    StitchDefaults,
-)
-from stitchtoon.utils.errors import EmptyImageDir, SizeLimitError
+from stitchtoon.services.progressbar import DefaultCliProgress
+from stitchtoon.services.progressbar import ProgressHandler
+from stitchtoon.utils.constants import DETECTION_TYPE
+from stitchtoon.utils.constants import FORMAT_NAME_MAPPER
+from stitchtoon.utils.constants import FORMAT_SIZE_MAPPER
+from stitchtoon.utils.constants import SIZE_LIMITS
+from stitchtoon.utils.constants import ProcessDefaults
+from stitchtoon.utils.constants import StitchDefaults
+from stitchtoon.utils.errors import EmptyImageDir
+from stitchtoon.utils.errors import SizeLimitError
 
 # Must have a sum of 100
 PROGRESS_PERCENTAGE = {
     "scan": 10,
     "stitch": 70,
     "loading": 10,
     "save": 10,
 }
 
 
 @logFunc()
 def process(
     input: PathLike,
     output: PathLike,
-    split_height: int,
     *,
+    split_height: int = 0,
+    images_number: int = 0,
     output_format: str = ProcessDefaults.OUTPUT_FORMAT,
     recursive: bool = ProcessDefaults.RECURSIVE,
     as_archive: bool = ProcessDefaults.AS_ARCHIVE,
     lossy_quality: int = ProcessDefaults.LOSSY_QUALITY,
     show_progress: bool = ProcessDefaults.SHOW_PROGRESS,
     progress: ProgressHandler = None,
     params: dict[str, any],
@@ -57,14 +61,19 @@
         FileNotFoundError: When input directory could not be found
         EmptyImageDir: When input directory does not contain supported images
         Exception: When output is not provided
     """
     handler = ImageHandler()
     progress = progress or _get_progressbar(show_progress)
 
+    if not split_height and not images_number:
+        raise Exception(
+            "split_height and images_number are not provided, Must provide one of theme"
+        )
+
     format = _get_format_for_size(
         output_format, max(split_height, params.get("custom_width", 0))
     )
 
     if not osp.lexists(input):
         raise FileNotFoundError(f"Could not found {input}")
     if not output:
@@ -83,14 +92,21 @@
         images = handler.load(
             image_dir.images,
             progress=progress,
             increament=per_dir_percentage / images_len,
         )
         if not images:
             continue
+
+        total_images_length = sum(image.height for image in images)
+        if images_number:
+            split_height = total_images_length / images_number
+            format = _get_format_for_size(format, split_height)
+            params["detection_type"] = DETECTION_TYPE.NO_DETECTION.value
+
         per_dir_percentage = PROGRESS_PERCENTAGE["stitch"] / working_dirs_len
         images = stitch(
             images,
             split_height,
             progress=progress,
             increament=per_dir_percentage / images_len,
             **params,
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/services/progressbar.py` & `stitchtoon-1.1.0/src/stitchtoon/services/progressbar.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/src/stitchtoon/services/scanner.py` & `stitchtoon-1.1.0/src/stitchtoon/services/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import os
 import os.path as osp
-from typing import Callable, Iterable, Union
+from typing import Iterable
 
 from natsort import natsorted
 
-from ..utils.constants import PHOTOSHOP_FILE_TYPES, SUPPORTED_IMG_TYPES
+from ..utils.constants import SUPPORTED_IMG_TYPES
 from .global_logger import logFunc
-from .image_directory import Image, ImageDirectory
+from .image_directory import Image
+from .image_directory import ImageDirectory
 
 
 @logFunc()
 def is_supported_img(*, format: str = None, filename: os.PathLike = None) -> bool:
     """Checks if an image format is supported
 
     Args:
```

### Comparing `stitchtoon-1.0.0/src/stitchtoon/utils/constants.py` & `stitchtoon-1.1.0/src/stitchtoon/utils/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from enum import Enum, IntEnum
+from enum import Enum
 
 # Static Variables
 LOG_REL_DIR = "__logs__"
 SETTINGS_REL_DIR = "__settings__"
 OUTPUT_SUFFIX = "[stitched]"
+SMALLER_ALLOWD_HEIGHT = 10
 SUPPORTED_IMG_TYPES = (
     "png",
     "webp",
     "jpeg",
     "jpg",
     "psd",
     "psb",
@@ -34,14 +35,15 @@
 
 
 # Static Enums
 class WIDTH_ENFORCEMENT(Enum):
     NONE = "none"
     AUTO = "auto"
     FIXED = "fixed"
+    COPYWRITE = "copywrite"
 
 
 class DETECTION_TYPE(Enum):
     NO_DETECTION = "none"
     PIXEL_COMPARISON = "pixel"
```

### Comparing `stitchtoon-1.0.0/stitchtoon.spec` & `stitchtoon-1.1.0/stitchtoon.spec`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/tests/test/data/01.jpeg` & `stitchtoon-1.1.0/tests/test/data/01.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/tests/test/data/01.webp` & `stitchtoon-1.1.0/tests/test/data/01.webp`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/tests/test/data/02.jpeg` & `stitchtoon-1.1.0/tests/test/data/02.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/tests/test/data/03.jpeg` & `stitchtoon-1.1.0/tests/test/data/03.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/tests/test/data/04.jpeg` & `stitchtoon-1.1.0/tests/test/data/04.jpeg`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/tests/test/test_manipulator.py` & `stitchtoon-1.1.0/tests/test/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/tests/test/test_scan.py` & `stitchtoon-1.1.0/tests/test/test_scan.py`

 * *Files identical despite different names*

### Comparing `stitchtoon-1.0.0/PKG-INFO` & `stitchtoon-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stitchtoon
-Version: 1.0.0
+Version: 1.1.0
 Summary: A powerful program for stitching and cutting webtoons/manhwa/manhua raws.
 Keywords: manga,webtoon,stitch,slice,combin
 Author-email: Beshr Alghalil <beshrghalil@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stitchtoon Version: 1.0.0 Summary: A powerful
+Metadata-Version: 2.1 Name: stitchtoon Version: 1.1.0 Summary: A powerful
 program for stitching and cutting webtoons/manhwa/manhua raws. Keywords:
 manga,webtoon,stitch,slice,combin Author-email: Beshr Alghalil
 protonmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Dist: psd_tools Requires-Dist: natsort Requires-Dist: pillow Requires-
 Dist: progress Requires-Dist: black ; extra == "dev" Requires-Dist: flake8 ;
```

