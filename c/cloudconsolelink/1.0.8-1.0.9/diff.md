# Comparing `tmp/cloudconsolelink-1.0.8.tar.gz` & `tmp/cloudconsolelink-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudconsolelink-1.0.8.tar", last modified: Wed Sep 28 16:19:11 2022, max compression
+gzip compressed data, was "cloudconsolelink-1.0.9.tar", last modified: Fri Sep 30 03:53:19 2022, max compression
```

## Comparing `cloudconsolelink-1.0.8.tar` & `cloudconsolelink-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/
--rw-r--r--   0 apple      (501) staff       (20)     4751 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     3187 2022-08-23 04:38:55.000000 cloudconsolelink-1.0.8/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/cloudconsolelink/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-08-23 04:38:55.000000 cloudconsolelink-1.0.8/cloudconsolelink/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-08-23 04:38:55.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/aws/
--rw-r--r--   0 apple      (501) staff       (20)     3703 2022-08-23 04:38:55.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/aws/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    34228 2022-09-14 07:00:16.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/aws/links.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/azure/
--rw-r--r--   0 apple      (501) staff       (20)     1291 2022-09-14 07:00:16.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/azure/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/gcp/
--rw-r--r--   0 apple      (501) staff       (20)     9097 2022-09-28 16:09:16.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/gcp/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    19360 2022-09-28 16:09:16.000000 cloudconsolelink-1.0.8/cloudconsolelink/clouds/gcp/links.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/cloudconsolelink.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     4751 2022-09-28 16:19:10.000000 cloudconsolelink-1.0.8/cloudconsolelink.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      449 2022-09-28 16:19:10.000000 cloudconsolelink-1.0.8/cloudconsolelink.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2022-09-28 16:19:10.000000 cloudconsolelink-1.0.8/cloudconsolelink.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       17 2022-09-28 16:19:10.000000 cloudconsolelink-1.0.8/cloudconsolelink.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)      201 2022-09-28 16:19:11.000000 cloudconsolelink-1.0.8/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)     1243 2022-09-28 16:18:18.000000 cloudconsolelink-1.0.8/setup.py
+drwxr-xr-x   0 puru       (501) staff       (20)        0 2022-09-30 03:53:19.038911 cloudconsolelink-1.0.9/
+-rw-r--r--   0 puru       (501) staff       (20)    11357 2022-06-30 18:42:49.000000 cloudconsolelink-1.0.9/LICENSE
+-rw-r--r--   0 puru       (501) staff       (20)     3742 2022-09-30 03:53:19.039148 cloudconsolelink-1.0.9/PKG-INFO
+-rw-r--r--   0 puru       (501) staff       (20)     3187 2022-06-30 18:42:49.000000 cloudconsolelink-1.0.9/README.md
+drwxr-xr-x   0 puru       (501) staff       (20)        0 2022-09-30 03:53:18.988839 cloudconsolelink-1.0.9/cloudconsolelink/
+-rw-r--r--   0 puru       (501) staff       (20)        0 2022-06-14 07:27:26.000000 cloudconsolelink-1.0.9/cloudconsolelink/__init__.py
+drwxr-xr-x   0 puru       (501) staff       (20)        0 2022-09-30 03:53:18.998134 cloudconsolelink-1.0.9/cloudconsolelink/clouds/
+-rw-r--r--   0 puru       (501) staff       (20)        0 2022-06-14 07:27:26.000000 cloudconsolelink-1.0.9/cloudconsolelink/clouds/__init__.py
+drwxr-xr-x   0 puru       (501) staff       (20)        0 2022-09-30 03:53:19.025292 cloudconsolelink-1.0.9/cloudconsolelink/clouds/aws/
+-rw-r--r--   0 puru       (501) staff       (20)     3703 2022-06-30 18:42:49.000000 cloudconsolelink-1.0.9/cloudconsolelink/clouds/aws/__init__.py
+-rw-r--r--   0 puru       (501) staff       (20)    35605 2022-09-29 20:35:42.000000 cloudconsolelink-1.0.9/cloudconsolelink/clouds/aws/links.py
+drwxr-xr-x   0 puru       (501) staff       (20)        0 2022-09-30 03:53:19.033550 cloudconsolelink-1.0.9/cloudconsolelink/clouds/azure/
+-rw-r--r--   0 puru       (501) staff       (20)     1560 2022-09-29 20:35:42.000000 cloudconsolelink-1.0.9/cloudconsolelink/clouds/azure/__init__.py
+drwxr-xr-x   0 puru       (501) staff       (20)        0 2022-09-30 03:53:19.037559 cloudconsolelink-1.0.9/cloudconsolelink/clouds/gcp/
+-rw-r--r--   0 puru       (501) staff       (20)     9194 2022-09-30 03:49:52.000000 cloudconsolelink-1.0.9/cloudconsolelink/clouds/gcp/__init__.py
+-rw-r--r--   0 puru       (501) staff       (20)    19360 2022-09-29 20:35:42.000000 cloudconsolelink-1.0.9/cloudconsolelink/clouds/gcp/links.py
+drwxr-xr-x   0 puru       (501) staff       (20)        0 2022-09-30 03:53:18.992868 cloudconsolelink-1.0.9/cloudconsolelink.egg-info/
+-rw-r--r--   0 puru       (501) staff       (20)     3742 2022-09-30 03:53:18.000000 cloudconsolelink-1.0.9/cloudconsolelink.egg-info/PKG-INFO
+-rw-r--r--   0 puru       (501) staff       (20)      457 2022-09-30 03:53:18.000000 cloudconsolelink-1.0.9/cloudconsolelink.egg-info/SOURCES.txt
+-rw-r--r--   0 puru       (501) staff       (20)        1 2022-09-30 03:53:18.000000 cloudconsolelink-1.0.9/cloudconsolelink.egg-info/dependency_links.txt
+-rw-r--r--   0 puru       (501) staff       (20)       17 2022-09-30 03:53:18.000000 cloudconsolelink-1.0.9/cloudconsolelink.egg-info/top_level.txt
+-rw-r--r--   0 puru       (501) staff       (20)      201 2022-09-30 03:53:19.040422 cloudconsolelink-1.0.9/setup.cfg
+-rw-r--r--   0 puru       (501) staff       (20)     1243 2022-09-30 03:52:41.000000 cloudconsolelink-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cloudconsolelink-1.0.8/README.md` & `cloudconsolelink-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudconsolelink-1.0.8/cloudconsolelink/clouds/aws/__init__.py` & `cloudconsolelink-1.0.9/cloudconsolelink/clouds/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudconsolelink-1.0.8/cloudconsolelink/clouds/aws/links.py` & `cloudconsolelink-1.0.9/cloudconsolelink/clouds/aws/links.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,14 +186,15 @@
             "aggregation-authorization": None,
             "config-aggregator": None,
             "config-rule": None,
             "conformance-pack": None,
             "organization-config-rule": None,
             "organization-conformance-pack": None,
             "remediation-configuration": None,
