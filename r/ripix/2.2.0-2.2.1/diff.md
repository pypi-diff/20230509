# Comparing `tmp/ripix-2.2.0.tar.gz` & `tmp/ripix-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripix-2.2.0.tar", max compression
+gzip compressed data, was "ripix-2.2.1.tar", max compression
```

## Comparing `ripix-2.2.0.tar` & `ripix-2.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      692 2023-05-09 19:29:45.958722 ripix-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1958 2023-05-09 19:29:45.957722 ripix-2.2.0/README.md
--rw-r--r--   0        0        0       66 2023-05-09 19:29:45.959722 ripix-2.2.0/ripix/__init__.py
--rw-r--r--   0        0        0      670 2023-05-09 19:29:45.959722 ripix-2.2.0/ripix/functions.py
--rw-r--r--   0        0        0      735 2023-05-09 19:29:45.959722 ripix-2.2.0/ripix/functions.pyi
--rw-r--r--   0        0        0     8710 2023-05-09 19:29:45.959722 ripix-2.2.0/ripix/pixel.py
--rw-r--r--   0        0        0        0 2023-05-09 19:29:45.959722 ripix-2.2.0/ripix/py.typed
--rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 ripix-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      822 2023-05-09 20:50:18.338843 ripix-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1958 2023-05-09 19:29:45.957722 ripix-2.2.1/README.md
+-rw-r--r--   0        0        0       66 2023-05-09 19:29:45.959722 ripix-2.2.1/ripix/__init__.py
+-rw-r--r--   0        0        0      682 2023-05-09 19:52:26.098621 ripix-2.2.1/ripix/functions.py
+-rw-r--r--   0        0        0      735 2023-05-09 19:29:45.959722 ripix-2.2.1/ripix/functions.pyi
+-rw-r--r--   0        0        0     8832 2023-05-09 20:51:06.347844 ripix-2.2.1/ripix/pixel.py
+-rw-r--r--   0        0        0        0 2023-05-09 19:29:45.959722 ripix-2.2.1/ripix/py.typed
+-rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 ripix-2.2.1/PKG-INFO
```

### Comparing `ripix-2.2.0/pyproject.toml` & `ripix-2.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "ripix"
-version = "2.2.0"
+version = "2.2.1"
 description = "A Rich-compatible library for writing pixel images and ASCII art to the terminal."
 authors = ["Darren Burns <darrenb900@gmail.com>", "Romanin <semina054@gmail.com>"]
