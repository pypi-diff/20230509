# Comparing `tmp/ccdt-2.0.4.tar.gz` & `tmp/ccdt-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.0.4.tar", last modified: Thu May  4 05:52:42 2023, max compression
+gzip compressed data, was "ccdt-2.0.5.tar", last modified: Tue May  9 03:39:17 2023, max compression
```

## Comparing `ccdt-2.0.4.tar` & `ccdt-2.0.5.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.561290 ccdt-2.0.4/
--rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.4/LICENSE
--rw-rw-rw-   0        0        0     4319 2023-05-04 05:52:42.560298 ccdt-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.501431 ccdt-2.0.4/ccdt/
--rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.4/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.523372 ccdt-2.0.4/ccdt/dataset/
--rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.4/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.528358 ccdt-2.0.4/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.4/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.4/ccdt/dataset/base_coco/coco.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.536337 ccdt-2.0.4/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.4/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.4/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    60750 2023-05-04 05:50:19.000000 ccdt-2.0.4/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.538357 ccdt-2.0.4/ccdt/dataset/logs/
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.4/ccdt/dataset/logs/__init__.py
--rw-rw-rw-   0        0        0    11343 2023-04-27 08:58:08.000000 ccdt-2.0.4/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.549301 ccdt-2.0.4/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      200 2023-04-17 07:06:14.000000 ccdt-2.0.4/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.4/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    10182 2023-04-25 10:32:57.000000 ccdt-2.0.4/ccdt/dataset/utils/labelme_load.py
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.4/ccdt/dataset/utils/logs.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.556315 ccdt-2.0.4/ccdt/video_tool/
--rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.4/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.4/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.4/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.517418 ccdt-2.0.4/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4319 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 05:52:42.562268 ccdt-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2278 2023-05-04 05:52:04.000000 ccdt-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.702766 ccdt-2.0.5/
+-rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4319 2023-05-09 03:39:17.700771 ccdt-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.618990 ccdt-2.0.5/ccdt/
+-rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.5/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.644921 ccdt-2.0.5/ccdt/dataset/
+-rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.5/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.650905 ccdt-2.0.5/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.5/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.5/ccdt/dataset/base_coco/coco.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.667859 ccdt-2.0.5/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.5/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.5/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    63557 2023-05-09 03:33:39.000000 ccdt-2.0.5/ccdt/dataset/base_labelme/base_labelme.py
+-rw-rw-rw-   0        0        0      471 2023-05-08 06:44:57.000000 ccdt-2.0.5/ccdt/dataset/base_labelme/test_async_io.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.670851 ccdt-2.0.5/ccdt/dataset/logs/
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.5/ccdt/dataset/logs/__init__.py
+-rw-rw-rw-   0        0        0    12313 2023-05-09 02:47:26.000000 ccdt-2.0.5/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.688803 ccdt-2.0.5/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      269 2023-05-09 02:06:21.000000 ccdt-2.0.5/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      843 2023-05-09 02:18:17.000000 ccdt-2.0.5/ccdt/dataset/utils/async_dirIterator.py
+-rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.5/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    17244 2023-05-09 03:37:25.000000 ccdt-2.0.5/ccdt/dataset/utils/labelme_load.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.5/ccdt/dataset/utils/logs.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.697780 ccdt-2.0.5/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.5/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.5/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.5/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:39:17.637939 ccdt-2.0.5/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4319 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-09 03:39:17.000000 ccdt-2.0.5/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 03:39:17.703763 ccdt-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2278 2023-05-09 03:37:58.000000 ccdt-2.0.5/setup.py
```

### Comparing `ccdt-2.0.4/LICENSE` & `ccdt-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.4/PKG-INFO` & `ccdt-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.4
+Version: 2.0.5
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.4/README.md` & `ccdt-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.4/ccdt/dataset/base_coco/coco.py` & `ccdt-2.0.5/ccdt/dataset/base_coco/coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.4/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.0.5/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.4/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.0.5/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,23 +52,23 @@
         self.datasets = args[0]
         self.check_error_dataset = list()  # 存储错误图像数据变量列表
         self.error_output_path = ''  # 定义全局错误输出路径变量
         self.error_image_path = ''  # 定义全局图像路径变量
         self.automatic_correction = list()  # 定义存放逻辑处理后封装数据的存放列表
         self.output_dir = ''  # 自定义数据保存输入目录，用于传参时灵活使用
 