+
         },
         "connect": {  # Amazon Connect
             "instance": None,
         },
         "cur": {  # AWS Cost and Usage Report
             "definition": None,
         },
@@ -319,14 +320,15 @@
                 {data.get("region", "")}#VpcDetails:VpcId={data.get("resource", "")}',
             "vpc-endpoint": None,
             "vpc-endpoint-service": None,
             "vpc-flow-log": 'https://{data.get("region", "")}.{data.get("console", "")}/vpc/home?region={data.get("region", "")}#subnets:',
             "vpc-peering-connection": None,
             "vpn-connection": None,
             "vpn-gateway": None,
+
         },
         "ecr": {  # Amazon Elastic Container Registry
             "repository": 'https://{data.get("region", "")}.{data.get("console", "")}/ecr/repositories/{data.get\
                 ("resource", "")}?region={data.get("region", "")}',
         },
         "ecs": {  # Amazon Elastic Container Service
             "cluster": None,
@@ -351,15 +353,15 @@
             "configurationtemplate": None,
             "environment": None,
             "platform": None,
             "solutionstack": None,
         },
         "elasticfilesystem": {  # Amazon Elastic File System
             "access-point": None,
-            "file-system": None,
+            "file-system": 'https://https://{data.get("region", "")}.{data.get("console", "")}/efs/home?region={data.get("region", "")}#/file-systems/{data.get("resource", "")}',
         },
         "elasticloadbalancing": {  # AWS WAF V2
             "listener": None,
             "listener-rule": None,
             "loadbalancer": None,
             "targetgroup": None,
         },
