# Comparing `tmp/resource-lister-1.1.0.tar.gz` & `tmp/resource-lister-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Abhijit\AWS\GIT-Publishing\repository\resource-lister\dist\.tmp-suubc6e6\resource-lister-1.1.0.tar", last modified: Thu Apr 13 03:08:47 2023, max compression
+gzip compressed data, was "C:\Abhijit\AWS\GIT-Publishing\repository\resource-lister\dist\.tmp-g65wz54v\resource-lister-1.2.0.tar", last modified: Tue May  9 02:56:00 2023, max compression
```

## Comparing `resource-lister-1.1.0.tar` & `resource-lister-1.2.0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.482880 resource-lister-1.1.0/
--rw-rw-rw-   0        0        0    11525 2023-03-20 16:57:45.000000 resource-lister-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      122 2023-02-18 03:26:18.000000 resource-lister-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0       68 2023-04-11 18:33:31.000000 resource-lister-1.1.0/NOTICE
--rw-rw-rw-   0        0        0    10284 2023-04-13 03:08:47.477078 resource-lister-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9724 2023-04-12 19:06:59.000000 resource-lister-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.892903 resource-lister-1.1.0/cfn/
--rw-rw-rw-   0        0        0     4006 2023-03-03 17:37:23.000000 resource-lister-1.1.0/cfn/cfn_s3_bucket_master_account.json
--rw-rw-rw-   0        0        0     3949 2023-03-03 03:24:49.000000 resource-lister-1.1.0/cfn/master_account_IAM_role.json
--rw-rw-rw-   0        0        0      732 2023-04-13 02:53:53.000000 resource-lister-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 03:08:47.484486 resource-lister-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.865393 resource-lister-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.901448 resource-lister-1.1.0/src/resource_lister/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/__init__.py
--rw-rw-rw-   0        0        0       64 2023-03-25 17:10:45.000000 resource-lister-1.1.0/src/resource_lister/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.975969 resource-lister-1.1.0/src/resource_lister/boto_formatter/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/__init__.py
--rw-rw-rw-   0        0        0     7595 2023-02-27 03:30:46.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/core_formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.990001 resource-lister-1.1.0/src/resource_lister/boto_formatter/json_util/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/json_util/__init__.py
--rw-rw-rw-   0        0        0    10769 2023-01-30 03:32:28.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/json_util/json_util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.006600 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/__init__.py
--rw-rw-rw-   0        0        0     5848 2022-12-29 03:55:50.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_config.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.281917 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json
--rw-rw-rw-   0        0        0     1086 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/apigateway.json
--rw-rw-rw-   0        0        0     2104 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/budgets.json
--rw-rw-rw-   0        0        0     1037 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudformation.json
--rw-rw-rw-   0        0        0    10697 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudfront.json
--rw-rw-rw-   0        0        0      623 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudtrail.json
--rw-rw-rw-   0        0        0     1350 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudwatch.json
--rw-rw-rw-   0        0        0      643 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/codecommit.json
--rw-rw-rw-   0        0        0       73 2023-01-27 22:09:30.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/describe_cache_clusters.json
--rw-rw-rw-   0        0        0      555 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/dynamodb.json
--rw-rw-rw-   0        0        0    34336 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ec2.json
--rw-rw-rw-   0        0        0     1510 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ecs.json
--rw-rw-rw-   0        0        0     1464 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/efs.json
--rw-rw-rw-   0        0        0     3576 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/eks.json
--rw-rw-rw-   0        0        0     4475 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elasticache.json
--rw-rw-rw-   0        0        0     1594 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elbv2.json
--rw-rw-rw-   0        0        0     1795 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr-serverless.json
--rw-rw-rw-   0        0        0     5490 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr.json
--rw-rw-rw-   0        0        0     7276 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/iam.json
--rw-rw-rw-   0        0        0      585 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/kms.json
--rw-rw-rw-   0        0        0     3425 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/lambda.json
--rw-rw-rw-   0        0        0     1447 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/organizations.json
--rw-rw-rw-   0        0        0    17897 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/rds.json
--rw-rw-rw-   0        0        0     2630 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json
--rw-rw-rw-   0        0        0     7405 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json
--rw-rw-rw-   0        0        0     3129 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json
--rw-rw-rw-   0        0        0     1753 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json
--rw-rw-rw-   0        0        0     2526 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json
--rw-rw-rw-   0        0        0     3480 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json
--rw-rw-rw-   0        0        0     1212 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json
--rw-rw-rw-   0        0        0      548 2023-03-13 03:17:54.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json
--rw-rw-rw-   0        0        0     7440 2023-02-27 03:30:45.000000 resource-lister-1.1.0/src/resource_lister/boto_formatter/service_formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.305704 resource-lister-1.1.0/src/resource_lister/config_mgr/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/config_mgr/__init__.py
--rw-rw-rw-   0        0        0      129 2023-02-21 16:45:05.000000 resource-lister-1.1.0/src/resource_lister/config_mgr/config.json
--rw-rw-rw-   0        0        0     4276 2023-03-22 01:14:18.000000 resource-lister-1.1.0/src/resource_lister/config_mgr/config_menu_processor.py
--rw-rw-rw-   0        0        0     2264 2023-03-22 01:14:33.000000 resource-lister-1.1.0/src/resource_lister/config_mgr/config_util.py
--rw-rw-rw-   0        0        0      103 2023-03-25 16:15:33.000000 resource-lister-1.1.0/src/resource_lister/main.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.341962 resource-lister-1.1.0/src/resource_lister/menu/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/menu/__init__.py
--rw-rw-rw-   0        0        0     3888 2023-03-22 01:19:46.000000 resource-lister-1.1.0/src/resource_lister/menu/batch_processing.py
--rw-rw-rw-   0        0        0    34834 2023-03-13 03:36:33.000000 resource-lister-1.1.0/src/resource_lister/menu/menu_config.json
--rw-rw-rw-   0        0        0    12825 2023-04-12 16:26:38.000000 resource-lister-1.1.0/src/resource_lister/menu/menu_processor.py
--rw-rw-rw-   0        0        0     6134 2023-03-14 16:30:15.000000 resource-lister-1.1.0/src/resource_lister/menu/menu_util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.379737 resource-lister-1.1.0/src/resource_lister/processor/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/processor/__init__.py
--rw-rw-rw-   0        0        0     3635 2023-03-22 01:23:29.000000 resource-lister-1.1.0/src/resource_lister/processor/_global_no_paginate.py
--rw-rw-rw-   0        0        0     3771 2023-02-27 03:30:43.000000 resource-lister-1.1.0/src/resource_lister/processor/_global_paginate.py
--rw-rw-rw-   0        0        0     4502 2023-02-27 04:04:32.000000 resource-lister-1.1.0/src/resource_lister/processor/_regional_no_paginate.py
--rw-rw-rw-   0        0        0     4877 2023-02-27 04:06:31.000000 resource-lister-1.1.0/src/resource_lister/processor/_regional_paginate.py
--rw-rw-rw-   0        0        0      426 2023-03-22 01:21:21.000000 resource-lister-1.1.0/src/resource_lister/processor/core_processor.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.419504 resource-lister-1.1.0/src/resource_lister/session_mgr/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:19:16.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/__init__.py
--rw-rw-rw-   0        0        0      242 2023-04-11 14:46:14.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/account_config.json
--rw-rw-rw-   0        0        0     8919 2023-04-11 14:55:49.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/account_config_util.py
--rw-rw-rw-   0        0        0     4805 2023-04-11 15:24:28.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/accounts_menu_processor.py
--rw-rw-rw-   0        0        0    10969 2023-04-11 15:22:16.000000 resource-lister-1.1.0/src/resource_lister/session_mgr/iam_session_mgr.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:47.468175 resource-lister-1.1.0/src/resource_lister/util/
--rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.1.0/src/resource_lister/util/__init__.py
--rw-rw-rw-   0        0        0     7075 2023-04-11 14:42:54.000000 resource-lister-1.1.0/src/resource_lister/util/menu_configs.py
--rw-rw-rw-   0        0        0     9176 2023-03-23 14:48:06.000000 resource-lister-1.1.0/src/resource_lister/util/menu_util.py
--rw-rw-rw-   0        0        0      231 2023-03-23 13:53:26.000000 resource-lister-1.1.0/src/resource_lister/util/resource_lister_exceptions.py
--rw-rw-rw-   0        0        0     2297 2023-04-11 13:25:41.000000 resource-lister-1.1.0/src/resource_lister/util/s3_util.py
--rw-rw-rw-   0        0        0     1264 2023-04-11 15:21:36.000000 resource-lister-1.1.0/src/resource_lister/util/session_util.py
--rw-rw-rw-   0        0        0      670 2023-02-24 02:30:16.000000 resource-lister-1.1.0/src/resource_lister/util/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:08:46.943965 resource-lister-1.1.0/src/resource_lister.egg-info/
--rw-rw-rw-   0        0        0    10284 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4811 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 03:08:46.000000 resource-lister-1.1.0/src/resource_lister.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.958988 resource-lister-1.2.0/
+-rw-rw-rw-   0        0        0    11525 2023-03-20 16:57:45.000000 resource-lister-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      122 2023-02-18 03:26:18.000000 resource-lister-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0       68 2023-04-11 18:33:31.000000 resource-lister-1.2.0/NOTICE
+-rw-rw-rw-   0        0        0    14104 2023-05-09 02:56:00.956245 resource-lister-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13544 2023-05-09 02:45:13.000000 resource-lister-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.388155 resource-lister-1.2.0/cfn/
+-rw-rw-rw-   0        0        0     4006 2023-03-03 17:37:23.000000 resource-lister-1.2.0/cfn/cfn_s3_bucket_master_account.json
+-rw-rw-rw-   0        0        0     3949 2023-03-03 03:24:49.000000 resource-lister-1.2.0/cfn/master_account_IAM_role.json
+-rw-rw-rw-   0        0        0      732 2023-05-09 02:55:37.000000 resource-lister-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 02:56:00.959555 resource-lister-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.328875 resource-lister-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.410514 resource-lister-1.2.0/src/resource_lister/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.2.0/src/resource_lister/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-03-25 17:10:45.000000 resource-lister-1.2.0/src/resource_lister/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.460174 resource-lister-1.2.0/src/resource_lister/boto_formatter/
+-rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/__init__.py
+-rw-rw-rw-   0        0        0     7595 2023-02-27 03:30:46.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/core_formatter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.475574 resource-lister-1.2.0/src/resource_lister/boto_formatter/json_util/
+-rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/json_util/__init__.py
+-rw-rw-rw-   0        0        0    10769 2023-01-30 03:32:28.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/json_util/json_util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.496710 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/
+-rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/__init__.py
+-rw-rw-rw-   0        0        0     5848 2022-12-29 03:55:50.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_config.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.703774 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/
+-rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/__init__.py
+-rw-rw-rw-   0        0        0     2064 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json
+-rw-rw-rw-   0        0        0     1086 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/apigateway.json
+-rw-rw-rw-   0        0        0     2104 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/budgets.json
+-rw-rw-rw-   0        0        0     1037 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudformation.json
+-rw-rw-rw-   0        0        0    10697 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudfront.json
+-rw-rw-rw-   0        0        0      623 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudtrail.json
+-rw-rw-rw-   0        0        0     1350 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudwatch.json
+-rw-rw-rw-   0        0        0      643 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/codecommit.json
+-rw-rw-rw-   0        0        0       73 2023-01-27 22:09:30.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/describe_cache_clusters.json
+-rw-rw-rw-   0        0        0      555 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/dynamodb.json
+-rw-rw-rw-   0        0        0    34336 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ec2.json
+-rw-rw-rw-   0        0        0     1510 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ecs.json
+-rw-rw-rw-   0        0        0     1464 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/efs.json
+-rw-rw-rw-   0        0        0     3576 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/eks.json
+-rw-rw-rw-   0        0        0     4475 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elasticache.json
+-rw-rw-rw-   0        0        0     1594 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elbv2.json
+-rw-rw-rw-   0        0        0     1795 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr-serverless.json
+-rw-rw-rw-   0        0        0     5490 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr.json
+-rw-rw-rw-   0        0        0     7276 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/iam.json
+-rw-rw-rw-   0        0        0      585 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/kms.json
+-rw-rw-rw-   0        0        0     3425 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/lambda.json
+-rw-rw-rw-   0        0        0     1447 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/organizations.json
+-rw-rw-rw-   0        0        0    17897 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/rds.json
+-rw-rw-rw-   0        0        0     2630 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json
+-rw-rw-rw-   0        0        0     7405 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json
+-rw-rw-rw-   0        0        0     3129 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json
+-rw-rw-rw-   0        0        0     1753 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json
+-rw-rw-rw-   0        0        0     2526 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json
+-rw-rw-rw-   0        0        0     3480 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json
+-rw-rw-rw-   0        0        0     1212 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json
+-rw-rw-rw-   0        0        0      548 2023-03-13 03:17:54.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json
+-rw-rw-rw-   0        0        0     1472 2023-05-09 01:39:46.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ssm.json
+-rw-rw-rw-   0        0        0     7440 2023-02-27 03:30:45.000000 resource-lister-1.2.0/src/resource_lister/boto_formatter/service_formatter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.730625 resource-lister-1.2.0/src/resource_lister/config_mgr/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.2.0/src/resource_lister/config_mgr/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-02-21 16:45:05.000000 resource-lister-1.2.0/src/resource_lister/config_mgr/config.json
+-rw-rw-rw-   0        0        0     4276 2023-03-22 01:14:18.000000 resource-lister-1.2.0/src/resource_lister/config_mgr/config_menu_processor.py
+-rw-rw-rw-   0        0        0     2264 2023-03-22 01:14:33.000000 resource-lister-1.2.0/src/resource_lister/config_mgr/config_util.py
+-rw-rw-rw-   0        0        0      103 2023-03-25 16:15:33.000000 resource-lister-1.2.0/src/resource_lister/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.774774 resource-lister-1.2.0/src/resource_lister/menu/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.2.0/src/resource_lister/menu/__init__.py
+-rw-rw-rw-   0        0        0     3888 2023-03-22 01:19:46.000000 resource-lister-1.2.0/src/resource_lister/menu/batch_processing.py
+-rw-rw-rw-   0        0        0    35731 2023-05-09 01:43:01.000000 resource-lister-1.2.0/src/resource_lister/menu/menu_config.json
+-rw-rw-rw-   0        0        0    12825 2023-04-12 16:26:38.000000 resource-lister-1.2.0/src/resource_lister/menu/menu_processor.py
+-rw-rw-rw-   0        0        0     6134 2023-03-14 16:30:15.000000 resource-lister-1.2.0/src/resource_lister/menu/menu_util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.838717 resource-lister-1.2.0/src/resource_lister/processor/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.2.0/src/resource_lister/processor/__init__.py
+-rw-rw-rw-   0        0        0     3635 2023-03-22 01:23:29.000000 resource-lister-1.2.0/src/resource_lister/processor/_global_no_paginate.py
+-rw-rw-rw-   0        0        0     3771 2023-02-27 03:30:43.000000 resource-lister-1.2.0/src/resource_lister/processor/_global_paginate.py
+-rw-rw-rw-   0        0        0     4502 2023-02-27 04:04:32.000000 resource-lister-1.2.0/src/resource_lister/processor/_regional_no_paginate.py
+-rw-rw-rw-   0        0        0     4877 2023-02-27 04:06:31.000000 resource-lister-1.2.0/src/resource_lister/processor/_regional_paginate.py
+-rw-rw-rw-   0        0        0      426 2023-03-22 01:21:21.000000 resource-lister-1.2.0/src/resource_lister/processor/core_processor.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.899349 resource-lister-1.2.0/src/resource_lister/session_mgr/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:19:16.000000 resource-lister-1.2.0/src/resource_lister/session_mgr/__init__.py
+-rw-rw-rw-   0        0        0      242 2023-04-11 14:46:14.000000 resource-lister-1.2.0/src/resource_lister/session_mgr/account_config.json
+-rw-rw-rw-   0        0        0     8919 2023-04-11 14:55:49.000000 resource-lister-1.2.0/src/resource_lister/session_mgr/account_config_util.py
+-rw-rw-rw-   0        0        0     4805 2023-04-11 15:24:28.000000 resource-lister-1.2.0/src/resource_lister/session_mgr/accounts_menu_processor.py
+-rw-rw-rw-   0        0        0    10969 2023-04-11 15:22:16.000000 resource-lister-1.2.0/src/resource_lister/session_mgr/iam_session_mgr.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.946717 resource-lister-1.2.0/src/resource_lister/util/
+-rw-rw-rw-   0        0        0        0 2023-01-25 16:20:16.000000 resource-lister-1.2.0/src/resource_lister/util/__init__.py
+-rw-rw-rw-   0        0        0     7075 2023-04-11 14:42:54.000000 resource-lister-1.2.0/src/resource_lister/util/menu_configs.py
+-rw-rw-rw-   0        0        0     9176 2023-03-23 14:48:06.000000 resource-lister-1.2.0/src/resource_lister/util/menu_util.py
+-rw-rw-rw-   0        0        0      231 2023-03-23 13:53:26.000000 resource-lister-1.2.0/src/resource_lister/util/resource_lister_exceptions.py
+-rw-rw-rw-   0        0        0     2297 2023-04-11 13:25:41.000000 resource-lister-1.2.0/src/resource_lister/util/s3_util.py
+-rw-rw-rw-   0        0        0     1264 2023-04-11 15:21:36.000000 resource-lister-1.2.0/src/resource_lister/util/session_util.py
+-rw-rw-rw-   0        0        0      670 2023-02-24 02:30:16.000000 resource-lister-1.2.0/src/resource_lister/util/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:56:00.442712 resource-lister-1.2.0/src/resource_lister.egg-info/
+-rw-rw-rw-   0        0        0    14104 2023-05-09 02:56:00.000000 resource-lister-1.2.0/src/resource_lister.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4890 2023-05-09 02:56:00.000000 resource-lister-1.2.0/src/resource_lister.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 02:56:00.000000 resource-lister-1.2.0/src/resource_lister.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-09 02:56:00.000000 resource-lister-1.2.0/src/resource_lister.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-09 02:56:00.000000 resource-lister-1.2.0/src/resource_lister.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 02:56:00.000000 resource-lister-1.2.0/src/resource_lister.egg-info/top_level.txt
```

### Comparing `resource-lister-1.1.0/LICENSE` & `resource-lister-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/PKG-INFO` & `resource-lister-1.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,194 @@
-Metadata-Version: 2.1
-Name: resource-lister
-Version: 1.1.0
-Summary: Resource Lister
-Author-email: Abhijit Rajeshirke <rajeabh@amazon.com>
-Project-URL: Homepage, https://github.com/awslabs/resource-lister
-Project-URL: Bug Tracker, https://github.com/awslabs/resource-lister/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
-#  Resource Lister (Multi Accounts)
-Resource Lister is  open source, interactive, python-based command line **NO CODE** utility. Resource Lister can generate list of AWS resources in single or multiple accounts in consumable CSV, or flatten JSON format in near real time. Resource Lister uses boto3 sessions and underlying List APIs to connect multiple configured child accounts and generate the list. Resource Lister also provides an option to output generated list to command line, file ,and s3.
-Multi Account Resource Lister can be configured to run from Cloud9, EC2 or from your local laptop.
-
-# Usage : 
-
-Resource lister utility is open source interactive command line tool for Developers, Solution Architect, Account Owners, Cloud Ops team or anyone who wants to simply list AWS Resources (for **supported services**) in an account or multiple accounts in consumable format like .csv without writing a code 
+#  Resource Lister (Multi Accounts) 
+Resource Lister is an open source, **NO CODE**, interactive, python-based command line utility. Resource Lister can generate **centralized**list of AWS resources (for **supported services**) in single or multiple accounts in consumable CSV, or flatten JSON format. Resource Lister uses AWS SDK for Python(Boto3) sessions and underlying Boto3 List APIs to connect multiple configured child accounts and generate the  resource list. It essentially **simplifies** accessing of Boto3 list APIs. Resource Lister also provides an option to send generated list to  file,  s3, or print on command line.
+Resource Lister can be configured to run from Cloud9, Cloudshell, EC2 or from your machine.
+
+# Usage: 
+
+Resource Lister Utility can be helpful to addresses following usecase
+
+* Resource Lister is handy utility for Developers, Solution Architect, Account Owners, Cloud Ops team or anyone who simply wants to generate list of AWS Resources (for **supported services**) across accounts and across regions without writing any custom code. 
+
+* Utility can help generate list of inventory of AWS resources across region and across accounts in near real time. For example, operation team wants to verify there is no lambda function created in restricted regions in near real time. You can also run the utility in batch mode across all the configured AWS services and create inventory.
+
+* Utility can help enforce budgetary constraints. For example, utility can help Account owners to identify which AWS accounts doesn't have AWS budget setup.
+
+* Utility can help identify particular type of list of resources.
+for example, you can generate list of lambda function and filter lambda function using python 2.6 version.
+
+* Utility flattens the response in consumable csv format.
 
