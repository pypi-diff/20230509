# Comparing `tmp/cloud-governance-1.1.93.tar.gz` & `tmp/cloud-governance-1.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-governance-1.1.93.tar", last modified: Tue May  2 07:26:19 2023, max compression
+gzip compressed data, was "cloud-governance-1.1.94.tar", last modified: Tue May  9 08:24:43 2023, max compression
```

## Comparing `cloud-governance-1.1.93.tar` & `cloud-governance-1.1.94.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/short_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cost_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/aws/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/azure/cost_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/azure/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/gcp/google_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/classic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/google_drive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/google_drive/google_drive_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/jira/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/jira/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/jira/jira_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/ldap/ldap_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/logger/init_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/logger/logger_time_stamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.400153 cloud-governance-1.1.93/cloud_governance/common/mails/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/mails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/mails/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/mails/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/mails/postfix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/common/tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/common/tool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/main/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/main/environment_variables_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/main/es_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/main/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/policy/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/cost_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/ebs_in_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/ebs_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/empty_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/ip_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/monthly_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/s3_inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/skipped_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/unused_nat_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/aws/zombie_snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/policy/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/azure/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/policy/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/gcp/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/policy/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/ibm/tag_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/ibm/tag_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.404153 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.408154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.408154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.408154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.408154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.408154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.408154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gitleaks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:19.396153 cloud-governance-1.1.93/cloud_governance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-02 07:26:19.000000 cloud-governance-1.1.93/cloud_governance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-02 07:26:19.000000 cloud-governance-1.1.93/cloud_governance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:26:19.000000 cloud-governance-1.1.93/cloud_governance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:26:19.000000 cloud-governance-1.1.93/cloud_governance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-02 07:26:19.000000 cloud-governance-1.1.93/cloud_governance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:26:19.000000 cloud-governance-1.1.93/cloud_governance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 07:26:19.412154 cloud-governance-1.1.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-02 07:26:02.000000 cloud-governance-1.1.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-09 08:24:43.193559 cloud-governance-1.1.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/short_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/common/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/resources_pricing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/sts/sts_oprations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/aws/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/azure/cost_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/azure/cost_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/azure/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/azure/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/gcp/google_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/google_drive/google_drive_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/google_drive/upload_to_gsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/jira/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/jira/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/jira/jira_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/ldap/ldap_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.181559 cloud-governance-1.1.94/cloud_governance/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/logger/init_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/logger/logger_time_stamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/common/mails/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/mails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/mails/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/mails/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/mails/postfix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/common/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/common/tool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/main/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/main/environment_variables_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/main/es_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/main/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/policy/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/cost_billing_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/cost_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/cost_explorer_payer_billings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/ebs_in_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/ebs_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/empty_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/ip_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/monthly_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/s3_inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/skipped_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/unused_nat_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/aws/zombie_snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/policy/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/azure/cost_billing_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/policy/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/gcp/cost_billing_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/policy/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/ibm/cost_billing_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/ibm/ibm_cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/ibm/ibm_cost_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/ibm/tag_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.185559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/cost_expenditure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gitleaks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gitleaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.189559 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:24:43.177559 cloud-governance-1.1.94/cloud_governance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-09 08:24:43.000000 cloud-governance-1.1.94/cloud_governance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-09 08:24:43.000000 cloud-governance-1.1.94/cloud_governance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:24:43.000000 cloud-governance-1.1.94/cloud_governance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:24:43.000000 cloud-governance-1.1.94/cloud_governance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-09 08:24:43.000000 cloud-governance-1.1.94/cloud_governance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 08:24:43.000000 cloud-governance-1.1.94/cloud_governance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 08:24:43.193559 cloud-governance-1.1.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-09 08:24:26.000000 cloud-governance-1.1.94/setup.py
```

### Comparing `cloud-governance-1.1.93/LICENSE` & `cloud-governance-1.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/PKG-INFO` & `cloud-governance-1.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.93
+Version: 1.1.94
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloud-governance-1.1.93/README.md` & `cloud-governance-1.1.94/README.md`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py` & `cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py` & `cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py` & `cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py` & `cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py` & `cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py` & `cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,51 +6,90 @@
 class CostExplorerOperations:
     """
     This class extracts the price data from AWS Cost Explorer
     """
 
     START_DAY = 1
     END_DAY = 31
-    PURCHASE_OPTIONS = ['On Demand Instances', 'Savings Plans', 'Spot Instances', 'Standard Reserved Instances']
+    DIMENSIONS = 'Dimensions'
+    KEY = 'Key'
+    VALUES = 'Values'
+    PURCHASE_TYPE = 'PURCHASE_TYPE'
+    SPOT_INSTANCES = 'Spot Instances'
+    FILTER = 'Filter'
+    PURCHASE_OPTIONS = ['On Demand Instances', 'Savings Plans', SPOT_INSTANCES, 'Standard Reserved Instances']
+    CE_COST_TYPES = {'CHARGETYPE': 'RECORD_TYPE', 'PURCHASETYPE': PURCHASE_TYPE}
+    CE_FILTER_TEMPLATE = {
+        DIMENSIONS: {
+            KEY: '',
+            VALUES: []
+        }
+    }
+    CE_COST_FILTERS = {'SPOT': {KEY: PURCHASE_TYPE, VALUES: [SPOT_INSTANCES]}}
 
     def __init__(self, ce_client=''):
         self.cost_explorer_client = boto3.client('ce') if not ce_client else ce_client
 
+    def __get_ce_tag_filters(self, tag: str, ce_default_filter: dict):
+        """
+        This method returns the ce filter values
+        :return:
+        """
+        if ':' in tag:
+            tag, tag_filter = tag.split(':')
+            tag_filter = tag_filter.upper()
+            ce_filter = self.CE_FILTER_TEMPLATE
+            if tag_filter in self.CE_COST_FILTERS:
+                ce_filter[self.DIMENSIONS][self.KEY] = self.CE_COST_FILTERS[tag_filter][self.KEY]
+                ce_filter[self.DIMENSIONS][self.VALUES] = self.CE_COST_FILTERS[tag_filter][self.VALUES]
+            if ce_default_filter:
+                ce_default_filter = {
+                    'And': [
+                        ce_default_filter,
+                        ce_filter
+                    ]
+                }
+            else:
+                ce_default_filter = ce_filter
+        return ce_default_filter
+
     def get_cost_by_tags(self, tag: str, granularity: str = 'DAILY', cost_metric: str = 'UnblendedCost',
-                         start_date: str = '', end_date: str = ''):
+                         start_date: str = '', end_date: str = '', **kwargs):
         """
         This method extracts the price by Tag provided
         @return:
         """
         if not start_date and not end_date:
             end_date = datetime.now() + timedelta(self.START_DAY)
             start_date = end_date - timedelta(self.END_DAY)
             start_date = str(start_date.strftime('%Y-%m-%d'))
             end_date = str(end_date.strftime('%Y-%m-%d'))
-        if tag.upper() == 'ChargeType'.upper():
-            return self.get_cost_and_usage_from_aws(start_date=start_date, end_date=end_date, granularity=granularity,
-                                                    GroupBy=[{'Type': 'DIMENSION', 'Key': 'RECORD_TYPE'}])
-        elif tag.upper() == 'PURCHASETYPE':
+        if tag.upper() in self.CE_COST_TYPES:
             return self.get_cost_and_usage_from_aws(start_date=start_date, end_date=end_date, granularity=granularity,
-                                                    GroupBy=[{'Type': 'DIMENSION', 'Key': 'PURCHASE_TYPE'}])
+                                                    GroupBy=[{'Type': 'DIMENSION', 'Key': self.CE_COST_TYPES[tag.upper()]}], **kwargs)
         else:
+            kwargs[self.FILTER] = self.__get_ce_tag_filters(tag=tag, ce_default_filter=kwargs.get(self.FILTER))
+            if ':' in tag:
+                tag, tag_filter = tag.split(':')
             return self.get_cost_and_usage_from_aws(start_date=start_date, end_date=end_date, granularity=granularity,
-                                                    cost_metric=cost_metric, GroupBy=[{'Type': 'TAG', 'Key': tag}])
+                                                    cost_metric=cost_metric, GroupBy=[{'Type': 'TAG', 'Key': tag}], **kwargs)
 
     def get_cost_and_usage_from_aws(self, start_date: str, end_date: str, granularity: str = 'DAILY',
                                     cost_metric: str = 'UnblendedCost', **kwargs):
         """
         This method returns the cost and usage reports
         @param start_date:
         @param end_date:
         @param granularity:
         @param cost_metric:
         @param kwargs:
         @return:
         """
+        if self.FILTER in kwargs and not kwargs.get('Filter'):
+            kwargs.pop('Filter')
         usage_cost = {}
         response = self.cost_explorer_client.get_cost_and_usage(TimePeriod={
             'Start': start_date,
             'End': end_date
         }, Granularity=granularity, Metrics=[cost_metric], **kwargs)
         usage_cost['GroupDefinitions'] = response.get('GroupDefinitions')
         usage_cost['ResultsByTime'] = response.get('ResultsByTime')
```

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/iam/iam_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/iam/iam_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/price.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/price.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/resources_pricing.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/resources_pricing.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/aws/utils/utils.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/aws/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/gcp/google_account.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/gcp/google_account.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/account/ibm_account.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/account/ibm_account.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/classic/classic_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/classic/classic_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elastic_upload.py` & `cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elastic_upload.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elasticsearch_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elasticsearch_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from datetime import datetime, timedelta
 import time
 import pandas as pd
 from cloud_governance.main.environment_variables import environment_variables
 
 from elasticsearch_dsl import Search
 from elasticsearch import Elasticsearch
