# Comparing `tmp/air-df-0.1.1.tar.gz` & `tmp/air-df-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\air-df-0.1.1.tar", last modified: Tue May  9 02:52:48 2023, max compression
+gzip compressed data, was "dist\air-df-0.1.2.tar", last modified: Tue May  9 03:06:24 2023, max compression
```

## Comparing `air-df-0.1.1.tar` & `air-df-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 02:52:48.097839 air-df-0.1.1/
--rw-rw-rw-   0        0        0     1916 2023-05-09 02:52:48.096842 air-df-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1170 2023-05-09 02:45:52.000000 air-df-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 02:52:48.074901 air-df-0.1.1/air/
--rw-rw-rw-   0        0        0      292 2021-12-27 05:36:01.000000 air-df-0.1.1/air/__init__.py
--rw-rw-rw-   0        0        0     3037 2021-12-27 05:36:01.000000 air-df-0.1.1/air/base_handler.py
--rw-rw-rw-   0        0        0    23523 2023-05-09 02:51:45.000000 air-df-0.1.1/air/plugins.py
-drwxrwxrwx   0        0        0        0 2023-05-09 02:52:48.093850 air-df-0.1.1/air_df.egg-info/
--rw-rw-rw-   0        0        0     1916 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 02:52:48.098837 air-df-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1082 2023-05-09 02:50:34.000000 air-df-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:06:24.691954 air-df-0.1.2/
+-rw-rw-rw-   0        0        0     1916 2023-05-09 03:06:24.690956 air-df-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1170 2023-05-09 02:45:52.000000 air-df-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 03:06:24.669015 air-df-0.1.2/air/
+-rw-rw-rw-   0        0        0      292 2021-12-27 05:36:01.000000 air-df-0.1.2/air/__init__.py
+-rw-rw-rw-   0        0        0     3037 2021-12-27 05:36:01.000000 air-df-0.1.2/air/base_handler.py
+-rw-rw-rw-   0        0        0    23590 2023-05-09 03:06:17.000000 air-df-0.1.2/air/plugins.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:06:24.686967 air-df-0.1.2/air_df.egg-info/
+-rw-rw-rw-   0        0        0     1916 2023-05-09 03:06:24.000000 air-df-0.1.2/air_df.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-09 03:06:24.000000 air-df-0.1.2/air_df.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 03:06:24.000000 air-df-0.1.2/air_df.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-05-09 03:06:24.000000 air-df-0.1.2/air_df.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-09 03:06:24.000000 air-df-0.1.2/air_df.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 03:06:24.691954 air-df-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-05-09 03:06:17.000000 air-df-0.1.2/setup.py
```

### Comparing `air-df-0.1.1/PKG-INFO` & `air-df-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air-df
-Version: 0.1.1
+Version: 0.1.2
 Summary: 常用插件
 Home-page: https://github.com/Air-df
 Author: Damon
 Author-email: 527439@qq.com
 License: UNKNOWN
 Description: ## base_handler -- tornado handler 基类
```

### Comparing `air-df-0.1.1/README.md` & `air-df-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `air-df-0.1.1/air/base_handler.py` & `air-df-0.1.2/air/base_handler.py`

 * *Files identical despite different names*

### Comparing `air-df-0.1.1/air/plugins.py` & `air-df-0.1.2/air/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.conn_mongo.close()
         return
 
 
 class RedisClient:
-    def __init__(self, host='123.57.66.110', port=6379, db=0, password='W4096redis'):
+    def __init__(self, host='127.0.0.1', port=6379, db=0, password='W4096redis'):
         pool = redis.ConnectionPool(host=host, port=port, password=password, decode_responses=True)
         self.conn = redis.Redis(connection_pool=pool, db=db)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -437,24 +437,26 @@
         :return: 时间戳 (前10位)
         """
         ret = int(time.mktime(time.strptime(timestr, strformat)))
 
         return ret
 
     @staticmethod
-    def send_mail(mail_title, mail_content, recievers=['527439841@qq.com'], file_path=None, style='plain'):
+    def send_mail(mail_title, mail_content, recievers=None, mail_user="527439@qq.com", mail_pass='jvubnbbddirgcbbfr', file_path=None, style='plain'):
+        if not recievers:
+            return
         # 发送邮件
         import smtplib
         from email.mime.text import MIMEText
         from email.mime.multipart import MIMEMultipart
 
         # 第三方 SMTP 服务
         mail_host = "smtp.qq.com"  # SMTP服务器
-        mail_user = "527439841@qq.com"  # 用户名
-        mail_pass = "jvubnbbddlrgcbbf"  # 授权密码，非登录密码
+        mail_user = mail_user  # 用户名
+        mail_pass = mail_pass  # 授权密码，非登录密码
 
         content = mail_content
         title = mail_title  # 邮件主题
 
         message = MIMEMultipart()
         # 正文
         message.attach(MIMEText(content, style, 'utf-8'))
```

### Comparing `air-df-0.1.1/air_df.egg-info/PKG-INFO` & `air-df-0.1.2/air_df.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air-df
-Version: 0.1.1
+Version: 0.1.2
 Summary: 常用插件
 Home-page: https://github.com/Air-df
 Author: Damon
 Author-email: 527439@qq.com
 License: UNKNOWN
 Description: ## base_handler -- tornado handler 基类
```

### Comparing `air-df-0.1.1/setup.py` & `air-df-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", 'r', encoding='utf-8') as f:
     requirements = f.read().split()
 
 setuptools.setup(
     name="air-df",  					# pip install name
-    version="0.1.1",					# 版本，每次更新需修改，否则无法上传
+    version="0.1.2",					# 版本，每次更新需修改，否则无法上传
     author="Damon",
     author_email="527439@qq.com",
     description="常用插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Air-df",  	# git-hup 项目地址, 这里只放了主页地址，这个参数不重要
     packages=['air'],					# 文件夹名
```