-Cloud Operation team can generate inventory of AWS resources in near real time accorss accounts and across regions for **supported services** without writing any code.
 
-Operation team can identify which AWS accounts doesn't have budget setup.
 
-Utility can help generate list in particular account/region and then you can filter particular type of resource like lambda function using python 2.6 version.
 
-Resource list generated through utility is with 99% of attributes which python SDK sends back (Including configured Tags for the resource), Manually getting and formatting all the attributes and formatting in tabular/columnize format specifically .csv is tedious task utility does it for you.
 
 
 # How it works?
 
-Run the utility 
-Utility will start interactive Python session.
+<p align="center">
+  <img src="imgs/0_utility_interface.PNG"  title="Utility Interface">
 
-**Step 1**:  Utility will prompt you to select the AWS Service for example S3,lambda or ec2 etc..
+After you install and configure the Resource Lister you can run the Resource lister utility using pipx run.
 
-**Step 2** : Utility will display number of supported functions for selected AWS service . You chose a perticular function for example  **List of S3 Buckets **
+```
+pipx run resource_lister
+```
 
-**Step 3** : Utility will prompt you to select AWS Account for which you want list of AWS resources, you can select ALL accounts by entering ALL or specify comma seperated list of accounts
 
-**Step 4** : If it's regional resource (example Lambda) you will promopt to select AWS Region ; you can select ALL for all the regions or specify comma seperated list of regions
 