@@ -27,15 +26,16 @@
 
     def __init__(self, es_host: str, es_port: str, region: str = '', bucket: str = '', logs_bucket_key: str = '',
                  timeout: int = 2000):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__es_host = es_host
         self.__es_port = es_port
         self.__region = region
-        self.__timeout = int(self.__environment_variables_dict.get('ES_TIMEOUT')) if self.__environment_variables_dict.get('ES_TIMEOUT') else timeout
+        self.__timeout = int(
+            self.__environment_variables_dict.get('ES_TIMEOUT')) if self.__environment_variables_dict.get('ES_TIMEOUT') else timeout
         self.__es = Elasticsearch([{'host': self.__es_host, 'port': self.__es_port}], timeout=self.__timeout, max_retries=2)
 
     def __elasticsearch_get_index_hits(self, index: str, uuid: str = '', workload: str = '', fast_check: bool = False,
                                        id: bool = False):
         """
         This method search for data per index in last 2 minutes and return the number of docs or zero
         :param index:
@@ -127,15 +127,15 @@
         if es_add_items:
             for key, value in es_add_items.items():
                 data[key] = value
 
         # utcnow - solve timestamp issue
         if not data.get('timestamp'):
             data['timestamp'] = datetime.utcnow()  # datetime.now()
-
+        data['policy'] = self.__environment_variables_dict.get('policy')
         # Upload data to elastic search server
         try:
             if isinstance(data, dict):  # JSON Object
                 self.__es.index(index=index, doc_type=doc_type, body=data, **kwargs)
             else:  # JSON Array
                 for record in data:
                     self.__es.index(index=index, doc_type=doc_type, body=record, **kwargs)
@@ -204,28 +204,46 @@
         }
         query['query']['bool']['filter']['range']['timestamp']['lte'] = str(end_datetime.replace(microsecond=0))
         query['query']['bool']['filter']['range']['timestamp']['gte'] = str(start_datetime.replace(microsecond=0))
         return query
 
     @typechecked()
     @logger_time_stamp
-    def fetch_data_between_range(self, es_index: str, start_datetime: datetime, end_datetime: datetime):
+    def fetch_data_by_es_query(self, es_index: str, query: dict = None, start_datetime: datetime = None,
+                               end_datetime: datetime = None, result_agg: bool = False, group_by: str = ''):
         """