+repository = "https://github.com/romanin-rf/ripix"
+keywords = ["ripix", "rich", "textual", "image", "ascii-art", "rich_pixels"]
 readme = "README.md"
 packages = [{ include = "ripix" }]
 include = ["ripix/py.typed", "ripix/functions.pyi"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 rich = ">=12.0.0"
```

### Comparing `ripix-2.2.0/README.md` & `ripix-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ripix-2.2.0/ripix/functions.py` & `ripix-2.2.1/ripix/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 from functools import partial
 
 async def aiter(it):
     for item in it:
         yield item
-        asyncio.sleep(0)
+        await asyncio.sleep(0)
 
 async def arange(*args, **kwargs) -> int:
     for i in range(*args, **kwargs):
         yield i
-        asyncio.sleep(0)
+        await asyncio.sleep(0)
 
 async def run_in_executor(loop, executor, func, *args, **kwargs):
     if loop is None: loop = asyncio.get_running_loop()
     return await loop.run_in_executor(executor, partial(func, *args, **kwargs))
 
 def wrapper_run_in_executor(loop, executor, func):
     async def wrapped_func(*args, **kwargs):
```

### Comparing `ripix-2.2.0/ripix/functions.pyi` & `ripix-2.2.1/ripix/functions.pyi`

 * *Files identical despite different names*

### Comparing `ripix-2.2.0/ripix/pixel.py` & `ripix-2.2.1/ripix/pixel.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from PIL.Image import Resampling
 from rich.console import Console, ConsoleOptions, RenderResult
 from rich.segment import Segment, Segments
 from rich.style import Style
 # > Local Imports
 from .functions import arange, aiter, wrapper_run_in_executor, run_in_executor
 
-
 # ! Just Pixels
 class Pixels:
     def __init__(self) -> None:
         self._segments: Optional[Segments] = None
 
     @staticmethod
     def from_image(
@@ -62,21 +61,20 @@
         for y in range(height):
             this_row: List[Segment] = []
             row_append = this_row.append
 
             for x in range(width):
                 r, g, b, a = get_pixel((x, y))
                 style = parse_style(f"on rgb({r},{g},{b})") if a > 0 else null_style
-                row_append(Segment("  ", style))
+                row_append(Segment(" ", style))
 
             row_append(Segment("\n", null_style))
 
             # TODO: Double-check if this is required - I've forgotten...
-            if not all(t[1] == "" for t in this_row[:-1]):
-                segments += this_row
+            segments += this_row
 
         return segments
 
     @staticmethod
     def from_segments(
         segments: Iterable[Segment],
     ) -> Pixels:
@@ -124,49 +122,56 @@
     def __init__(self) -> None:
         self._segments: Optional[Segments] = None
 
     @staticmethod
     async def from_image(
         image: Image,
         resize: Optional[Tuple[int, int]] = None,
+        resample: Optional[Resampling] = None,
         loop: Optional[AbstractEventLoop] = None
     ) -> AsyncPixels:
         if loop is None: loop = get_running_loop()
+        resample = resample or Resampling.NEAREST
         
-        segments = await AsyncPixels._segments_from_image(image, resize, loop)
+        segments = await AsyncPixels._segments_from_image(image, resize, resample, loop)
         return AsyncPixels.from_segments(segments)
 
     @staticmethod
     async def from_image_path(
         path: Union[PurePath, str],
         resize: Optional[Tuple[int, int]] = None,
+        resample: Optional[Resampling] = None,
         loop: Optional[AbstractEventLoop] = None
     ) -> AsyncPixels:
         """Create a Pixels object from an image. Requires 'image' extra dependencies.
 
         Args:
             path: The path to the image file.
             resize: A tuple of (width, height) to resize the image to.
         """
+        resample = resample or Resampling.NEAREST
+        
         if loop is None: loop = get_running_loop()
         pilopen = wrapper_run_in_executor(loop, None, PILImageModule.open)
         
         with await pilopen(Path(path)) as image:
-            segments = await AsyncPixels._segments_from_image(image, resize, loop)
+            segments = await AsyncPixels._segments_from_image(image, resize, resample, loop)
 
         return await AsyncPixels.from_segments(segments)
     
     @staticmethod
     async def _segments_from_image(
         image: Image,
         resize: Optional[Tuple[int, int]] = None,
+        resize_resample: Optional[Resampling] = None,
         loop: Optional[AbstractEventLoop] = None
     ) -> List[Segment]:
+        resample = resize_resample or Resampling.NEAREST
         if loop is None: loop = get_running_loop()
-        if resize is not None: image = await run_in_executor(loop, None, image.resize, resize, resample=Resampling.NEAREST)
+        if resize is not None: image = await run_in_executor(loop, None, image.resize, resize, resample=resample)
 
         width, height = image.width, image.height
         rgba_image = await run_in_executor(loop, None, image.convert, "RGBA") if image.mode != "RGBA" else image
         get_pixel = wrapper_run_in_executor(loop, None, rgba_image.getpixel)
         parse_style = wrapper_run_in_executor(loop, None, Style.parse)
         null_style = Style.null()
         segments = []
@@ -174,21 +179,18 @@
         async for y in arange(height):
             this_row: List[Segment] = []
             row_append = this_row.append
 
             async for x in arange(width):
                 r, g, b, a = await get_pixel((x, y))
                 style = await parse_style(f"on rgb({r},{g},{b})") if (a > 0) else null_style
-                row_append(Segment("  ", style))
-
+                row_append(Segment(" ", style))
             row_append(Segment("\n", null_style))
-
-            # TODO: Double-check if this is required - I've forgotten...
-            if not all(t[1] == "" async for t in aiter(this_row[:-1])):
-                segments += this_row
+            
+            segments += this_row
 
         return segments
 
     @staticmethod
     async def from_segments(
         segments: Iterable[Segment],
     ) -> AsyncPixels:
```

### Comparing `ripix-2.2.0/PKG-INFO` & `ripix-2.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: ripix
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Rich-compatible library for writing pixel images and ASCII art to the terminal.
+Home-page: https://github.com/romanin-rf/ripix
+Keywords: ripix,rich,textual,image,ascii-art,rich_pixels
 Author: Darren Burns
 Author-email: darrenb900@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: pillow (>=9.0.0,<10.0.0)
 Requires-Dist: rich (>=12.0.0)
+Project-URL: Repository, https://github.com/romanin-rf/ripix
 Description-Content-Type: text/markdown
 
 # Ripix
 
 A Rich-compatible library for writing pixel images and other colourful grids to the
 terminal.
```