+    # async def process_item(self, item, custom_label):
+    #     # 在协程中进行数据处理
+    #     # 模拟处理1秒钟
+    #     await asyncio.sleep(1)
+    #     print(f'封装的数据，{item}传递的参数{custom_label}')
+    #     # 返回处理结果
+    #     return f"Process item {item} with label {custom_label}"
+
     def save_labelme(self, output_dir, index, custom_label):
-        """
-        保存数据功能，主要实现图片拷贝、json文件重写
-        使用异步编程：Python的asyncio模块提供了异步编程的支持，可以在执行IO操作期间允许程序在其他任务中并行执行。
-        :param output_dir: 形参变量，传递列表、字符串、None
-        :param index: 形参变量，传递索引数字、bool值
-        :param custom_label:自定义标签名称，用于抽取份数时重组目录
-        :return:
-        """
         # ==============================异步写内存数据到磁盘操作==================================================
         tasks = list()
         loop = asyncio.get_event_loop()
         async_time = time.time()
         if isinstance(output_dir, str) or output_dir is None:
             tasks = [AsyncIoTask.json_dump(data_info, output_dir, None, custom_label) for data_info in
                      tqdm(self.datasets)]
@@ -79,14 +79,48 @@
             print(output_dir)
             print(self.datasets)
             exit()
         loop.run_until_complete(asyncio.wait(tasks))
         print('异步耗时')
         print(time.time() - async_time)
         # ==============================异步写内存数据到磁盘操作==================================================
+        # async def save_labelme(self, output_dir, index, custom_label):
+        """
+        保存数据功能，主要实现图片拷贝、json文件重写
+        使用异步编程：Python的asyncio模块提供了异步编程的支持，可以在执行IO操作期间允许程序在其他任务中并行执行。
+        :param output_dir: 形参变量，传递列表、字符串、None
+        :param index: 形参变量，传递索引数字、bool值
+        :param custom_label:自定义标签名称，用于抽取份数时重组目录
+        :return:
+        """
+        # *******************************定义任务的协程函数，并用asyncio.gather()协程函数来并发执行所有协程任务*******************
+        # 在协程中处理数据
+        # async_time = time.time()
+        # try:
+        #     # 创建协程任务列表
+        #     tasks = []
+        #     if isinstance(output_dir, list) and output_dir != []:  # 传递列表，传递索引
+        #         for item in output_dir:
+        #             # 创建协程任务
+        #             task = asyncio.create_task(AsyncIoTask.json_dump(item, True, index, custom_label))
+        #             tasks.append(task)
+        #     if isinstance(output_dir, str) or output_dir is None:
+        #         for item in self.datasets:
+        #             # 创建协程任务
+        #             task = asyncio.create_task(AsyncIoTask.json_dump(item, True, index, custom_label))
+        #             tasks.append(task)
+        #     # 同时执行所有的协程任务
+        #     await asyncio.wait_for(asyncio.gather(*tasks), timeout=0)  # 无需返回结果
+        #     # results = await asyncio.wait_for(asyncio.gather(*tasks), timeout=0)
+        #     # return results
+        # except Exception as e:
+        #     print(f'执行协程出错，报告开发人员{e}')
+        # print('异步耗时')
+        # print(time.time() - async_time)
+        # *******************************定义任务的协程函数，并用asyncio.gather()协程函数来并发执行所有协程任务*******************
 
     def rename_labelme(self, parameter):
         """
         重命名功能实现，包含label和flags
         :param parameter:
         """
         print(f'重命名label标签名称')
@@ -211,14 +245,27 @@
             print(f'拷贝labelme数据处理')
             # 按指定份数抽取labelme数据集
             if parameter.extract_portion and parameter.extract_portion > 0:
                 self.split_list(parameter)
                 # 指定张数抽取
             elif parameter.extract_amount and parameter.extract_amount > 0:
                 self.save_labelme(random.sample(self.datasets, parameter.extract_amount), parameter.select_cut, None)
+            elif isinstance(parameter.extract_text, list):
+                print(f'抽取text字段的文本内容数据处理')
+                # text_list = list()
+                for index, dataset in tqdm(enumerate(self.datasets)):
+                    if dataset.get('background') is False:
+                        for shape in dataset.get('labelme_info').get('shapes'):
+                            num_rounded = shape.get('text')[:shape.get('text').find('.') + 2]  # 取小数点后一位并截断  # 保留一位小数
+                            if num_rounded in parameter.extract_text:
+                                continue
+                            else:
+                                del self.datasets[index]
+                print(f'保存抽取数据集')
+                self.save_labelme(parameter.output_dir, None, None)
             else:
                 print(f'抽取份数不能为零：{parameter.extract_portion}{parameter.extract_amount}')
                 exit()
         if parameter.select_cut is True:  # 剪切
             print(f'剪切labelme数据处理')
             # 按照指定数量抽取labelme数据集
             if parameter.extract_amount and parameter.extract_amount > 0:
@@ -570,15 +617,15 @@
         这个算法的时间复杂度为 O(n)，其中n 是多边形的点数。
         :param polygon:
         :param file_path:
         """
         if len(polygon.get('points')) == 4:
             # 初始化最左、最右、最上和最下的点为多边形的第一个点
             leftmost, rightmost, topmost, bottommost = polygon.get('points')[0], polygon.get('points')[0], \
-                                                       polygon.get('points')[0], polygon.get('points')[0]
+                polygon.get('points')[0], polygon.get('points')[0]
 
             # 遍历多边形的每一个点，并更新最左、最右、最上和最下的点的坐标值
             for point in polygon.get('points'):
                 if point[0] < leftmost[0]:
                     leftmost = point
                 if point[0] > rightmost[0]:
                     rightmost = point
@@ -720,15 +767,16 @@
             if repeat_data.get('md5_value') not in md5_list:  # 如果md5值重复直接删除元素
                 md5_list.append(repeat_data.get('md5_value'))
             else:
                 # del self.datasets[index]
                 del_num += 1
                 os.remove(repeat_data.get('full_path'))
                 os.remove(repeat_data.get('json_path'))
-        print(f'去重前文件数量有{len(self.datasets)}，去重后文件数量有{len(self.datasets)- del_num}，删除重复的文件有{del_num}')
+        print(
+            f'去重前文件数量有{len(self.datasets)}，去重后文件数量有{len(self.datasets) - del_num}，删除重复的文件有{del_num}')
 
     def check_group_labelme(self, parameter):
         """
         labelme数据集检查功能实现，包含标注多边形点数错误、标注分组错误、标注越界错误、标注flags属性错误、
         :param parameter:
         """
         if isinstance(parameter.judging_polygon, int):  # 检查多边形点是否超出5个点
```

### Comparing `ccdt-2.0.4/ccdt/dataset/main.py` & `ccdt-2.0.5/ccdt/dataset/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 # -*- coding: utf-8 -*-
 # @Time : 2023/3/30 16:23
 # @Author : Zhan Yong
 # @System : jk
 import argparse
 import ast
+import asyncio
 from ccdt.dataset import *
 
 
 def parser_args():
     parser = argparse.ArgumentParser()
     parser.add_argument('input_datasets', type=ast.literal_eval, help="labelme数据集路径、coco数据集路径，列表字典传参")
     parser.add_argument('--output-dir', type=str, help="保存路径")
     # parser.add_argument('--replace-dir', type=str, help="替换路径")
     parser.add_argument('--output-format', type=str, help="输出功能格式，有labelme、coco")
     parser.add_argument('-f', '--function', type=str, required=True,
                         help="功能参数:print,convert,filter,matting,rename,visualize,merge，只能输入单个")
     parser.add_argument('--filter-label', type=ast.literal_eval, help="类别筛选参数，单个与多个都可以输入")
     # 当不输入--only_annotation，默认为False；输入--only_annotation，才会触发True值。False处理labelme和图片，True只处理labelme
-    parser.add_argument('--only-annotation', action="store_true", help="默认False，是否只处理注释文件。是为True，否为False")
+    parser.add_argument('--only-annotation', action="store_true",
+                        help="默认False，是否只处理注释文件。是为True，否为False")
     parser.add_argument('--filter-shape-type', type=ast.literal_eval, help="形状筛选参数，单个与多个都可以输入")
     parser.add_argument('--input-coco-file', type=str, help="输入形状筛选参数，单个与多个都可以输入")
     parser.add_argument('--rename-attribute', type=ast.literal_eval, help="属性重命名，包含label、flags")
     parser.add_argument('--select-empty', action="store_true", help="默认False，是否保留背景类。是为True，否为False")
-    parser.add_argument('--only-select-empty', action="store_true", help="默认False，是否只筛选背景数据。是为True，否为False")
-    parser.add_argument('--only-select-shapes', action="store_true", help="默认False，是否只筛选标注有框的数据。是为True，否为False")
+    parser.add_argument('--only-select-empty', action="store_true",
+                        help="默认False，是否只筛选背景数据。是为True，否为False")
+    parser.add_argument('--only-select-shapes', action="store_true",
+                        help="默认False，是否只筛选标注有框的数据。是为True，否为False")
     # parser.add_argument('--only-empty', action="store_true", help="默认False，不保留背景类。传参则设置为True，只保留背景类")
-    parser.add_argument('--shapes-attribute', type=str, help="筛选属性，包含label（类别）、shape_type（类别形状）、flags（类别属性）")
+    parser.add_argument('--shapes-attribute', type=str,
+                        help="筛选属性，包含label（类别）、shape_type（类别形状）、flags（类别属性）")
     parser.add_argument('--filter-flags', type=ast.literal_eval,
                         help="类别属性筛选，输入类别属性字典列表。比如person类下有，手、脚、头")
     parser.add_argument('--file_formats', default=['.jpg', '.jpeg', '.png', '.JPEG', '.JPG', '.PNG'], type=str,
                         help="文件格式")
     parser.add_argument('--filter-combin', action="store_true", help="是否组合筛选，是为True，否为False")
     parser.add_argument('--extract-portion', type=int, help='按照指定份数平均抽取，比如400张图像，抽取10分，每份40张')
+    parser.add_argument('--extract-text', type=ast.literal_eval, help='按照text字段的文本内容抽取')
     parser.add_argument('--select-cut', action="store_true", help="默认False即拷贝，是拷贝还是剪切。是为True，否为False")
     parser.add_argument('--extract-amount', type=int, help='按照指定数量抽取，比如400张图像，抽取100张')
     parser.add_argument('--print-more', action="store_true", help="打印详细信息")
-    parser.add_argument('--del-label', type=str, help="删除label标签")
+    parser.add_argument('--del-label', type=ast.literal_eval, help="删除label标签")
     parser.add_argument('--label-name', type=str, help="自定义label标签，用于抽取份数时区别标注目录")
     parser.add_argument('--http-url', type=str,
                         help="minio文件对象存储中，网络文件统一资源定位器，http://192.168.1.235:9393/chipeak-dataset")
-    parser.add_argument('--min-pixel', type=int, default=512, help='最小像素截图设置，默认512像素。即大于512像素的矩形框才进行截图')
+    parser.add_argument('--min-pixel', type=int, default=512,
+                        help='最小像素截图设置，默认512像素。即大于512像素的矩形框才进行截图')
     parser.add_argument('--judging-group', type=int, help='默认值为2个shape元素为一组，用于判断分组元素的数量')
     # parser.add_argument('--judging-flags', type=json.loads, help="检查flags默认标注属性，是否符合标注准则")
     parser.add_argument('--judging-flags', type=ast.literal_eval, help="检查flags默认标注属性，是否符合标注准则")
-    parser.add_argument('--judging-polygon', type=int, help='检查多边形标注的点是否超出预期数量，比如4个点的多边形，不能出现5个')
+    parser.add_argument('--judging-polygon', type=int,
+                        help='检查多边形标注的点是否超出预期数量，比如4个点的多边形，不能出现5个')
     parser.add_argument('--judging-cross-the-border', type=str, help="检查标注形状是否超越原始图像边界")
-    parser.add_argument('--point-number', type=int, help='点标注的数量，用于标注点排序时，追加标注点到列表中然后判断，是否满足标注规则')
-    parser.add_argument('--automatic-correction', action="store_true", help="默认False，是否自动矫正标注形状超越图像边界情况。是为True，否为False")
+    parser.add_argument('--point-number', type=int,
+                        help='点标注的数量，用于标注点排序时，追加标注点到列表中然后判断，是否满足标注规则')
+    parser.add_argument('--automatic-correction', action="store_true",
+                        help="默认False，是否自动矫正标注形状超越图像边界情况。是为True，否为False")
 
     args = parser.parse_args()
     if args.function == 'filter_positive':  # 筛选正样本
         return args
     elif args.function == 'filter_negative':  # 筛选负样本
         return args
     elif args.function == 'filter_label':  # 筛选负样本
@@ -96,22 +106,32 @@
         return args
     elif args.function == 'cross':  # 针对标注形状超越图像边界情况，使用程序自动矫正
         return args
     else:
         assert not args.function, '传入的操作功能参数不对:{}'.format(args.function)
 
 
+# async def main():
 def main():
     args = parser_args()
     data_info = LabelmeLoad(args)  # 初始化输入参数
+    # async_obj = AsyncDirIterator(args)
+    # data_info = await async_obj.load_data_info()
+
     if args.function == 'compress':  # 对抽取数据集进行压缩。数据压缩无需对数据进行封装后操作
         zip_package = data_info.compress_labelme()  # 封装压缩路径及压缩对象
         data_info.make_compress(zip_package)  # 开始压缩
     else:
-        dataset_info = data_info.get_dir_currency()
+        import time
+        async_time = time.time()
+        data_info = LabelmeLoad(args)  # 初始化输入参数
+        dataset_info = data_info.get_multiprocess_dir_currency()  # 多进程封装数据处理
+        # dataset_info = data_info.get_dir_currency()  # 单进程封装数据处理
+        print('异步耗时')
+        print(time.time() - async_time)
         dataset = BaseLabelme(dataset_info)  # 初始化labelme基类
         if args.function == 'merge':  # 合并功能
             dataset.merge_labelme(args)
             # BaseLabelme.merge(datasets)
         elif args.function == 'matting':  # 抠出标注位置保存labelme
             dataset.intercept_coordinates()
         elif args.function == 'duplicate':  # 对labelme数据集进行去重，重复的图片就删除
@@ -140,23 +160,26 @@
         elif args.function == 'print':  # 打印功能
             dataset.__repr__()
         elif args.function == 'check_image_path':  # 检查image_path功能
             dataset.check_image_path()
         elif args.function == 'delete':  # 删除指定标签类别标注数据集
             dataset.del_label(args.del_label)
             print(f'保存指定label类别进行删除的labelme数据集')
-            dataset.save_labelme(args.output_dir, None, None)
+            # await dataset.save_labelme(args.output_dir, None, None)
         elif args.function == 'extract':  # 抽取labelme数据集功能，指定份数抽取，只允许拷贝；指定图像张数抽取，允许剪切、拷贝
+            # await dataset.extract_labelme(args)
             dataset.extract_labelme(args)
         elif args.function == 'relation':  # 寻找标注形状包含关系，进行自动打组
             dataset.relation_labelme(args)
         elif args.function == 'check':  # 检查分组标注常见错误，包含：一组标注少一个标注框或点，一组标注的group_id值不对。
             dataset.check_group_labelme(args)
         # correct为排序并矫正后的车牌截取，original为不排序也不矫正的车牌截取
         elif args.function == 'correct' or args.function == 'original':  # 排序，按照多边形，左上、右上、右下、左下的顺序排列4个顶点，截取图像，矫正形状摆放位置
             dataset.sort_correct_labelme(args)
         elif args.function == 'cross':  # 针对标注形状超越图像边界情况，使用程序自动矫正
             dataset.cross_boundary_correction(args)
 
 
 if __name__ == '__main__':
     main()
+    # 使用了asyncio.run()函数来启动，协程事件循环，则不需要手动关闭事件循环
+    # asyncio.run(main())
```

### Comparing `ccdt-2.0.4/ccdt/dataset/utils/encoder.py` & `ccdt-2.0.5/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.4/ccdt/video_tool/split.py` & `ccdt-2.0.5/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.4/ccdt/video_tool/video_main.py` & `ccdt-2.0.5/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.4/ccdt.egg-info/PKG-INFO` & `ccdt-2.0.5/ccdt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.4
+Version: 2.0.5
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.4/ccdt.egg-info/SOURCES.txt` & `ccdt-2.0.5/ccdt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 ccdt/dataset/__init__.py
 ccdt/dataset/main.py
 ccdt/dataset/base_coco/__init__.py
 ccdt/dataset/base_coco/coco.py
 ccdt/dataset/base_labelme/__init__.py
 ccdt/dataset/base_labelme/async_io_task.py
 ccdt/dataset/base_labelme/base_labelme.py
+ccdt/dataset/base_labelme/test_async_io.py
 ccdt/dataset/logs/__init__.py
 ccdt/dataset/utils/__init__.py
+ccdt/dataset/utils/async_dirIterator.py
 ccdt/dataset/utils/encoder.py
 ccdt/dataset/utils/labelme_load.py
 ccdt/dataset/utils/logs.py
 ccdt/video_tool/__init__.py
 ccdt/video_tool/split.py
 ccdt/video_tool/video_main.py
```

### Comparing `ccdt-2.0.4/setup.py` & `ccdt-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.0.4',
+    version='2.0.5',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

