# Comparing `tmp/cog-airflow-notify-sns-0.0.1.tar.gz` & `tmp/cog-airflow-notify-sns-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/cognitivo/projetos/cog.dataplatform.service.system.airflow.notification/dist/tmp86lo5z_q/cog-airflow-notify-sns-0.0.1.tar", last modified: Thu Nov 17 19:25:27 2022, max compression
+gzip compressed data, was "cog-airflow-notify-sns-1.0.2.tar", last modified: Tue May  9 13:20:21 2023, max compression
```

## Comparing `cog-airflow-notify-sns-0.0.1.tar` & `cog-airflow-notify-sns-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 experts\paulo.werneck (66696) experts\domain users (66049)        0 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)     1073 2022-11-07 19:31:22.000000 cog-airflow-notify-sns-0.0.1/LICENSE
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)     2461 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/PKG-INFO
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)     1975 2022-11-07 21:05:58.000000 cog-airflow-notify-sns-0.0.1/README.md
-drwxr-xr-x   0 experts\paulo.werneck (66696) experts\domain users (66049)        0 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/airflow_notify_sns/
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)       38 2022-11-07 19:31:22.000000 cog-airflow-notify-sns-0.0.1/airflow_notify_sns/__init__.py
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)     2354 2022-11-07 19:36:39.000000 cog-airflow-notify-sns-0.0.1/airflow_notify_sns/notify.py
-drwxr-xr-x   0 experts\paulo.werneck (66696) experts\domain users (66049)        0 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/cog_airflow_notify_sns.egg-info/
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)     2461 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/cog_airflow_notify_sns.egg-info/PKG-INFO
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)      315 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/cog_airflow_notify_sns.egg-info/SOURCES.txt
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)        1 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/cog_airflow_notify_sns.egg-info/dependency_links.txt
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)        1 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/cog_airflow_notify_sns.egg-info/not-zip-safe
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)       19 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/cog_airflow_notify_sns.egg-info/top_level.txt
--rw-r--r--   0 experts\paulo.werneck (66696) experts\domain users (66049)       38 2022-11-17 19:25:27.000000 cog-airflow-notify-sns-0.0.1/setup.cfg
--rwxr-xr-x   0 experts\paulo.werneck (66696) experts\domain users (66049)      917 2022-11-17 19:23:09.000000 cog-airflow-notify-sns-0.0.1/setup.py
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 13:20:21.248572 cog-airflow-notify-sns-1.0.2/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     1073 2023-05-09 11:14:23.000000 cog-airflow-notify-sns-1.0.2/LICENSE
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2540 2023-05-09 13:20:21.248572 cog-airflow-notify-sns-1.0.2/PKG-INFO
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2018 2023-05-09 12:22:01.000000 cog-airflow-notify-sns-1.0.2/README.md
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 13:20:21.244572 cog-airflow-notify-sns-1.0.2/airflow_notify_sns/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-05-09 11:14:23.000000 cog-airflow-notify-sns-1.0.2/airflow_notify_sns/__init__.py
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     3017 2023-05-09 13:19:45.000000 cog-airflow-notify-sns-1.0.2/airflow_notify_sns/notify.py
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-05-09 13:20:21.248572 cog-airflow-notify-sns-1.0.2/cog_airflow_notify_sns.egg-info/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2540 2023-05-09 13:20:21.000000 cog-airflow-notify-sns-1.0.2/cog_airflow_notify_sns.egg-info/PKG-INFO
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)      315 2023-05-09 13:20:21.000000 cog-airflow-notify-sns-1.0.2/cog_airflow_notify_sns.egg-info/SOURCES.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-05-09 13:20:21.000000 cog-airflow-notify-sns-1.0.2/cog_airflow_notify_sns.egg-info/dependency_links.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-05-09 13:20:21.000000 cog-airflow-notify-sns-1.0.2/cog_airflow_notify_sns.egg-info/not-zip-safe
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       19 2023-05-09 13:20:21.000000 cog-airflow-notify-sns-1.0.2/cog_airflow_notify_sns.egg-info/top_level.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-05-09 13:20:21.248572 cog-airflow-notify-sns-1.0.2/setup.cfg
+-rwxrwxr-x   0 werneck   (1000) werneck   (1000)      917 2023-05-09 13:19:58.000000 cog-airflow-notify-sns-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cog-airflow-notify-sns-0.0.1/LICENSE` & `cog-airflow-notify-sns-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cog-airflow-notify-sns-0.0.1/PKG-INFO` & `cog-airflow-notify-sns-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cog-airflow-notify-sns
-Version: 0.0.1
+Version: 1.0.2
 Summary: Publish Airflow notification errors to SNS Topic
 Home-page: https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification
 Author: Cognitivo.ai
 Author-email: engenharia@cognitivo.ai
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
@@ -21,15 +23,15 @@
 
 This package adds a callback function to use in failures to DAGs and Tasks in a Airflow project. 
 
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification.git
+pip install cog-airflow-notify-sns==1.0.0
 ```
 
 
 ## Usage
 
 ```python
 from datetime import timedelta
