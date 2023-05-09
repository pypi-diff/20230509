# Comparing `tmp/whatsappy-py-3.3.5.tar.gz` & `tmp/whatsappy-py-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsappy-py-3.3.5.tar", last modified: Sun Feb 13 20:15:59 2022, max compression
+gzip compressed data, was "whatsappy-py-4.0.0.tar", last modified: Tue May  9 19:27:41 2023, max compression
```

## Comparing `whatsappy-py-3.3.5.tar` & `whatsappy-py-4.0.0.tar`

### file list

```diff
@@ -1,22 +1,3018 @@
-drwxrwxrwx   0        0        0        0 2022-02-13 20:15:59.800722 whatsappy-py-3.3.5/
--rw-rw-rw-   0        0        0     1087 2021-07-22 12:44:34.000000 whatsappy-py-3.3.5/LICENSE
--rw-rw-rw-   0        0        0       62 2021-07-22 12:44:34.000000 whatsappy-py-3.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0    10598 2022-02-13 20:15:59.797721 whatsappy-py-3.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    10036 2022-01-28 20:02:11.000000 whatsappy-py-3.3.5/README.md
--rw-rw-rw-   0        0        0      109 2022-02-13 20:00:43.000000 whatsappy-py-3.3.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-02-13 20:15:59.800722 whatsappy-py-3.3.5/setup.cfg
--rw-rw-rw-   0        0        0      959 2022-02-13 20:15:22.000000 whatsappy-py-3.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-13 20:15:59.712773 whatsappy-py-3.3.5/tests/
--rw-rw-rw-   0        0        0      248 2022-02-13 20:03:19.000000 whatsappy-py-3.3.5/tests/teste.py
-drwxrwxrwx   0        0        0        0 2022-02-13 20:15:59.732762 whatsappy-py-3.3.5/whatsappy/
--rw-rw-rw-   0        0        0       26 2022-02-09 16:26:44.000000 whatsappy-py-3.3.5/whatsappy/__init__.py
--rw-rw-rw-   0        0        0      415 2022-01-26 14:41:42.000000 whatsappy-py-3.3.5/whatsappy/error.py
--rw-rw-rw-   0        0        0    31863 2022-02-13 20:12:25.000000 whatsappy-py-3.3.5/whatsappy/main.py
--rw-rw-rw-   0        0        0    11914 2022-02-13 20:00:45.000000 whatsappy-py-3.3.5/whatsappy/message.py
--rw-rw-rw-   0        0        0     1612 2022-02-13 20:00:36.000000 whatsappy-py-3.3.5/whatsappy/tool.py
-drwxrwxrwx   0        0        0        0 2022-02-13 20:15:59.793723 whatsappy-py-3.3.5/whatsappy_py.egg-info/
--rw-rw-rw-   0        0        0    10598 2022-02-13 20:15:57.000000 whatsappy-py-3.3.5/whatsappy_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2022-02-13 20:15:58.000000 whatsappy-py-3.3.5/whatsappy_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-13 20:15:57.000000 whatsappy-py-3.3.5/whatsappy_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2022-02-13 20:15:57.000000 whatsappy-py-3.3.5/whatsappy_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-02-13 20:15:57.000000 whatsappy-py-3.3.5/whatsappy_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.974738 whatsappy-py-4.0.0/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.844929 whatsappy-py-4.0.0/.venv/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.713516 whatsappy-py-4.0.0/.venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.861481 whatsappy-py-4.0.0/.venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.978631 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/
+-rw-rw-rw-   0        0        0     3359 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/BdfFontFile.py
+-rw-rw-rw-   0        0        0    16483 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/BlpImagePlugin.py
+-rw-rw-rw-   0        0        0    18138 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/BmpImagePlugin.py
+-rw-rw-rw-   0        0        0     1629 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/BufrStubImagePlugin.py
+-rw-rw-rw-   0        0        0     3003 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ContainerIO.py
+-rw-rw-rw-   0        0        0     1796 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/CurImagePlugin.py
+-rw-rw-rw-   0        0        0     2037 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/DcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9637 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/DdsImagePlugin.py
+-rw-rw-rw-   0        0        0    15413 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/EpsImagePlugin.py
+-rw-rw-rw-   0        0        0    10098 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ExifTags.py
+-rw-rw-rw-   0        0        0     2132 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/FitsImagePlugin.py
+-rw-rw-rw-   0        0        0     1749 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/FitsStubImagePlugin.py
+-rw-rw-rw-   0        0        0     4614 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/FliImagePlugin.py
+-rw-rw-rw-   0        0        0     2874 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/FontFile.py
+-rw-rw-rw-   0        0        0     7214 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/FpxImagePlugin.py
+-rw-rw-rw-   0        0        0     3980 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/FtexImagePlugin.py
+-rw-rw-rw-   0        0        0     3010 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/GbrImagePlugin.py
+-rw-rw-rw-   0        0        0     2704 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/GdImageFile.py
+-rw-rw-rw-   0        0        0    36797 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/GifImagePlugin.py
+-rw-rw-rw-   0        0        0     3533 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/GimpGradientFile.py
+-rw-rw-rw-   0        0        0     1401 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/GimpPaletteFile.py
+-rw-rw-rw-   0        0        0     1623 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/GribStubImagePlugin.py
+-rw-rw-rw-   0        0        0     1626 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
+-rw-rw-rw-   0        0        0    12329 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/IcnsImagePlugin.py
+-rw-rw-rw-   0        0        0    11980 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/IcoImagePlugin.py
+-rw-rw-rw-   0        0        0    11238 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImImagePlugin.py
+-rw-rw-rw-   0        0        0   137510 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/Image.py
+-rw-rw-rw-   0        0        0     7306 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageChops.py
+-rw-rw-rw-   0        0        0    38772 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageCms.py
+-rw-rw-rw-   0        0        0     9097 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageColor.py
+-rw-rw-rw-   0        0        0    39813 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageDraw.py
+-rw-rw-rw-   0        0        0     6210 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageDraw2.py
+-rw-rw-rw-   0        0        0     3293 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageEnhance.py
+-rw-rw-rw-   0        0        0    24312 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageFile.py
+-rw-rw-rw-   0        0        0    17019 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageFilter.py
+-rw-rw-rw-   0        0        0    51659 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageFont.py
+-rw-rw-rw-   0        0        0     4834 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageGrab.py
+-rw-rw-rw-   0        0        0     7620 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageMath.py
+-rw-rw-rw-   0        0        0     3004 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageMode.py
+-rw-rw-rw-   0        0        0     8231 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageMorph.py
+-rw-rw-rw-   0        0        0    21590 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageOps.py
+-rw-rw-rw-   0        0        0     8421 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImagePalette.py
+-rw-rw-rw-   0        0        0      355 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImagePath.py
+-rw-rw-rw-   0        0        0     7119 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageQt.py
+-rw-rw-rw-   0        0        0     1948 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageSequence.py
+-rw-rw-rw-   0        0        0    11813 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageShow.py
+-rw-rw-rw-   0        0        0     4072 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageStat.py
+-rw-rw-rw-   0        0        0     8988 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageTk.py
+-rw-rw-rw-   0        0        0     2985 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageTransform.py
+-rw-rw-rw-   0        0        0     7421 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImageWin.py
+-rw-rw-rw-   0        0        0     2680 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/ImtImagePlugin.py
+-rw-rw-rw-   0        0        0     6007 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/IptcImagePlugin.py
+-rw-rw-rw-   0        0        0    11982 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
+-rw-rw-rw-   0        0        0    30012 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/JpegImagePlugin.py
+-rw-rw-rw-   0        0        0    12583 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/JpegPresets.py
+-rw-rw-rw-   0        0        0     1871 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/McIdasImagePlugin.py
+-rw-rw-rw-   0        0        0     2699 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/MicImagePlugin.py
+-rw-rw-rw-   0        0        0     1905 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/MpegImagePlugin.py
+-rw-rw-rw-   0        0        0     6486 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/MpoImagePlugin.py
+-rw-rw-rw-   0        0        0     5806 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/MspImagePlugin.py
+-rw-rw-rw-   0        0        0     6754 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PSDraw.py
+-rw-rw-rw-   0        0        0     1179 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PaletteFile.py
+-rw-rw-rw-   0        0        0     9369 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PalmImagePlugin.py
+-rw-rw-rw-   0        0        0     1558 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PcdImagePlugin.py
+-rw-rw-rw-   0        0        0     7013 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PcfFontFile.py
+-rw-rw-rw-   0        0        0     6242 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9264 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PdfImagePlugin.py
+-rw-rw-rw-   0        0        0    35563 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PdfParser.py
+-rw-rw-rw-   0        0        0     1720 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PixarImagePlugin.py
+-rw-rw-rw-   0        0        0    48199 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PngImagePlugin.py
+-rw-rw-rw-   0        0        0    11746 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PpmImagePlugin.py
+-rw-rw-rw-   0        0        0     7838 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PsdImagePlugin.py
+-rw-rw-rw-   0        0        0    10189 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/PyAccess.py
+-rw-rw-rw-   0        0        0     3722 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/QoiImagePlugin.py
+-rw-rw-rw-   0        0        0     6409 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/SgiImagePlugin.py
+-rw-rw-rw-   0        0        0     9792 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/SpiderImagePlugin.py
+-rw-rw-rw-   0        0        0     4537 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/SunImagePlugin.py
+-rw-rw-rw-   0        0        0     1557 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/TarIO.py
+-rw-rw-rw-   0        0        0     6830 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/TgaImagePlugin.py
+-rw-rw-rw-   0        0        0    79211 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/TiffImagePlugin.py
+-rw-rw-rw-   0        0        0    17374 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/TiffTags.py
+-rw-rw-rw-   0        0        0     5642 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/WalImageFile.py
+-rw-rw-rw-   0        0        0    11732 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/WebPImagePlugin.py
+-rw-rw-rw-   0        0        0     4867 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/WmfImagePlugin.py
+-rw-rw-rw-   0        0        0     2064 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/XVThumbImagePlugin.py
+-rw-rw-rw-   0        0        0     2581 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/XbmImagePlugin.py
+-rw-rw-rw-   0        0        0     3312 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/XpmImagePlugin.py
+-rw-rw-rw-   0        0        0     2091 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/__main__.py
+-rw-rw-rw-   0        0        0     2145 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/_binary.py
+-rw-rw-rw-   0        0        0     2071 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/_deprecate.py
+-rw-rw-rw-   0        0        0      691 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/_tkinter_finder.py
+-rw-rw-rw-   0        0        0      388 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/_util.py
+-rw-rw-rw-   0        0        0       52 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/_version.py
+-rw-rw-rw-   0        0        0     9949 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/features.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.979632 whatsappy-py-4.0.0/.venv/Lib/site-packages/Pillow-9.5.0.dist-info/
+-rw-rw-rw-   0        0        0        4 2023-04-24 12:00:05.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/Pillow-9.5.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.979632 whatsappy-py-4.0.0/.venv/Lib/site-packages/PySocks-1.7.1.dist-info/
+-rw-rw-rw-   0        0        0       19 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/PySocks-1.7.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.982145 whatsappy-py-4.0.0/.venv/Lib/site-packages/Pygments-2.15.1.dist-info/
+-rw-rw-rw-   0        0        0       53 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/Pygments-2.15.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/Pygments-2.15.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.984645 whatsappy-py-4.0.0/.venv/Lib/site-packages/_distutils_hack/
+-rw-rw-rw-   0        0        0     6128 2023-04-22 16:56:02.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-04-22 16:56:02.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_distutils_hack/override.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.037417 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/
+-rw-rw-rw-   0        0        0      356 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/__init__.py
+-rw-rw-rw-   0        0        0     3794 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_argcomplete.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.040922 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_code/
+-rw-rw-rw-   0        0        0      483 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_code/__init__.py
+-rw-rw-rw-   0        0        0    45167 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_code/code.py
+-rw-rw-rw-   0        0        0     7436 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_code/source.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.044923 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_io/
+-rw-rw-rw-   0        0        0      154 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_io/__init__.py
+-rw-rw-rw-   0        0        0     5394 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_io/saferepr.py
+-rw-rw-rw-   0        0        0     8152 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_io/terminalwriter.py
+-rw-rw-rw-   0        0        0     1253 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_io/wcwidth.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.048444 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_py/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_py/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_py/error.py
+-rw-rw-rw-   0        0        0    49148 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_py/path.py
+-rw-rw-rw-   0        0        0      160 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.053945 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/assertion/
+-rw-rw-rw-   0        0        0     6458 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/assertion/__init__.py
+-rw-rw-rw-   0        0        0    45544 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/assertion/rewrite.py
+-rw-rw-rw-   0        0        0     4382 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/assertion/truncate.py
+-rw-rw-rw-   0        0        0    18009 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/assertion/util.py
+-rw-rw-rw-   0        0        0    20915 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/cacheprovider.py
+-rw-rw-rw-   0        0        0    34738 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/capture.py
+-rw-rw-rw-   0        0        0    13200 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/compat.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.059471 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/config/
+-rw-rw-rw-   0        0        0    61575 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/config/__init__.py
+-rw-rw-rw-   0        0        0    21225 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/config/argparsing.py
+-rw-rw-rw-   0        0        0     2393 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/config/compat.py
+-rw-rw-rw-   0        0        0      260 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/config/exceptions.py
+-rw-rw-rw-   0        0        0     7884 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/config/findpaths.py
+-rw-rw-rw-   0        0        0    13498 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/debugging.py
+-rw-rw-rw-   0        0        0     5487 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/deprecated.py
+-rw-rw-rw-   0        0        0    25961 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/doctest.py
+-rw-rw-rw-   0        0        0     3186 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/faulthandler.py
+-rw-rw-rw-   0        0        0    65966 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/fixtures.py
+-rw-rw-rw-   0        0        0     1339 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/freeze_support.py
+-rw-rw-rw-   0        0        0     8520 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/helpconfig.py
+-rw-rw-rw-   0        0        0    32465 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/hookspec.py
+-rw-rw-rw-   0        0        0    25716 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/junitxml.py
+-rw-rw-rw-   0        0        0    16929 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/legacypath.py
+-rw-rw-rw-   0        0        0    30626 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/logging.py
+-rw-rw-rw-   0        0        0    32448 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.062970 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/mark/
+-rw-rw-rw-   0        0        0     8468 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/mark/__init__.py
+-rw-rw-rw-   0        0        0     6385 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/mark/expression.py
+-rw-rw-rw-   0        0        0    21179 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/mark/structures.py
+-rw-rw-rw-   0        0        0    14341 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/monkeypatch.py
+-rw-rw-rw-   0        0        0    26522 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/nodes.py
+-rw-rw-rw-   0        0        0     1688 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/nose.py
+-rw-rw-rw-   0        0        0    10256 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/outcomes.py
+-rw-rw-rw-   0        0        0     3949 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/pastebin.py
+-rw-rw-rw-   0        0        0    25439 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/pathlib.py
+-rw-rw-rw-   0        0        0    61900 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/pytester.py
+-rw-rw-rw-   0        0        0     2327 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/pytester_assertions.py
+-rw-rw-rw-   0        0        0    71523 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/python.py
+-rw-rw-rw-   0        0        0    38571 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/python_api.py
+-rw-rw-rw-   0        0        0      709 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/python_path.py
+-rw-rw-rw-   0        0        0    10930 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/recwarn.py
+-rw-rw-rw-   0        0        0    20698 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/reports.py
+-rw-rw-rw-   0        0        0    18447 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/runner.py
+-rw-rw-rw-   0        0        0     2882 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/scope.py
+-rw-rw-rw-   0        0        0     3261 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/setuponly.py
+-rw-rw-rw-   0        0        0     1214 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/setupplan.py
+-rw-rw-rw-   0        0        0    10200 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/skipping.py
+-rw-rw-rw-   0        0        0     3055 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/stash.py
+-rw-rw-rw-   0        0        0     4714 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/stepwise.py
+-rw-rw-rw-   0        0        0    52060 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/terminal.py
+-rw-rw-rw-   0        0        0     2915 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/threadexception.py
+-rw-rw-rw-   0        0        0      375 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/timing.py
+-rw-rw-rw-   0        0        0    11709 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/tmpdir.py
+-rw-rw-rw-   0        0        0    14756 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/unittest.py
+-rw-rw-rw-   0        0        0     3191 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/unraisableexception.py
+-rw-rw-rw-   0        0        0     4474 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/warning_types.py
+-rw-rw-rw-   0        0        0     5070 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/_pytest/warnings.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.067481 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/
+-rw-rw-rw-   0        0        0      454 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/__init__.py
+-rw-rw-rw-   0        0        0    16106 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/_impl.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.073489 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/_tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/_tests/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/_tests/conftest.py
+-rw-rw-rw-   0        0        0    27936 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/_tests/test_async_generator.py
+-rw-rw-rw-   0        0        0     6373 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/_tests/test_util.py
+-rw-rw-rw-   0        0        0     4358 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/_util.py
+-rw-rw-rw-   0        0        0       21 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.068988 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator-1.10.dist-info/
+-rw-rw-rw-   0        0        0       16 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/async_generator-1.10.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.089101 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/
+-rw-rw-rw-   0        0        0     3241 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/__init__.py
+-rw-rw-rw-   0        0        0     4098 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/_cmp.py
+-rw-rw-rw-   0        0        0     5803 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/_compat.py
+-rw-rw-rw-   0        0        0      826 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/_config.py
+-rw-rw-rw-   0        0        0    16730 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/_funcs.py
+-rw-rw-rw-   0        0        0    96979 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/_make.py
+-rw-rw-rw-   0        0        0     6271 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/_next_gen.py
+-rw-rw-rw-   0        0        0     2121 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/_version_info.py
+-rw-rw-rw-   0        0        0     3602 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/converters.py
+-rw-rw-rw-   0        0        0     1890 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/exceptions.py
+-rw-rw-rw-   0        0        0     1470 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/filters.py
+-rw-rw-rw-   0        0        0     1400 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/setters.py
+-rw-rw-rw-   0        0        0    20702 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attr/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.095101 whatsappy-py-4.0.0/.venv/Lib/site-packages/attrs/
+-rw-rw-rw-   0        0        0     1039 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attrs/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attrs/converters.py
+-rw-rw-rw-   0        0        0       70 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attrs/exceptions.py
+-rw-rw-rw-   0        0        0       67 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attrs/filters.py
+-rw-rw-rw-   0        0        0       67 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attrs/setters.py
+-rw-rw-rw-   0        0        0       70 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/attrs/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.103627 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/
+-rw-rw-rw-   0        0        0     3649 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.108145 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.118161 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/
+-rw-rw-rw-   0        0        0     1143 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/__init__.py
+-rw-rw-rw-   0        0        0    16728 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py
+-rw-rw-rw-   0        0        0    32300 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py
+-rw-rw-rw-   0        0        0    77028 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.123173 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/
+-rw-rw-rw-   0        0        0      109 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
+-rw-rw-rw-   0        0        0     1013 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py
+-rw-rw-rw-   0        0        0     1763 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py
+-rw-rw-rw-   0        0        0     4919 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/_utils.py
+-rw-rw-rw-   0        0        0    83464 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.132685 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/__init__.py
+-rw-rw-rw-   0        0        0      919 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-rw-rw-   0        0        0      286 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/base.py
+-rw-rw-rw-   0        0        0     2945 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-rw-rw-   0        0        0     3631 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py
+-rw-rw-rw-   0        0        0    10588 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
+-rw-rw-rw-   0        0        0    26885 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
+-rw-rw-rw-   0        0        0     1214 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
+-rw-rw-rw-   0        0        0   117174 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py
+-rw-rw-rw-   0        0        0    15747 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.136196 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/
+-rw-rw-rw-   0        0        0      650 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
+-rw-rw-rw-   0        0        0     1715 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
+-rw-rw-rw-   0        0        0     1776 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.141709 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/
+-rw-rw-rw-   0        0        0     3592 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
+-rw-rw-rw-   0        0        0    14553 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
+-rw-rw-rw-   0        0        0     8925 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
+-rw-rw-rw-   0        0        0    12824 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
+-rw-rw-rw-   0        0        0    14754 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.148798 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/
+-rw-rw-rw-   0        0        0     5719 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
+-rw-rw-rw-   0        0        0     7476 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
+-rw-rw-rw-   0        0        0     1413 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
+-rw-rw-rw-   0        0        0     4539 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
+-rw-rw-rw-   0        0        0     6345 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-rw-rw-   0        0        0     2309 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.119666 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/
+-rw-rw-rw-   0        0        0        9 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
+-rw-rw-rw-   0        0        0    39023 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/parse.py
+-rw-rw-rw-   0        0        0      184 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/_vendor/vendor.txt
+-rw-rw-rw-   0        0        0      752 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/callbacks.py
+-rw-rw-rw-   0        0        0     2526 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/css_sanitizer.py
+-rw-rw-rw-   0        0        0    22779 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/html5lib_shim.py
+-rw-rw-rw-   0        0        0    22350 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/linkifier.py
+-rw-rw-rw-   0        0        0       50 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/parse_shim.py
+-rw-rw-rw-   0        0        0    21934 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach/sanitizer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.105126 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach-6.0.0.dist-info/
+-rw-rw-rw-   0        0        0        7 2023-05-09 19:20:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bleach-6.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.155299 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/
+-rw-rw-rw-   0        0        0    33822 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.161323 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/builder/
+-rw-rw-rw-   0        0        0    24393 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/builder/__init__.py
+-rw-rw-rw-   0        0        0    19078 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/builder/_html5lib.py
+-rw-rw-rw-   0        0        0    14919 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/builder/_htmlparser.py
+-rw-rw-rw-   0        0        0    14904 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/builder/_lxml.py
+-rw-rw-rw-   0        0        0    10077 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/css.py
+-rw-rw-rw-   0        0        0    41158 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/dammit.py
+-rw-rw-rw-   0        0        0     7195 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/diagnose.py
+-rw-rw-rw-   0        0        0    92716 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/element.py
+-rw-rw-rw-   0        0        0     7184 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/formatter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.180379 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/
+-rw-rw-rw-   0        0        0    48391 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1115 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_builder.py
+-rw-rw-rw-   0        0        0     5114 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_builder_registry.py
+-rw-rw-rw-   0        0        0    17279 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_css.py
+-rw-rw-rw-   0        0        0    15451 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_dammit.py
+-rw-rw-rw-   0        0        0     1127 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_docs.py
+-rw-rw-rw-   0        0        0     2377 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_element.py
+-rw-rw-rw-   0        0        0     4148 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     3637 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_fuzz.py
+-rw-rw-rw-   0        0        0     8322 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_html5lib.py
+-rw-rw-rw-   0        0        0     6256 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_htmlparser.py
+-rw-rw-rw-   0        0        0     7635 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_lxml.py
+-rw-rw-rw-   0        0        0     5081 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_navigablestring.py
+-rw-rw-rw-   0        0        0    14274 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_pageelement.py
+-rw-rw-rw-   0        0        0    19877 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_soup.py
+-rw-rw-rw-   0        0        0     9016 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_tag.py
+-rw-rw-rw-   0        0        0    48129 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4/tests/test_tree.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.156818 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4-0.0.1.dist-info/
+-rw-rw-rw-   0        0        0        1 2023-05-06 16:48:12.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/bs4-0.0.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.184886 whatsappy-py-4.0.0/.venv/Lib/site-packages/build/
+-rw-rw-rw-   0        0        0    19190 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/build/__init__.py
+-rw-rw-rw-   0        0        0    12200 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/build/__main__.py
+-rw-rw-rw-   0        0        0    12636 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/build/env.py
+-rw-rw-rw-   0        0        0     1632 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/build/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.186401 whatsappy-py-4.0.0/.venv/Lib/site-packages/build-0.10.0.dist-info/
+-rw-rw-rw-   0        0        0      105 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/build-0.10.0.dist-info/entry_points.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.189408 whatsappy-py-4.0.0/.venv/Lib/site-packages/certifi/
+-rw-rw-rw-   0        0        0       94 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/certifi/__init__.py
+-rw-rw-rw-   0        0        0      243 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4219 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.190907 whatsappy-py-4.0.0/.venv/Lib/site-packages/certifi-2022.12.7.dist-info/
+-rw-rw-rw-   0        0        0        8 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/certifi-2022.12.7.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.209957 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/
+-rw-rw-rw-   0        0        0      527 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/__init__.py
+-rw-rw-rw-   0        0        0    43029 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/api.py
+-rw-rw-rw-   0        0        0    43575 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/backend_ctypes.py
+-rw-rw-rw-   0        0        0     5911 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/cffi_opcode.py
+-rw-rw-rw-   0        0        0     2769 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/commontypes.py
+-rw-rw-rw-   0        0        0    45237 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/cparser.py
+-rw-rw-rw-   0        0        0      908 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/error.py
+-rw-rw-rw-   0        0        0     4173 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/ffiplatform.py
+-rw-rw-rw-   0        0        0      777 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/lock.py
+-rw-rw-rw-   0        0        0    22385 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/model.py
+-rw-rw-rw-   0        0        0     4495 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/pkgconfig.py
+-rw-rw-rw-   0        0        0    66179 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/recompiler.py
+-rw-rw-rw-   0        0        0     9150 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/setuptools_ext.py
+-rw-rw-rw-   0        0        0    44396 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/vengine_cpy.py
+-rw-rw-rw-   0        0        0    27359 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/vengine_gen.py
+-rw-rw-rw-   0        0        0    11560 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi/verifier.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.211957 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi-1.15.1.dist-info/
+-rw-rw-rw-   0        0        0       75 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi-1.15.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/cffi-1.15.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.222475 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/
+-rw-rw-rw-   0        0        0     1594 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/__init__.py
+-rw-rw-rw-   0        0        0    19178 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/api.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.224976 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/assets/
+-rw-rw-rw-   0        0        0    21509 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/assets/__init__.py
+-rw-rw-rw-   0        0        0    12944 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/cd.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.227492 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/cli/__init__.py
+-rw-rw-rw-   0        0        0    10040 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/cli/normalizer.py
+-rw-rw-rw-   0        0        0    19596 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/constant.py
+-rw-rw-rw-   0        0        0     2125 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/legacy.py
+-rw-rw-rw-   0        0        0    18829 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/md.py
+-rw-rw-rw-   0        0        0    11829 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/models.py
+-rw-rw-rw-   0        0        0    11958 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/utils.py
+-rw-rw-rw-   0        0        0       85 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.224475 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer-3.1.0.dist-info/
+-rw-rw-rw-   0        0        0       76 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer-3.1.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/charset_normalizer-3.1.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.233999 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/
+-rw-rw-rw-   0        0        0      266 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/ansi.py
+-rw-rw-rw-   0        0        0    11128 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     3325 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/initialise.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.242526 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/tests/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/tests/ansi_test.py
+-rw-rw-rw-   0        0        0    10678 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/tests/ansitowin32_test.py
+-rw-rw-rw-   0        0        0     6741 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/tests/initialise_test.py
+-rw-rw-rw-   0        0        0     1866 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/tests/isatty_test.py
+-rw-rw-rw-   0        0        0     1079 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/tests/utils.py
+-rw-rw-rw-   0        0        0     3709 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/tests/winterm_test.py
+-rw-rw-rw-   0        0        0     6181 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/win32.py
+-rw-rw-rw-   0        0        0     7134 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.730561 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama-0.4.6.dist-info/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.235001 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/
+-rw-rw-rw-   0        0        0     1491 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.246035 whatsappy-py-4.0.0/.venv/Lib/site-packages/datefinder/
+-rw-rw-rw-   0        0        0    12093 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/datefinder/__init__.py
+-rw-rw-rw-   0        0        0     8346 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/datefinder/constants.py
+-rw-rw-rw-   0        0        0      628 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/datefinder/date_fragment.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.247543 whatsappy-py-4.0.0/.venv/Lib/site-packages/datefinder-0.7.3.dist-info/
+-rw-rw-rw-   0        0        0       11 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/datefinder-0.7.3.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.257068 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/
+-rw-rw-rw-   0        0        0      222 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/__init__.py
+-rw-rw-rw-   0        0        0      932 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/_common.py
+-rw-rw-rw-   0        0        0      142 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/_version.py
+-rw-rw-rw-   0        0        0     2678 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/easter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.260574 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/parser/
+-rw-rw-rw-   0        0        0     1766 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/parser/__init__.py
+-rw-rw-rw-   0        0        0    58796 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/parser/_parser.py
+-rw-rw-rw-   0        0        0    13247 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/parser/isoparser.py
+-rw-rw-rw-   0        0        0    24904 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/relativedelta.py
+-rw-rw-rw-   0        0        0    66556 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/rrule.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.265072 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/tz/
+-rw-rw-rw-   0        0        0      444 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/tz/__init__.py
+-rw-rw-rw-   0        0        0    12977 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/tz/_common.py
+-rw-rw-rw-   0        0        0     2569 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/tz/_factories.py
+-rw-rw-rw-   0        0        0    62857 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/tz/tz.py
+-rw-rw-rw-   0        0        0    12935 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/tz/win.py
+-rw-rw-rw-   0        0        0       59 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/tzwin.py
+-rw-rw-rw-   0        0        0     1965 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.268097 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/zoneinfo/
+-rw-rw-rw-   0        0        0     5889 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/zoneinfo/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dateutil/zoneinfo/rebuild.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.278112 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/
+-rw-rw-rw-   0        0        0    10291 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/__main__.py
+-rw-rw-rw-   0        0        0    33045 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/core.py
+-rw-rw-rw-   0        0        0     3961 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/examples.py
+-rw-rw-rw-   0        0        0    40002 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/frontend.py
+-rw-rw-rw-   0        0        0    23958 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/io.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.315189 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/
+-rw-rw-rw-   0        0        0     2921 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/__init__.py
+-rw-rw-rw-   0        0        0     1831 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/af.py
+-rw-rw-rw-   0        0        0     1943 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/ar.py
+-rw-rw-rw-   0        0        0     1912 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/ca.py
+-rw-rw-rw-   0        0        0     1900 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/cs.py
+-rw-rw-rw-   0        0        0     1856 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/da.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/de.py
+-rw-rw-rw-   0        0        0     1854 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/en.py
+-rw-rw-rw-   0        0        0     1931 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/eo.py
+-rw-rw-rw-   0        0        0     1906 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/es.py
+-rw-rw-rw-   0        0        0     1958 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/fa.py
+-rw-rw-rw-   0        0        0     1964 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/fi.py
+-rw-rw-rw-   0        0        0     1831 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/fr.py
+-rw-rw-rw-   0        0        0     1990 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/gl.py
+-rw-rw-rw-   0        0        0     2692 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/he.py
+-rw-rw-rw-   0        0        0     1814 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/it.py
+-rw-rw-rw-   0        0        0     1890 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/ja.py
+-rw-rw-rw-   0        0        0     1832 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/ko.py
+-rw-rw-rw-   0        0        0     1919 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/lt.py
+-rw-rw-rw-   0        0        0     1851 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/lv.py
+-rw-rw-rw-   0        0        0     1871 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/nl.py
+-rw-rw-rw-   0        0        0     1866 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/pl.py
+-rw-rw-rw-   0        0        0     1929 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/pt_br.py
+-rw-rw-rw-   0        0        0     2070 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/ru.py
+-rw-rw-rw-   0        0        0     1832 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/sk.py
+-rw-rw-rw-   0        0        0     1863 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/sv.py
+-rw-rw-rw-   0        0        0     2062 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/uk.py
+-rw-rw-rw-   0        0        0     1974 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/zh_cn.py
+-rw-rw-rw-   0        0        0     2742 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/languages/zh_tw.py
+-rw-rw-rw-   0        0        0    81006 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/nodes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.320720 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/
+-rw-rw-rw-   0        0        0     3724 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1765 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
+-rw-rw-rw-   0        0        0      445 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/null.py
+-rw-rw-rw-   0        0        0     5426 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.325220 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/
+-rw-rw-rw-   0        0        0    15954 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.335243 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/
+-rw-rw-rw-   0        0        0    14652 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
+-rw-rw-rw-   0        0        0     9883 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/body.py
+-rw-rw-rw-   0        0        0      695 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/html.py
+-rw-rw-rw-   0        0        0     6799 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/images.py
+-rw-rw-rw-   0        0        0    26302 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py
+-rw-rw-rw-   0        0        0     4247 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py
+-rw-rw-rw-   0        0        0      831 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/references.py
+-rw-rw-rw-   0        0        0    23825 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.375824 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/
+-rw-rw-rw-   0        0        0      670 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/README.txt
+-rw-rw-rw-   0        0        0    10925 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
+-rw-rw-rw-   0        0        0     7242 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
+-rw-rw-rw-   0        0        0     1723 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
+-rw-rw-rw-   0        0        0     6721 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
+-rw-rw-rw-   0        0        0     3825 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
+-rw-rw-rw-   0        0        0    11763 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
+-rw-rw-rw-   0        0        0     3101 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
+-rw-rw-rw-   0        0        0     4241 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
+-rw-rw-rw-   0        0        0     1882 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
+-rw-rw-rw-   0        0        0      869 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
+-rw-rw-rw-   0        0        0     3010 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
+-rw-rw-rw-   0        0        0     1705 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
+-rw-rw-rw-   0        0        0     2880 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
+-rw-rw-rw-   0        0        0     3035 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
+-rw-rw-rw-   0        0        0      372 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
+-rw-rw-rw-   0        0        0     4397 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
+-rw-rw-rw-   0        0        0     8466 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
+-rw-rw-rw-   0        0        0     3334 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
+-rw-rw-rw-   0        0        0      519 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
+-rw-rw-rw-   0        0        0     1931 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
+-rw-rw-rw-   0        0        0      639 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
+-rw-rw-rw-   0        0        0     3231 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
+-rw-rw-rw-   0        0        0      776 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
+-rw-rw-rw-   0        0        0     4066 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
+-rw-rw-rw-   0        0        0     4613 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
+-rw-rw-rw-   0        0        0     9726 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
+-rw-rw-rw-   0        0        0    45428 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
+-rw-rw-rw-   0        0        0     9010 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
+-rw-rw-rw-   0        0        0     6800 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
+-rw-rw-rw-   0        0        0     1036 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
+-rw-rw-rw-   0        0        0     6112 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
+-rw-rw-rw-   0        0        0     1945 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
+-rw-rw-rw-   0        0        0     7028 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.418430 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/
+-rw-rw-rw-   0        0        0     1222 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
+-rw-rw-rw-   0        0        0     3727 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/af.py
+-rw-rw-rw-   0        0        0     3051 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py
+-rw-rw-rw-   0        0        0     4406 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py
+-rw-rw-rw-   0        0        0     4808 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py
+-rw-rw-rw-   0        0        0     3719 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/da.py
+-rw-rw-rw-   0        0        0     3547 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/de.py
+-rw-rw-rw-   0        0        0     3514 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/en.py
+-rw-rw-rw-   0        0        0     3825 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py
+-rw-rw-rw-   0        0        0     4158 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/es.py
+-rw-rw-rw-   0        0        0     3171 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py
+-rw-rw-rw-   0        0        0     3526 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py
+-rw-rw-rw-   0        0        0     3652 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py
+-rw-rw-rw-   0        0        0     3632 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py
+-rw-rw-rw-   0        0        0     3641 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/he.py
+-rw-rw-rw-   0        0        0     3322 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/it.py
+-rw-rw-rw-   0        0        0     3776 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py
+-rw-rw-rw-   0        0        0     3377 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py
+-rw-rw-rw-   0        0        0     3519 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py
+-rw-rw-rw-   0        0        0     3376 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py
+-rw-rw-rw-   0        0        0     3761 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py
+-rw-rw-rw-   0        0        0     3443 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py
+-rw-rw-rw-   0        0        0     3960 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
+-rw-rw-rw-   0        0        0     3398 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py
+-rw-rw-rw-   0        0        0     3947 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py
+-rw-rw-rw-   0        0        0     3261 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py
+-rw-rw-rw-   0        0        0     3441 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py
+-rw-rw-rw-   0        0        0     3925 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
+-rw-rw-rw-   0        0        0     5160 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
+-rw-rw-rw-   0        0        0    16119 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/roles.py
+-rw-rw-rw-   0        0        0   132550 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/states.py
+-rw-rw-rw-   0        0        0    20912 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/parsers/rst/tableparser.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.423429 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/readers/
+-rw-rw-rw-   0        0        0     3520 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/readers/__init__.py
+-rw-rw-rw-   0        0        0     1607 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/readers/doctree.py
+-rw-rw-rw-   0        0        0     1523 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/readers/pep.py
+-rw-rw-rw-   0        0        0     2324 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/readers/standalone.py
+-rw-rw-rw-   0        0        0    56956 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/statemachine.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.435970 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/
+-rw-rw-rw-   0        0        0     6870 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2151 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/components.py
+-rw-rw-rw-   0        0        0    21371 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/frontmatter.py
+-rw-rw-rw-   0        0        0     4873 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/misc.py
+-rw-rw-rw-   0        0        0     6912 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/parts.py
+-rw-rw-rw-   0        0        0    11111 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/peps.py
+-rw-rw-rw-   0        0        0    36819 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/references.py
+-rw-rw-rw-   0        0        0    12548 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/universal.py
+-rw-rw-rw-   0        0        0     3057 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/transforms/writer_aux.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.444486 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/
+-rw-rw-rw-   0        0        0    29382 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/__init__.py
+-rw-rw-rw-   0        0        0     4920 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/code_analyzer.py
+-rw-rw-rw-   0        0        0     8105 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/error_reporting.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.451600 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/math/
+-rw-rw-rw-   0        0        0     1825 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/math/__init__.py
+-rw-rw-rw-   0        0        0    51496 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/math/latex2mathml.py
+-rw-rw-rw-   0        0        0   107993 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/math/math2html.py
+-rw-rw-rw-   0        0        0     6760 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
+-rw-rw-rw-   0        0        0    37497 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/math/tex2unichar.py
+-rw-rw-rw-   0        0        0    18393 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/math/unichar2tex.py
+-rw-rw-rw-   0        0        0     5747 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/punctuation_chars.py
+-rw-rw-rw-   0        0        0     2695 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/roman.py
+-rw-rw-rw-   0        0        0    38972 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/smartquotes.py
+-rw-rw-rw-   0        0        0     6260 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/utils/urischemes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.458629 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/
+-rw-rw-rw-   0        0        0     4945 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/__init__.py
+-rw-rw-rw-   0        0        0    70896 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/_html_base.py
+-rw-rw-rw-   0        0        0     6763 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/docutils_xml.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.460628 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/html4css1/
+-rw-rw-rw-   0        0        0    37675 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/html4css1/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/html4css1/template.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.462629 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/html5_polyglot/
+-rw-rw-rw-   0        0        0    16718 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.464129 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/latex2e/
+-rw-rw-rw-   0        0        0   137132 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/latex2e/__init__.py
+-rw-rw-rw-   0        0        0    36654 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/manpage.py
+-rw-rw-rw-   0        0        0      568 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/null.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.466647 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/odf_odt/
+-rw-rw-rw-   0        0        0   132358 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py
+-rw-rw-rw-   0        0        0     4681 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.468654 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/pep_html/
+-rw-rw-rw-   0        0        0     3505 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/pep_html/__init__.py
+-rw-rw-rw-   0        0        0     1001 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/pep_html/template.txt
+-rw-rw-rw-   0        0        0     1032 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/pseudoxml.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.470153 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/s5_html/
+-rw-rw-rw-   0        0        0    14517 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/s5_html/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.471152 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/s5_html/themes/
+-rw-rw-rw-   0        0        0      278 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.472153 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/xetex/
+-rw-rw-rw-   0        0        0     5736 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils/writers/xetex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.282128 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils-0.20.dist-info/
+-rw-rw-rw-   0        0        0     6292 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils-0.20.dist-info/COPYING.txt
+-rw-rw-rw-   0        0        0       53 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils-0.20.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/docutils-0.20.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.481692 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/
+-rw-rw-rw-   0        0        0     1292 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/__main__.py
+-rw-rw-rw-   0        0        0     5809 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/cli.py
+-rw-rw-rw-   0        0        0     1303 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/ipython.py
+-rw-rw-rw-   0        0        0    11932 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/main.py
+-rw-rw-rw-   0        0        0     5186 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/parser.py
+-rw-rw-rw-   0        0        0     2348 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/variables.py
+-rw-rw-rw-   0        0        0       22 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/dotenv/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.487206 whatsappy-py-4.0.0/.venv/Lib/site-packages/exceptiongroup/
+-rw-rw-rw-   0        0        0      920 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/exceptiongroup/__init__.py
+-rw-rw-rw-   0        0        0     3578 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/exceptiongroup/_catch.py
+-rw-rw-rw-   0        0        0     9772 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/exceptiongroup/_exceptions.py
+-rw-rw-rw-   0        0        0    19475 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/exceptiongroup/_formatting.py
+-rw-rw-rw-   0        0        0      160 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/exceptiongroup/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.498732 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/
+-rw-rw-rw-   0        0        0     1507 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/__init__.py
+-rw-rw-rw-   0        0        0     4815 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_abnf.py
+-rw-rw-rw-   0        0        0    26539 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_connection.py
+-rw-rw-rw-   0        0        0    11816 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_events.py
+-rw-rw-rw-   0        0        0    10230 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_headers.py
+-rw-rw-rw-   0        0        0     8383 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_readers.py
+-rw-rw-rw-   0        0        0     5252 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_receivebuffer.py
+-rw-rw-rw-   0        0        0    13300 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_state.py
+-rw-rw-rw-   0        0        0     4888 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_util.py
+-rw-rw-rw-   0        0        0      686 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_version.py
+-rw-rw-rw-   0        0        0     5081 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/_writers.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.512756 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/helpers.py
+-rw-rw-rw-   0        0        0     3995 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_against_stdlib_http.py
+-rw-rw-rw-   0        0        0    38720 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_connection.py
+-rw-rw-rw-   0        0        0     4657 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_events.py
+-rw-rw-rw-   0        0        0     5612 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_headers.py
+-rw-rw-rw-   0        0        0      794 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_helpers.py
+-rw-rw-rw-   0        0        0    16386 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_io.py
+-rw-rw-rw-   0        0        0     3454 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_receivebuffer.py
+-rw-rw-rw-   0        0        0     8928 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_state.py
+-rw-rw-rw-   0        0        0     2970 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.501230 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11-0.14.0.dist-info/
+-rw-rw-rw-   0        0        0     1124 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11-0.14.0.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/h11-0.14.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.521290 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/
+-rw-rw-rw-   0        0        0      849 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.531306 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/
+-rw-rw-rw-   0        0        0    29949 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     2454 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     2096 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1615 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     1098 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/_py39compat.py
+-rw-rw-rw-   0        0        0     2166 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.532309 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata-6.6.0.dist-info/
+-rw-rw-rw-   0        0        0       19 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/importlib_metadata-6.6.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.536313 whatsappy-py-4.0.0/.venv/Lib/site-packages/iniconfig/
+-rw-rw-rw-   0        0        0     5473 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/iniconfig/__init__.py
+-rw-rw-rw-   0        0        0     2436 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/iniconfig/_parse.py
+-rw-rw-rw-   0        0        0      160 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/iniconfig/_version.py
+-rw-rw-rw-   0        0        0      501 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/iniconfig/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.747105 whatsappy-py-4.0.0/.venv/Lib/site-packages/jaraco/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.541328 whatsappy-py-4.0.0/.venv/Lib/site-packages/jaraco/classes/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/jaraco/classes/__init__.py
+-rw-rw-rw-   0        0        0     1464 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/jaraco/classes/ancestry.py
+-rw-rw-rw-   0        0        0     1853 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/jaraco/classes/meta.py
+-rw-rw-rw-   0        0        0     3996 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/jaraco/classes/properties.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.537320 whatsappy-py-4.0.0/.venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/
+-rw-rw-rw-   0        0        0        7 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/jaraco.classes-3.2.3.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.556366 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/
+-rw-rw-rw-   0        0        0      271 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/__main__.py
+-rw-rw-rw-   0        0        0      185 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/_compat.py
+-rw-rw-rw-   0        0        0     3886 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/_properties_compat.py
+-rw-rw-rw-   0        0        0     7587 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backend.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.568395 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/
+-rw-rw-rw-   0        0        0      222 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/OS_X.py
+-rw-rw-rw-   0        0        0     4685 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/SecretService.py
+-rw-rw-rw-   0        0        0     5807 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/Windows.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/__init__.py
+-rw-rw-rw-   0        0        0     2167 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/chainer.py
+-rw-rw-rw-   0        0        0      836 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/fail.py
+-rw-rw-rw-   0        0        0     5821 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/kwallet.py
+-rw-rw-rw-   0        0        0     5973 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/libsecret.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.569899 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/macOS/
+-rw-rw-rw-   0        0        0     2363 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/macOS/__init__.py
+-rw-rw-rw-   0        0        0     4341 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/macOS/api.py
+-rw-rw-rw-   0        0        0      360 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/backends/null.py
+-rw-rw-rw-   0        0        0     4000 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/cli.py
+-rw-rw-rw-   0        0        0     1324 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/completion.py
+-rw-rw-rw-   0        0        0     5215 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/core.py
+-rw-rw-rw-   0        0        0     1593 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/credentials.py
+-rw-rw-rw-   0        0        0      752 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/devpi_client.py
+-rw-rw-rw-   0        0        0     1430 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/errors.py
+-rw-rw-rw-   0        0        0     1231 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/http.py
+-rw-rw-rw-   0        0        0      175 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/py312compat.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.573396 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/testing/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/testing/__init__.py
+-rw-rw-rw-   0        0        0     6598 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/testing/backend.py
+-rw-rw-rw-   0        0        0     1918 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/testing/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.576413 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/util/
+-rw-rw-rw-   0        0        0      868 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/util/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/util/platform_.py
+-rw-rw-rw-   0        0        0      318 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring/util/properties.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.558367 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring-23.13.1.dist-info/
+-rw-rw-rw-   0        0        0      334 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring-23.13.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/keyring-23.13.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.589450 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/
+-rw-rw-rw-   0        0        0      113 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/_compat.py
+-rw-rw-rw-   0        0        0     2317 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/_punycode.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.591450 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/cli/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/cli/__init__.py
+-rw-rw-rw-   0        0        0     2901 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/cli/parse.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.597975 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/common/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/common/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/common/entities.py
+-rw-rw-rw-   0        0        0      932 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/common/html_blocks.py
+-rw-rw-rw-   0        0        0      929 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/common/html_re.py
+-rw-rw-rw-   0        0        0     2631 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/common/normalize_url.py
+-rw-rw-rw-   0        0        0    10894 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.602475 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/helpers/
+-rw-rw-rw-   0        0        0      253 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1953 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
+-rw-rw-rw-   0        0        0     1070 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py
+-rw-rw-rw-   0        0        0     1410 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py
+-rw-rw-rw-   0        0        0    12228 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/main.py
+-rw-rw-rw-   0        0        0     3662 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/parser_block.py
+-rw-rw-rw-   0        0        0      835 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/parser_core.py
+-rw-rw-rw-   0        0        0     4130 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/parser_inline.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.606493 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/presets/
+-rw-rw-rw-   0        0        0      898 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/presets/__init__.py
+-rw-rw-rw-   0        0        0     2809 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/presets/commonmark.py
+-rw-rw-rw-   0        0        0     1765 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/presets/default.py
+-rw-rw-rw-   0        0        0     2006 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/presets/zero.py
+-rw-rw-rw-   0        0        0    10041 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/renderer.py
+-rw-rw-rw-   0        0        0     8376 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/ruler.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.621522 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/
+-rw-rw-rw-   0        0        0      553 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/__init__.py
+-rw-rw-rw-   0        0        0     9057 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/blockquote.py
+-rw-rw-rw-   0        0        0      886 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/code.py
+-rw-rw-rw-   0        0        0     2704 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/fence.py
+-rw-rw-rw-   0        0        0     1879 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/heading.py
+-rw-rw-rw-   0        0        0     1309 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/hr.py
+-rw-rw-rw-   0        0        0     2808 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/html_block.py
+-rw-rw-rw-   0        0        0     2798 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/lheading.py
+-rw-rw-rw-   0        0        0     9944 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/list.py
+-rw-rw-rw-   0        0        0     1851 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/paragraph.py
+-rw-rw-rw-   0        0        0     6323 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/reference.py
+-rw-rw-rw-   0        0        0     7226 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/state_block.py
+-rw-rw-rw-   0        0        0     7226 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_block/table.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.630046 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/
+-rw-rw-rw-   0        0        0      344 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/block.py
+-rw-rw-rw-   0        0        0      325 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/inline.py
+-rw-rw-rw-   0        0        0     4833 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/linkify.py
+-rw-rw-rw-   0        0        0      402 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/normalize.py
+-rw-rw-rw-   0        0        0     3560 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/replacements.py
+-rw-rw-rw-   0        0        0     7251 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py
+-rw-rw-rw-   0        0        0      584 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_core/state_core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.647080 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/
+-rw-rw-rw-   0        0        0      649 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/__init__.py
+-rw-rw-rw-   0        0        0     2131 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/autolink.py
+-rw-rw-rw-   0        0        0     2112 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/backticks.py
+-rw-rw-rw-   0        0        0     4062 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rw-rw-rw-   0        0        0     2948 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py
+-rw-rw-rw-   0        0        0     1653 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/entity.py
+-rw-rw-rw-   0        0        0     1116 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/escape.py
+-rw-rw-rw-   0        0        0     1019 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py
+-rw-rw-rw-   0        0        0     4260 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/image.py
+-rw-rw-rw-   0        0        0     4362 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/link.py
+-rw-rw-rw-   0        0        0     1176 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/newline.py
+-rw-rw-rw-   0        0        0     5388 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py
+-rw-rw-rw-   0        0        0     3390 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
+-rw-rw-rw-   0        0        0     1427 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/text.py
+-rw-rw-rw-   0        0        0     1491 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/rules_inline/text_collapse.py
+-rw-rw-rw-   0        0        0     6374 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/token.py
+-rw-rw-rw-   0        0        0    11052 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/tree.py
+-rw-rw-rw-   0        0        0     3262 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.648587 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/
+-rw-rw-rw-   0        0        0       58 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/markdown_it_py-2.2.0.dist-info/entry_points.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.655088 whatsappy-py-4.0.0/.venv/Lib/site-packages/mdurl/
+-rw-rw-rw-   0        0        0      547 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/mdurl/__init__.py
+-rw-rw-rw-   0        0        0     3004 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/mdurl/_decode.py
+-rw-rw-rw-   0        0        0     2602 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/mdurl/_encode.py
+-rw-rw-rw-   0        0        0      626 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/mdurl/_format.py
+-rw-rw-rw-   0        0        0    11374 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/mdurl/_parse.py
+-rw-rw-rw-   0        0        0      284 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/mdurl/_url.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.659113 whatsappy-py-4.0.0/.venv/Lib/site-packages/more_itertools/
+-rw-rw-rw-   0        0        0      148 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   134968 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/more_itertools/more.py
+-rw-rw-rw-   0        0        0    25416 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.660111 whatsappy-py-4.0.0/.venv/Lib/site-packages/multimethod/
+-rw-rw-rw-   0        0        0    16958 2023-05-01 17:55:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/multimethod/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.662112 whatsappy-py-4.0.0/.venv/Lib/site-packages/multimethod-1.9.1.dist-info/
+-rw-rw-rw-   0        0        0      576 2023-05-01 17:55:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/multimethod-1.9.1.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 17:55:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/multimethod-1.9.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.666627 whatsappy-py-4.0.0/.venv/Lib/site-packages/outcome/
+-rw-rw-rw-   0        0        0      351 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/outcome/__init__.py
+-rw-rw-rw-   0        0        0     4705 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/outcome/_impl.py
+-rw-rw-rw-   0        0        0      689 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/outcome/_util.py
+-rw-rw-rw-   0        0        0       89 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/outcome/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.667624 whatsappy-py-4.0.0/.venv/Lib/site-packages/outcome-1.2.0.dist-info/
+-rw-rw-rw-   0        0        0        8 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/outcome-1.2.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.683667 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/
+-rw-rw-rw-   0        0        0      501 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     8926 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2524 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0    10194 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5292 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8208 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/markers.py
+-rw-rw-rw-   0        0        0    16397 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/metadata.py
+-rw-rw-rw-   0        0        0     3287 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39206 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18106 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/tags.py
+-rw-rw-rw-   0        0        0     4355 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/utils.py
+-rw-rw-rw-   0        0        0    16326 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.687180 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/
+-rw-rw-rw-   0        0        0      357 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/__main__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/__pip-runner__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.702209 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/
+-rw-rw-rw-   0        0        0      573 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0    10243 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0     9661 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.715236 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     8176 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    30030 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      774 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2472 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     4338 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10817 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     1968 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    18328 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5118 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.736291 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3882 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7581 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1684 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     4129 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     9815 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6591 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     5182 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     2951 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4793 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0     3188 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-rw-   0        0        0    28722 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12343 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     6419 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3886 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     6324 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    13529 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.742813 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      729 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     6494 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1164 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    23741 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.746827 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    16504 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    37873 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     6556 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.752331 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    15365 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     6100 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7680 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     2556 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.757346 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     4280 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-rw-   0        0        0    25277 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/base.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.761853 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-rw-   0        0        0      107 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-rw-   0        0        0     8181 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-rw-   0        0        0     7457 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-rw-   0        0        0     9773 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.776401 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     6931 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2520 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     2619 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-rw-   0        0        0    18817 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4643 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     3858 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3600 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.786439 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    20435 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     2145 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6096 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7638 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    18442 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4073 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1791 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.791448 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.801065 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-rw-   0        0        0     1422 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1474 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     2198 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1075 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1417 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3064 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     5122 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9816 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.804567 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0    27475 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    27696 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     7161 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.811602 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2738 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    16610 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17872 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    32782 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     2858 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0    24678 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.813102 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.815101 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24128 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.825129 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    18864 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    27845 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9824 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     3094 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5454 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0    11538 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     8167 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.856732 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     3351 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-rw-rw-   0        0        0     1015 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     3627 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     2118 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     3064 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5122 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3110 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     5118 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0      795 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-rw-   0        0        0    11632 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    22216 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2108 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     4435 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0     9200 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     7702 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8821 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3456 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     4549 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.863736 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     3519 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    18116 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     5238 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11729 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22811 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    11842 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.867751 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0     4966 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.879791 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      465 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1379 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     5033 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0     1535 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.883409 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0      242 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0     1033 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0      778 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-   0        0        0    16416 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     3946 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4154 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7105 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0      774 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.886414 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       94 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4279 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.951740 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     4797 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31274 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1763 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0    10032 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3915 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     5420 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.954238 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3732 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0      542 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-rw-   0        0        0     1860 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1683 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     4006 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    12176 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3934 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13566 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    36913 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20735 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1759 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    14537 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25796 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    42498 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-rw-   0        0        0     1752 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-rw-   0        0        0    27055 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   104562 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    98484 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98196 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   101363 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   128035 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   102774 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95372 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5380 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     6077 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-rw-   0        0        0     3715 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2131 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    30391 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.956751 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    13560 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0      402 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-rw-   0        0        0     6400 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4137 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     4007 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    14848 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     8505 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-rw-   0        0        0     2812 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      244 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.963256 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      266 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    11128 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     3325 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.971338 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-rw-   0        0        0    10678 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-rw-   0        0        0     6741 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-rw-   0        0        0     1866 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-rw-   0        0        0     1079 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-rw-   0        0        0     3709 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-rw-   0        0        0     6181 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     7134 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.987393 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      581 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-   0        0        0    41259 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51697 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20834 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51991 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14811 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     5058 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39801 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    18102 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    66262 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23513 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    43898 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.991401 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distro/
+-rw-rw-rw-   0        0        0      981 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-rw-   0        0        0    49330 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/distro/distro.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.999934 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.004935 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1132 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6079 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    34544 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.017478 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.018486 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   108515 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.027998 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    18003 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4303 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     5706 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2800 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     7448 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     7098 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.049605 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/
+-rw-rw-rw-   0        0        0     2999 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23685 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.051107 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-rw-   0        0        0    40386 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.072148 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-rw-   0        0        0     4800 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4104 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3314 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5086 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35601 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21938 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     4981 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19351 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5073 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2212 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     5014 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7335 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4674 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11753 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    32064 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.076670 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-rw-   0        0        0    11164 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0    71556 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    53572 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0      986 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2591 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-rw-   0        0        0     6882 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6257 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.077672 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-rw-   0        0        0     3419 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-rw-   0        0        0    63187 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-rw-   0        0        0     9110 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.091230 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9171 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213344 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.092731 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23685 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.096744 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-rw-   0        0        0      491 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-rw-   0        0        0    11920 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.099754 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-rw-   0        0        0      546 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-rw-   0        0        0    10927 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.118857 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5178 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21443 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6377 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      575 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     1286 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3823 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    35288 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    33240 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.124357 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.126372 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5871 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1601 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    20511 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4963 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.213290 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/
+-rw-rw-rw-   0        0        0     6090 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-rw-   0        0        0     8478 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2100 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-rw-   0        0        0      265 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-rw-   0        0        0      799 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
+-rw-rw-rw-   0        0        0     9695 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3225 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-rw-   0        0        0     1387 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7063 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-rw-   0        0        0     5472 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-rw-   0        0        0    22820 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1926 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-rw-   0        0        0     2783 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-rw-   0        0        0      890 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-rw-   0        0        0    10368 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-rw-rw-   0        0        0     6906 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-rw-   0        0        0     9842 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-rw-rw-   0        0        0     4509 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-rw-   0        0        0    18224 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-rw-   0        0        0    99195 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-rw-   0        0        0     6630 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-rw-rw-   0        0        0     8082 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-rw-   0        0        0      972 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2501 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-rw-   0        0        0     1683 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2508 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-rw-   0        0        0     9584 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5032 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-rw-rw-   0        0        0     3252 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14007 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-rw-   0        0        0    14273 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-rw-rw-   0        0        0     3667 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-rw-   0        0        0    11903 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-rw-   0        0        0     8198 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-rw-   0        0        0     4970 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-rw-   0        0        0     3396 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-rw-   0        0        0    10574 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-rw-   0        0        0    35852 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-rw-   0        0        0    59706 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-rw-   0        0        0     8165 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11303 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-rw-   0        0        0     1391 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-rw-rw-   0        0        0     4431 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-rw-   0        0        0     4602 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-rw-   0        0        0     2843 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-rw-   0        0        0     1591 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-rw-   0        0        0    24247 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-rw-   0        0        0     4339 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-rw-rw-   0        0        0    27073 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-rw-rw-   0        0        0     1258 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-rw-   0        0        0    35153 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-rw-   0        0        0    39684 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    45525 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-rw-rw-   0        0        0     3777 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-rw-   0        0        0    29604 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-rw-   0        0        0     9169 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-rw-   0        0        0    34549 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.224812 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    20493 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3551 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     2179 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1682 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1562 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     2372 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     8746 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     3086 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2142 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     8024 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.229344 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    84101 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.241872 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20300 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39128 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.249402 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.252904 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11036 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4528 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17081 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34448 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.254904 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.257426 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    30641 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.271961 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     3997 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22003 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10168 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14296 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-rw-   0        0        0      476 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/vendor.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.276981 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:39.691691 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip-23.1.1.dist-info/
+-rw-rw-rw-   0        0        0     9953 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip-23.1.1.dist-info/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1093 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip-23.1.1.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0      125 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip-23.1.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-04-22 17:07:56.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pip-23.1.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.277979 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/
+-rw-rw-rw-   0        0        0   108568 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.281575 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-rw-rw-   0        0        0    24701 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.291095 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.294096 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13515 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.295095 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15526 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.298617 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       83 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   132569 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    18410 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.315138 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8496 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4706 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.326675 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.327673 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-rw-rw-   0        0        0     8425 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.329180 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2426 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.339702 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/
+-rw-rw-rw-   0        0        0      266 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/bdist.py
+-rw-rw-rw-   0        0        0     7415 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/commandline.py
+-rw-rw-rw-   0        0        0     1577 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/develop.py
+-rw-rw-rw-   0        0        0     4627 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/distribution.py
+-rw-rw-rw-   0        0        0      518 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/index.py
+-rw-rw-rw-   0        0        0     2492 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/installed.py
+-rw-rw-rw-   0        0        0     2347 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/sdist.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.353720 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/
+-rw-rw-rw-   0        0        0     1342 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/__init__.py
+-rw-rw-rw-   0        0        0     2279 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_bdist.py
+-rw-rw-rw-   0        0        0    11722 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_commandline.py
+-rw-rw-rw-   0        0        0      831 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_develop.py
+-rw-rw-rw-   0        0        0    19377 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_distribution.py
+-rw-rw-rw-   0        0        0     2636 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_index.py
+-rw-rw-rw-   0        0        0     5460 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_installed.py
+-rw-rw-rw-   0        0        0     5481 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_sdist.py
+-rw-rw-rw-   0        0        0     6835 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_utils.py
+-rw-rw-rw-   0        0        0     4443 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/tests/test_wheel.py
+-rw-rw-rw-   0        0        0     1786 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/utils.py
+-rw-rw-rw-   0        0        0     1586 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo/wheel.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.343201 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo-1.9.6.dist-info/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0       54 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo-1.9.6.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 19:20:57.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pkginfo-1.9.6.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.361737 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy/
+-rw-rw-rw-   0        0        0      489 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy/__init__.py
+-rw-rw-rw-   0        0        0     2097 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy/_callers.py
+-rw-rw-rw-   0        0        0    11496 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy/_hooks.py
+-rw-rw-rw-   0        0        0    14752 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy/_manager.py
+-rw-rw-rw-   0        0        0     1535 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy/_result.py
+-rw-rw-rw-   0        0        0     1541 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy/_tracing.py
+-rw-rw-rw-   0        0        0      142 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.362740 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy-1.0.0.dist-info/
+-rw-rw-rw-   0        0        0        7 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pluggy-1.0.0.dist-info/top_level.txt
+-rw-rw-rw-   0        0        0    82781 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/png.py
+-rw-rw-rw-   0        0        0      263 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/py.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.375265 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/
+-rw-rw-rw-   0        0        0     2815 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/__init__.py
+-rw-rw-rw-   0        0        0    10555 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/_ast_gen.py
+-rw-rw-rw-   0        0        0     1039 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/_build_tables.py
+-rw-rw-rw-   0        0        0     5691 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/ast_transforms.py
+-rw-rw-rw-   0        0        0    31445 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/c_ast.py
+-rw-rw-rw-   0        0        0    17772 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/c_generator.py
+-rw-rw-rw-   0        0        0    17167 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/c_lexer.py
+-rw-rw-rw-   0        0        0    73680 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/c_parser.py
+-rw-rw-rw-   0        0        0     8504 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/lextab.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.384297 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/ply/
+-rw-rw-rw-   0        0        0      102 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/ply/__init__.py
+-rw-rw-rw-   0        0        0    33282 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/ply/cpp.py
+-rw-rw-rw-   0        0        0     3177 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/ply/ctokens.py
+-rw-rw-rw-   0        0        0    42918 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/ply/lex.py
+-rw-rw-rw-   0        0        0   137323 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/ply/yacc.py
+-rw-rw-rw-   0        0        0     2251 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/ply/ygen.py
+-rw-rw-rw-   0        0        0     4875 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/plyparser.py
+-rw-rw-rw-   0        0        0   205652 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser/yacctab.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.376779 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser-2.21.dist-info/
+-rw-rw-rw-   0        0        0       10 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pycparser-2.21.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.401839 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/
+-rw-rw-rw-   0        0        0     2959 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/__init__.py
+-rw-rw-rw-   0        0        0      348 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23530 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.403338 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/filters/
+-rw-rw-rw-   0        0        0    40338 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     4154 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.418380 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/
+-rw-rw-rw-   0        0        0     5388 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4176 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3290 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5070 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35574 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21914 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     4945 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19303 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5025 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2200 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     4990 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7299 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4626 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11717 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    34541 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.663505 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/
+-rw-rw-rw-   0        0        0    12082 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0     1543 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_ada_builtins.py
+-rw-rw-rw-   0        0        0    27287 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_asy_builtins.py
+-rw-rw-rw-   0        0        0    13994 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_cl_builtins.py
+-rw-rw-rw-   0        0        0   105182 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
+-rw-rw-rw-   0        0        0    18414 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_csound_builtins.py
+-rw-rw-rw-   0        0        0    12446 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_css_builtins.py
+-rw-rw-rw-   0        0        0    11883 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_julia_builtins.py
+-rw-rw-rw-   0        0        0   134510 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py
+-rw-rw-rw-   0        0        0   108094 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
+-rw-rw-rw-   0        0        0     8116 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_lua_builtins.py
+-rw-rw-rw-   0        0        0    65633 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    24713 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_mql_builtins.py
+-rw-rw-rw-   0        0        0    25842 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py
+-rw-rw-rw-   0        0        0    49398 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py
+-rw-rw-rw-   0        0        0   107930 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_php_builtins.py
+-rw-rw-rw-   0        0        0    13355 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py
+-rw-rw-rw-   0        0        0    12595 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py
+-rw-rw-rw-   0        0        0    32564 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py
+-rw-rw-rw-   0        0        0    52413 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py
+-rw-rw-rw-   0        0        0    26781 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rw-rw-rw-   0        0        0    13445 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_stan_builtins.py
+-rw-rw-rw-   0        0        0    27227 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_stata_builtins.py
+-rw-rw-rw-   0        0        0    15460 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py
+-rw-rw-rw-   0        0        0     1658 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_usd_builtins.py
+-rw-rw-rw-   0        0        0     4225 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
+-rw-rw-rw-   0        0        0    57066 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/_vim_builtins.py
+-rw-rw-rw-   0        0        0    11676 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/actionscript.py
+-rw-rw-rw-   0        0        0     5320 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ada.py
+-rw-rw-rw-   0        0        0      876 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/agile.py
+-rw-rw-rw-   0        0        0     9873 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/algebra.py
+-rw-rw-rw-   0        0        0     2606 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ambient.py
+-rw-rw-rw-   0        0        0     1670 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/amdgpu.py
+-rw-rw-rw-   0        0        0     4177 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ampl.py
+-rw-rw-rw-   0        0        0    30766 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/apdlexer.py
+-rw-rw-rw-   0        0        0     3405 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/apl.py
+-rw-rw-rw-   0        0        0    11469 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/archetype.py
+-rw-rw-rw-   0        0        0     3565 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/arrow.py
+-rw-rw-rw-   0        0        0    11417 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/arturo.py
+-rw-rw-rw-   0        0        0     1621 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/asc.py
+-rw-rw-rw-   0        0        0    41243 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/asm.py
+-rw-rw-rw-   0        0        0    19815 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/automation.py
+-rw-rw-rw-   0        0        0     3021 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/bare.py
+-rw-rw-rw-   0        0        0    27923 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/basic.py
+-rw-rw-rw-   0        0        0     1652 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/bdd.py
+-rw-rw-rw-   0        0        0     3211 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/berry.py
+-rw-rw-rw-   0        0        0     4723 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/bibtex.py
+-rw-rw-rw-   0        0        0     3915 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/boa.py
+-rw-rw-rw-   0        0        0    28112 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/business.py
+-rw-rw-rw-   0        0        0    17791 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/c_cpp.py
+-rw-rw-rw-   0        0        0    29206 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/c_like.py
+-rw-rw-rw-   0        0        0     2175 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/capnproto.py
+-rw-rw-rw-   0        0        0     3231 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/carbon.py
+-rw-rw-rw-   0        0        0     5182 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/cddl.py
+-rw-rw-rw-   0        0        0     5157 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/chapel.py
+-rw-rw-rw-   0        0        0     6395 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/clean.py
+-rw-rw-rw-   0        0        0     3156 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/comal.py
+-rw-rw-rw-   0        0        0     1407 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/compiled.py
+-rw-rw-rw-   0        0        0    42338 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/configs.py
+-rw-rw-rw-   0        0        0     4148 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/console.py
+-rw-rw-rw-   0        0        0     1390 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/cplint.py
+-rw-rw-rw-   0        0        0    15756 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/crystal.py
+-rw-rw-rw-   0        0        0    16994 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/csound.py
+-rw-rw-rw-   0        0        0    25322 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/css.py
+-rw-rw-rw-   0        0        0     9875 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/d.py
+-rw-rw-rw-   0        0        0     4607 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/dalvik.py
+-rw-rw-rw-   0        0        0    26940 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/data.py
+-rw-rw-rw-   0        0        0     8099 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/dax.py
+-rw-rw-rw-   0        0        0     4020 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/devicetree.py
+-rw-rw-rw-   0        0        0     5278 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/diff.py
+-rw-rw-rw-   0        0        0    37623 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/dotnet.py
+-rw-rw-rw-   0        0        0    36774 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/dsls.py
+-rw-rw-rw-   0        0        0    10380 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/dylan.py
+-rw-rw-rw-   0        0        0     6372 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ecl.py
+-rw-rw-rw-   0        0        0     2690 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/eiffel.py
+-rw-rw-rw-   0        0        0     3152 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/elm.py
+-rw-rw-rw-   0        0        0     6370 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/elpi.py
+-rw-rw-rw-   0        0        0     4742 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/email.py
+-rw-rw-rw-   0        0        0    19170 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/erlang.py
+-rw-rw-rw-   0        0        0    10396 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/esoteric.py
+-rw-rw-rw-   0        0        0     3273 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ezhil.py
+-rw-rw-rw-   0        0        0    19531 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/factor.py
+-rw-rw-rw-   0        0        0    10197 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/fantom.py
+-rw-rw-rw-   0        0        0     9646 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/felix.py
+-rw-rw-rw-   0        0        0     1621 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/fift.py
+-rw-rw-rw-   0        0        0     2668 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/floscript.py
+-rw-rw-rw-   0        0        0     7194 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/forth.py
+-rw-rw-rw-   0        0        0    10336 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/fortran.py
+-rw-rw-rw-   0        0        0    26212 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/foxpro.py
+-rw-rw-rw-   0        0        0    26914 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/freefem.py
+-rw-rw-rw-   0        0        0     3622 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/func.py
+-rw-rw-rw-   0        0        0      674 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/functional.py
+-rw-rw-rw-   0        0        0     3732 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/futhark.py
+-rw-rw-rw-   0        0        0      826 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/gcodelexer.py
+-rw-rw-rw-   0        0        0     7543 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/gdscript.py
+-rw-rw-rw-   0        0        0     3761 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/go.py
+-rw-rw-rw-   0        0        0     7980 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/grammar_notation.py
+-rw-rw-rw-   0        0        0     3861 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/graph.py
+-rw-rw-rw-   0        0        0    39026 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/graphics.py
+-rw-rw-rw-   0        0        0     1935 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/graphviz.py
+-rw-rw-rw-   0        0        0     3991 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/gsql.py
+-rw-rw-rw-   0        0        0    32898 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/haskell.py
+-rw-rw-rw-   0        0        0    30976 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/haxe.py
+-rw-rw-rw-   0        0        0    22520 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/hdl.py
+-rw-rw-rw-   0        0        0     3603 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/hexdump.py
+-rw-rw-rw-   0        0        0    19879 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/html.py
+-rw-rw-rw-   0        0        0    15450 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/idl.py
+-rw-rw-rw-   0        0        0    30631 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/igor.py
+-rw-rw-rw-   0        0        0     3136 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/inferno.py
+-rw-rw-rw-   0        0        0    13178 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/installers.py
+-rw-rw-rw-   0        0        0    57119 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/int_fiction.py
+-rw-rw-rw-   0        0        0     1906 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/iolang.py
+-rw-rw-rw-   0        0        0     4854 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/j.py
+-rw-rw-rw-   0        0        0    62859 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/javascript.py
+-rw-rw-rw-   0        0        0     2059 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/jmespath.py
+-rw-rw-rw-   0        0        0     3701 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/jslt.py
+-rw-rw-rw-   0        0        0     5635 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/jsonnet.py
+-rw-rw-rw-   0        0        0    11646 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/julia.py
+-rw-rw-rw-   0        0        0    72929 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/jvm.py
+-rw-rw-rw-   0        0        0    11406 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/kuin.py
+-rw-rw-rw-   0        0        0     9753 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/lilypond.py
+-rw-rw-rw-   0        0        0   144039 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/lisp.py
+-rw-rw-rw-   0        0        0    31914 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/macaulay2.py
+-rw-rw-rw-   0        0        0     7618 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/make.py
+-rw-rw-rw-   0        0        0    58129 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/markup.py
+-rw-rw-rw-   0        0        0      676 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/math.py
+-rw-rw-rw-   0        0        0   132852 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/matlab.py
+-rw-rw-rw-   0        0        0     2716 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/maxima.py
+-rw-rw-rw-   0        0        0     4337 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/meson.py
+-rw-rw-rw-   0        0        0     7538 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/mime.py
+-rw-rw-rw-   0        0        0    13846 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/minecraft.py
+-rw-rw-rw-   0        0        0     4604 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/mips.py
+-rw-rw-rw-   0        0        0    35324 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ml.py
+-rw-rw-rw-   0        0        0    13524 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/modeling.py
+-rw-rw-rw-   0        0        0    53073 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/modula2.py
+-rw-rw-rw-   0        0        0     6290 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/monte.py
+-rw-rw-rw-   0        0        0     9187 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/mosel.py
+-rw-rw-rw-   0        0        0    63962 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ncl.py
+-rw-rw-rw-   0        0        0     6416 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/nimrod.py
+-rw-rw-rw-   0        0        0     2726 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/nit.py
+-rw-rw-rw-   0        0        0     4015 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/nix.py
+-rw-rw-rw-   0        0        0     4169 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/oberon.py
+-rw-rw-rw-   0        0        0    22961 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/objective.py
+-rw-rw-rw-   0        0        0     2982 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ooc.py
+-rw-rw-rw-   0        0        0     1744 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/other.py
+-rw-rw-rw-   0        0        0     2720 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/parasail.py
+-rw-rw-rw-   0        0        0    25904 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/parsers.py
+-rw-rw-rw-   0        0        0    30880 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/pascal.py
+-rw-rw-rw-   0        0        0     8146 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/pawn.py
+-rw-rw-rw-   0        0        0    39170 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/perl.py
+-rw-rw-rw-   0        0        0    23252 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/phix.py
+-rw-rw-rw-   0        0        0    13040 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/php.py
+-rw-rw-rw-   0        0        0     1975 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/pointless.py
+-rw-rw-rw-   0        0        0     3244 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/pony.py
+-rw-rw-rw-   0        0        0    12677 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/praat.py
+-rw-rw-rw-   0        0        0     1156 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/procfile.py
+-rw-rw-rw-   0        0        0    12351 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/prolog.py
+-rw-rw-rw-   0        0        0     4715 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/promql.py
+-rw-rw-rw-   0        0        0    53376 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0     6932 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/q.py
+-rw-rw-rw-   0        0        0     3665 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/qlik.py
+-rw-rw-rw-   0        0        0     6072 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/qvt.py
+-rw-rw-rw-   0        0        0     6185 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/r.py
+-rw-rw-rw-   0        0        0    15790 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/rdf.py
+-rw-rw-rw-   0        0        0    18248 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/rebol.py
+-rw-rw-rw-   0        0        0     2902 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/resource.py
+-rw-rw-rw-   0        0        0     5056 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ride.py
+-rw-rw-rw-   0        0        0     1128 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/rita.py
+-rw-rw-rw-   0        0        0     1973 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/rnc.py
+-rw-rw-rw-   0        0        0     1962 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/roboconf.py
+-rw-rw-rw-   0        0        0    18449 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/robotframework.py
+-rw-rw-rw-   0        0        0    22775 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ruby.py
+-rw-rw-rw-   0        0        0     8216 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/rust.py
+-rw-rw-rw-   0        0        0     9400 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/sas.py
+-rw-rw-rw-   0        0        0     4645 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/savi.py
+-rw-rw-rw-   0        0        0     2239 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/scdoc.py
+-rw-rw-rw-   0        0        0    70014 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/scripting.py
+-rw-rw-rw-   0        0        0     1986 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/sgf.py
+-rw-rw-rw-   0        0        0    36466 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/shell.py
+-rw-rw-rw-   0        0        0     2441 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/sieve.py
+-rw-rw-rw-   0        0        0     8482 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/slash.py
+-rw-rw-rw-   0        0        0     7206 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/smalltalk.py
+-rw-rw-rw-   0        0        0     2660 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/smithy.py
+-rw-rw-rw-   0        0        0     2773 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/smv.py
+-rw-rw-rw-   0        0        0     2732 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/snobol.py
+-rw-rw-rw-   0        0        0     3127 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/solidity.py
+-rw-rw-rw-   0        0        0     3330 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/sophia.py
+-rw-rw-rw-   0        0        0     3414 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/special.py
+-rw-rw-rw-   0        0        0     2733 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/spice.py
+-rw-rw-rw-   0        0        0    42086 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/sql.py
+-rw-rw-rw-   0        0        0     1693 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/srcinfo.py
+-rw-rw-rw-   0        0        0     6416 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/stata.py
+-rw-rw-rw-   0        0        0     3698 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/supercollider.py
+-rw-rw-rw-   0        0        0     2639 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/tal.py
+-rw-rw-rw-   0        0        0     5513 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/tcl.py
+-rw-rw-rw-   0        0        0     3523 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/teal.py
+-rw-rw-rw-   0        0        0    72610 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/templates.py
+-rw-rw-rw-   0        0        0     9719 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/teraterm.py
+-rw-rw-rw-   0        0        0    10767 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/testing.py
+-rw-rw-rw-   0        0        0     1029 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/text.py
+-rw-rw-rw-   0        0        0     7609 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/textedit.py
+-rw-rw-rw-   0        0        0    15192 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/textfmts.py
+-rw-rw-rw-   0        0        0    20157 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/theorem.py
+-rw-rw-rw-   0        0        0     4228 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/thingsdb.py
+-rw-rw-rw-   0        0        0     1377 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/tlb.py
+-rw-rw-rw-   0        0        0    10457 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/tnt.py
+-rw-rw-rw-   0        0        0     1474 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/trafficscript.py
+-rw-rw-rw-   0        0        0     8207 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/typoscript.py
+-rw-rw-rw-   0        0        0     8956 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/ul4.py
+-rw-rw-rw-   0        0        0    18512 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/unicon.py
+-rw-rw-rw-   0        0        0     6037 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/urbi.py
+-rw-rw-rw-   0        0        0     3513 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/usd.py
+-rw-rw-rw-   0        0        0     7273 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/varnish.py
+-rw-rw-rw-   0        0        0     3885 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/verification.py
+-rw-rw-rw-   0        0        0      894 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/web.py
+-rw-rw-rw-   0        0        0     5699 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/webassembly.py
+-rw-rw-rw-   0        0        0    10517 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/webidl.py
+-rw-rw-rw-   0        0        0    40549 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/webmisc.py
+-rw-rw-rw-   0        0        0    11920 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/wgsl.py
+-rw-rw-rw-   0        0        0     4018 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/whiley.py
+-rw-rw-rw-   0        0        0     4021 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/wowtoc.py
+-rw-rw-rw-   0        0        0     3239 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/wren.py
+-rw-rw-rw-   0        0        0     1920 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/x10.py
+-rw-rw-rw-   0        0        0      902 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/xorg.py
+-rw-rw-rw-   0        0        0     4500 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/yang.py
+-rw-rw-rw-   0        0        0     3953 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/lexers/zig.py
+-rw-rw-rw-   0        0        0      986 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2579 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/scanner.py
+-rw-rw-rw-   0        0        0     6816 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6245 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.716143 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/
+-rw-rw-rw-   0        0        0     3676 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0      705 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/abap.py
+-rw-rw-rw-   0        0        0     2216 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/algol.py
+-rw-rw-rw-   0        0        0     2231 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/algol_nu.py
+-rw-rw-rw-   0        0        0     4443 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/arduino.py
+-rw-rw-rw-   0        0        0     2096 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/autumn.py
+-rw-rw-rw-   0        0        0     1514 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/borland.py
+-rw-rw-rw-   0        0        0     1308 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/bw.py
+-rw-rw-rw-   0        0        0     2730 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/colorful.py
+-rw-rw-rw-   0        0        0     2488 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/default.py
+-rw-rw-rw-   0        0        0     3314 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/dracula.py
+-rw-rw-rw-   0        0        0     2439 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/emacs.py
+-rw-rw-rw-   0        0        0     2502 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/friendly.py
+-rw-rw-rw-   0        0        0     2707 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/friendly_grayscale.py
+-rw-rw-rw-   0        0        0     1274 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/fruity.py
+-rw-rw-rw-   0        0        0     3481 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/gh_dark.py
+-rw-rw-rw-   0        0        0     3230 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/gruvbox.py
+-rw-rw-rw-   0        0        0      692 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/igor.py
+-rw-rw-rw-   0        0        0     2302 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/inkpot.py
+-rw-rw-rw-   0        0        0     2016 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/lilypond.py
+-rw-rw-rw-   0        0        0     3117 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/lovelace.py
+-rw-rw-rw-   0        0        0     2350 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/manni.py
+-rw-rw-rw-   0        0        0     4083 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/material.py
+-rw-rw-rw-   0        0        0     5063 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/monokai.py
+-rw-rw-rw-   0        0        0     2703 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/murphy.py
+-rw-rw-rw-   0        0        0     1948 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/native.py
+-rw-rw-rw-   0        0        0     5244 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/nord.py
+-rw-rw-rw-   0        0        0     1664 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/onedark.py
+-rw-rw-rw-   0        0        0     5526 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/paraiso_dark.py
+-rw-rw-rw-   0        0        0     5530 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/paraiso_light.py
+-rw-rw-rw-   0        0        0     2425 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/pastie.py
+-rw-rw-rw-   0        0        0     2128 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/perldoc.py
+-rw-rw-rw-   0        0        0     2432 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/rainbow_dash.py
+-rw-rw-rw-   0        0        0      874 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/rrt.py
+-rw-rw-rw-   0        0        0     1393 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/sas.py
+-rw-rw-rw-   0        0        0     4078 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/solarized.py
+-rw-rw-rw-   0        0        0      770 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/staroffice.py
+-rw-rw-rw-   0        0        0     1198 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/stata_dark.py
+-rw-rw-rw-   0        0        0     1227 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/stata_light.py
+-rw-rw-rw-   0        0        0     7039 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/tango.py
+-rw-rw-rw-   0        0        0     1885 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/trac.py
+-rw-rw-rw-   0        0        0     1922 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/vim.py
+-rw-rw-rw-   0        0        0     1026 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/vs.py
+-rw-rw-rw-   0        0        0     1453 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/xcode.py
+-rw-rw-rw-   0        0        0     2148 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/styles/zenburn.py
+-rw-rw-rw-   0        0        0     6184 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/token.py
+-rw-rw-rw-   0        0        0    63223 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/unistring.py
+-rw-rw-rw-   0        0        0    10230 2023-05-09 19:20:55.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.718152 whatsappy-py-4.0.0/.venv/Lib/site-packages/pypng-0.20220715.0.dist-info/
+-rw-rw-rw-   0        0        0        4 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pypng-0.20220715.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.722161 whatsappy-py-4.0.0/.venv/Lib/site-packages/pyproject_hooks/
+-rw-rw-rw-   0        0        0      491 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pyproject_hooks/__init__.py
+-rw-rw-rw-   0        0        0      121 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pyproject_hooks/_compat.py
+-rw-rw-rw-   0        0        0    11920 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pyproject_hooks/_impl.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.725162 whatsappy-py-4.0.0/.venv/Lib/site-packages/pyproject_hooks/_in_process/
+-rw-rw-rw-   0        0        0      546 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
+-rw-rw-rw-   0        0        0    10927 2023-05-09 19:23:59.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.728184 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytest/
+-rw-rw-rw-   0        0        0     5163 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytest/__init__.py
+-rw-rw-rw-   0        0        0      116 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytest/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.731184 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytest-7.3.1.dist-info/
+-rw-rw-rw-   0        0        0       77 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytest-7.3.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-04-22 16:57:52.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytest-7.3.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.732685 whatsappy-py-4.0.0/.venv/Lib/site-packages/python_dateutil-2.8.2.dist-info/
+-rw-rw-rw-   0        0        0        9 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/python_dateutil-2.8.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.735186 whatsappy-py-4.0.0/.venv/Lib/site-packages/python_dotenv-1.0.0.dist-info/
+-rw-rw-rw-   0        0        0       47 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/python_dotenv-1.0.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/python_dotenv-1.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.743212 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz/
+-rw-rw-rw-   0        0        0    35101 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz/__init__.py
+-rw-rw-rw-   0        0        0     1571 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz/exceptions.py
+-rw-rw-rw-   0        0        0     5404 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz/lazy.py
+-rw-rw-rw-   0        0        0     3778 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz/reference.py
+-rw-rw-rw-   0        0        0     4723 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz/tzfile.py
+-rw-rw-rw-   0        0        0    19272 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz/tzinfo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.745213 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz-2023.3.dist-info/
+-rw-rw-rw-   0        0        0     1088 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz-2023.3.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0        5 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pytz-2023.3.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.748744 whatsappy-py-4.0.0/.venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/
+-rw-rw-rw-   0        0        0     1644 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0       12 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.760261 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/
+-rw-rw-rw-   0        0        0     3599 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/LUT.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/__init__.py
+-rw-rw-rw-   0        0        0     7288 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/base.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.765262 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/compat/
+-rw-rw-rw-   0        0        0        0 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/compat/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/compat/etree.py
+-rw-rw-rw-   0        0        0      362 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/compat/pil.py
+-rw-rw-rw-   0        0        0     5571 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/console_scripts.py
+-rw-rw-rw-   0        0        0      106 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/constants.py
+-rw-rw-rw-   0        0        0       45 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.772787 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/
+-rw-rw-rw-   0        0        0        0 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/__init__.py
+-rw-rw-rw-   0        0        0     4984 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/base.py
+-rw-rw-rw-   0        0        0     1524 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/pil.py
+-rw-rw-rw-   0        0        0     1412 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/pure.py
+-rw-rw-rw-   0        0        0     4477 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styledpil.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.774788 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styles/
+-rw-rw-rw-   0        0        0        0 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styles/__init__.py
+-rw-rw-rw-   0        0        0     7601 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styles/colormasks.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.779310 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styles/moduledrawers/
+-rw-rw-rw-   0        0        0      430 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styles/moduledrawers/__init__.py
+-rw-rw-rw-   0        0        0     1067 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styles/moduledrawers/base.py
+-rw-rw-rw-   0        0        0     9852 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styles/moduledrawers/pil.py
+-rw-rw-rw-   0        0        0     3952 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/styles/moduledrawers/svg.py
+-rw-rw-rw-   0        0        0     5246 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/image/svg.py
+-rw-rw-rw-   0        0        0    16462 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/main.py
+-rw-rw-rw-   0        0        0     1079 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/release.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.786845 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/tests/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/tests/test_example.py
+-rw-rw-rw-   0        0        0    17398 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/tests/test_qrcode.py
+-rw-rw-rw-   0        0        0     1644 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/tests/test_qrcode_svg.py
+-rw-rw-rw-   0        0        0     1468 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/tests/test_release.py
+-rw-rw-rw-   0        0        0     3807 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/tests/test_script.py
+-rw-rw-rw-   0        0        0      277 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/tests/test_util.py
+-rw-rw-rw-   0        0        0    17128 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.762761 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode-7.4.2.dist-info/
+-rw-rw-rw-   0        0        0       51 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode-7.4.2.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/qrcode-7.4.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.794349 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer/
+-rw-rw-rw-   0        0        0     1119 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer/__about__.py
+-rw-rw-rw-   0        0        0      573 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer/__main__.py
+-rw-rw-rw-   0        0        0     4290 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer/clean.py
+-rw-rw-rw-   0        0        0     3595 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer/markdown.py
+-rw-rw-rw-   0        0        0     4460 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer/rst.py
+-rw-rw-rw-   0        0        0      823 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer/txt.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.795354 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer-37.3.dist-info/
+-rw-rw-rw-   0        0        0       16 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/readme_renderer-37.3.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.800366 whatsappy-py-4.0.0/.venv/Lib/site-packages/regex/
+-rw-rw-rw-   0        0        0       68 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/regex/__init__.py
+-rw-rw-rw-   0        0        0   145648 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/regex/_regex_core.py
+-rw-rw-rw-   0        0        0    33561 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/regex/regex.py
+-rw-rw-rw-   0        0        0   224004 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/regex/test_regex.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.803864 whatsappy-py-4.0.0/.venv/Lib/site-packages/regex-2023.5.5.dist-info/
+-rw-rw-rw-   0        0        0    11792 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/regex-2023.5.5.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 17:01:14.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/regex-2023.5.5.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.823908 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/
+-rw-rw-rw-   0        0        0     4972 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/__version__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21287 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/adapters.py
+-rw-rw-rw-   0        0        0     6377 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/auth.py
+-rw-rw-rw-   0        0        0      429 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/certs.py
+-rw-rw-rw-   0        0        0     1451 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/cookies.py
+-rw-rw-rw-   0        0        0     3811 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3875 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/hooks.py
+-rw-rw-rw-   0        0        0    35223 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/models.py
+-rw-rw-rw-   0        0        0      957 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/structures.py
+-rw-rw-rw-   0        0        0    33228 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.824908 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests-2.28.2.dist-info/
+-rw-rw-rw-   0        0        0        9 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests-2.28.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.830940 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/
+-rw-rw-rw-   0        0        0     1188 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/__init__.py
+-rw-rw-rw-   0        0        0     9260 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/_compat.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.841962 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/
+-rw-rw-rw-   0        0        0      370 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/__init__.py
+-rw-rw-rw-   0        0        0     7539 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py
+-rw-rw-rw-   0        0        0     1404 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
+-rw-rw-rw-   0        0        0     1396 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
+-rw-rw-rw-   0        0        0     4789 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
+-rw-rw-rw-   0        0        0     2608 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/source.py
+-rw-rw-rw-   0        0        0     2399 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py
+-rw-rw-rw-   0        0        0     7854 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/adapters/x509.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.847982 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/auth/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/auth/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
+-rw-rw-rw-   0        0        0     4944 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/auth/guess.py
+-rw-rw-rw-   0        0        0     4407 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/auth/handler.py
+-rw-rw-rw-   0        0        0     3706 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.849983 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/cookies/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/cookies/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.853482 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/downloadutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
+-rw-rw-rw-   0        0        0     6024 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
+-rw-rw-rw-   0        0        0     4365 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
+-rw-rw-rw-   0        0        0      695 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.856998 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/multipart/
+-rw-rw-rw-   0        0        0      854 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py
+-rw-rw-rw-   0        0        0     4861 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py
+-rw-rw-rw-   0        0        0    20769 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py
+-rw-rw-rw-   0        0        0     3102 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/sessions.py
+-rw-rw-rw-   0        0        0     4044 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.860506 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/threaded/
+-rw-rw-rw-   0        0        0     3213 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py
+-rw-rw-rw-   0        0        0     6628 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/threaded/pool.py
+-rw-rw-rw-   0        0        0     1465 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/threaded/thread.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.866011 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2558 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py
+-rw-rw-rw-   0        0        0     6522 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/utils/dump.py
+-rw-rw-rw-   0        0        0     3233 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/utils/formdata.py
+-rw-rw-rw-   0        0        0     4524 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.831945 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/
+-rw-rw-rw-   0        0        0       18 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.880551 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/
+-rw-rw-rw-   0        0        0     1565 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/__init__.py
+-rw-rw-rw-   0        0        0    13297 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/_mixin.py
+-rw-rw-rw-   0        0        0     9048 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/abnf_regexp.py
+-rw-rw-rw-   0        0        0     3862 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/api.py
+-rw-rw-rw-   0        0        0    12709 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/builder.py
+-rw-rw-rw-   0        0        0     1620 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/compat.py
+-rw-rw-rw-   0        0        0     3614 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/exceptions.py
+-rw-rw-rw-   0        0        0     5477 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/iri.py
+-rw-rw-rw-   0        0        0     4114 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/misc.py
+-rw-rw-rw-   0        0        0     5261 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/normalizers.py
+-rw-rw-rw-   0        0        0    14599 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/parseresult.py
+-rw-rw-rw-   0        0        0     5183 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/uri.py
+-rw-rw-rw-   0        0        0    13676 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.881545 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/
+-rw-rw-rw-   0        0        0        8 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.972758 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/
+-rw-rw-rw-   0        0        0     6066 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/__init__.py
+-rw-rw-rw-   0        0        0     8334 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2100 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_export_format.py
+-rw-rw-rw-   0        0        0      241 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_extension.py
+-rw-rw-rw-   0        0        0      799 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_fileno.py
+-rw-rw-rw-   0        0        0     9695 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3213 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_loop.py
+-rw-rw-rw-   0        0        0     1387 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7063 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_pick.py
+-rw-rw-rw-   0        0        0     5460 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_timer.py
+-rw-rw-rw-   0        0        0    22784 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1902 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_windows.py
+-rw-rw-rw-   0        0        0     2759 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/_wrap.py
+-rw-rw-rw-   0        0        0      878 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/abc.py
+-rw-rw-rw-   0        0        0    10320 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/align.py
+-rw-rw-rw-   0        0        0     6906 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/bar.py
+-rw-rw-rw-   0        0        0     9794 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/box.py
+-rw-rw-rw-   0        0        0     4509 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/cells.py
+-rw-rw-rw-   0        0        0    18224 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/columns.py
+-rw-rw-rw-   0        0        0    99146 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/containers.py
+-rw-rw-rw-   0        0        0     6606 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/control.py
+-rw-rw-rw-   0        0        0     8046 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/default_styles.py
+-rw-rw-rw-   0        0        0      924 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2465 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/errors.py
+-rw-rw-rw-   0        0        0     1683 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2508 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/filesize.py
+-rw-rw-rw-   0        0        0     9584 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5020 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/json.py
+-rw-rw-rw-   0        0        0     3228 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/jupyter.py
+-rw-rw-rw-   0        0        0    13947 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/layout.py
+-rw-rw-rw-   0        0        0    14273 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/live.py
+-rw-rw-rw-   0        0        0     3655 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/live_render.py
+-rw-rw-rw-   0        0        0    11891 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/logging.py
+-rw-rw-rw-   0        0        0    22368 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/markdown.py
+-rw-rw-rw-   0        0        0     8174 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/measure.py
+-rw-rw-rw-   0        0        0     4958 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/pager.py
+-rw-rw-rw-   0        0        0     3288 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/palette.py
+-rw-rw-rw-   0        0        0    10574 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/panel.py
+-rw-rw-rw-   0        0        0    35816 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/pretty.py
+-rw-rw-rw-   0        0        0    59694 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/progress.py
+-rw-rw-rw-   0        0        0     8165 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11291 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/prompt.py
+-rw-rw-rw-   0        0        0     1367 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/region.py
+-rw-rw-rw-   0        0        0     4419 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/repr.py
+-rw-rw-rw-   0        0        0     4590 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/rule.py
+-rw-rw-rw-   0        0        0     2831 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/scope.py
+-rw-rw-rw-   0        0        0     1579 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/screen.py
+-rw-rw-rw-   0        0        0    24211 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/segment.py
+-rw-rw-rw-   0        0        0     4339 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/status.py
+-rw-rw-rw-   0        0        0    27073 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/style.py
+-rw-rw-rw-   0        0        0     1234 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/styled.py
+-rw-rw-rw-   0        0        0    35065 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/syntax.py
+-rw-rw-rw-   0        0        0    39648 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    45513 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/text.py
+-rw-rw-rw-   0        0        0     3777 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/themes.py
+-rw-rw-rw-   0        0        0    29532 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/traceback.py
+-rw-rw-rw-   0        0        0     9109 2023-05-09 19:21:00.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/rich/tree.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.974758 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/
+-rw-rw-rw-   0        0        0      811 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.976771 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/common/
+-rw-rw-rw-   0        0        0     3546 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/common/__init__.py
+-rw-rw-rw-   0        0        0     8865 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/common/exceptions.py
+-rw-rw-rw-   0        0        0     1010 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/types.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.978284 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/
+-rw-rw-rw-   0        0        0     2415 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.982789 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chrome/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chrome/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chrome/options.py
+-rw-rw-rw-   0        0        0     2169 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chrome/service.py
+-rw-rw-rw-   0        0        0     3997 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chrome/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:40.988315 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chromium/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chromium/__init__.py
+-rw-rw-rw-   0        0        0     7362 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chromium/options.py
+-rw-rw-rw-   0        0        0     2604 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chromium/remote_connection.py
+-rw-rw-rw-   0        0        0     2417 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chromium/service.py
+-rw-rw-rw-   0        0        0     9392 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/chromium/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.008459 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/__init__.py
+-rw-rw-rw-   0        0        0    12955 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/action_chains.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.019983 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/__init__.py
+-rw-rw-rw-   0        0        0     3500 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/action_builder.py
+-rw-rw-rw-   0        0        0     1184 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/input_device.py
+-rw-rw-rw-   0        0        0     1438 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/interaction.py
+-rw-rw-rw-   0        0        0     1786 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/key_actions.py
+-rw-rw-rw-   0        0        0     1804 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/key_input.py
+-rw-rw-rw-   0        0        0      879 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/mouse_button.py
+-rw-rw-rw-   0        0        0     5850 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/pointer_actions.py
+-rw-rw-rw-   0        0        0     2982 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/pointer_input.py
+-rw-rw-rw-   0        0        0     1331 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/wheel_actions.py
+-rw-rw-rw-   0        0        0     2610 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/actions/wheel_input.py
+-rw-rw-rw-   0        0        0     2512 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/alert.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.022981 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/bidi/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/bidi/__init__.py
+-rw-rw-rw-   0        0        0    17766 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/bidi/cdp.py
+-rw-rw-rw-   0        0        0      885 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/bidi/console.py
+-rw-rw-rw-   0        0        0     1091 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/by.py
+-rw-rw-rw-   0        0        0     2925 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/desired_capabilities.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:38.810355 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.078130 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/
+-rw-rw-rw-   0        0        0     1293 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/__init__.py
+-rw-rw-rw-   0        0        0    22199 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/accessibility.py
+-rw-rw-rw-   0        0        0    11112 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/animation.py
+-rw-rw-rw-   0        0        0    48312 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/audits.py
+-rw-rw-rw-   0        0        0     5919 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/background_service.py
+-rw-rw-rw-   0        0        0    20794 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/browser.py
+-rw-rw-rw-   0        0        0     8286 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/cache_storage.py
+-rw-rw-rw-   0        0        0     4382 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/cast.py
+-rw-rw-rw-   0        0        0     2765 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/console.py
+-rw-rw-rw-   0        0        0    59547 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/css.py
+-rw-rw-rw-   0        0        0     3925 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/database.py
+-rw-rw-rw-   0        0        0    49095 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/debugger.py
+-rw-rw-rw-   0        0        0     1209 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/device_orientation.py
+-rw-rw-rw-   0        0        0    61726 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/dom.py
+-rw-rw-rw-   0        0        0     9459 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/dom_debugger.py
+-rw-rw-rw-   0        0        0    36732 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/dom_snapshot.py
+-rw-rw-rw-   0        0        0     5765 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/dom_storage.py
+-rw-rw-rw-   0        0        0    25819 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/emulation.py
+-rw-rw-rw-   0        0        0     1289 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/event_breakpoints.py
+-rw-rw-rw-   0        0        0    19105 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/fetch.py
+-rw-rw-rw-   0        0        0     4576 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/headless_experimental.py
+-rw-rw-rw-   0        0        0    13806 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/heap_profiler.py
+-rw-rw-rw-   0        0        0    15159 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/indexed_db.py
+-rw-rw-rw-   0        0        0    27841 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/input_.py
+-rw-rw-rw-   0        0        0     1718 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/inspector.py
+-rw-rw-rw-   0        0        0     3036 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/io.py
+-rw-rw-rw-   0        0        0    15049 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/layer_tree.py
+-rw-rw-rw-   0        0        0     5264 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/log.py
+-rw-rw-rw-   0        0        0     7627 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/media.py
+-rw-rw-rw-   0        0        0     6808 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/memory.py
+-rw-rw-rw-   0        0        0   126116 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/network.py
+-rw-rw-rw-   0        0        0    50256 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/overlay.py
+-rw-rw-rw-   0        0        0   107219 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/page.py
+-rw-rw-rw-   0        0        0     2927 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/performance.py
+-rw-rw-rw-   0        0        0     6623 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/performance_timeline.py
+-rw-rw-rw-   0        0        0    12930 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/profiler.py
+-rw-rw-rw-   0        0        0    57994 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/runtime.py
+-rw-rw-rw-   0        0        0     1111 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/schema.py
+-rw-rw-rw-   0        0        0    16861 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/security.py
+-rw-rw-rw-   0        0        0    11066 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/service_worker.py
+-rw-rw-rw-   0        0        0    31381 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/storage.py
+-rw-rw-rw-   0        0        0    11517 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/system_info.py
+-rw-rw-rw-   0        0        0    23888 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/target.py
+-rw-rw-rw-   0        0        0     1538 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/tethering.py
+-rw-rw-rw-   0        0        0    12886 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/tracing.py
+-rw-rw-rw-   0        0        0      455 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/util.py
+-rw-rw-rw-   0        0        0    16895 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/web_audio.py
+-rw-rw-rw-   0        0        0    15154 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v110/web_authn.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.132760 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/
+-rw-rw-rw-   0        0        0     1293 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/__init__.py
+-rw-rw-rw-   0        0        0    22199 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/accessibility.py
+-rw-rw-rw-   0        0        0    11112 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/animation.py
+-rw-rw-rw-   0        0        0    48898 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/audits.py
+-rw-rw-rw-   0        0        0     5919 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/background_service.py
+-rw-rw-rw-   0        0        0    20861 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/browser.py
+-rw-rw-rw-   0        0        0     8286 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/cache_storage.py
+-rw-rw-rw-   0        0        0     4382 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/cast.py
+-rw-rw-rw-   0        0        0     2765 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/console.py
+-rw-rw-rw-   0        0        0    59547 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/css.py
+-rw-rw-rw-   0        0        0     3925 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/database.py
+-rw-rw-rw-   0        0        0    49095 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/debugger.py
+-rw-rw-rw-   0        0        0     1209 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/device_orientation.py
+-rw-rw-rw-   0        0        0    61726 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/dom.py
+-rw-rw-rw-   0        0        0     9459 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/dom_debugger.py
+-rw-rw-rw-   0        0        0    36732 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/dom_snapshot.py
+-rw-rw-rw-   0        0        0     5765 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/dom_storage.py
+-rw-rw-rw-   0        0        0    25913 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/emulation.py
+-rw-rw-rw-   0        0        0     1289 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/event_breakpoints.py
+-rw-rw-rw-   0        0        0    19105 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/fetch.py
+-rw-rw-rw-   0        0        0     4576 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/headless_experimental.py
+-rw-rw-rw-   0        0        0    13806 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/heap_profiler.py
+-rw-rw-rw-   0        0        0    15159 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/indexed_db.py
+-rw-rw-rw-   0        0        0    27841 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/input_.py
+-rw-rw-rw-   0        0        0     1718 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/inspector.py
+-rw-rw-rw-   0        0        0     3036 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/io.py
+-rw-rw-rw-   0        0        0    15049 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/layer_tree.py
+-rw-rw-rw-   0        0        0     5264 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/log.py
+-rw-rw-rw-   0        0        0     7627 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/media.py
+-rw-rw-rw-   0        0        0     6808 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/memory.py
+-rw-rw-rw-   0        0        0   126787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/network.py
+-rw-rw-rw-   0        0        0    50256 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/overlay.py
+-rw-rw-rw-   0        0        0   107897 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/page.py
+-rw-rw-rw-   0        0        0     2927 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/performance.py
+-rw-rw-rw-   0        0        0     6623 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/performance_timeline.py
+-rw-rw-rw-   0        0        0    12930 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/profiler.py
+-rw-rw-rw-   0        0        0    58743 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/runtime.py
+-rw-rw-rw-   0        0        0     1111 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/schema.py
+-rw-rw-rw-   0        0        0    16861 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/security.py
+-rw-rw-rw-   0        0        0    11066 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/service_worker.py
+-rw-rw-rw-   0        0        0    31857 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/storage.py
+-rw-rw-rw-   0        0        0    11517 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/system_info.py
+-rw-rw-rw-   0        0        0    24094 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/target.py
+-rw-rw-rw-   0        0        0     1538 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/tethering.py
+-rw-rw-rw-   0        0        0    12886 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/tracing.py
+-rw-rw-rw-   0        0        0      455 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/util.py
+-rw-rw-rw-   0        0        0    16895 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/web_audio.py
+-rw-rw-rw-   0        0        0    15500 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v111/web_authn.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.191972 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/
+-rw-rw-rw-   0        0        0     1343 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/__init__.py
+-rw-rw-rw-   0        0        0    22200 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/accessibility.py
+-rw-rw-rw-   0        0        0    11112 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/animation.py
+-rw-rw-rw-   0        0        0    45147 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/audits.py
+-rw-rw-rw-   0        0        0     5919 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/background_service.py
+-rw-rw-rw-   0        0        0    20861 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/browser.py
+-rw-rw-rw-   0        0        0     8286 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/cache_storage.py
+-rw-rw-rw-   0        0        0     4382 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/cast.py
+-rw-rw-rw-   0        0        0     2765 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/console.py
+-rw-rw-rw-   0        0        0    59551 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/css.py
+-rw-rw-rw-   0        0        0     3925 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/database.py
+-rw-rw-rw-   0        0        0    49095 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/debugger.py
+-rw-rw-rw-   0        0        0     3322 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/device_access.py
+-rw-rw-rw-   0        0        0     1209 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/device_orientation.py
+-rw-rw-rw-   0        0        0    61795 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/dom.py
+-rw-rw-rw-   0        0        0     9459 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/dom_debugger.py
+-rw-rw-rw-   0        0        0    36732 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/dom_snapshot.py
+-rw-rw-rw-   0        0        0     5765 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/dom_storage.py
+-rw-rw-rw-   0        0        0    26059 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/emulation.py
+-rw-rw-rw-   0        0        0     1289 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/event_breakpoints.py
+-rw-rw-rw-   0        0        0    19105 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/fetch.py
+-rw-rw-rw-   0        0        0     4576 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/headless_experimental.py
+-rw-rw-rw-   0        0        0    13806 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/heap_profiler.py
+-rw-rw-rw-   0        0        0    15160 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/indexed_db.py
+-rw-rw-rw-   0        0        0    27841 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/input_.py
+-rw-rw-rw-   0        0        0     1718 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/inspector.py
+-rw-rw-rw-   0        0        0     3036 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/io.py
+-rw-rw-rw-   0        0        0    15049 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/layer_tree.py
+-rw-rw-rw-   0        0        0     5264 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/log.py
+-rw-rw-rw-   0        0        0     7627 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/media.py
+-rw-rw-rw-   0        0        0     6808 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/memory.py
+-rw-rw-rw-   0        0        0   126787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/network.py
+-rw-rw-rw-   0        0        0    50256 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/overlay.py
+-rw-rw-rw-   0        0        0   110999 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/page.py
+-rw-rw-rw-   0        0        0     2927 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/performance.py
+-rw-rw-rw-   0        0        0     6623 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/performance_timeline.py
+-rw-rw-rw-   0        0        0     2580 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/preload.py
+-rw-rw-rw-   0        0        0    12930 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/profiler.py
+-rw-rw-rw-   0        0        0    58743 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/runtime.py
+-rw-rw-rw-   0        0        0     1111 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/schema.py
+-rw-rw-rw-   0        0        0    16861 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/security.py
+-rw-rw-rw-   0        0        0    11066 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/service_worker.py
+-rw-rw-rw-   0        0        0    31857 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/storage.py
+-rw-rw-rw-   0        0        0    11517 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/system_info.py
+-rw-rw-rw-   0        0        0    24094 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/target.py
+-rw-rw-rw-   0        0        0     1538 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/tethering.py
+-rw-rw-rw-   0        0        0    12886 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/tracing.py
+-rw-rw-rw-   0        0        0      455 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/util.py
+-rw-rw-rw-   0        0        0    16895 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/web_audio.py
+-rw-rw-rw-   0        0        0    15500 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v112/web_authn.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.251187 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/
+-rw-rw-rw-   0        0        0     1258 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/__init__.py
+-rw-rw-rw-   0        0        0    15011 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/accessibility.py
+-rw-rw-rw-   0        0        0    11112 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/animation.py
+-rw-rw-rw-   0        0        0     5735 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/application_cache.py
+-rw-rw-rw-   0        0        0    17067 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/audits.py
+-rw-rw-rw-   0        0        0     5760 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/background_service.py
+-rw-rw-rw-   0        0        0    17298 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/browser.py
+-rw-rw-rw-   0        0        0     7810 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/cache_storage.py
+-rw-rw-rw-   0        0        0     3982 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/cast.py
+-rw-rw-rw-   0        0        0     2765 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/console.py
+-rw-rw-rw-   0        0        0    42907 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/css.py
+-rw-rw-rw-   0        0        0     3925 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/database.py
+-rw-rw-rw-   0        0        0    43473 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/debugger.py
+-rw-rw-rw-   0        0        0     1209 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/device_orientation.py
+-rw-rw-rw-   0        0        0    54390 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/dom.py
+-rw-rw-rw-   0        0        0     8592 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/dom_debugger.py
+-rw-rw-rw-   0        0        0    34069 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/dom_snapshot.py
+-rw-rw-rw-   0        0        0     5026 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/dom_storage.py
+-rw-rw-rw-   0        0        0    20775 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/emulation.py
+-rw-rw-rw-   0        0        0    16053 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/fetch.py
+-rw-rw-rw-   0        0        0     4791 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/headless_experimental.py
+-rw-rw-rw-   0        0        0    11207 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/heap_profiler.py
+-rw-rw-rw-   0        0        0    12762 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/indexed_db.py
+-rw-rw-rw-   0        0        0    19701 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/input_.py
+-rw-rw-rw-   0        0        0     1718 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/inspector.py
+-rw-rw-rw-   0        0        0     3034 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/io.py
+-rw-rw-rw-   0        0        0    15049 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/layer_tree.py
+-rw-rw-rw-   0        0        0     5062 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/log.py
+-rw-rw-rw-   0        0        0     6605 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/media.py
+-rw-rw-rw-   0        0        0     6808 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/memory.py
+-rw-rw-rw-   0        0        0    86888 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/network.py
+-rw-rw-rw-   0        0        0    24823 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/overlay.py
+-rw-rw-rw-   0        0        0    70797 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/page.py
+-rw-rw-rw-   0        0        0     2927 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/performance.py
+-rw-rw-rw-   0        0        0    17177 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/profiler.py
+-rw-rw-rw-   0        0        0    51695 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/runtime.py
+-rw-rw-rw-   0        0        0     1111 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/schema.py
+-rw-rw-rw-   0        0        0    16913 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/security.py
+-rw-rw-rw-   0        0        0    11066 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/service_worker.py
+-rw-rw-rw-   0        0        0     8277 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/storage.py
+-rw-rw-rw-   0        0        0    11049 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/system_info.py
+-rw-rw-rw-   0        0        0    18516 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/target.py
+-rw-rw-rw-   0        0        0     1538 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/tethering.py
+-rw-rw-rw-   0        0        0    10556 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/tracing.py
+-rw-rw-rw-   0        0        0      455 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/util.py
+-rw-rw-rw-   0        0        0    16894 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/web_audio.py
+-rw-rw-rw-   0        0        0     9424 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/devtools/v85/web_authn.py
+-rw-rw-rw-   0        0        0     1660 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/driver_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.254687 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/html5/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/html5/__init__.py
+-rw-rw-rw-   0        0        0     1626 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/html5/application_cache.py
+-rw-rw-rw-   0        0        0     2317 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/keys.py
+-rw-rw-rw-   0        0        0     5913 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/log.py
+-rw-rw-rw-   0        0        0     9123 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/options.py
+-rw-rw-rw-   0        0        0     8607 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/print_page_options.py
+-rw-rw-rw-   0        0        0    10533 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/proxy.py
+-rw-rw-rw-   0        0        0     4475 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/selenium_manager.py
+-rw-rw-rw-   0        0        0     8476 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/service.py
+-rw-rw-rw-   0        0        0     3804 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/timeouts.py
+-rw-rw-rw-   0        0        0     4458 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/utils.py
+-rw-rw-rw-   0        0        0     7827 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/virtual_authenticator.py
+-rw-rw-rw-   0        0        0      927 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/common/window.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.261211 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/edge/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/edge/__init__.py
+-rw-rw-rw-   0        0        0     1711 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/edge/options.py
+-rw-rw-rw-   0        0        0     2725 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/edge/service.py
+-rw-rw-rw-   0        0        0     3619 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/edge/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.275236 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/__init__.py
+-rw-rw-rw-   0        0        0     2801 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/extension_connection.py
+-rw-rw-rw-   0        0        0     8991 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/firefox_binary.py
+-rw-rw-rw-   0        0        0    14364 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/firefox_profile.py
+-rw-rw-rw-   0        0        0     5684 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/options.py
+-rw-rw-rw-   0        0        0     1683 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/remote_connection.py
+-rw-rw-rw-   0        0        0     2709 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/service.py
+-rw-rw-rw-   0        0        0    14528 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/firefox/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.281769 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/ie/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/ie/__init__.py
+-rw-rw-rw-   0        0        0    11497 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/ie/options.py
+-rw-rw-rw-   0        0        0     2473 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/ie/service.py
+-rw-rw-rw-   0        0        0     5653 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/ie/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.297318 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/bidi_connection.py
+-rw-rw-rw-   0        0        0     4997 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/command.py
+-rw-rw-rw-   0        0        0    11677 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/errorhandler.py
+-rw-rw-rw-   0        0        0     1803 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/file_detector.py
+-rw-rw-rw-   0        0        0     2625 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/mobile.py
+-rw-rw-rw-   0        0        0    16829 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/remote_connection.py
+-rw-rw-rw-   0        0        0     1084 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/script_key.py
+-rw-rw-rw-   0        0        0     2949 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/shadowroot.py
+-rw-rw-rw-   0        0        0     5015 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/switch_to.py
+-rw-rw-rw-   0        0        0      996 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/utils.py
+-rw-rw-rw-   0        0        0    43299 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/webdriver.py
+-rw-rw-rw-   0        0        0    17016 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/remote/webelement.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.307349 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/safari/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/safari/__init__.py
+-rw-rw-rw-   0        0        0     4284 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/safari/options.py
+-rw-rw-rw-   0        0        0      922 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/safari/permissions.py
+-rw-rw-rw-   0        0        0     1531 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/safari/remote_connection.py
+-rw-rw-rw-   0        0        0     3155 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/safari/service.py
+-rw-rw-rw-   0        0        0     6326 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/safari/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.319875 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/__init__.py
+-rw-rw-rw-   0        0        0     2178 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/abstract_event_listener.py
+-rw-rw-rw-   0        0        0    12207 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/color.py
+-rw-rw-rw-   0        0        0     9193 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/event_firing_webdriver.py
+-rw-rw-rw-   0        0        0      920 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/events.py
+-rw-rw-rw-   0        0        0    14812 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/expected_conditions.py
+-rw-rw-rw-   0        0        0     5930 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/relative_locator.py
+-rw-rw-rw-   0        0        0     9276 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/select.py
+-rw-rw-rw-   0        0        0      863 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/ui.py
+-rw-rw-rw-   0        0        0     4868 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/support/wait.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.324875 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/webkitgtk/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/webkitgtk/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/webkitgtk/options.py
+-rw-rw-rw-   0        0        0     2301 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/webkitgtk/service.py
+-rw-rw-rw-   0        0        0     3136 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/webkitgtk/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.328897 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/wpewebkit/
+-rw-rw-rw-   0        0        0      787 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/wpewebkit/__init__.py
+-rw-rw-rw-   0        0        0     2207 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/wpewebkit/options.py
+-rw-rw-rw-   0        0        0     2292 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/wpewebkit/service.py
+-rw-rw-rw-   0        0        0     2932 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/selenium/webdriver/wpewebkit/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.362970 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/
+-rw-rw-rw-   0        0        0     8429 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_deprecation_warning.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.402817 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      537 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-rw-   0        0        0      411 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-rw-   0        0        0      239 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-rw-   0        0        0    19672 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8603 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14789 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    47369 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    17973 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.431384 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      430 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-rw-   0        0        0     5441 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4701 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    22051 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     5617 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     7728 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31558 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16568 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5624 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     4888 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2603 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13137 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30221 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2779 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2785 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1189 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8434 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     1936 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0      672 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-rw-   0        0        0    11765 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19241 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7477 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-rw-   0        0        0     4920 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9451 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    12537 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0     3423 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     8082 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50186 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3589 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10270 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17910 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     8226 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13713 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1972 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30235 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23602 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      217 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0      639 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-rw-   0        0        0     3517 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    18858 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12096 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    15641 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    18128 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    12952 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5248 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     1972 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-rw-rw-   0        0        0     2392 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_imp.py
+-rw-rw-rw-   0        0        0     1311 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_importlib.py
+-rw-rw-rw-   0        0        0      675 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_itertools.py
+-rw-rw-rw-   0        0        0      749 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_path.py
+-rw-rw-rw-   0        0        0      501 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_reqs.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.436394 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.445910 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-rw-   0        0        0    30130 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     1862 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1828 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1154 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     2166 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.454923 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.459451 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13512 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.460448 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15517 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.464451 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117959 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.475982 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8493 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4700 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.487031 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.488540 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.492541 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    87149 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-rw-   0        0        0     7346 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    19539 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.521108 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/
+-rw-rw-rw-   0        0        0      396 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16623 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1182 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     6595 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/build.py
+-rw-rw-rw-   0        0        0     4415 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    15821 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0    14115 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     7012 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0     4800 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    85662 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    31188 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-rw-   0        0        0    26795 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     5163 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2226 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3875 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2612 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0     4946 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-rw-rw-   0        0        0      468 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2128 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      658 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     7071 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     5086 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8102 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7494 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/command/upload_docs.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.527122 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/
+-rw-rw-rw-   0        0        0     1121 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-rw-rw-   0        0        0    13398 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.533629 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-rw-   0        0        0     1038 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-rw-   0        0        0    11266 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-rw-   0        0        0     1153 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-rw-   0        0        0     1612 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-rw-   0        0        0   269900 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-rw-   0        0        0     8736 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-rw-   0        0        0    16319 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/expand.py
+-rw-rw-rw-   0        0        0    19304 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-rw-   0        0        0    25198 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-rw-rw-   0        0        0      949 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5499 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-   0        0        0    20799 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/discovery.py
+-rw-rw-rw-   0        0        0    45578 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-   0        0        0     2464 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/errors.py
+-rw-rw-rw-   0        0        0     5591 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.535130 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/extern/
+-rw-rw-rw-   0        0        0     2512 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4873 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-   0        0        0     3824 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-   0        0        0     1210 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/logging.py
+-rw-rw-rw-   0        0        0     4857 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    47724 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3093 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    40020 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-   0        0        0      245 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/py34compat.py
+-rw-rw-rw-   0        0        0    14348 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      941 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      144 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-   0        0        0     8376 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      718 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools/windows_support.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.364970 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/
+-rw-rw-rw-   0        0        0     2740 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-04-22 16:56:03.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.536138 whatsappy-py-4.0.0/.venv/Lib/site-packages/six-1.16.0.dist-info/
+-rw-rw-rw-   0        0        0        4 2023-05-01 17:38:33.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/six-1.16.0.dist-info/top_level.txt
+-rw-rw-rw-   0        0        0    34549 2023-05-01 17:38:33.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/six.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.539154 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio/
+-rw-rw-rw-   0        0        0      310 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio/__init__.py
+-rw-rw-rw-   0        0        0     2843 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio/_impl.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.542158 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio/_tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2110 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio/_tests/test_sniffio.py
+-rw-rw-rw-   0        0        0       89 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.540155 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio-1.3.0.dist-info/
+-rw-rw-rw-   0        0        0        8 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sniffio-1.3.0.dist-info/top_level.txt
+-rw-rw-rw-   0        0        0    31086 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/socks.py
+-rw-rw-rw-   0        0        0     3966 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sockshandler.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.546160 whatsappy-py-4.0.0/.venv/Lib/site-packages/sortedcontainers/
+-rw-rw-rw-   0        0        0     2131 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sortedcontainers/__init__.py
+-rw-rw-rw-   0        0        0    22712 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sortedcontainers/sorteddict.py
+-rw-rw-rw-   0        0        0    76331 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sortedcontainers/sortedlist.py
+-rw-rw-rw-   0        0        0    19825 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sortedcontainers/sortedset.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.547669 whatsappy-py-4.0.0/.venv/Lib/site-packages/sortedcontainers-2.4.0.dist-info/
+-rw-rw-rw-   0        0        0       17 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/sortedcontainers-2.4.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.555177 whatsappy-py-4.0.0/.venv/Lib/site-packages/soupsieve/
+-rw-rw-rw-   0        0        0     4630 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/soupsieve/__init__.py
+-rw-rw-rw-   0        0        0     6842 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/soupsieve/__meta__.py
+-rw-rw-rw-   0        0        0    58152 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/soupsieve/css_match.py
+-rw-rw-rw-   0        0        0    47063 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/soupsieve/css_parser.py
+-rw-rw-rw-   0        0        0    10337 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/soupsieve/css_types.py
+-rw-rw-rw-   0        0        0     4053 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/soupsieve/pretty.py
+-rw-rw-rw-   0        0        0     3374 2023-05-06 16:48:11.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/soupsieve/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.557192 whatsappy-py-4.0.0/.venv/Lib/site-packages/tests_negative/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tests_negative/__init__.py
+-rw-rw-rw-   0        0        0     1664 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tests_negative/test_browsers_not_installed.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.561198 whatsappy-py-4.0.0/.venv/Lib/site-packages/tests_xdist/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tests_xdist/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tests_xdist/conftest.py
+-rw-rw-rw-   0        0        0      292 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tests_xdist/test_cuncurent_1.py
+-rw-rw-rw-   0        0        0      292 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tests_xdist/test_cuncurent_2.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.584763 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/
+-rw-rw-rw-   0        0        0     1572 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/_dist_ver.py
+-rw-rw-rw-   0        0        0      283 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/_main.py
+-rw-rw-rw-   0        0        0     3699 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/_monitor.py
+-rw-rw-rw-   0        0        0      283 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/_tqdm.py
+-rw-rw-rw-   0        0        0      287 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/_tqdm_gui.py
+-rw-rw-rw-   0        0        0      307 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/_tqdm_notebook.py
+-rw-rw-rw-   0        0        0      888 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/_tqdm_pandas.py
+-rw-rw-rw-   0        0        0      553 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/_utils.py
+-rw-rw-rw-   0        0        0     2775 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/asyncio.py
+-rw-rw-rw-   0        0        0      871 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/auto.py
+-rw-rw-rw-   0        0        0      956 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/autonotebook.py
+-rw-rw-rw-   0        0        0    10727 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.595283 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/
+-rw-rw-rw-   0        0        0     2513 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/__init__.py
+-rw-rw-rw-   0        0        0      837 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/bells.py
+-rw-rw-rw-   0        0        0     3986 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/concurrent.py
+-rw-rw-rw-   0        0        0     3955 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/discord.py
+-rw-rw-rw-   0        0        0      774 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/itertools.py
+-rw-rw-rw-   0        0        0     3804 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/logging.py
+-rw-rw-rw-   0        0        0     4061 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/slack.py
+-rw-rw-rw-   0        0        0     5093 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/telegram.py
+-rw-rw-rw-   0        0        0     1207 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/contrib/utils_worker.py
+-rw-rw-rw-   0        0        0     1337 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/dask.py
+-rw-rw-rw-   0        0        0     5800 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/gui.py
+-rw-rw-rw-   0        0        0     4359 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/keras.py
+-rw-rw-rw-   0        0        0    11049 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/notebook.py
+-rw-rw-rw-   0        0        0     5018 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/rich.py
+-rw-rw-rw-   0        0        0    57678 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/std.py
+-rw-rw-rw-   0        0        0     6718 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/tk.py
+-rw-rw-rw-   0        0        0     9510 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/utils.py
+-rw-rw-rw-   0        0        0      333 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.586778 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm-4.65.0.dist-info/
+-rw-rw-rw-   0        0        0       39 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm-4.65.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/tqdm-4.65.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.628371 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/
+-rw-rw-rw-   0        0        0     4025 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/__init__.py
+-rw-rw-rw-   0        0        0    23835 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_abc.py
+-rw-rw-rw-   0        0        0    14352 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_channel.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.654910 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/
+-rw-rw-rw-   0        0        0     2040 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/__init__.py
+-rw-rw-rw-   0        0        0     8976 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_asyncgens.py
+-rw-rw-rw-   0        0        0     8428 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_entry_queue.py
+-rw-rw-rw-   0        0        0     4165 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_exceptions.py
+-rw-rw-rw-   0        0        0     1619 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_generated_instrumentation.py
+-rw-rw-rw-   0        0        0     1125 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_generated_io_epoll.py
+-rw-rw-rw-   0        0        0     1948 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_generated_io_kqueue.py
+-rw-rw-rw-   0        0        0     2855 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_generated_io_windows.py
+-rw-rw-rw-   0        0        0    10045 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_generated_run.py
+-rw-rw-rw-   0        0        0     3788 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_instrumentation.py
+-rw-rw-rw-   0        0        0      637 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_io_common.py
+-rw-rw-rw-   0        0        0    14491 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_io_epoll.py
+-rw-rw-rw-   0        0        0     7169 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_io_kqueue.py
+-rw-rw-rw-   0        0        0    36970 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_io_windows.py
+-rw-rw-rw-   0        0        0     7941 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_ki.py
+-rw-rw-rw-   0        0        0     2749 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_local.py
+-rw-rw-rw-   0        0        0     6196 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_mock_clock.py
+-rw-rw-rw-   0        0        0    16977 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_multierror.py
+-rw-rw-rw-   0        0        0     8437 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_parking_lot.py
+-rw-rw-rw-   0        0        0    99530 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_run.py
+-rw-rw-rw-   0        0        0     6807 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_thread_cache.py
+-rw-rw-rw-   0        0        0    11228 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_traps.py
+-rw-rw-rw-   0        0        0     4626 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_unbounded_queue.py
+-rw-rw-rw-   0        0        0     2590 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_wakeup_socketpair.py
+-rw-rw-rw-   0        0        0     8863 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/_windows_cffi.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.674962 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/__init__.py
+-rw-rw-rw-   0        0        0      703 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/conftest.py
+-rw-rw-rw-   0        0        0    10700 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_asyncgen.py
+-rw-rw-rw-   0        0        0    18314 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_guest_mode.py
+-rw-rw-rw-   0        0        0     7365 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_instrumentation.py
+-rw-rw-rw-   0        0        0    14974 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_io.py
+-rw-rw-rw-   0        0        0    14466 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_ki.py
+-rw-rw-rw-   0        0        0     2623 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_local.py
+-rw-rw-rw-   0        0        0     5022 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_mock_clock.py
+-rw-rw-rw-   0        0        0    15948 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_multierror.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.681987 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_multierror_scripts/
+-rw-rw-rw-   0        0        0      155 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_multierror_scripts/__init__.py
+-rw-rw-rw-   0        0        0      171 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_multierror_scripts/_common.py
+-rw-rw-rw-   0        0        0      390 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_multierror_scripts/apport_excepthook.py
+-rw-rw-rw-   0        0        0      728 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_multierror_scripts/ipython_custom_exc.py
+-rw-rw-rw-   0        0        0      342 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_multierror_scripts/simple_excepthook.py
+-rw-rw-rw-   0        0        0      172 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_multierror_scripts/simple_excepthook_IPython.py
+-rw-rw-rw-   0        0        0     5772 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_parking_lot.py
+-rw-rw-rw-   0        0        0    78134 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_run.py
+-rw-rw-rw-   0        0        0     5019 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_thread_cache.py
+-rw-rw-rw-   0        0        0      451 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_tutil.py
+-rw-rw-rw-   0        0        0     4088 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_unbounded_queue.py
+-rw-rw-rw-   0        0        0       14 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_util.py
+-rw-rw-rw-   0        0        0     7807 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/test_windows.py
+-rw-rw-rw-   0        0        0     4658 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_core/tests/tutil.py
+-rw-rw-rw-   0        0        0     4692 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_deprecate.py
+-rw-rw-rw-   0        0        0    51369 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_dtls.py
+-rw-rw-rw-   0        0        0     4554 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_file_io.py
+-rw-rw-rw-   0        0        0     3928 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_highlevel_generic.py
+-rw-rw-rw-   0        0        0     9181 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_highlevel_open_tcp_listeners.py
+-rw-rw-rw-   0        0        0    17687 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_highlevel_open_tcp_stream.py
+-rw-rw-rw-   0        0        0     1247 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_highlevel_open_unix_stream.py
+-rw-rw-rw-   0        0        0     4250 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_highlevel_serve_listeners.py
+-rw-rw-rw-   0        0        0    14501 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_highlevel_socket.py
+-rw-rw-rw-   0        0        0     5784 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_highlevel_ssl_helpers.py
+-rw-rw-rw-   0        0        0     6315 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_path.py
+-rw-rw-rw-   0        0        0     6479 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_signals.py
+-rw-rw-rw-   0        0        0    30094 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_socket.py
+-rw-rw-rw-   0        0        0    44430 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_ssl.py
+-rw-rw-rw-   0        0        0    31847 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_subprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.687016 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_subprocess_platform/
+-rw-rw-rw-   0        0        0     4601 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_subprocess_platform/__init__.py
+-rw-rw-rw-   0        0        0     1677 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_subprocess_platform/kqueue.py
+-rw-rw-rw-   0        0        0     3671 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_subprocess_platform/waitid.py
+-rw-rw-rw-   0        0        0      208 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_subprocess_platform/windows.py
+-rw-rw-rw-   0        0        0    27439 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_sync.py
+-rw-rw-rw-   0        0        0    14033 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_threads.py
+-rw-rw-rw-   0        0        0     3913 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_timeouts.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.689024 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_tools/__init__.py
+-rw-rw-rw-   0        0        0     5902 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_tools/gen_exports.py
+-rw-rw-rw-   0        0        0     7882 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_unix_pipes.py
+-rw-rw-rw-   0        0        0    11997 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_util.py
+-rw-rw-rw-   0        0        0       90 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_version.py
+-rw-rw-rw-   0        0        0     2006 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_wait_for_object.py
+-rw-rw-rw-   0        0        0     4741 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/_windows_pipes.py
+-rw-rw-rw-   0        0        0      624 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/abc.py
+-rw-rw-rw-   0        0        0      263 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/from_thread.py
+-rw-rw-rw-   0        0        0     1897 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/lowlevel.py
+-rw-rw-rw-   0        0        0     9946 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.697548 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/
+-rw-rw-rw-   0        0        0      765 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/__init__.py
+-rw-rw-rw-   0        0        0    20078 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/_check_streams.py
+-rw-rw-rw-   0        0        0     1816 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/_checkpoints.py
+-rw-rw-rw-   0        0        0    12649 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/_fake_net.py
+-rw-rw-rw-   0        0        0    21350 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/_memory_streams.py
+-rw-rw-rw-   0        0        0     1116 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/_network.py
+-rw-rw-rw-   0        0        0     2650 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/_sequencer.py
+-rw-rw-rw-   0        0        0      828 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/testing/_trio_test.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.733142 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/conftest.py
+-rw-rw-rw-   0        0        0      601 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/module_with_deprecations.py
+-rw-rw-rw-   0        0        0     1310 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_abc.py
+-rw-rw-rw-   0        0        0    12202 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_channel.py
+-rw-rw-rw-   0        0        0     1381 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_contextvars.py
+-rw-rw-rw-   0        0        0     6497 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_deprecate.py
+-rw-rw-rw-   0        0        0    31954 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_dtls.py
+-rw-rw-rw-   0        0        0     5202 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_exports.py
+-rw-rw-rw-   0        0        0     1084 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_fakenet.py
+-rw-rw-rw-   0        0        0     4994 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_file_io.py
+-rw-rw-rw-   0        0        0     2651 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_highlevel_generic.py
+-rw-rw-rw-   0        0        0     9639 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_highlevel_open_tcp_listeners.py
+-rw-rw-rw-   0        0        0    18142 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_highlevel_open_tcp_stream.py
+-rw-rw-rw-   0        0        0     1897 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_highlevel_open_unix_stream.py
+-rw-rw-rw-   0        0        0     4437 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_highlevel_serve_listeners.py
+-rw-rw-rw-   0        0        0     8921 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_highlevel_socket.py
+-rw-rw-rw-   0        0        0     4038 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_highlevel_ssl_helpers.py
+-rw-rw-rw-   0        0        0     6585 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_path.py
+-rw-rw-rw-   0        0        0     1137 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_scheduler_determinism.py
+-rw-rw-rw-   0        0        0     6976 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_signals.py
+-rw-rw-rw-   0        0        0    35617 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_socket.py
+-rw-rw-rw-   0        0        0    48894 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_ssl.py
+-rw-rw-rw-   0        0        0    20269 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_subprocess.py
+-rw-rw-rw-   0        0        0    16158 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_sync.py
+-rw-rw-rw-   0        0        0    19086 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_testing.py
+-rw-rw-rw-   0        0        0    25178 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_threads.py
+-rw-rw-rw-   0        0        0     3335 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_timeouts.py
+-rw-rw-rw-   0        0        0     9706 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_unix_pipes.py
+-rw-rw-rw-   0        0        0     5542 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_util.py
+-rw-rw-rw-   0        0        0     8050 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_wait_for_object.py
+-rw-rw-rw-   0        0        0     3098 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/test_windows_pipes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.735146 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/tools/__init__.py
+-rw-rw-rw-   0        0        0     1945 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/tests/tools/test_gen_exports.py
+-rw-rw-rw-   0        0        0      106 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio/to_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.629374 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio-0.22.0.dist-info/
+-rw-rw-rw-   0        0        0        5 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio-0.22.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.738674 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio_websocket/
+-rw-rw-rw-   0        0        0      434 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio_websocket/__init__.py
+-rw-rw-rw-   0        0        0    56673 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio_websocket/_impl.py
+-rw-rw-rw-   0        0        0       23 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio_websocket/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.739674 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio_websocket-0.10.2.dist-info/
+-rw-rw-rw-   0        0        0       15 2023-04-22 16:57:38.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/trio_websocket-0.10.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.751200 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/
+-rw-rw-rw-   0        0        0     1343 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/__init__.py
+-rw-rw-rw-   0        0        0     1475 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/__main__.py
+-rw-rw-rw-   0        0        0     3129 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/auth.py
+-rw-rw-rw-   0        0        0     3738 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.757217 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/commands/
+-rw-rw-rw-   0        0        0     1802 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/commands/__init__.py
+-rw-rw-rw-   0        0        0     5727 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/commands/check.py
+-rw-rw-rw-   0        0        0     2904 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/commands/register.py
+-rw-rw-rw-   0        0        0     7469 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/commands/upload.py
+-rw-rw-rw-   0        0        0     3814 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/exceptions.py
+-rw-rw-rw-   0        0        0    11024 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/package.py
+-rw-rw-rw-   0        0        0     8713 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/repository.py
+-rw-rw-rw-   0        0        0    12269 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/settings.py
+-rw-rw-rw-   0        0        0    10867 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/utils.py
+-rw-rw-rw-   0        0        0     3049 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/wheel.py
+-rw-rw-rw-   0        0        0     1795 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine/wininst.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.753202 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine-4.0.2.dist-info/
+-rw-rw-rw-   0        0        0      185 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine-4.0.2.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 19:21:01.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/twine-4.0.2.dist-info/top_level.txt
+-rw-rw-rw-   0        0        0    84065 2023-04-22 22:46:46.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.769263 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20300 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39128 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.779296 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.782292 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11012 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4528 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17055 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34416 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.784813 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.786825 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/request.py
+-rw-rw-rw-   0        0        0    30761 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.804849 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     4225 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22003 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17165 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10168 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14279 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3/util/wait.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.771261 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3-1.26.15.dist-info/
+-rw-rw-rw-   0        0        0     1115 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3-1.26.15.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 16:57:36.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/urllib3-1.26.15.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.812372 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/
+-rw-rw-rw-   0        0        0       22 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/__init__.py
+-rw-rw-rw-   0        0        0     1422 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/chrome.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.827917 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/__init__.py
+-rw-rw-rw-   0        0        0     1807 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/archive.py
+-rw-rw-rw-   0        0        0      740 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/config.py
+-rw-rw-rw-   0        0        0      218 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/constants.py
+-rw-rw-rw-   0        0        0      810 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/download_manager.py
+-rw-rw-rw-   0        0        0     2894 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/driver.py
+-rw-rw-rw-   0        0        0     5177 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/driver_cache.py
+-rw-rw-rw-   0        0        0     1403 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/http.py
+-rw-rw-rw-   0        0        0      686 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/logger.py
+-rw-rw-rw-   0        0        0     1133 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/manager.py
+-rw-rw-rw-   0        0        0    11755 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.835931 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/drivers/
+-rw-rw-rw-   0        0        0        0 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/drivers/__init__.py
+-rw-rw-rw-   0        0        0     2164 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/drivers/chrome.py
+-rw-rw-rw-   0        0        0     1954 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/drivers/edge.py
+-rw-rw-rw-   0        0        0     2288 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/drivers/firefox.py
+-rw-rw-rw-   0        0        0     2722 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/drivers/ie.py
+-rw-rw-rw-   0        0        0     1700 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/drivers/opera.py
+-rw-rw-rw-   0        0        0     1409 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/firefox.py
+-rw-rw-rw-   0        0        0     2335 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/microsoft.py
+-rw-rw-rw-   0        0        0     1743 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager/opera.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.814373 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager-3.8.6.dist-info/
+-rw-rw-rw-   0        0        0       45 2023-04-22 17:00:07.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webdriver_manager-3.8.6.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.842447 whatsappy-py-4.0.0/.venv/Lib/site-packages/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.843446 whatsappy-py-4.0.0/.venv/Lib/site-packages/webencodings-0.5.1.dist-info/
+-rw-rw-rw-   0        0        0       13 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/webencodings-0.5.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.848466 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/
+-rw-rw-rw-   0        0        0       30 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.856983 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/chat/
+-rw-rw-rw-   0        0        0       70 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/chat/__init__.py
+-rw-rw-rw-   0        0        0     4368 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/chat/chat.py
+-rw-rw-rw-   0        0        0    14381 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/chat/conversation.py
+-rw-rw-rw-   0        0        0     3031 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/chat/group.py
+-rw-rw-rw-   0        0        0       86 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/chat/groupchat.py
+-rw-rw-rw-   0        0        0     1854 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/chat/unread.py
+-rw-rw-rw-   0        0        0     2291 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/chat/unread_message.py
+-rw-rw-rw-   0        0        0      693 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.865994 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/
+-rw-rw-rw-   0        0        0      217 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/audio.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/contact.py
+-rw-rw-rw-   0        0        0      840 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/document.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/image.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/location.py
+-rw-rw-rw-   0        0        0     4194 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/message.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/sticker.py
+-rw-rw-rw-   0        0        0     2297 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/unread_message.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/messages/video.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.873008 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util/
+-rw-rw-rw-   0        0        0      117 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util/__init__.py
+-rw-rw-rw-   0        0        0      623 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util/exceptions.py
+-rw-rw-rw-   0        0        0     1632 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util/me.py
+-rw-rw-rw-   0        0        0      306 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util/my_thread.py
+-rw-rw-rw-   0        0        0      820 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util/other.py
+-rw-rw-rw-   0        0        0     4204 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util/selectors.py
+-rw-rw-rw-   0        0        0     1869 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util/selenium.py
+-rw-rw-rw-   0        0        0      672 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/util.py
+-rw-rw-rw-   0        0        0    10078 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy/whatsapp.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.848967 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy-4.0.0.dist-info/
+-rw-rw-rw-   0        0        0       10 2023-05-09 19:13:15.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/whatsappy-4.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.878531 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/
+-rw-rw-rw-   0        0        0      214 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.881531 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/
+-rw-rw-rw-   0        0        0     1864 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/__init__.py
+-rw-rw-rw-   0        0        0      199 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/_winerrors.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.890561 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/__init__.py
+-rw-rw-rw-   0        0        0     4964 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
+-rw-rw-rw-   0        0        0      554 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/_common.py
+-rw-rw-rw-   0        0        0      866 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py
+-rw-rw-rw-   0        0        0      355 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
+-rw-rw-rw-   0        0        0     4584 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py
+-rw-rw-rw-   0        0        0      882 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
+-rw-rw-rw-   0        0        0      374 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/_time.py
+-rw-rw-rw-   0        0        0     2723 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/cffi/_util.py
+-rw-rw-rw-   0        0        0      560 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/compat.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.900573 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
+-rw-rw-rw-   0        0        0     3627 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
+-rw-rw-rw-   0        0        0     1502 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py
+-rw-rw-rw-   0        0        0      594 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
+-rw-rw-rw-   0        0        0      357 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
+-rw-rw-rw-   0        0        0     4252 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
+-rw-rw-rw-   0        0        0      983 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
+-rw-rw-rw-   0        0        0      384 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/_time.py
+-rw-rw-rw-   0        0        0     2049 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.904577 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/pywin32/
+-rw-rw-rw-   0        0        0      396 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/pywin32/__init__.py
+-rw-rw-rw-   0        0        0      954 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
+-rw-rw-rw-   0        0        0     7768 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/pywin32/win32api.py
+-rw-rw-rw-   0        0        0     2850 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py
+-rw-rw-rw-   0        0        0      342 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/pywintypes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.908599 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/tests/
+-rw-rw-rw-   0        0        0      612 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/tests/__init__.py
+-rw-rw-rw-   0        0        0     2545 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/tests/compat.py
+-rw-rw-rw-   0        0        0    11110 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/tests/test_win32api.py
+-rw-rw-rw-   0        0        0     5710 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/version.py
+-rw-rw-rw-   0        0        0      338 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/win32api.py
+-rw-rw-rw-   0        0        0      340 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/win32ctypes/win32cred.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.917116 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/
+-rw-rw-rw-   0        0        0     2887 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/__init__.py
+-rw-rw-rw-   0        0        0     6813 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/connection.py
+-rw-rw-rw-   0        0        0     7979 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/events.py
+-rw-rw-rw-   0        0        0    11211 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/extensions.py
+-rw-rw-rw-   0        0        0    23401 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/frame_protocol.py
+-rw-rw-rw-   0        0        0    18036 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/handshake.py
+-rw-rw-rw-   0        0        0       68 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/typing.py
+-rw-rw-rw-   0        0        0     2816 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.918114 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto-1.2.0.dist-info/
+-rw-rw-rw-   0        0        0        8 2023-04-22 16:57:37.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/wsproto-1.2.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.920120 whatsappy-py-4.0.0/.venv/Lib/site-packages/zipp/
+-rw-rw-rw-   0        0        0    10676 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/zipp/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/zipp/py310compat.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.921124 whatsappy-py-4.0.0/.venv/Lib/site-packages/zipp-3.15.0.dist-info/
+-rw-rw-rw-   0        0        0        5 2023-05-09 19:20:54.000000 whatsappy-py-4.0.0/.venv/Lib/site-packages/zipp-3.15.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.933139 whatsappy-py-4.0.0/.venv/Scripts/
+-rw-rw-rw-   0        0        0      659 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2html.py
+-rw-rw-rw-   0        0        0      781 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2html4.py
+-rw-rw-rw-   0        0        0     1116 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2html5.py
+-rw-rw-rw-   0        0        0      858 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2latex.py
+-rw-rw-rw-   0        0        0      681 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2man.py
+-rw-rw-rw-   0        0        0      847 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2odt.py
+-rw-rw-rw-   0        0        0     2203 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2odt_prepstyles.py
+-rw-rw-rw-   0        0        0      666 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2pseudoxml.py
+-rw-rw-rw-   0        0        0      702 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2s5.py
+-rw-rw-rw-   0        0        0      938 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2xetex.py
+-rw-rw-rw-   0        0        0      667 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rst2xml.py
+-rw-rw-rw-   0        0        0      735 2023-05-09 19:20:58.000000 whatsappy-py-4.0.0/.venv/Scripts/rstpep2html.py
+-rw-rw-rw-   0        0        0     1087 2023-04-22 19:17:33.000000 whatsappy-py-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0       64 2023-04-22 19:18:38.000000 whatsappy-py-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5427 2023-05-09 19:27:41.974738 whatsappy-py-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4833 2023-05-09 19:03:35.000000 whatsappy-py-4.0.0/README.md
+-rw-rw-rw-   0        0        0      109 2023-04-22 19:16:25.000000 whatsappy-py-4.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      128 2023-05-06 17:01:40.000000 whatsappy-py-4.0.0/requirements.txt
+-rw-rw-rw-   0        0        0      673 2023-05-09 19:27:41.980761 whatsappy-py-4.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.936149 whatsappy-py-4.0.0/tests/
+-rw-rw-rw-   0        0        0      338 2023-05-09 19:11:54.000000 whatsappy-py-4.0.0/tests/test.py
+-rw-rw-rw-   0        0        0     2160 2023-05-06 20:22:22.000000 whatsappy-py-4.0.0/tests/test_pytest.py
+-rw-rw-rw-   0        0        0       62 2023-05-09 19:25:47.000000 whatsappy-py-4.0.0/tests/upload.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.938161 whatsappy-py-4.0.0/whatsappy/
+-rw-rw-rw-   0        0        0       30 2023-04-22 22:17:40.000000 whatsappy-py-4.0.0/whatsappy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.942164 whatsappy-py-4.0.0/whatsappy/chat/
+-rw-rw-rw-   0        0        0       70 2023-05-06 17:46:28.000000 whatsappy-py-4.0.0/whatsappy/chat/__init__.py
+-rw-rw-rw-   0        0        0     4368 2023-05-07 15:49:31.000000 whatsappy-py-4.0.0/whatsappy/chat/chat.py
+-rw-rw-rw-   0        0        0    14381 2023-05-09 19:12:59.000000 whatsappy-py-4.0.0/whatsappy/chat/conversation.py
+-rw-rw-rw-   0        0        0     3031 2023-05-07 00:00:50.000000 whatsappy-py-4.0.0/whatsappy/chat/group.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.951183 whatsappy-py-4.0.0/whatsappy/messages/
+-rw-rw-rw-   0        0        0      217 2023-05-06 17:46:22.000000 whatsappy-py-4.0.0/whatsappy/messages/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:04:50.000000 whatsappy-py-4.0.0/whatsappy/messages/audio.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 16:59:53.000000 whatsappy-py-4.0.0/whatsappy/messages/contact.py
+-rw-rw-rw-   0        0        0      840 2023-05-06 17:05:43.000000 whatsappy-py-4.0.0/whatsappy/messages/document.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:02:58.000000 whatsappy-py-4.0.0/whatsappy/messages/image.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:04:27.000000 whatsappy-py-4.0.0/whatsappy/messages/location.py
+-rw-rw-rw-   0        0        0     4194 2023-05-08 21:28:45.000000 whatsappy-py-4.0.0/whatsappy/messages/message.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 16:59:56.000000 whatsappy-py-4.0.0/whatsappy/messages/sticker.py
+-rw-rw-rw-   0        0        0     2297 2023-05-06 17:58:57.000000 whatsappy-py-4.0.0/whatsappy/messages/unread_message.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 17:03:01.000000 whatsappy-py-4.0.0/whatsappy/messages/video.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.957201 whatsappy-py-4.0.0/whatsappy/util/
+-rw-rw-rw-   0        0        0      117 2023-04-30 00:22:26.000000 whatsappy-py-4.0.0/whatsappy/util/__init__.py
+-rw-rw-rw-   0        0        0      623 2023-05-09 19:00:15.000000 whatsappy-py-4.0.0/whatsappy/util/exceptions.py
+-rw-rw-rw-   0        0        0     1632 2023-05-04 01:11:08.000000 whatsappy-py-4.0.0/whatsappy/util/me.py
+-rw-rw-rw-   0        0        0      820 2023-05-09 18:28:28.000000 whatsappy-py-4.0.0/whatsappy/util/other.py
+-rw-rw-rw-   0        0        0     4204 2023-05-09 19:01:33.000000 whatsappy-py-4.0.0/whatsappy/util/selectors.py
+-rw-rw-rw-   0        0        0     1869 2023-05-06 23:50:24.000000 whatsappy-py-4.0.0/whatsappy/util/selenium.py
+-rw-rw-rw-   0        0        0    10078 2023-05-09 00:47:44.000000 whatsappy-py-4.0.0/whatsappy/whatsapp.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:27:41.973736 whatsappy-py-4.0.0/whatsappy_py.egg-info/
+-rw-rw-rw-   0        0        0     5427 2023-05-09 19:27:37.000000 whatsappy-py-4.0.0/whatsappy_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0   148310 2023-05-09 19:27:38.000000 whatsappy-py-4.0.0/whatsappy_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:27:37.000000 whatsappy-py-4.0.0/whatsappy_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-05-09 19:27:37.000000 whatsappy-py-4.0.0/whatsappy_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 19:27:37.000000 whatsappy-py-4.0.0/whatsappy_py.egg-info/top_level.txt
```

### Comparing `whatsappy-py-3.3.5/LICENSE` & `whatsappy-py-4.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Italo Seara
+Copyright (c) 2023 Italo Seara
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `whatsappy-py-3.3.5/whatsappy/message.py` & `whatsappy-py-4.0.0/.venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,403 +1,399 @@
-from dataclasses import dataclass, field
-from email.policy import default
-from PIL import Image as PILImage
-from datetime import datetime
-from typing import Any, List
-from pathlib import Path
-from io import BytesIO
-from time import sleep
-import mimetypes
-import json
-import re
-
-from selenium.webdriver.common.action_chains import ActionChains
-from selenium.webdriver.remote.webelement import WebElement
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.common.by import By
-
-from .tool import to_soup, parse_message, blob_to_bytes
-
-
-@dataclass
-class Text:
-
-    @dataclass
-    class Quote:
-        text: str
-        author: str
-
-    text: str = ""
-    author: str = None
-    quote: Quote = None
-    time: datetime = None
-    forwarded: bool = False
-    _chat: Any = field(repr=False, default=None)
-    _element: WebElement = field(repr=False, default=None)
-
-    def __post_init__(self):
-
-        self._driver = self._element.parent
-        
-        soup = to_soup(self._element)
-
-        if copyable_text := soup.find(class_="copyable-text"):
-
-            msg_metadata = copyable_text["data-pre-plain-text"]
-            self.text = parse_message(copyable_text.find(class_="copyable-text").span)
-            
-            time_msg = re.compile(r"(\d+:\d+(\s)?(AM|PM)?)").findall(msg_metadata)[0][0]
-            date_msg = re.compile(r"(\d+/\d+/\d+)").findall(msg_metadata)[0]
-            self.author = re.compile(r"] (.*):").findall(msg_metadata)[0]
-
-            self.time = (
-                datetime.strptime(f"{date_msg} {time_msg}", "%m/%d/%Y %I:%M %p")
-                if ("AM" in time_msg) or ("PM" in time_msg)
-                else datetime.strptime(f"{date_msg} {time_msg}", "%d/%m/%Y %H:%M")
+#
+# The Python Imaging Library
+# $Id$
+#
+# JPEG2000 file handling
+#
+# History:
+# 2014-03-12 ajh  Created
+# 2021-06-30 rogermb  Extract dpi information from the 'resc' header box
+#
+# Copyright (c) 2014 Coriolis Systems Limited
+# Copyright (c) 2014 Alastair Houghton
+#
+# See the README file for information on usage and redistribution.
+#
+import io
+import os
+import struct
+
+from . import Image, ImageFile, _binary
+
+
+class BoxReader:
+    """
+    A small helper class to read fields stored in JPEG2000 header boxes
+    and to easily step into and read sub-boxes.
+    """
+
+    def __init__(self, fp, length=-1):
+        self.fp = fp
+        self.has_length = length >= 0
+        self.length = length
+        self.remaining_in_box = -1
+
+    def _can_read(self, num_bytes):
+        if self.has_length and self.fp.tell() + num_bytes > self.length:
+            # Outside box: ensure we don't read past the known file length
+            return False
+        if self.remaining_in_box >= 0:
+            # Inside box contents: ensure read does not go past box boundaries
+            return num_bytes <= self.remaining_in_box
+        else:
+            return True  # No length known, just read
+
+    def _read_bytes(self, num_bytes):
+        if not self._can_read(num_bytes):
+            msg = "Not enough data in header"
+            raise SyntaxError(msg)
+
+        data = self.fp.read(num_bytes)
+        if len(data) < num_bytes:
+            msg = f"Expected to read {num_bytes} bytes but only got {len(data)}."
+            raise OSError(msg)
+
+        if self.remaining_in_box > 0:
+            self.remaining_in_box -= num_bytes
+        return data
+
+    def read_fields(self, field_format):
+        size = struct.calcsize(field_format)
+        data = self._read_bytes(size)
+        return struct.unpack(field_format, data)
+
+    def read_boxes(self):
+        size = self.remaining_in_box
+        data = self._read_bytes(size)
+        return BoxReader(io.BytesIO(data), size)
+
+    def has_next_box(self):
+        if self.has_length:
+            return self.fp.tell() + self.remaining_in_box < self.length
+        else:
+            return True
+
+    def next_box_type(self):
+        # Skip the rest of the box if it has not been read
+        if self.remaining_in_box > 0:
+            self.fp.seek(self.remaining_in_box, os.SEEK_CUR)
+        self.remaining_in_box = -1
+
+        # Read the length and type of the next box
+        lbox, tbox = self.read_fields(">I4s")
+        if lbox == 1:
+            lbox = self.read_fields(">Q")[0]
+            hlen = 16
+        else:
+            hlen = 8
+
+        if lbox < hlen or not self._can_read(lbox - hlen):
+            msg = "Invalid header length"
+            raise SyntaxError(msg)
+
+        self.remaining_in_box = lbox - hlen
+        return tbox
+
+
+def _parse_codestream(fp):
+    """Parse the JPEG 2000 codestream to extract the size and component
+    count from the SIZ marker segment, returning a PIL (size, mode) tuple."""
+
+    hdr = fp.read(2)
+    lsiz = _binary.i16be(hdr)
+    siz = hdr + fp.read(lsiz - 2)
+    lsiz, rsiz, xsiz, ysiz, xosiz, yosiz, _, _, _, _, csiz = struct.unpack_from(
+        ">HHIIIIIIIIH", siz
+    )
+    ssiz = [None] * csiz
+    xrsiz = [None] * csiz
+    yrsiz = [None] * csiz
+    for i in range(csiz):
+        ssiz[i], xrsiz[i], yrsiz[i] = struct.unpack_from(">BBB", siz, 36 + 3 * i)
+
+    size = (xsiz - xosiz, ysiz - yosiz)
+    if csiz == 1:
+        if (yrsiz[0] & 0x7F) > 8:
+            mode = "I;16"
+        else:
+            mode = "L"
+    elif csiz == 2:
+        mode = "LA"
+    elif csiz == 3:
+        mode = "RGB"
+    elif csiz == 4:
+        mode = "RGBA"
+    else:
+        mode = None
+
+    return size, mode
+
+
+def _res_to_dpi(num, denom, exp):
+    """Convert JPEG2000's (numerator, denominator, exponent-base-10) resolution,
+    calculated as (num / denom) * 10^exp and stored in dots per meter,
+    to floating-point dots per inch."""
+    if denom != 0:
+        return (254 * num * (10**exp)) / (10000 * denom)
+
+
+def _parse_jp2_header(fp):
+    """Parse the JP2 header box to extract size, component count,
+    color space information, and optionally DPI information,
+    returning a (size, mode, mimetype, dpi) tuple."""
+
+    # Find the JP2 header box
+    reader = BoxReader(fp)
+    header = None
+    mimetype = None
+    while reader.has_next_box():
+        tbox = reader.next_box_type()
+
+        if tbox == b"jp2h":
+            header = reader.read_boxes()
+            break
+        elif tbox == b"ftyp":
+            if reader.read_fields(">4s")[0] == b"jpx ":
+                mimetype = "image/jpx"
+
+    size = None
+    mode = None
+    bpc = None
+    nc = None
+    dpi = None  # 2-tuple of DPI info, or None
+
+    while header.has_next_box():
+        tbox = header.next_box_type()
+
+        if tbox == b"ihdr":
+            height, width, nc, bpc = header.read_fields(">IIHB")
+            size = (width, height)
+            if nc == 1 and (bpc & 0x7F) > 8:
+                mode = "I;16"
+            elif nc == 1:
+                mode = "L"
+            elif nc == 2:
+                mode = "LA"
+            elif nc == 3:
+                mode = "RGB"
+            elif nc == 4:
+                mode = "RGBA"
+        elif tbox == b"res ":
+            res = header.read_boxes()
+            while res.has_next_box():
+                tres = res.next_box_type()
+                if tres == b"resc":
+                    vrcn, vrcd, hrcn, hrcd, vrce, hrce = res.read_fields(">HHHHBB")
+                    hres = _res_to_dpi(hrcn, hrcd, hrce)
+                    vres = _res_to_dpi(vrcn, vrcd, vrce)
+                    if hres is not None and vres is not None:
+                        dpi = (hres, vres)
+                    break
+
+    if size is None or mode is None:
+        msg = "Malformed JP2 header"
+        raise SyntaxError(msg)
+
+    return size, mode, mimetype, dpi
+
+
+##
+# Image plugin for JPEG2000 images.
+
+
+class Jpeg2KImageFile(ImageFile.ImageFile):
+    format = "JPEG2000"
+    format_description = "JPEG 2000 (ISO 15444)"
+
+    def _open(self):
+        sig = self.fp.read(4)
+        if sig == b"\xff\x4f\xff\x51":
+            self.codec = "j2k"
+            self._size, self.mode = _parse_codestream(self.fp)
+        else:
+            sig = sig + self.fp.read(8)
+
+            if sig == b"\x00\x00\x00\x0cjP  \x0d\x0a\x87\x0a":
+                self.codec = "jp2"
+                header = _parse_jp2_header(self.fp)
+                self._size, self.mode, self.custom_mimetype, dpi = header
+                if dpi is not None:
+                    self.info["dpi"] = dpi
+                if self.fp.read(12).endswith(b"jp2c\xff\x4f\xff\x51"):
+                    self._parse_comment()
+            else:
+                msg = "not a JPEG 2000 file"
+                raise SyntaxError(msg)
+
+        if self.size is None or self.mode is None:
+            msg = "unable to determine size/mode"
+            raise SyntaxError(msg)
+
+        self._reduce = 0
+        self.layers = 0
+
+        fd = -1
+        length = -1
+
+        try:
+            fd = self.fp.fileno()
+            length = os.fstat(fd).st_size
+        except Exception:
+            fd = -1
+            try:
+                pos = self.fp.tell()
+                self.fp.seek(0, io.SEEK_END)
+                length = self.fp.tell()
+                self.fp.seek(pos)
+            except Exception:
+                length = -1
+
+        self.tile = [
+            (
+                "jpeg2k",
+                (0, 0) + self.size,
+                0,
+                (self.codec, self._reduce, self.layers, fd, length),
             )
-        
-        if quoted := soup.find(class_="quoted-mention"):
-
-            self.quote = self.Quote(
-                text=parse_message(quoted), 
-                author=quoted.parent.parent.span.text
-            )
-        
-        if soup.find("span", attrs={"data-testid": "forwarded"}):
-            self.forwarded = True
-
-    def _get_options(self):
-
-        self._driver.execute_script("""
-            var event = new MouseEvent('mouseover', {
-                'view': window,
-                'bubbles': true,
-                'cancelable': true
-            });
-
-            var element = arguments[0].querySelector("div");
-
-            element.dispatchEvent(event);
-        """, self._element)
-
-        self._element.find_elements(By.CSS_SELECTOR, 'span[data-testid="down-context"]').click()
-
-        return self._driver.find_elements(By.CSS_SELECTOR, "ul > div > li")
-
-    def forward(self, contacts: List[str]) -> None:
-        """Forwards the selected message to all listed contacts
-
-        Keep in mind that the message won't be avaliable anymore,
-        because it will leave the current chat
-
-        Args:
-            contacts (List[str]): A list with contacts name
-        """
-
-        options = self._get_options()
-        options[-3 if (self._chat.__class__.__name__ == "Contact") else -4].click()
-        
-        self._driver.find_element(By.CSS_SELECTOR, "span[data-testid=forward]").click()
-
-        search_box = self._driver.find_element(By.CSS_SELECTOR, 'div[role="textbox"]')
-
-        for contact in contacts:
-            search_box.send_keys(contact)
-            search_box.send_keys(Keys.ENTER)
-        
-        self._driver.find_element(By.CSS_SELECTOR, 'div[role="button"]').click()
-
-        self._chat._open_chat()
-
-    def reply(self, message: str = "", file: str = "") -> None:
-        """Replies to the selected message
-
-        Args:
-            message (str): The message you want to send
-        """
-
-        _actionChains = ActionChains(self._element.parent)
-
-        _actionChains.double_click(self._element).perform()
-        self._chat.send(message, file)
-
-    def reply_privately(self, message: str = "", file: str = "") -> None:
-        """Sends a message message privatly to the selected message
-
-        Args:
-            message (str): The message you want to send
-        """
-
-        if self._chat.__class__.__name__ == "Contact":
-            raise PermissionError("You cannot reply privately in a private chat")
-
-        options = self._get_options()
-        options[1].click()
-        sleep(.1)
-        
-        self._chat.send(message, file)
-        self._chat._open_chat()
-
-    def delete(self) -> None:
-        """Deletes the selected message"""
-
-        options = self._get_options()
-        options[-1 if (self._chat.__class__.__name__ == "Contact") else -2].click()
-        
-        self._driver.find_element(By.CSS_SELECTOR, 'div:nth-child(2)[role="button"]').click()
-
-    def star(self) -> None:
-        """Stars the selected message"""
-
-        options = self._get_options()
-        options[-2 if (self._chat.__class__.__name__ == "Contact") else -3].click()
-
-
-@dataclass
-class Document(Text):
-
-    @dataclass
-    class File:
-        size: int = 0
-        name: str = ""
-        mimetype: str = ""
-        content: bytes = field(repr=False, default=b"")
-
-    file: File = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        mimetypes.init()
-
-        soup = to_soup(self._element)
-        for span in soup.find_all("span"):
-            file_name = span.text
-            if Path(file_name).suffix:
-                file_type = mimetypes.types_map[Path(file_name).suffix]
-                break
-
-        # Download file
-        self._element.find_element(By.CSS_SELECTOR, 'button').click()
+        ]
 
-        file_path = str(Path.home()/"Downloads"/file_name)
+    def _parse_comment(self):
+        hdr = self.fp.read(2)
+        length = _binary.i16be(hdr)
+        self.fp.seek(length - 2, os.SEEK_CUR)
 
         while True:
-            if Path(file_path).is_file():
+            marker = self.fp.read(2)
+            if not marker:
                 break
+            typ = marker[1]
+            if typ in (0x90, 0xD9):
+                # Start of tile or end of codestream
+                break
+            hdr = self.fp.read(2)
+            length = _binary.i16be(hdr)
+            if typ == 0x64:
+                # Comment
+                self.info["comment"] = self.fp.read(length - 2)[2:]
+                break
+            else:
+                self.fp.seek(length - 2, os.SEEK_CUR)
 
-        with open(file_path, "rb") as f:
-            file_content = f.read()
-            file_size = len(file_content)
-
-        Path(file_path).unlink()
-        self.file = self.File(
-            name=file_name, 
-            mimetype=file_type, 
-            size=file_size, 
-            content=file_content
-        )
-
-
-@dataclass
-class Video(Text):
-
-    length: int = 0
-
-    def __post_init__(self):
-        super().__post_init__()
-        soup = to_soup(self._element)
-
-        length_str = (
-            soup.find("span", attrs={"data-testid": "msg-video"})
-            .parent.parent.text
-            .split(":")
-        )
-        self.length = (int(length_str[0]) * 60) + int(length_str[1])
-    
-    def forward(self):
-        if self.forwarded:
-            raise PermissionError("You cannot forward a forwarded Video")
-
-        super().forward()
-
-
-@dataclass
-class Audio(Text):
-
-    @dataclass
-    class File:
-        size: int = 0
-        length: int = 0
-        content: bytes = field(repr=False, default=b"")
-
-    file: File = None
-    isrecorded: bool = False
-
-    def __post_init__(self):
-        super().__post_init__()
-
-        def process_browser_log_entry(entry):
-            response = json.loads(entry['message'])['message']
-            return response
-        
-        soup = to_soup(self._element)
-
-        length_str = soup.find("div", attrs={"aria-hidden": "true"}).text.split(":")
-        length = (int(length_str[0]) * 60) + int(length_str[1])
-
-        # Play Audio
-        self._element.find_element(By.CSS_SELECTOR, 'button').click()
-        sleep(.05)
-        # Stop Audio
-        self._element.find_element(By.CSS_SELECTOR, 'button').click()
-
-        logs = self._driver.get_log('performance') 
-        events = [process_browser_log_entry(entry) for entry in logs]
-        events = [
-            event for event in events 
-            if 'Network.response' in event['method'] and
-            "response" in event["params"].keys() and
-            "blob" in event["params"]["response"]["url"]
-        ]
-
-        content = blob_to_bytes(
-            self._driver, 
-            events[-1]["params"]["response"]["url"]
-        )
-
-        size = len(content)
-
-        self.file = self.File(size=size, length=length, content=content)
-
-
-@dataclass
-class ContactCard(Text):
-
-    @dataclass
-    class Contact:
-        name: str = ""
-        numbers: List[str] = field(default_factory=list)
-
-    contacts: List[Contact] = field(default_factory=list)
-
-    def __post_init__(self):
-        super().__post_init__()
-        self._element.find_element(By.CSS_SELECTOR, 'div[role="button"]').click()
-
-        soup = to_soup(self._driver.find_element(By.CSS_SELECTOR, "body"))
-        contact_elements = [
-            contact.parent for contact in soup
-            .select(".copyable-area:not(.overlay)")[0]
-            .find_all("div", attrs={"data-testid": "cell-frame-container"})
-        ]
-        
-        for contact in contact_elements:
-
-            self.contacts.append( 
-                self.Contact(
-                    name=contact.find("span", attrs={"dir": "auto"}, class_="copyable-text").text,
-                    numbers=[number.text for number in contact.find_all("div", class_="copyable-text")]
-                )
-            )
-
-        sleep(0.1)
-        self._driver.find_element(By.CSS_SELECTOR, 'button[aria-label="Close"]').click()
-
-
-@dataclass
-class Location(Text):
-
-    coords: tuple = ()
-    link: str = ""
-
-    def __post_init__(self):
-        soup = to_soup(self._element)
-
-        self.link = soup.find("a")["href"]
-        self.coords = tuple(
-            re.compile("[-]?[\d]+[.][\d]*")
-            .findall(self.link)
-        )
-
-
-@dataclass
-class LiveLocation(Location):
-
-    until: datetime = None
-
-    def __post_init__(self):
-        soup = to_soup(self._element)
-        driver_find = self._element.parent.find_element_by_css_selector
-        
-        if active := soup.find("span", attrs={"data-testid": "live-location-active-android"}):
-
-            regex = re.compile("(\d{1,2}\:\d{2}\s?(?:AM|PM|am|pm))")
-            until_str = active.parent.parent.text
-            time_msg = regex.findall(until_str)[0]
-
-            self.until = (
-                datetime.strptime(time_msg, "%I:%M %p")
-                if ("AM" in time_msg) or ("PM" in time_msg)
-                else datetime.strptime(time_msg, "%H:%M")
+    @property
+    def reduce(self):
+        # https://github.com/python-pillow/Pillow/issues/4343 found that the
+        # new Image 'reduce' method was shadowed by this plugin's 'reduce'
+        # property. This attempts to allow for both scenarios
+        return self._reduce or super().reduce
+
+    @reduce.setter
+    def reduce(self, value):
+        self._reduce = value
+
+    def load(self):
+        if self.tile and self._reduce:
+            power = 1 << self._reduce
+            adjust = power >> 1
+            self._size = (
+                int((self.size[0] + adjust) / power),
+                int((self.size[1] + adjust) / power),
             )
-        
-
-        today = datetime.now()
-        self.until.replace(
-            year=today.year,
-            month=today.month,
-            day=today.day
-        )
 
-        self._element.find_element_by_css_selector("img")\
-            .find_element_by_xpath('..')\
-            .click()
-        
-        while not driver_find("a[rel=noopener]").is_displayed():
-            pass
-
-        self.link = (
-            driver_find("a[rel=noopener]")
-            .get_property("href")
+            # Update the reduce and layers settings
+            t = self.tile[0]
+            t3 = (t[3][0], self._reduce, self.layers, t[3][3], t[3][4])
+            self.tile = [(t[0], (0, 0) + self.size, t[2], t3)]
+
+        return ImageFile.ImageFile.load(self)
+
+
+def _accept(prefix):
+    return (
+        prefix[:4] == b"\xff\x4f\xff\x51"
+        or prefix[:12] == b"\x00\x00\x00\x0cjP  \x0d\x0a\x87\x0a"
+    )
+
+
+# ------------------------------------------------------------
+# Save support
+
+
+def _save(im, fp, filename):
+    # Get the keyword arguments
+    info = im.encoderinfo
+
+    if filename.endswith(".j2k") or info.get("no_jp2", False):
+        kind = "j2k"
+    else:
+        kind = "jp2"
+
+    offset = info.get("offset", None)
+    tile_offset = info.get("tile_offset", None)
+    tile_size = info.get("tile_size", None)
+    quality_mode = info.get("quality_mode", "rates")
+    quality_layers = info.get("quality_layers", None)
+    if quality_layers is not None and not (
+        isinstance(quality_layers, (list, tuple))
+        and all(
+            [
+                isinstance(quality_layer, (int, float))
+                for quality_layer in quality_layers
+            ]
         )
-        self.coords = tuple(
-            re.compile("[-]?[\d]+[.][\d]*")
-            .findall(self.link)
-        )
-        
-        driver_find('button[aria-label="Close"]').click()
-
-    def forward(self):
-        raise PermissionError("You cannot forward a LiveLocation")
-
-
-@dataclass
-class Image(Text):
-
-    @dataclass
-    class File:
-        size: int = 0
-        resolution: tuple = ()
-        content: bytes = field(repr=False, default=b"")
-
-    file: File = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        soup = to_soup(self._element)
-
-        for img in soup.findAll("img"):
-            if "web.whatsapp.com" in img["src"]:
-                content = blob_to_bytes(driver=self._element.parent, url=img["src"])
-                break
-
-        size = len(content)
-        
-        image = PILImage.open(BytesIO(content))
-        resolution = image.size
-
-        self.file = self.File(size=size, resolution=resolution, content=content)
-
+    ):
+        msg = "quality_layers must be a sequence of numbers"
+        raise ValueError(msg)
+
+    num_resolutions = info.get("num_resolutions", 0)
+    cblk_size = info.get("codeblock_size", None)
+    precinct_size = info.get("precinct_size", None)
+    irreversible = info.get("irreversible", False)
+    progression = info.get("progression", "LRCP")
+    cinema_mode = info.get("cinema_mode", "no")
+    mct = info.get("mct", 0)
+    signed = info.get("signed", False)
+    comment = info.get("comment")
+    if isinstance(comment, str):
+        comment = comment.encode()
+    plt = info.get("plt", False)
+
+    fd = -1
+    if hasattr(fp, "fileno"):
+        try:
+            fd = fp.fileno()
+        except Exception:
+            fd = -1
+
+    im.encoderconfig = (
+        offset,
+        tile_offset,
+        tile_size,
+        quality_mode,
+        quality_layers,
+        num_resolutions,
+        cblk_size,
+        precinct_size,
+        irreversible,
+        progression,
+        cinema_mode,
+        mct,
+        signed,
+        fd,
+        comment,
+        plt,
+    )
+
+    ImageFile._save(im, fp, [("jpeg2k", (0, 0) + im.size, 0, kind)])
+
+
+# ------------------------------------------------------------
+# Registry stuff
+
+
+Image.register_open(Jpeg2KImageFile.format, Jpeg2KImageFile, _accept)
+Image.register_save(Jpeg2KImageFile.format, _save)
+
+Image.register_extensions(
+    Jpeg2KImageFile.format, [".jp2", ".j2k", ".jpc", ".jpf", ".jpx", ".j2c"]
+)
 
-@dataclass
-class Sticker(Image):
-    ...
+Image.register_mime(Jpeg2KImageFile.format, "image/jp2")
```

