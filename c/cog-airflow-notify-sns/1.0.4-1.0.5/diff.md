# Comparing `tmp/cog-airflow-notify-sns-1.0.4.tar.gz` & `tmp/cog-airflow-notify-sns-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog-airflow-notify-sns-1.0.4.tar", last modified: Tue May  9 14:39:33 2023, max compression
+gzip compressed data, was "cog-airflow-notify-sns-1.0.5.tar", last modified: Tue May  9 15:00:56 2023, max compression
```

## Comparing `cog-airflow-notify-sns-1.0.4.tar` & `cog-airflow-notify-sns-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 14:39:33.168357 cog-airflow-notify-sns-1.0.4/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     1073 2023-05-09 11:14:23.000000 cog-airflow-notify-sns-1.0.4/LICENSE
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2540 2023-05-09 14:39:33.168357 cog-airflow-notify-sns-1.0.4/PKG-INFO
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2018 2023-05-09 12:22:01.000000 cog-airflow-notify-sns-1.0.4/README.md
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 14:39:33.164357 cog-airflow-notify-sns-1.0.4/airflow_notify_sns/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-05-09 11:14:23.000000 cog-airflow-notify-sns-1.0.4/airflow_notify_sns/__init__.py
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     3051 2023-05-09 14:36:47.000000 cog-airflow-notify-sns-1.0.4/airflow_notify_sns/notify.py
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 14:39:33.168357 cog-airflow-notify-sns-1.0.4/cog_airflow_notify_sns.egg-info/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2540 2023-05-09 14:39:33.000000 cog-airflow-notify-sns-1.0.4/cog_airflow_notify_sns.egg-info/PKG-INFO
--rw-rw-r--   0 werneck   (1000) werneck   (1000)      315 2023-05-09 14:39:33.000000 cog-airflow-notify-sns-1.0.4/cog_airflow_notify_sns.egg-info/SOURCES.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-05-09 14:39:33.000000 cog-airflow-notify-sns-1.0.4/cog_airflow_notify_sns.egg-info/dependency_links.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-05-09 14:39:33.000000 cog-airflow-notify-sns-1.0.4/cog_airflow_notify_sns.egg-info/not-zip-safe
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       19 2023-05-09 14:39:33.000000 cog-airflow-notify-sns-1.0.4/cog_airflow_notify_sns.egg-info/top_level.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-05-09 14:39:33.168357 cog-airflow-notify-sns-1.0.4/setup.cfg
--rwxrwxr-x   0 werneck   (1000) werneck   (1000)      917 2023-05-09 14:39:23.000000 cog-airflow-notify-sns-1.0.4/setup.py
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 15:00:56.927851 cog-airflow-notify-sns-1.0.5/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     1073 2023-05-09 11:14:23.000000 cog-airflow-notify-sns-1.0.5/LICENSE
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2540 2023-05-09 15:00:56.927851 cog-airflow-notify-sns-1.0.5/PKG-INFO
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2018 2023-05-09 12:22:01.000000 cog-airflow-notify-sns-1.0.5/README.md
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 15:00:56.923851 cog-airflow-notify-sns-1.0.5/airflow_notify_sns/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-05-09 11:14:23.000000 cog-airflow-notify-sns-1.0.5/airflow_notify_sns/__init__.py
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     3048 2023-05-09 14:59:45.000000 cog-airflow-notify-sns-1.0.5/airflow_notify_sns/notify.py
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 15:00:56.927851 cog-airflow-notify-sns-1.0.5/cog_airflow_notify_sns.egg-info/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2540 2023-05-09 15:00:56.000000 cog-airflow-notify-sns-1.0.5/cog_airflow_notify_sns.egg-info/PKG-INFO
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)      315 2023-05-09 15:00:56.000000 cog-airflow-notify-sns-1.0.5/cog_airflow_notify_sns.egg-info/SOURCES.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-05-09 15:00:56.000000 cog-airflow-notify-sns-1.0.5/cog_airflow_notify_sns.egg-info/dependency_links.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-05-09 15:00:56.000000 cog-airflow-notify-sns-1.0.5/cog_airflow_notify_sns.egg-info/not-zip-safe
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       19 2023-05-09 15:00:56.000000 cog-airflow-notify-sns-1.0.5/cog_airflow_notify_sns.egg-info/top_level.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-05-09 15:00:56.927851 cog-airflow-notify-sns-1.0.5/setup.cfg
+-rwxrwxr-x   0 werneck   (1000) werneck   (1000)      917 2023-05-09 15:00:51.000000 cog-airflow-notify-sns-1.0.5/setup.py
```

### Comparing `cog-airflow-notify-sns-1.0.4/LICENSE` & `cog-airflow-notify-sns-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cog-airflow-notify-sns-1.0.4/PKG-INFO` & `cog-airflow-notify-sns-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog-airflow-notify-sns
-Version: 1.0.4
+Version: 1.0.5
 Summary: Publish Airflow notification errors to SNS Topic
 Home-page: https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification
 Author: Cognitivo.ai
 Author-email: engenharia@cognitivo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cog-airflow-notify-sns-1.0.4/README.md` & `cog-airflow-notify-sns-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cog-airflow-notify-sns-1.0.4/airflow_notify_sns/notify.py` & `cog-airflow-notify-sns-1.0.5/airflow_notify_sns/notify.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             dag=context.get('task_instance').dag_id,
             ti=context.get('task_instance'),
             exec_date=context.get('execution_date'),
             log_url=url.replace("localhost:8080", self.airflow_url),
         )
 
 
-    def send(self, context, **kwargs):
+    def send(self, context):
         """ 
         Publish Airflow Error Notification to a SNS Topic
 
         Parameters:
             context: Airflow task execution context
         
         Returns:
@@ -98,8 +98,8 @@
     sns_topic_arn = alerts_config.get('sns_topic_arn')
     airflow_url = alerts_config.get('airflow_url')
     
     notification = Notify(
         aws_sns_topic_arn = sns_topic_arn,
         airflow_url = airflow_url
     )
-    notification.send()
+    notification.send(context)
```

### Comparing `cog-airflow-notify-sns-1.0.4/cog_airflow_notify_sns.egg-info/PKG-INFO` & `cog-airflow-notify-sns-1.0.5/cog_airflow_notify_sns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog-airflow-notify-sns
-Version: 1.0.4
+Version: 1.0.5
 Summary: Publish Airflow notification errors to SNS Topic
 Home-page: https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification
 Author: Cognitivo.ai
 Author-email: engenharia@cognitivo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cog-airflow-notify-sns-1.0.4/setup.py` & `cog-airflow-notify-sns-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MYDIR = path.abspath(path.dirname(__file__))
 
 cmdclass = {}
 ext_modules = []
 
 setup(
     name='cog-airflow-notify-sns',  
-    version='1.0.4',
+    version='1.0.5',
     author="Cognitivo.ai",
     author_email="engenharia@cognitivo.ai",
     description="Publish Airflow notification errors to SNS Topic",
     url='https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification',
     long_description=io.open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests']),
```