@@ -66,10 +68,19 @@
 )
 ```
 
 When DAG or tasks ends in error, a notification will be send to a SNS Topic using AWS default connection (`aws_default`). 
 
 ## Required Variable
 
-This module will try to find a variable named `airflow_notify_sns_arn` in your Airflow environment, containing SNS Topic ARN where message will be published to. 
+This module will try to find a variable named `airflow_alerts_config` in your Airflow environment. <br>
+
+Example
+```json
+{
+    "sns_topic_arn": "arn:aws:sns:us-east-1:012345678901:topic-name",
+    "airflow_url": "http://xpto.us-east-1.elb.amazonaws.com:8080"
+}
+```
 
 If variable is not found, function will abort execution with no error. 
+
```

### Comparing `cog-airflow-notify-sns-0.0.1/README.md` & `cog-airflow-notify-sns-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 This package adds a callback function to use in failures to DAGs and Tasks in a Airflow project. 
 
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification.git
+pip install cog-airflow-notify-sns==1.0.0
 ```
 
 
 ## Usage
 
 ```python
 from datetime import timedelta
@@ -53,10 +53,18 @@
 )
 ```
 
 When DAG or tasks ends in error, a notification will be send to a SNS Topic using AWS default connection (`aws_default`). 
 
 ## Required Variable
 
-This module will try to find a variable named `airflow_notify_sns_arn` in your Airflow environment, containing SNS Topic ARN where message will be published to. 
+This module will try to find a variable named `airflow_alerts_config` in your Airflow environment. <br>
+
+Example
+```json
+{
+    "sns_topic_arn": "arn:aws:sns:us-east-1:012345678901:topic-name",
+    "airflow_url": "http://xpto.us-east-1.elb.amazonaws.com:8080"
+}
+```
 
 If variable is not found, function will abort execution with no error.
```

### Comparing `cog-airflow-notify-sns-0.0.1/airflow_notify_sns/notify.py` & `cog-airflow-notify-sns-1.0.2/airflow_notify_sns/notify.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,73 +3,103 @@
 
 LOGGING = logging.getLogger(__name__)
 
 from airflow.models.variable import Variable
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 
-def airflow_notify_sns(context, **kwargs):
-    """ 
-    Publish Airflow Error Notification to a SNS Topic
+class Notify:
 
-    Parameters:
-        context (dict): Airflow task execution context
-    
-    Returns:
-        boto3 sns_client.publish() response
-    """
-    sns_client = AwsBaseHook(client_type="sns", aws_conn_id='aws_default')
-    sns_topic_arn = Variable.get('airflow_notify_sns_arn', None)
+    def __init__(
+        self,
+        aws_sns_topic_arn: str,
+        airflow_url: str
+    ):
+        """
+        params:
+            aws_sns_topic_arn: AWS SNS topic ARN where airflow send error messages
+            airflow_url: AWS load balancer DNS by airflow
+        """
+
+        self.aws_sns_topic_arn = aws_sns_topic_arn
+        self.airflow_url = airflow_url
+
+
+    def _format_message_text(self, context):
+        """
+        Function to format airflow message
+
+        params:
+            context:  Airflow task execution context
+
+        return:
+            Message error formated
+        """
+        
+        url = context.get('task_instance').log_url
+        return """Airflow task execution failed. 
+        *Time*: {time}  
+        *Task*: {task}  
+        *Dag*: {dag} 
+        *Execution Time*: {exec_date}  
+        *Log Url*: {log_url} 
+        """.format(
+            time=datetime.now(),
+            task=context.get('task_instance').task_id,
+            dag=context.get('task_instance').dag_id,
+            ti=context.get('task_instance'),
+            exec_date=context.get('execution_date'),
+            log_url=url.replace("localhost:8080", self.airflow_url),
+        )
 
-    # Make variable required
-    if sns_topic_arn is None:
-        LOGGING.error("Variable [airflow_notify_sns_arn] not found in Airflow")
-        return None
 