-        This method fetches the data in between range
+        This method fetches the data in between range, if you need aggregation results pass you own query with aggegation
         @param es_index:
         @param start_datetime:
         @param end_datetime:
+        @param query:
+        @param result_agg:
+        @param group_by:
         @return:
         """
+        es_data = []
         if self.__es.indices.exists(index=es_index):
-            query_body = self.get_query_data_between_range(start_datetime=start_datetime, end_datetime=end_datetime)
-            data = self.__es.search(index=es_index, body=query_body, doc_type='_doc').get('hits')
-            if data:
-                return data['hits']
-        return []
+            if not query:
+                if start_datetime and end_datetime:
+                    query = self.get_query_data_between_range(start_datetime=start_datetime, end_datetime=end_datetime)
+            if query:
+                response = self.__es.search(index=es_index, body=query, doc_type='_doc', size=100, scroll='1h')
+                if result_agg:
+                    es_data.extend(response.get('aggregations').get(group_by).get('buckets'))
+                else:
+                    scroll_id = response.get('_scroll_id')
+                    if response.get('hits').get('hits'):
+                        es_data.extend(response.get('hits').get('hits'))
+                    while scroll_id:
+                        response = self.__es.scroll(scroll_id=scroll_id, scroll="1h")
+                        if len(response.get('hits').get('hits')) > 0:
+                            es_data.extend(response.get('hits').get('hits'))
+                        else:
+                            break
+        return es_data
 
     @typechecked()
     @logger_time_stamp
     def delete_data_in_between_in_es(self, es_index: str, start_datetime: datetime, end_datetime: datetime):
         """
         This method deletes the data in between two ranges
         @param es_index:
```

### Comparing `cloud-governance-1.1.93/cloud_governance/common/google_drive/google_drive_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/google_drive/upload_to_gsheet.py` & `cloud-governance-1.1.94/cloud_governance/common/google_drive/upload_to_gsheet.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/jira/jira.py` & `cloud-governance-1.1.94/cloud_governance/common/jira/jira.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/jira/jira_operations.py` & `cloud-governance-1.1.94/cloud_governance/common/jira/jira_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/ldap/ldap_search.py` & `cloud-governance-1.1.94/cloud_governance/common/ldap/ldap_search.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/logger/logger_time_stamp.py` & `cloud-governance-1.1.94/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/mails/gmail.py` & `cloud-governance-1.1.94/cloud_governance/common/mails/gmail.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/mails/mail_message.py` & `cloud-governance-1.1.94/cloud_governance/common/mails/mail_message.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/common/mails/postfix.py` & `cloud-governance-1.1.94/cloud_governance/common/mails/postfix.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/main/environment_variables.py` & `cloud-governance-1.1.94/cloud_governance/main/environment_variables.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/main/es_uploader.py` & `cloud-governance-1.1.94/cloud_governance/main/es_uploader.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/main/main.py` & `cloud-governance-1.1.94/cloud_governance/main/main.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/cost_billing_reports.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/cost_explorer.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/cost_explorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from ast import literal_eval
 
 from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
 from cloud_governance.common.elasticsearch.elastic_upload import ElasticUpload
 from cloud_governance.common.clouds.aws.cost_explorer.cost_explorer_operations import CostExplorerOperations
 from cloud_governance.common.logger.init_logger import logger
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
@@ -12,14 +11,26 @@
 class CostExplorer:
     """
     This class fetches the cost_explorer report from the AWS based on two days ago data and upload to ElasticSearch.
     fetching AWS cost explorer of two days ago because day ago cost calculation is not closed.
     """
 
     BULK_UPLOAD_THREADS = 8