-**Step 5**: Finally, utility will generate the list of AWS Resources for selected Accounts and Regions send the output to File or S3 Bucket or Print on command prompt depending upon your configuration.
+**1** .  **Select AWS Service** : Resource Lister Utility will prompt you to select the AWS Service: You can select any of 27 services example S3, lambda or ec2
 
-You can also run the utility in batch mode across all the services in selected AWS Account 
+**2** .  **Select Function**: Resource Lister Utility will display number of supported functions for selected AWS service: Example List of S3 buckets or List of Aurora DB clusters or List of Lambda functions depending upon service you selected.
+
+**3** . **Select Account(s)**: Resource Lister Utility will prompt you to select AWS Account for which you want to generate list of AWS resources:  You can enter ALL to select all the accounts or you can enter single account or comma separated list of accounts. If you don’t know the account number you just press ENTER and utility will prompt you with list of configured accounts. 
+
+**4** . **Select Region(s) for Regional services**: If it's regional resource (example Lambda) you will prompt to select AWS Region; you can select ALL for all the regions or specify comma separated list of regions
+
+**5** . **Result**: Resource lister utility will then generates the list of AWS Resources for selected accounts and regions send the output to file or S3 Bucket or print on command prompt depending upon your configuration.
 
 <p align="center">
   <img src="imgs/01_utility_interface.PNG"  title="Utility Interface">
 
 **Output**
 <p align="center">
   <img src="imgs/02_utility_output.PNG"  title="Utility Interface">
 