-    # Message attributes
-    subject = "{company}: [WARN] - Airflow task execution failed".format(
-        company=_get_load_balancer().split('-')[0].capitalize()
-    )
-    message = get_message_text(context)
+    def send(self, context, **kwargs):
+        """ 
+        Publish Airflow Error Notification to a SNS Topic
+
+        Parameters:
+            context: Airflow task execution context
+        
+        Returns:
+            boto3 sns_client.publish() response
+        """
+
+        sns_client = AwsBaseHook(client_type="sns", aws_conn_id='aws_default')
+
+        # Message attributes
+        subject = "ERROR - Airflow task execution failed"
+        message = self._format_message_text(context)
+
+        # Sending message to topic
+        LOGGING.info(f"Error message to send: {message}")
+        LOGGING.info(f"Sending error message to SNS Topic ARN [{self.aws_sns_topic_arn}]")
+        try:
+            response = sns_client.get_conn().publish(
+                TopicArn=self.aws_sns_topic_arn,
+                Subject=subject,
+                Message=message
+            )
+            LOGGING.info("Message successfully sent do SNS Topic")
+            return response
+        except Exception as ex:
+            LOGGING.error(f"Error sending message to SNS: [{ex}]")
+            return None
 
-    # Sending message to topic
-    LOGGING.info(f"Error message to send: {message}")
-    LOGGING.info(f"Sending error message to SNS Topic ARN [{sns_topic_arn}]")
-    try:
-        response = sns_client.get_conn().publish(
-            TopicArn=sns_topic_arn,
-            Subject=subject,
-            Message=message
-        )
-        LOGGING.info("Message successfully sent do SNS Topic")
-        return response
-    except Exception as ex:
-        LOGGING.error(f"Error sending message to SNS: [{ex}]")
         return None
 
-    return None
 
+def airflow_notify_sns():
+    alerts_config = Variable.get('airflow_alerts_config', None)
+    
+    # Make variable required
+    if not alerts_config:
+        LOGGING.error("Variable [airflow_alerts_config] not found in Airflow")
+        return None
 
-def get_message_text(context):
-    url = context.get('task_instance').log_url
-    return """Airflow task execution failed. 
-    *Time*: {time}  
-    *Task*: {task}  
-    *Dag*: {dag} 
-    *Execution Time*: {exec_date}  
-    *Log Url*: {log_url} 
-    """.format(
-        time=datetime.now(),
-        task=context.get('task_instance').task_id,
-        dag=context.get('task_instance').dag_id,
-        ti=context.get('task_instance'),
-        exec_date=context.get('execution_date'),
-        log_url=url.replace("localhost:8080", _get_load_balancer()),
+    sns_topic_arn = alerts_config.get('sns_topic_arn')
+    airflow_url = alerts_config.get('airflow_url')
+    
+    notification = Notify(
+        aws_sns_topic_arn = sns_topic_arn,
+        airflow_url = airflow_url
     )
-
-
-def _get_load_balancer():
-    elb_client = AwsBaseHook(client_type="elbv2", aws_conn_id='aws_default')
-    response = elb_client.get_conn().describe_load_balancers()
-    for elb in response["LoadBalancers"]:
-        if "airflow-web" in elb["LoadBalancerName"]:
-            return elb["DNSName"]
+    notification.send()
```

### Comparing `cog-airflow-notify-sns-0.0.1/cog_airflow_notify_sns.egg-info/PKG-INFO` & `cog-airflow-notify-sns-1.0.2/cog_airflow_notify_sns.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cog-airflow-notify-sns
-Version: 0.0.1
+Version: 1.0.2
 Summary: Publish Airflow notification errors to SNS Topic
 Home-page: https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification
 Author: Cognitivo.ai
 Author-email: engenharia@cognitivo.ai
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
@@ -21,15 +23,15 @@
 
 This package adds a callback function to use in failures to DAGs and Tasks in a Airflow project. 
 
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification.git
+pip install cog-airflow-notify-sns==1.0.0
 ```
 
 
 ## Usage
 
 ```python
 from datetime import timedelta
@@ -66,10 +68,19 @@
 )
 ```
 
 When DAG or tasks ends in error, a notification will be send to a SNS Topic using AWS default connection (`aws_default`). 
 
 ## Required Variable
 
-This module will try to find a variable named `airflow_notify_sns_arn` in your Airflow environment, containing SNS Topic ARN where message will be published to. 
+This module will try to find a variable named `airflow_alerts_config` in your Airflow environment. <br>
+
+Example
+```json
+{
+    "sns_topic_arn": "arn:aws:sns:us-east-1:012345678901:topic-name",
+    "airflow_url": "http://xpto.us-east-1.elb.amazonaws.com:8080"
+}
+```
 
 If variable is not found, function will abort execution with no error. 
+
```

### Comparing `cog-airflow-notify-sns-0.0.1/setup.py` & `cog-airflow-notify-sns-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MYDIR = path.abspath(path.dirname(__file__))
 
 cmdclass = {}
 ext_modules = []
 
 setup(
     name='cog-airflow-notify-sns',  
-    version='0.0.1',
+    version='1.0.2',
     author="Cognitivo.ai",
     author_email="engenharia@cognitivo.ai",
     description="Publish Airflow notification errors to SNS Topic",
     url='https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification',
     long_description=io.open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests']),
```