@@ -378,16 +380,20 @@
         "events": {  # Amazon EventBridge
             "event-bus": 'https://{data.get("region", "")}.{data.get("console", "")}/events/home?region={data.get("region", "")}#/eventbus/{data.get("resource", "")}',
             "event-source": None,
             "rule": None,
         },
         "execute-api": {  # Amazon API Gateway
         },
+        "emr": {
+            #Amazon EMR
+            "cluster": 'https://{data.get("region", "")}.{data.get("console", "")}/elasticmapreduce/home?region={data.get("region", "")}#cluster-details:{data.get("resource", "")}'
+        },
         "firehose": {  # Amazon Kinesis Firehose
-            "deliverystream": None,
+            "deliverystream": 'https://{data.get("region", "")}.{data.get("console", "")}/firehose/home?region={data.get("region", "")}#/details/{data.get("resource", "")}/monitoring',
         },
         "fms": {  # AWS Firewall Manager
             "policy": None,
         },
         "forecast": {  # Amazon Forecast
             "algorithm": None,
             "dataset": None,
@@ -535,15 +541,15 @@
         "kafka": {  # Amazon Managed Streaming for Kafka
             "cluster": None,
         },
         "kendra": {  # Amazon Kendra
             "index": None,
         },
         "kinesis": {  # Amazon Kinesis
-            "stream": None,
+            "stream": 'https://{data.get("region", "")}.{data.get("console", "")}/kinesis/home?region={data.get("region", "")}#/streams/details/{data.get("resource", "")}/monitoring',
         },
         "kinesisanalytics": {  # Amazon Kinesis Analytics V2
             "application": None,
         },
         "kinesisvideo": {  # Amazon Kinesis Video Streams
             "channel": None,
             "stream": None,
@@ -666,15 +672,15 @@
         },
         "opsworks": {  # AWS OpsWorks
             "stack": None,
         },
         "organizations": {  # AWS Organizations
             "account": None,
             "handshake": None,
-            "organization": None,
+            "organization": 'https://{data.get("region", "")}.{data.get("console", "")}/organizations/v2/home/accounts/{data.get("resource", "")}',
             "ou": None,
             "policy": None,
             "root": None,
         },
         "outposts": {  # AWS Outposts
             "order": None,
             "outpost": None,
@@ -806,15 +812,15 @@
             "human-loop": None,
             "human-task-ui": None,
             "hyper-parameter-tuning-job": None,
             "labeling-job": None,
             "model": None,
             "model-package": None,
             "monitoring-schedule": None,
-            "notebook-instance": None,
+            "notebook-instance": 'https://{data.get("region", "")}.{data.get("console", "")}/sagemaker/home?region={data.get("region", "")}#/notebook-instances/{data.get("resource", "")}',
             "notebook-instance-lifecycle-config": None,
             "processing-job": None,
             "training-job": None,
             "transform-job": None,
             "user-profile": None,
             "workforce": None,
             "workteam": None,
@@ -827,15 +833,15 @@
             "registry": None,
             "schema": None,
         },
         "sdb": {  # Amazon SimpleDB
             "domain": None,
         },
         "secretsmanager": {  # AWS Secrets Manager
-            "secret": None,
+            "secret": 'https://{data.get("region", "")}.{data.get("console", "")}/secretsmanager/secret?name={data.get("resource", "")}&region ={data.get("region", "")}',
         },
         "securityhub": {  # AWS Security Hub
             "hub": None,
             "product": None,
         },
         "serverlessrepo": {  # AWS Serverless Application Repository
             "applications": None,
@@ -876,19 +882,19 @@
             "automation-definition": None,
             "automation-execution": None,
             "document": None,
             "maintenancewindow": None,
             "managed-instance": None,
             "managed-instance-inventory": None,
             "opsitem": None,
-            "parameter": None,
+            "parameter": 'https://{data.get("region", "")}.{data.get("console", "")}/systems-manager/parameters/{data.get("resource", "")}/description?region={data.get("region", "")}&tab=Table',
             "patchbaseline": None,
             "resource-data-sync": None,
             "servicesetting": None,
-            "session": None,
+            "session": 'https://{data.get("region", "")}.{data.get("console", "")}/systems-manager/session-manager?region={data.get("region", "")}',
             "windowtarget": None,
             "windowtask": None,
         },
         "states": {  # AWS Step Functions
             "activity": None,
             "execution": None,
             "stateMachine": 'https://{data.get("region", "")}.{data.get("console", "")}/states/home?region=\
```

### Comparing `cloudconsolelink-1.0.8/cloudconsolelink/clouds/azure/__init__.py` & `cloudconsolelink-1.0.9/cloudconsolelink/clouds/azure/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,22 @@
                  `primary_ad_domain_name`")
             raise ValueError("Invalid parameters provided")
         iam_entities = {
             "user": 'https://portal.azure.com/#blade/Microsoft_AAD_IAM/UserDetailsMenuBlade/Profile/userId/{id}',
             "group": 'https://portal.azure.com/#blade/Microsoft_AAD_IAM/GroupDetailsMenuBlade/Overview/groupId/{id}',
             "application": 'https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationMenuBlade\
             /Overview/appId/{id}',
+            "role": 'https://portal.azure.com/#@{primary_ad_domain_name}/resource/{id}/roles',
         }
 
         if iam_entity_type and id and iam_entities.get(iam_entity_type, None):
-            return eval(f"f'{iam_entities[iam_entity_type]}'").replace(" ", "")
+            if iam_entity_type == 'role' and primary_ad_domain_name:
+                return eval(f"f'{iam_entities[iam_entity_type]}'").replace(" ", "")
+            else:
+                return eval(f"f'{iam_entities[iam_entity_type]}'").replace(" ", "")
 
         elif primary_ad_domain_name and id:
             return f"https://portal.azure.com/#@{primary_ad_domain_name}/resource{id}/overview"
 
         else:
             logger.error('entity id required')
             raise ValueError("Invalid parameters provided")
-
```

### Comparing `cloudconsolelink-1.0.8/cloudconsolelink/clouds/gcp/__init__.py` & `cloudconsolelink-1.0.9/cloudconsolelink/clouds/gcp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     cloud_function_name=None,
     kms_key_ring_name=None,
     kms_key_name=None,
     dns_zone_name=None,
     dns_rrset_name=None,
     dns_type=None,
     gke_cluster_name=None,
+    disk_name=None,
+    topic_id=None,
     sql_instance_name=None,
     service_account_unique_id=None,
     role_id=None,
     group_unique_id=None,
     firestore_collection_name=None,
     cloud_run_service_name=None,
     dataproc_cluster_name=None,
@@ -68,14 +70,16 @@
         "cloud_function_name": cloud_function_name,
         "kms_key_ring_name": kms_key_ring_name,
         "kms_key_name": kms_key_name,
         "dns_zone_name": dns_zone_name,
         "dns_rrset_name": dns_rrset_name,
         "dns_type": dns_type,
         "gke_cluster_name": gke_cluster_name,
+        disk_name: disk_name,
+        topic_id: topic_id,
         "sql_instance_name": sql_instance_name,
         "service_account_unique_id": service_account_unique_id,
         "role_id": role_id,
         "group_unique_id": group_unique_id,
         "firestore_collection_name": firestore_collection_name,
         "cloud_run_service_name": cloud_run_service_name,
         "dataproc_cluster_name": dataproc_cluster_name,
```

### Comparing `cloudconsolelink-1.0.8/cloudconsolelink/clouds/gcp/links.py` & `cloudconsolelink-1.0.9/cloudconsolelink/clouds/gcp/links.py`

 * *Files identical despite different names*

### Comparing `cloudconsolelink-1.0.8/setup.py` & `cloudconsolelink-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 # version of the module
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 
 
 setuptools.setup(
     # Here is the module name.
     name="cloudconsolelink",
 
     # version of the module
```