-# Prerequisite
-1. python3
-2. boto3
 
 
-# Installation
+**Note** : You can also run the utility in batch mode across all the services in selected AWS Account by going to help --> option # 6
 
 
+# Prerequisite
+1. [Python](https://www.python.org/)
+2. [AWS CLI](https://aws.amazon.com/cli/)
+
+# Installation
 
-**resource-lister** is distributed on PyPI. Easiest way to install it is with pip
-Create a virtual environment (optional):
+You can install and run **Resource lister** using [pipx](https://pypa.github.io/pipx/)
 
+**On macOS, Linux, install via pip (requires pip 19.0 or later)**
 ```
-python3 -m venv .venv
-
+python3 -m pip install  pipx
+python3 -m pip install  boto3
+python3 -m pipx install resource-lister
 ```
-Activate enviornment
+**On Windows, install via pip (requires pip 19.0 or later)**
 
+If you installed python using the app-store, replace `python` with `python3` in the next line.
 ```
-source .venv/bin/activate
+python -m pip install pipx
+python -m pip install boto3
+python -m pipx install resource-lister
 ```
 
-Install resource-lister
+**Run the Resource Lister Utility using pipx**
 
+**On macOS, Linux, install via pip (requires pip 19.0 or later)**
 ```
-pip install resource-lister
+python3 -m pipx run resource_lister
 ```
+**On Windows, install via pip (requires pip 19.0 or later)**
 
-# Run Resource Lister Utility
+```
+python -m pipx run resource_lister
+```
 
-Download main.py from github
+Resource lister utility will open in command prompt
 
-https://github.com/awslabs/resource-lister/blob/main/install/main.py
+<p align="center">
+  <img src="imgs/05_install_01.PNG"  title="Utility Interface">
 
-Run main.py python file with below command
+# Setup
+<details>
 
-```
-python3 main.py
-```
+  <summary>
+  <b>Express setup for single account using default credentials. </b>
+  </summary>
+You will use default IAM credentials for this setup. Ensure your current default credentials should have <b>read only permissions</b> 
+
+
+<b>Step1 : Navigate to  "Add Master Account"  </b>
 
-Utility will open in command prompt
+Type <b>help</b>--><b>1</b> [Manage AWS Account]--><b>1</b> [Add Master Account.]
 
 <p align="center">
-  <img src="imgs/05_install_01.PNG"  title="Utility Interface">
+  <img src="imgs/express_setup_01.PNG"  title="Utility Interface">
+
+
+
+<b>Step2 : Configure Master account with dummy values </b>
+
+Since express setup we are using default credentials. Use dummy values for Master Account ARN like **arn:aws:iam::<Your 12 Digit Account>:role/dummy_role** and for child account role name enter **dummy_role**
+
+
+<p align="center">
+  <img src="imgs/express_setup_02.PNG"  title="Utility Interface">
+
+<b>Congratulations! AWS Account is successfully configured. </b>
+
+<b>Step3: Navigate back to main search </b>
+
+
+Type 0 to exit
+<b>0</b>--><b>0</b>
+
+<p align="center">
+  <img src="imgs/express_setup_03.PNG"  title="Utility Interface">
+
+
+<b>Step4 : Test Utility by generating list of s3 buckets .csv file  </b>
+
+Enter AWS service for help (help) for Exit (0) :--><b>s3</b>
+
+Please select any of following options:
+1. [List of S3 buckets]
+2. [List of the objects in a S3 Bucket]
+Please enter option HERE--><b>1</b>
+
+Please enter comma separated account id(s) or ALL  HERE--><b>ALL</b>
+
+
+<p align="center">
+  <img src="imgs/01_utility_interface.PNG"  title="Utility Interface">
+
+Utility will create output folder and generate the .csv file with list of s3 buckets in your account.
+
+<p align="center">
+  <img src="imgs/02_utility_output.PNG"  title="Utility Interface">
+
+
+
+  </details>
+
+
+
+<details> 
+<summary>
+<b>Multi Account configurations.
+</b>
+</summary>
 
-# setup
 
-Click on enviornment specific installation setup.
 
 - [Cloud9 setup](https://github.com/awslabs/resource-lister/blob/main/docs/cloud_9_setup.md)
 
-- [Cloudshell setup](https://github.com/awslabs/resource-lister/blob/main/docs/cloud_9_setup.md)
+- [Cloudshell setup](https://github.com/awslabs/resource-lister/blob/main/docs/cloudshell_setup.md)
 
-- [Desktop setup](https://github.com/awslabs/resource-lister/blob/main/docs/cloud_9_setup.md)
 
 
+</details>
 
 # Help
 [General help](https://github.com/awslabs/resource-lister/blob/main/docs/help_guide.md)
 
-
-# Supported Services and Functionality 
+# Supported Services and Functionality
+<details> 
+<summary>
+<b> Supported Services and Functionality  </b>
+</summary>
 <table>
 <tbody>
 <tr>
 <th>Service</th>
 <th>Functions</th>
 </tr>
 <tr>
@@ -190,221 +259,239 @@
 </td>
 </tr>
 <tr>
 <td> ec2</td>
 <td>
 <ul>
 <li>12.List of EC2 instances </li>
-<li>13.List of VPCs</li>
-<li>14.List of EBS volumes</li>
-<li>15.List of flow logs </li>
-<li>16.List of Network ACLs</li>
-<li>17.List of Route tables</li>
-<li>18.List of Security Groups</li>
-<li>19.List of Security Group Rules</li>
-<li>20.List of all the snapshots (self taken)</li>
-<li>21.List of Subnets</li>
-<li>22.List of Transit Gateways (TGW)</li>
-<li>23.List of VPC endpoints</li>
-<li>24.List of all the VPC Peering connections</li>
-<li>25.List of VPN connections</li>
+<li>13.Describes the specified Elastic IP addresses </li>
+<li>14.List of VPCs</li>
+<li>15.List of EBS volumes</li>
+<li>16.List of flow logs </li>
+<li>17.List of Network ACLs</li>
+<li>18.List of Route tables</li>
+<li>19.List of Security Groups</li>
+<li>20.List of Security Group Rules</li>
+<li>21.List of all the snapshots (self taken)</li>
+<li>22.List of Subnets</li>
+<li>23.List of Transit Gateways (TGW)</li>
+<li>24.List of VPC endpoints</li>
+<li>25.List of all the VPC Peering connections</li>
+<li>26.List of VPN connections</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> ecs</td>
 <td>
 <ul>
-<li>26.List of ECS clusters</li>
-<li>27.List of  ECS Services in specified ECS Cluster</li>
-<li>28.List ECS Tasks in specified ECS Cluster</li>
+<li>27.List of ECS clusters</li>
+<li>28.List of  ECS Services in specified ECS Cluster</li>
+<li>29.List ECS Tasks in specified ECS Cluster</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> efs</td>
 <td>
 <ul>
-<li>29.List of EFS</li>
+<li>30.List of EFS</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> eks</td>
 <td>
 <ul>
-<li>30.Describe details of specified EKS Cluster</li>
-<li>31.List of EKS Clusters</li>
-<li>32.List EKS Fargate profiles in specified EKS Cluster</li>
+<li>31.Describe details of specified EKS Cluster</li>
+<li>32.List of EKS Clusters</li>
+<li>33.List EKS Fargate profiles in specified EKS Cluster</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> elbv2</td>
 <td>
 <ul>
-<li>33.List of load balancers (Application, Network) </li>
+<li>34.List of load balancers (Application, Network) </li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> emr</td>
 <td>
 <ul>
-<li>34.List of Provisioned EMR Clusters</li>
-<li>35.List of notebook executions.</li>
-<li>36.List of all the EMR Studios </li>
-<li>37.List of Instance fleets for specific EMR cluster</li>
+<li>35.List of Provisioned EMR Clusters</li>
+<li>36.List of notebook executions.</li>
+<li>37.List of all the EMR Studios </li>
+<li>38.List of Instance fleets for specific EMR cluster</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> emr-serverless</td>
 <td>
 <ul>
-<li>38.List of EMR Serverless applications</li>
-<li>39.List of EMR Serverless Job runs for specified EMR serverless application</li>
+<li>39.List of EMR Serverless applications</li>
+<li>40.List of EMR Serverless Job runs for specified EMR serverless application</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> iam</td>
 <td>
 <ul>
-<li>40.List of IAM Roles</li>
-<li>41. List of Managed policies (AWS and Your owned)</li>
-<li>42. List of IAM users</li>
+<li>41.List of IAM Roles</li>
+<li>42. List of Managed policies (AWS and Your owned)</li>
+<li>43. List of IAM users</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> kms</td>
 <td>
 <ul>
-<li>43.List of KMS keys</li>
+<li>44.List of KMS keys</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> lambda</td>
 <td>
 <ul>
-<li>44.List of Lambda functions</li>
-<li>45.List of  Lambda layers </li>
+<li>45.List of Lambda functions</li>
+<li>46.List of  Lambda layers </li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> organizations</td>
 <td>
 <ul>
-<li>46. List of accounts in the organization </li>
-<li>47. List of Service Control Policies (SCP) in an organization </li>
+<li>47. List of accounts in the organization </li>
+<li>48. List of Service Control Policies (SCP) in an organization </li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> rds</td>
 <td>
 <ul>
-<li>48.List of Aurora DB clusters</li>
-<li>49.List of provisioned RDS instances </li>
-<li>50.List  of DB Security Groups</li>
-<li>51.List of Database Sanpshots</li>
-<li>52.List of Global aurora clusters</li>
+<li>49.List of Aurora DB clusters</li>
+<li>50.List of provisioned RDS instances </li>
+<li>51.List  of DB Security Groups</li>
+<li>52.List of Database Sanpshots</li>
+<li>53.List of Global aurora clusters</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> redshift</td>
 <td>
 <ul>
-<li>53.List of Redshift clusters</li>
+<li>54.List of Redshift clusters</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> redshift-serverless</td>
 <td>
 <ul>
-<li>54.List of Redshift serverless namespaces</li>
-<li>55.List of Redshift serverless workgroups</li>
+<li>55.List of Redshift serverless namespaces</li>
+<li>56.List of Redshift serverless workgroups</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> route53</td>
 <td>
 <ul>
-<li>56.List of all the Route53 CIDRs </li>
-<li>57.List of hosted zones(public and private)</li>
-<li>58.List of  private hosted zones associated with specified VPC</li>
+<li>57.List of all the Route53 CIDRs </li>
+<li>58.List of hosted zones(public and private)</li>
+<li>59.List of  private hosted zones associated with specified VPC</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> route53domains</td>
 <td>
 <ul>
-<li>59.List of Route53 Domains</li>
-<li>60.Info of Route53 Domain pricing</li>
+<li>60.List of Route53 Domains</li>
+<li>61.Info of Route53 Domain pricing</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> s3</td>
 <td>
 <ul>
-<li>61.List of S3 buckets</li>
-<li>62.List of the objects in a S3 Bucket</li>
+<li>62.List of S3 buckets</li>
+<li>63.List of the objects in a S3 Bucket</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> sagemaker</td>
 <td>
 <ul>
-<li>63.List of SageMaker Domains</li>
-<li>64.List of SageMaker Images</li>
-<li>65.List of SageMaker Models</li>
-<li>66.List of SageMaker Projects</li>
-<li>67.List of SageMaker User Profiles</li>
+<li>64.List of SageMaker Domains</li>
+<li>65.List of SageMaker Images</li>
+<li>66.List of SageMaker Models</li>
+<li>67.List of SageMaker Projects</li>
+<li>68.List of SageMaker User Profiles</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> sns</td>
 <td>
 <ul>
-<li>68.List of SNS subscriptions</li>
-<li>69.List of SNS topics</li>
+<li>69.List of SNS subscriptions</li>
+<li>70.List of SNS topics</li>
 </ul>
 </td>
 </tr>
 <tr>
 <td> sqs</td>
 <td>
 <ul>
-<li>70.List of SQS queues</li>
+<li>71.List of SQS queues</li>
+</ul>
+</td>
+</tr>
+<tr>
+<td> ssm</td>
+<td>
+<ul>
+<li>72.Describe Instance Information (OS version)</li>
 </ul>
 </td>
 </tr>
 </tbody>
-<table>
+</table>
+</details> 
+
 
-## Pricing
-Cloud9 Pricing: If you are using Cloud9 based setup.
 
 
 ## License
 This library is licensed under the Apache-2.0. See the LICENSE file.
 
 ## Considerations
-Resource-Lister creates boto3 sessions (master and child accounts) and invokes list APIs for the service you selected to list resources. These API calls will be applied to your account API Quotas. 
-If you configured Resource-lister for multiple accoutns.You can use existing master and child account roles or create new roles.
-If you decided to create new roles, You need to run cloudformation template in child account , cloudformation template will create IAM role in child account with read only permissions,this role will be assumed by master account.   
-Utility currrenlty supports only 70 functions. If you are interested in addtional functions /features, Please raise issue.
+* Resource-Lister makes list API calls using AWS SDK for Python(Boto3).These   list API calls will be applied to your [AWS Account List API Quotas](https://docs.aws.amazon.com/general/latest/gr/aws_service_limits.html). 
+
+* Utiliy provide options to use existing IAM roles or to create new roles using utility provided cloudformation templates. If you decided to use utility provided cloudformation templates.  Master account cloudformation template will create **ReadonlyAccess** IAM role in master account .Child account cloudformation template will create **ReadOnlyAccess** IAM role in child account.   
+
+
+* Most of the cases list generated by utility will have 99% of the attributes send back by Boto3 .Utility doesn't assure 100% attributes are covered. 
+
+* When running utility more than 5 accounts,to avoid **memory issues**,It's recommended to generate Account wise file. Account wise file can be generated by changing configuration settting in help section . 
+Help --> 6. [Manage Configurations (example : format_type, output_type)]-->5.[Modify  Seperate file for each AWS Account]-->change to **yes**
+
+* Utility currently supports only 27 services and 70 functions. Utility is configuration driven so adding new function is easy. If you are interested in additional functions /features, please raise issue.
+
+# Know issues/Pending items
+* Improvements in error handling messages
+* Help section is work in progress
 
-# Know issues
-Improvements in error handling messages
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `resource-lister-1.1.0/cfn/cfn_s3_bucket_master_account.json` & `resource-lister-1.2.0/cfn/cfn_s3_bucket_master_account.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/cfn/master_account_IAM_role.json` & `resource-lister-1.2.0/cfn/master_account_IAM_role.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/pyproject.toml` & `resource-lister-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resource-lister"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Abhijit Rajeshirke", email="rajeabh@amazon.com" },
 ]
 description = "Resource Lister"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/core_formatter.py` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/core_formatter.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/json_util/json_util.py` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/json_util/json_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_config.py` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_config.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/apigateway.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/apigateway.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/budgets.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/budgets.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudformation.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudformation.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudfront.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudfront.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudtrail.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudwatch.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/cloudwatch.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/codecommit.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/codecommit.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/dynamodb.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/dynamodb.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ec2.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ec2.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ecs.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/ecs.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/efs.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/efs.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/eks.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/eks.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elasticache.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elasticache.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elbv2.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/elbv2.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr-serverless.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr-serverless.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/emr.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/iam.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/iam.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/kms.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/kms.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/lambda.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/lambda.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/organizations.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/organizations.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/rds.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/rds.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/boto_formatter/service_formatter.py` & `resource-lister-1.2.0/src/resource_lister/boto_formatter/service_formatter.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/config_mgr/config_menu_processor.py` & `resource-lister-1.2.0/src/resource_lister/config_mgr/config_menu_processor.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/config_mgr/config_util.py` & `resource-lister-1.2.0/src/resource_lister/config_mgr/config_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/menu/batch_processing.py` & `resource-lister-1.2.0/src/resource_lister/menu/batch_processing.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/menu/menu_config.json` & `resource-lister-1.2.0/src/resource_lister/menu/menu_config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'menus'": "{insert: [(10, OrderedDict([('menu_index', 'describe_addresses'), ('menu_help', "*

 * *            "'Describes the specified Elastic IP addresses '), ('is_multi_account_support', "*

 * *            "'yes'), ('is_regional', 'yes'), ('service_name', 'ec2'), ('function_name', "*

 * *            "'describe_addresses'), ('implclass', '_regional_no_paginate'), ('implfunction', "*

 * *            "'process'), ('validation_functions', '')])), (71, OrderedDict([('menu_index', 'ssm'), "*

 * *            "('menu_help', 'Describe  […]*

```diff
@@ -123,14 +123,25 @@
             "is_regional": "yes",
             "menu_help": "List of EC2 instances ",
             "menu_index": "describe_instances",
             "service_name": "ec2",
             "validation_functions": ""
         },
         {
+            "function_name": "describe_addresses",
+            "implclass": "_regional_no_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "yes",
+            "is_regional": "yes",
+            "menu_help": "Describes the specified Elastic IP addresses ",
+            "menu_index": "describe_addresses",
+            "service_name": "ec2",
+            "validation_functions": ""
+        },
+        {
             "function_name": "describe_vpcs",
             "implclass": "_regional_paginate",
             "implfunction": "process",
             "is_multi_account_support": "yes",
             "is_regional": "yes",
             "menu_help": "List of VPCs",
             "menu_index": "describe_vpcs",
@@ -877,10 +888,21 @@
             "implfunction": "process",
             "is_multi_account_support": "yes",
             "is_regional": "yes",
             "menu_help": "List of SageMaker User Profiles",
             "menu_index": "sagemaker",
             "service_name": "sagemaker",
             "validation_functions": ""
+        },
+        {
+            "function_name": "describe_instance_information",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "yes",
+            "is_regional": "yes",
+            "menu_help": "Describe Instance Information (OS version)",
+            "menu_index": "ssm",
+            "service_name": "ssm",
+            "validation_functions": ""
         }
     ]
 }
```

### Comparing `resource-lister-1.1.0/src/resource_lister/menu/menu_processor.py` & `resource-lister-1.2.0/src/resource_lister/menu/menu_processor.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/menu/menu_util.py` & `resource-lister-1.2.0/src/resource_lister/menu/menu_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/processor/_global_no_paginate.py` & `resource-lister-1.2.0/src/resource_lister/processor/_global_no_paginate.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/processor/_global_paginate.py` & `resource-lister-1.2.0/src/resource_lister/processor/_global_paginate.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/processor/_regional_no_paginate.py` & `resource-lister-1.2.0/src/resource_lister/processor/_regional_no_paginate.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/processor/_regional_paginate.py` & `resource-lister-1.2.0/src/resource_lister/processor/_regional_paginate.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/session_mgr/account_config_util.py` & `resource-lister-1.2.0/src/resource_lister/session_mgr/account_config_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/session_mgr/accounts_menu_processor.py` & `resource-lister-1.2.0/src/resource_lister/session_mgr/accounts_menu_processor.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/session_mgr/iam_session_mgr.py` & `resource-lister-1.2.0/src/resource_lister/session_mgr/iam_session_mgr.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/util/menu_configs.py` & `resource-lister-1.2.0/src/resource_lister/util/menu_configs.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/util/menu_util.py` & `resource-lister-1.2.0/src/resource_lister/util/menu_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/util/s3_util.py` & `resource-lister-1.2.0/src/resource_lister/util/s3_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/util/session_util.py` & `resource-lister-1.2.0/src/resource_lister/util/session_util.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister/util/setup.py` & `resource-lister-1.2.0/src/resource_lister/util/setup.py`

 * *Files identical despite different names*

### Comparing `resource-lister-1.1.0/src/resource_lister.egg-info/SOURCES.txt` & `resource-lister-1.2.0/src/resource_lister.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 src/resource_lister/boto_formatter/service_config_mgr/service_configs/redshift.json
 src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53.json
 src/resource_lister/boto_formatter/service_config_mgr/service_configs/route53domains.json
 src/resource_lister/boto_formatter/service_config_mgr/service_configs/s3.json
 src/resource_lister/boto_formatter/service_config_mgr/service_configs/sagemaker.json
 src/resource_lister/boto_formatter/service_config_mgr/service_configs/sns.json
 src/resource_lister/boto_formatter/service_config_mgr/service_configs/sqs.json
+src/resource_lister/boto_formatter/service_config_mgr/service_configs/ssm.json
 src/resource_lister/config_mgr/__init__.py
 src/resource_lister/config_mgr/config.json
 src/resource_lister/config_mgr/config_menu_processor.py
 src/resource_lister/config_mgr/config_util.py
 src/resource_lister/menu/__init__.py
 src/resource_lister/menu/batch_processing.py
 src/resource_lister/menu/menu_config.json
```

