# Comparing `tmp/ccdt-2.0.5.tar.gz` & `tmp/ccdt-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.0.5.tar", last modified: Tue May  9 03:39:17 2023, max compression
+gzip compressed data, was "ccdt-2.0.6.tar", last modified: Tue May  9 03:48:11 2023, max compression
```

## Comparing `ccdt-2.0.5.tar` & `ccdt-2.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.702766 ccdt-2.0.5/
--rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.5/LICENSE
--rw-rw-rw-   0        0        0     4319 2023-05-09 03:39:17.700771 ccdt-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.618990 ccdt-2.0.5/ccdt/
--rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.5/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.644921 ccdt-2.0.5/ccdt/dataset/
--rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.5/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.650905 ccdt-2.0.5/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.5/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.5/ccdt/dataset/base_coco/coco.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.667859 ccdt-2.0.5/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.5/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.5/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    63557 2023-05-09 03:33:39.000000 ccdt-2.0.5/ccdt/dataset/base_labelme/base_labelme.py
--rw-rw-rw-   0        0        0      471 2023-05-08 06:44:57.000000 ccdt-2.0.5/ccdt/dataset/base_labelme/test_async_io.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.670851 ccdt-2.0.5/ccdt/dataset/logs/
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.5/ccdt/dataset/logs/__init__.py
--rw-rw-rw-   0        0        0    12313 2023-05-09 02:47:26.000000 ccdt-2.0.5/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.688803 ccdt-2.0.5/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      269 2023-05-09 02:06:21.000000 ccdt-2.0.5/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      843 2023-05-09 02:18:17.000000 ccdt-2.0.5/ccdt/dataset/utils/async_dirIterator.py
--rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.5/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    17244 2023-05-09 03:37:25.000000 ccdt-2.0.5/ccdt/dataset/utils/labelme_load.py
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.5/ccdt/dataset/utils/logs.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.697780 ccdt-2.0.5/ccdt/video_tool/
--rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.5/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.5/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.5/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.637939 ccdt-2.0.5/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4319 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 03:39:17.703763 ccdt-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2278 2023-05-09 03:37:58.000000 ccdt-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.501571 ccdt-2.0.6/
+-rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4319 2023-05-09 03:48:11.499577 ccdt-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.426772 ccdt-2.0.6/ccdt/
+-rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.6/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.450707 ccdt-2.0.6/ccdt/dataset/
+-rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.6/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.456690 ccdt-2.0.6/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.6/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.6/ccdt/dataset/base_coco/coco.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.469656 ccdt-2.0.6/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.6/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.6/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    63557 2023-05-09 03:33:39.000000 ccdt-2.0.6/ccdt/dataset/base_labelme/base_labelme.py
+-rw-rw-rw-   0        0        0      471 2023-05-08 06:44:57.000000 ccdt-2.0.6/ccdt/dataset/base_labelme/test_async_io.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.472648 ccdt-2.0.6/ccdt/dataset/logs/
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.6/ccdt/dataset/logs/__init__.py
+-rw-rw-rw-   0        0        0    12313 2023-05-09 02:47:26.000000 ccdt-2.0.6/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.487609 ccdt-2.0.6/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      251 2023-05-09 03:47:20.000000 ccdt-2.0.6/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      894 2023-05-09 03:47:20.000000 ccdt-2.0.6/ccdt/dataset/utils/async_dirIterator.py
+-rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.6/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    17244 2023-05-09 03:37:25.000000 ccdt-2.0.6/ccdt/dataset/utils/labelme_load.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.6/ccdt/dataset/utils/logs.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.496586 ccdt-2.0.6/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.6/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.6/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.6/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:48:11.443725 ccdt-2.0.6/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4319 2023-05-09 03:48:11.000000 ccdt-2.0.6/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2023-05-09 03:48:11.000000 ccdt-2.0.6/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 03:48:11.000000 ccdt-2.0.6/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-09 03:48:11.000000 ccdt-2.0.6/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-05-09 03:48:11.000000 ccdt-2.0.6/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-09 03:48:11.000000 ccdt-2.0.6/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 03:48:11.501571 ccdt-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2278 2023-05-09 03:47:20.000000 ccdt-2.0.6/setup.py
```

### Comparing `ccdt-2.0.5/LICENSE` & `ccdt-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/PKG-INFO` & `ccdt-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.5
+Version: 2.0.6
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.5/README.md` & `ccdt-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt/dataset/base_coco/coco.py` & `ccdt-2.0.6/ccdt/dataset/base_coco/coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.0.6/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.0.6/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt/dataset/main.py` & `ccdt-2.0.6/ccdt/dataset/main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt/dataset/utils/async_dirIterator.py` & `ccdt-2.0.6/ccdt/dataset/utils/async_dirIterator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import aiofiles
-import os
-from aiofiles.os import scandir
-
-
-class AsyncDirIterator(object):
-    def __init__(self, *args, **kwargs):
-        self.path = args[0]
-
-    async def load_data_info(self):
-        files = []
-
-        async for entry in aiofiles.os.scandir(self.path):
-            if entry.is_file():
-                files.append(os.path.abspath(entry.path))
-            # elif entry.is_dir():
-            #     subfiles = await list_files(entry.path)
-            #     files.extend(subfiles)
-        return files
-
-    # async def __aiter__(self):
-    #     async with aiofiles.os.scandir(self.path) as scan_dir:
-    #         async for entry in scan_dir:
-    #             if entry.is_file():
-    #                 yield entry.name
-    #
-    # async def __anext__(self):
-    #     raise StopAsyncIteration
+# import aiofiles
+# import os
+# from aiofiles.os import scandir
+#
+#
+# class AsyncDirIterator(object):
+#     def __init__(self, *args, **kwargs):
+#         self.path = args[0]
+#
+#     async def load_data_info(self):
+#         files = []
+#
+#         async for entry in aiofiles.os.scandir(self.path):
+#             if entry.is_file():
+#                 files.append(os.path.abspath(entry.path))
+#             # elif entry.is_dir():
+#             #     subfiles = await list_files(entry.path)
+#             #     files.extend(subfiles)
+#         return files
+#
+#     # async def __aiter__(self):
+#     #     async with aiofiles.os.scandir(self.path) as scan_dir:
+#     #         async for entry in scan_dir:
+#     #             if entry.is_file():
+#     #                 yield entry.name
+#     #
+#     # async def __anext__(self):
+#     #     raise StopAsyncIteration
```

### Comparing `ccdt-2.0.5/ccdt/dataset/utils/encoder.py` & `ccdt-2.0.6/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.0.6/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt/video_tool/split.py` & `ccdt-2.0.6/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt/video_tool/video_main.py` & `ccdt-2.0.6/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/ccdt.egg-info/PKG-INFO` & `ccdt-2.0.6/ccdt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.5
+Version: 2.0.6
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.5/ccdt.egg-info/SOURCES.txt` & `ccdt-2.0.6/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.5/setup.py` & `ccdt-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.0.5',
+    version='2.0.6',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

