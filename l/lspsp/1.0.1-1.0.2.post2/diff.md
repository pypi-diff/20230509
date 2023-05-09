# Comparing `tmp/lspsp-1.0.1.tar.gz` & `tmp/lspsp-1.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lspsp-1.0.1.tar", last modified: Mon May  8 02:53:26 2023, max compression
+gzip compressed data, was "lspsp-1.0.2.post2.tar", last modified: Tue May  9 04:44:49 2023, max compression
```

## Comparing `lspsp-1.0.1.tar` & `lspsp-1.0.2.post2.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:26.990557 lspsp-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 02:53:14.000000 lspsp-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 02:53:26.990557 lspsp-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 02:53:14.000000 lspsp-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 02:53:14.000000 lspsp-1.0.1/config.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:26.990557 lspsp-1.0.1/lspsp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/lspmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/lspnotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/lspsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:26.990557 lspsp-1.0.1/lspsp/resource/
--rw-r--r--   0 runner    (1001) docker     (123)    55908 2023-05-08 02:53:14.000000 lspsp-1.0.1/lspsp/resource/mail.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 02:53:26.990557 lspsp-1.0.1/lspsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 02:53:26.000000 lspsp-1.0.1/lspsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 02:53:26.990557 lspsp-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 02:53:14.000000 lspsp-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/config.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/lspsp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/lspmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/lspnotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/lspsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/mailbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/monexec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/lspsp/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/resource/mail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/resource/test.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/lspsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 04:44:49.832255 lspsp-1.0.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/setup.py
```

### Comparing `lspsp-1.0.1/lspsp/lspmon.py` & `lspsp-1.0.2.post2/lspsp/lspmon.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 from lspsp.lspsp import Lspsp
 
 
 class Lspmon:
     _interval = 60
     _current = {}
 
-    def __init__(self) -> None:
+    def __init__(self, mode) -> None:
         f = open('config.json', 'r')
         text = f.read()
         f.close()
         data = json.loads(text)
         self._notify_config = data['notify_config']
         self._interval = data['interval']
         self._api = Lspsp(data['loginuser'])
         logging.basicConfig(
             level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         self._logger = logging.getLogger(__name__)
-        self._notifier = LspNotify()
+        self._mode = mode
+        self._notifier = LspNotify(mode)
 
     def diff(self, data):
         diff = {}
         for key in data.keys():
             if self._current.get(key) == None:
                 diff[key] = data[key]
         return diff
@@ -41,11 +42,14 @@
         data = self._api.list()
         diff = self.diff(data)
         self._current = data
         if diff:
             self.notify(diff)
 
     def launch(self):
-        scheduler = BlockingScheduler(timezone='Asia/Shanghai')
-        scheduler.add_job(self.job, 'interval',
-                          seconds=self._interval, id='check_capicity')
-        scheduler.start()
+        if self._mode == 0:
+            self.notify({})
+        elif self._mode == 1:
+            scheduler = BlockingScheduler(timezone='Asia/Shanghai')
+            scheduler.add_job(self.job, 'interval',
+                              seconds=self._interval, id='check_capicity')
+            scheduler.start()
```

### Comparing `lspsp-1.0.1/lspsp/lspnotify.py` & `lspsp-1.0.2.post2/lspsp/lspnotify.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 from email.header import Header
 from email.mime.text import MIMEText
 import logging
 import smtplib
 from jinja2 import Environment, FileSystemLoader
 import os
 
+from lspsp.mailbuilder import MailBuilder
+
 
 class LspNotify:
-    def __init__(self) -> None:
+    def __init__(self, mode) -> None:
         self._logger = logging.getLogger(__name__)
+        self._mode = mode
+
+    def get_subject(self, content):
+        if self._mode == 0:
+            return '收件收发配置测试'
+        elif self._mode == 1:
+            return '发现LSPSP.ME新库存%d个' % (len(content))
+        else:
+            return '未知类型的邮件'
 
     def mail(self, config, content):
         root = os.path.dirname(__file__)
         path = os.path.join(root, 'resource')
         env = Environment(loader=FileSystemLoader(path))
-        template = env.get_template('mail.html')
-        html_content = template.render(content=content)
-
-        message = MIMEText(str(html_content), 'html', 'utf-8')
-        message['From'] = '%s <%s>' % (
-            Header(config['name'], 'utf-8').encode(), config['usn'])
-        message['To'] = config['recv']
-        message['Subject'] = Header(
-            '发现LSPSP.ME新库存%d个' % (len(content)), 'utf-8').encode()
+        template_name = ''
+        if self._mode == 0:
+            template_name = 'test'
+        else:
+            template_name = 'mail'
+        template = env.get_template(template_name + '.html')
+        html_content = str(template.render(content=content))
 
         smtp = None
         if config['ssl']:
             smtp = smtplib.SMTP_SSL(config['host'], config['port'])
         else:
             smtp = smtplib.SMTP(config['host'], config['port'])
         smtp.login(config['usn'], config['pwd'])
-        smtp.sendmail(config['usn'], config['recv'], message.as_string())
-        self._logger.info("Email sended to: %s", config['recv'])
+
+        for item in config['recv']:
+            builder = MailBuilder().content(html_content).frm(config['name'], config['usn']).to(
+                item).subject(self.get_subject(content))
+            message = builder.build()
+
+            smtp.sendmail(config['usn'], item, message.as_string())
+            self._logger.info("Email sended to: %s", item)
```

### Comparing `lspsp-1.0.1/lspsp/lspsp.py` & `lspsp-1.0.2.post2/lspsp/lspsp.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.1/setup.py` & `lspsp-1.0.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="lspsp",
-    version="1.0.1",
+    version="1.0.2-2",
     license='GPL',
     description='LSPSP.ME Monitor',
     long_description='LSPSP.ME Monitor Service',
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
     install_requires=[
```