+    SAVINGS_PLAN_FILTER = {  # savings plan usage for ce filter
+                            'Dimensions': {
+                                        'Key': 'RECORD_TYPE',
+                                        'Values': ['SavingsPlanRecurringFee', 'SavingsPlanNegation', 'SavingsPlanCoveredUsage']
+                                }
+                    }
+    EXCLUDE = 'exclude'
+    INCLUDE = 'include'
+    CE_KEY_RESULTS_BY_TIME = 'ResultsByTime'
+    INDEX_ID = 'index_id'
+    APPEND = 'a'
+    CE_OPERATION = 'Not'
 
     def __init__(self):
         super().__init__()
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.start_date = self.__environment_variables_dict.get('start_date', '')  # yyyy-mm-dd
         self.end_date = self.__environment_variables_dict.get('end_date', '')  # yyyy-mm-dd
         self.granularity = self.__environment_variables_dict.get('granularity', 'DAILY')
@@ -28,19 +39,20 @@
         self.file_name = self.__environment_variables_dict.get('file_name', '')
         self.__cost_explorer = CostExplorerOperations()
         self.region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', 'us-east-1')
         self._ec2_operations = EC2Operations(region=self.region)
         self._elastic_upload = ElasticUpload()
         self.__account = self.__environment_variables_dict.get('account').upper().replace('OPENSHIFT-', "").strip()
 
-    def filter_data_by_tag(self, groups: dict, tag: str):
+    def filter_data_by_tag(self, groups: dict, tag: str, savings_plan: str):
         """
         This method extract data by tag
         @param tag:
         @param groups: Data from the cloud explorer
+        @param savings_plan:
         @return: converted into dict format
         """
         data = {}
         start_time = groups.get('TimePeriod').get('Start')
         account = self.__account
         for group in groups.get('Groups'):
             name = ''
@@ -54,59 +66,64 @@
                 amount = group.get('Metrics').get(self.cost_metric).get('Amount')
             if name and amount:
                 if 'aws-go-sdk' in name:
                     name = 'aws-go-sdk'
                 else:
                     if 'vm_import_image' in name:
                         name = 'vm_import_image'
-                index_id = f'{start_time.lower()}-{account.lower()}-{tag.lower()}-{name.lower()}'
+                index_id = f'{start_time}-{account}-{tag}-savings-{savings_plan}-{name}'.lower()
                 if index_id not in data:
-                    upload_data = {tag: name if tag.upper() in ('ChargeType'.upper(), 'PurchaseType'.upper()) else name.upper(),
-                                   'Cost': round(float(amount), 3), 'index_id': index_id, 'timestamp': start_time}
+                    upload_data = {tag: name if tag.upper() in list(self.__cost_explorer.CE_COST_TYPES) else name.upper(),
+                                   'Cost': round(float(amount), 3), self.INDEX_ID: index_id, 'timestamp': start_time, 'savings_plan': savings_plan}
                     if 'global' in self._elastic_upload.es_index:
                         if 'Budget' not in upload_data:
                             upload_data['Budget'] = self._elastic_upload.account
+                    upload_data['tag'] = tag.lower()
                     data[index_id] = upload_data
                 else:
                     data[index_id]['Cost'] += round(float(amount), 3)
         return list(data.values())
 
     def __get_daily_cost_by_tags(self):
         """
         This method extracts the costs by tags and upload to elastic search
         @return:
         """
         data_house = {}
         for tag in self.cost_tags:
-            if self.start_date and self.end_date:
-                response = self.__cost_explorer.get_cost_by_tags(tag=tag, start_date=self.start_date, end_date=self.end_date, granularity=self.granularity, cost_metric=self.cost_metric)
-            else:
-                response = self.__cost_explorer.get_cost_by_tags(tag=tag, granularity=self.granularity, cost_metric=self.cost_metric)
-            results_by_time = response.get('ResultsByTime')
-            if results_by_time:
-                data_house[tag] = []
-                for result in results_by_time:
-                    data_house[tag].extend(self.filter_data_by_tag(result, tag))
+            for savings_plan in [self.EXCLUDE, self.INCLUDE]:
+                filters = {}
+                if savings_plan == self.EXCLUDE:
+                    filters = {self.CE_OPERATION: self.SAVINGS_PLAN_FILTER}
+                if self.start_date and self.end_date:
+                    response = self.__cost_explorer.get_cost_by_tags(tag=tag, start_date=self.start_date, end_date=self.end_date, granularity=self.granularity, cost_metric=self.cost_metric, Filter=filters)
+                else:
+                    response = self.__cost_explorer.get_cost_by_tags(tag=tag, granularity=self.granularity, cost_metric=self.cost_metric, Filter=filters)
+                results_by_time = response.get(self.CE_KEY_RESULTS_BY_TIME)
+                if results_by_time:
+                    data_house[f'{tag}-{savings_plan}'] = []
+                    for result in results_by_time:
+                        data_house[f'{tag}-{savings_plan}'].extend(self.filter_data_by_tag(result, tag, savings_plan))
         return data_house
 
     @logger_time_stamp
     def __upload_data(self, data: list, index: str):
         """
         This method upload to elastic search
         @param data:
         @param index:
         @return:
         """
         if self.file_name:
-            with open(f'/tmp/{self.file_name}', 'a') as file:
+            with open(f'/tmp/{self.file_name}', self.APPEND) as file:
                 for value in data:
                     file.write(f'{value}\n')
         else:
             for value in data:
-                self.upload_item_to_es(index=index, item=value, index_id=value['index_id'])
+                self.upload_item_to_es(index=index, item=value, index_id=value[self.INDEX_ID])
             logger.info(f'Data uploaded to {index}, Total Data: {len(data)}')
 
     def upload_item_to_es(self, item: dict, index: str, index_id: str = ''):
         """
         This method upload one item to es
         @param item:
         @param index:
@@ -122,16 +139,16 @@
         """
         This method upload daily tag cost into ElasticSearch
         @return:
         """
         logger.info(f'Get {self.granularity} Cost usage by metric: {self.cost_metric}')
         cost_data = self.__get_daily_cost_by_tags()
         for key, values in cost_data.items():
-            index = f'{self._elastic_upload.es_index}-{key.lower()}'
-            self.__upload_data(values, index)
+            logger.info(f"Uploading the data of {key} tag")
+            self.__upload_data(values, self._elastic_upload.es_index)
 
     def run(self):
         """
         This method run the operations
         @return:
         """
         self.upload_tags_cost_to_elastic_search()
```

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/cost_explorer_payer_billings.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/cost_explorer_payer_billings.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/cost_over_usage.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/ebs_in_use.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/ebs_in_use.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/ebs_unattached.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_idle.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_idle.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_run.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_stop.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_stop.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/empty_roles.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/empty_roles.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/ip_unattached.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/ip_unattached.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/monthly_report.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/monthly_report.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/s3_inactive.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/s3_inactive.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/skipped_resources.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/skipped_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/unused_nat_gateway.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/unused_nat_gateway.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/zombie_cluster_resource.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/aws/zombie_snapshots.py` & `cloud-governance-1.1.94/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/azure/cost_billing_reports.py` & `cloud-governance-1.1.94/cloud_governance/policy/azure/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/gcp/cost_billing_reports.py` & `cloud-governance-1.1.94/cloud_governance/policy/gcp/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/ibm/cost_billing_reports.py` & `cloud-governance-1.1.94/cloud_governance/policy/ibm/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/ibm/ibm_cost_over_usage.py` & `cloud-governance-1.1.94/cloud_governance/policy/ibm/ibm_cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/ibm/ibm_cost_report.py` & `cloud-governance-1.1.94/cloud_governance/policy/ibm/ibm_cost_report.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/ibm/tag_baremetal.py` & `cloud-governance-1.1.94/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/ibm/tag_vm.py` & `cloud-governance-1.1.94/cloud_governance/policy/ibm/tag_vm.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py` & `cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance.egg-info/PKG-INFO` & `cloud-governance-1.1.94/cloud_governance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.93
+Version: 1.1.94
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloud-governance-1.1.93/cloud_governance.egg-info/SOURCES.txt` & `cloud-governance-1.1.94/cloud_governance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/cloud_governance.egg-info/requires.txt` & `cloud-governance-1.1.94/cloud_governance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.93/setup.py` & `cloud-governance-1.1.94/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.1.93'
+__version__ = '1.1.94'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

