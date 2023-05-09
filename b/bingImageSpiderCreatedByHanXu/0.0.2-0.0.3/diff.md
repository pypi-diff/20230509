# Comparing `tmp/bingImageSpiderCreatedByHanXu-0.0.2.tar.gz` & `tmp/bingImageSpiderCreatedByHanXu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingImageSpiderCreatedByHanXu-0.0.2.tar", last modified: Sun Apr 23 13:57:51 2023, max compression
+gzip compressed data, was "bingImageSpiderCreatedByHanXu-0.0.3.tar", last modified: Tue May  9 12:06:46 2023, max compression
```

## Comparing `bingImageSpiderCreatedByHanXu-0.0.2.tar` & `bingImageSpiderCreatedByHanXu-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 13:57:51.622903 bingImageSpiderCreatedByHanXu-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-04-23 13:10:22.000000 bingImageSpiderCreatedByHanXu-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1527 2023-04-23 13:57:51.622903 bingImageSpiderCreatedByHanXu-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-04-23 13:56:09.000000 bingImageSpiderCreatedByHanXu-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 13:57:51.607902 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu/
--rw-rw-rw-   0        0        0     3762 2023-04-23 13:39:10.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu/Spider.py
--rw-rw-rw-   0        0        0        0 2023-04-23 13:39:10.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:57:51.618904 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/
--rw-rw-rw-   0        0        0     1527 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-23 13:57:51.000000 bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 13:57:51.622903 bingImageSpiderCreatedByHanXu-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     4264 2023-04-23 13:57:50.000000 bingImageSpiderCreatedByHanXu-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:06:46.456184 bingImageSpiderCreatedByHanXu-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-05-09 11:15:18.000000 bingImageSpiderCreatedByHanXu-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1527 2023-05-09 12:06:46.455131 bingImageSpiderCreatedByHanXu-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-05-09 11:15:18.000000 bingImageSpiderCreatedByHanXu-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 12:06:46.437814 bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu/
+-rw-rw-rw-   0        0        0     3800 2023-05-09 11:57:26.000000 bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:06:46.454131 bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu.egg-info/
+-rw-rw-rw-   0        0        0     1527 2023-05-09 12:06:46.000000 bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-09 12:06:46.000000 bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 12:06:46.000000 bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 12:06:46.000000 bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-09 12:06:46.000000 bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 12:06:46.456184 bingImageSpiderCreatedByHanXu-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     4225 2023-05-09 12:06:03.000000 bingImageSpiderCreatedByHanXu-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:06:46.454131 bingImageSpiderCreatedByHanXu-0.0.3/test/
+-rw-rw-rw-   0        0        0      956 2023-05-09 11:57:26.000000 bingImageSpiderCreatedByHanXu-0.0.3/test/test.py
```

### Comparing `bingImageSpiderCreatedByHanXu-0.0.2/LICENSE` & `bingImageSpiderCreatedByHanXu-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bingImageSpiderCreatedByHanXu-0.0.2/PKG-INFO` & `bingImageSpiderCreatedByHanXu-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingImageSpiderCreatedByHanXu
-Version: 0.0.2
+Version: 0.0.3
 Summary: get a large mount of images at Bing.
 Home-page: https://gitee.com/UnderTurrets/bing-image-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `bingImageSpiderCreatedByHanXu-0.0.2/README.md` & `bingImageSpiderCreatedByHanXu-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu/Spider.py` & `bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,17 +58,18 @@
 
     def get_image_url(self, urls):
         """
         @:brief Get the URLs of images.
         @:return a list of URLs of images
         """
         image_url = []
+        pattern_string="http[^%&]+.jpg"
+        pattern = re.compile(pattern=pattern_string)
         for url in urls:
             url_txt = requests.get(url, headers=self.headers).text
-            pattern = re.compile('[a-zA-z]+:[^&]*.jpg')
             url_list=pattern.findall(url_txt)
             for i in url_list:
                 if i:
                     image_url.append(i)
         return image_url
 
     def get_image(self,image_url):
```

### Comparing `bingImageSpiderCreatedByHanXu-0.0.2/bingImageSpiderCreatedByHanXu.egg-info/PKG-INFO` & `bingImageSpiderCreatedByHanXu-0.0.3/bingImageSpiderCreatedByHanXu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingImageSpiderCreatedByHanXu
-Version: 0.0.2
+Version: 0.0.3
 Summary: get a large mount of images at Bing.
 Home-page: https://gitee.com/UnderTurrets/bing-image-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `bingImageSpiderCreatedByHanXu-0.0.2/setup.py` & `bingImageSpiderCreatedByHanXu-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 
     #如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
     name="bingImageSpiderCreatedByHanXu",
-    version="0.0.2",
+    version="0.0.3",
     author="Han Xu",
     author_email="736946693@qq.com",
     description="get a large mount of images at Bing.",
 
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
@@ -68,18 +68,17 @@
     # 安装过程中，需要安装的静态文件，如配置文件、service文件、图片等
     # data_files=[
     #     ("", ["conf/*.conf"]),
     #     ("/usr/lib/systemd/system/", ["bin/*.service"]),
     #            ],
 
     # 希望被打包的文件
-    # package_data={
-    #     "":["*.txt"],
-    #     "bandwidth_reporter":["*.txt"]
-    #            },
+    package_data={
+        "test":["./test/*"],
+                 },
 
     # 不打包某些文件
     # exclude_package_data={
     #     "bandwidth_reporter":["*.txt"]
     #            },
 
     # 表明当前模块依赖哪些包，若环境中没有，则会从pypi中下载安装
```

