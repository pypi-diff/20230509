# Comparing `tmp/sparrowcloud-4.0.1.tar.gz` & `tmp/sparrowcloud-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparrowcloud-4.0.1.tar", last modified: Wed Mar 29 06:49:51 2023, max compression
+gzip compressed data, was "dist/sparrowcloud-4.1.0.tar", last modified: Tue May  9 06:27:51 2023, max compression
```

## Comparing `sparrowcloud-4.0.1.tar` & `sparrowcloud-4.1.0.tar`

### file list

```diff
@@ -1,206 +1,209 @@
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.828512 sparrowcloud-4.0.1/
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1068 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/LICENSE
--rw-r--r--   0 tigerlittle   (501) staff       (20)    20103 2023-03-29 06:49:51.828317 sparrowcloud-4.0.1/PKG-INFO
--rw-r--r--   0 tigerlittle   (501) staff       (20)    19594 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/README.md
--rw-r--r--   0 tigerlittle   (501) staff       (20)       38 2023-03-29 06:49:51.828561 sparrowcloud-4.0.1/setup.cfg
--rwxr-xr-x   0 tigerlittle   (501) staff       (20)     2402 2023-03-29 06:45:24.000000 sparrowcloud-4.0.1/setup.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.798884 sparrowcloud-4.0.1/sparrow_cloud/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.800021 sparrowcloud-4.0.1/sparrow_cloud/access_control/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/access_control/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1119 2020-10-27 08:32:03.000000 sparrowcloud-4.0.1/sparrow_cloud/access_control/access_verify.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      199 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/access_control/base_access_control.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     4570 2021-06-23 07:33:41.000000 sparrowcloud-4.0.1/sparrow_cloud/access_control/decorators.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.800398 sparrowcloud-4.0.1/sparrow_cloud/app_message/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-11-18 06:15:22.000000 sparrowcloud-4.0.1/sparrow_cloud/app_message/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1837 2021-02-07 06:05:50.000000 sparrowcloud-4.0.1/sparrow_cloud/app_message/sender.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.800568 sparrowcloud-4.0.1/sparrow_cloud/apps/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.802034 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      102 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/apps.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      896 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/example_access_control.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.802194 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/management/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/management/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.802427 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/management/commands/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/management/commands/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1679 2020-10-27 10:00:56.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/management/commands/register_access_control.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.802585 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.803503 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/admin.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.804273 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/
--rw-r--r--   0 tigerlittle   (501) staff       (20)      940 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider2.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1341 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider3.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      845 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/connection.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    14094 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/receiver.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      117 2023-03-07 08:29:29.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/apps.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.804448 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.805080 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/commands/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/commands/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    14060 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/commands/_controller.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2943 2020-11-10 08:04:05.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/commands/_sparrow_rabbitmq_consumer.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      643 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/commands/rabbitmq_consumer.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.805261 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/urls.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.806705 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      129 2023-03-07 09:09:03.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/apps.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    21443 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/generators_django_1.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    17804 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/generators_django_2.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.806858 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/management/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/management/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.807262 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/management/commands/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/management/commands/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1614 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/management/commands/_api.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     8069 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/management/commands/register_api_permission.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.807418 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      474 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      855 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      694 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/urls.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      456 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.808410 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      102 2023-03-07 08:30:32.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/apps.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.808566 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      165 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/urls.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      277 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/ping/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.811726 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      121 2023-03-07 08:30:15.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/apps.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      954 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/contributor.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.811939 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/management/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/management/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.812210 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/management/commands/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/management/commands/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1659 2020-10-28 07:54:35.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/management/commands/register_api_schema.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.812377 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/models.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.813850 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/
--rw-r--r--   0 tigerlittle   (501) staff       (20)      272 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1353 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/compat.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    14532 2023-03-29 03:35:53.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/generators.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      148 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/incompatible_settings.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    17462 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/inspectors.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     7418 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/patch.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1035 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/utils.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.815435 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      143 2023-03-07 09:21:53.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/apps.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.815619 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      268 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      190 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/serializers.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      130 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/urls.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1180 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.816067 sparrowcloud-4.0.1/sparrow_cloud/auth/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/auth/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      467 2021-06-18 03:25:54.000000 sparrowcloud-4.0.1/sparrow_cloud/auth/user.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2149 2021-07-29 06:08:19.000000 sparrowcloud-4.0.1/sparrow_cloud/auth/user_id_authentication.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.816358 sparrowcloud-4.0.1/sparrow_cloud/authorization/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/authorization/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      541 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/sparrow_cloud/authorization/token.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.816657 sparrowcloud-4.0.1/sparrow_cloud/cache/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/cache/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1425 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/cache/cache_manager.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.816933 sparrowcloud-4.0.1/sparrow_cloud/dingtalk/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/dingtalk/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1263 2020-10-28 07:54:06.000000 sparrowcloud-4.0.1/sparrow_cloud/dingtalk/sender.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.817195 sparrowcloud-4.0.1/sparrow_cloud/distributed_lock/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2021-02-07 06:05:50.000000 sparrowcloud-4.0.1/sparrow_cloud/distributed_lock/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2440 2021-02-07 06:05:50.000000 sparrowcloud-4.0.1/sparrow_cloud/distributed_lock/lock_op.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.817626 sparrowcloud-4.0.1/sparrow_cloud/message_service/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/message_service/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     4200 2020-10-28 07:54:22.000000 sparrowcloud-4.0.1/sparrow_cloud/message_service/sender.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2320 2020-10-27 06:12:38.000000 sparrowcloud-4.0.1/sparrow_cloud/message_service/sender_controller.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.818726 sparrowcloud-4.0.1/sparrow_cloud/middleware/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1730 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/acl_middleware.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.819000 sparrowcloud-4.0.1/sparrow_cloud/middleware/base/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/base/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      528 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/base/base_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      841 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/exception.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1530 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/jwt_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2432 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/lock_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      651 2020-10-30 09:30:11.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/methodconvert.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3433 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/middleware/tracing_middleware.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.819451 sparrowcloud-4.0.1/sparrow_cloud/registry/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/registry/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2333 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/registry/service_configuration.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3405 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/registry/service_discovery.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.820120 sparrowcloud-4.0.1/sparrow_cloud/restclient/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/restclient/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      593 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/restclient/exception.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3112 2021-07-29 06:08:19.000000 sparrowcloud-4.0.1/sparrow_cloud/restclient/requests_client.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     4190 2021-07-29 06:08:19.000000 sparrowcloud-4.0.1/sparrow_cloud/restclient/rest_client.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.820515 sparrowcloud-4.0.1/sparrow_cloud/service_log/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/service_log/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1010 2020-10-30 06:33:49.000000 sparrowcloud-4.0.1/sparrow_cloud/service_log/sender.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.822624 sparrowcloud-4.0.1/sparrow_cloud/utils/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      394 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/build_url.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      283 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/common_exceptions.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      685 2021-06-18 03:25:54.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/decode_jwt.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      341 2021-01-08 06:07:37.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/get_cm_value.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      692 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/get_hash_key.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      700 2020-10-27 08:08:15.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/get_settings_value.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      917 2020-10-27 09:57:27.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/get_user.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      374 2020-10-27 09:57:47.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/normalize_url.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      837 2020-10-27 10:01:08.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/resource_cls_attribute.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2063 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/send_alert.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1240 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/sparrow_cloud/utils/validation_acl.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.823500 sparrowcloud-4.0.1/sparrowcloud.egg-info/
--rw-r--r--   0 tigerlittle   (501) staff       (20)    20103 2023-03-29 06:49:51.000000 sparrowcloud-4.0.1/sparrowcloud.egg-info/PKG-INFO
--rw-r--r--   0 tigerlittle   (501) staff       (20)     7036 2023-03-29 06:49:51.000000 sparrowcloud-4.0.1/sparrowcloud.egg-info/SOURCES.txt
--rw-r--r--   0 tigerlittle   (501) staff       (20)        1 2023-03-29 06:49:51.000000 sparrowcloud-4.0.1/sparrowcloud.egg-info/dependency_links.txt
--rw-r--r--   0 tigerlittle   (501) staff       (20)        1 2023-03-29 06:49:51.000000 sparrowcloud-4.0.1/sparrowcloud.egg-info/not-zip-safe
--rw-r--r--   0 tigerlittle   (501) staff       (20)      155 2023-03-29 06:49:51.000000 sparrowcloud-4.0.1/sparrowcloud.egg-info/requires.txt
--rw-r--r--   0 tigerlittle   (501) staff       (20)       14 2023-03-29 06:49:51.000000 sparrowcloud-4.0.1/sparrowcloud.egg-info/top_level.txt
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-03-29 06:49:51.828027 sparrowcloud-4.0.1/tests/
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2820 2021-07-29 06:08:19.000000 sparrowcloud-4.0.1/tests/test_access_control.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2481 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/tests/test_acl_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     7264 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/tests/test_api_permission.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2332 2020-11-19 03:21:34.000000 sparrowcloud-4.0.1/tests/test_app_message.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3021 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/tests/test_consul_service.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1960 2020-10-28 04:56:56.000000 sparrowcloud-4.0.1/tests/test_ding_talk.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2663 2021-02-07 06:05:50.000000 sparrowcloud-4.0.1/tests/test_distributed_lock.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1663 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/tests/test_exception_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     4670 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/tests/test_get_token_sdk.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      820 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/tests/test_hash_key.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     5470 2023-03-07 09:49:19.000000 sparrowcloud-4.0.1/tests/test_jwtmiddleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3230 2021-06-03 09:44:22.000000 sparrowcloud-4.0.1/tests/test_lock_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1773 2020-10-28 05:14:21.000000 sparrowcloud-4.0.1/tests/test_message_client.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     8219 2022-05-30 04:53:46.000000 sparrowcloud-4.0.1/tests/test_rabbitmq_consumer_command.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2178 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/tests/test_register_access_control.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2221 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/tests/test_register_command.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2013 2020-10-28 06:20:10.000000 sparrowcloud-4.0.1/tests/test_register_schema_command.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3419 2020-10-28 05:11:47.000000 sparrowcloud-4.0.1/tests/test_requests_client.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     5741 2020-10-28 05:12:06.000000 sparrowcloud-4.0.1/tests/test_rest_client.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2182 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/tests/test_service_configuration.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2710 2020-10-30 06:34:59.000000 sparrowcloud-4.0.1/tests/test_service_log.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1450 2020-09-29 03:48:09.000000 sparrowcloud-4.0.1/tests/test_table_api.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1702 2020-10-26 04:41:02.000000 sparrowcloud-4.0.1/tests/test_tracing_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2989 2021-07-29 06:08:19.000000 sparrowcloud-4.0.1/tests/test_user_id_authentication.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.699163 sparrowcloud-4.1.0/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1068 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/LICENSE
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    22393 2023-05-09 06:27:51.698924 sparrowcloud-4.1.0/PKG-INFO
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    21884 2023-05-09 06:23:48.000000 sparrowcloud-4.1.0/README.md
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       38 2023-05-09 06:27:51.699225 sparrowcloud-4.1.0/setup.cfg
+-rwxr-xr-x   0 tigerlittle   (501) staff       (20)     2402 2023-05-08 07:02:04.000000 sparrowcloud-4.1.0/setup.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.661169 sparrowcloud-4.1.0/sparrow_cloud/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.662392 sparrowcloud-4.1.0/sparrow_cloud/access_control/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/access_control/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1119 2020-10-27 08:32:03.000000 sparrowcloud-4.1.0/sparrow_cloud/access_control/access_verify.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      199 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/access_control/base_access_control.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     4570 2021-06-23 07:33:41.000000 sparrowcloud-4.1.0/sparrow_cloud/access_control/decorators.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.662856 sparrowcloud-4.1.0/sparrow_cloud/app_message/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-11-18 06:15:22.000000 sparrowcloud-4.1.0/sparrow_cloud/app_message/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1837 2021-02-07 06:05:50.000000 sparrowcloud-4.1.0/sparrow_cloud/app_message/sender.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.663090 sparrowcloud-4.1.0/sparrow_cloud/apps/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.665010 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      102 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/apps.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      896 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/example_access_control.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.665312 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/management/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/management/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.665685 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/management/commands/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/management/commands/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1679 2020-10-27 10:00:56.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/management/commands/register_access_control.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.665927 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.667108 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/admin.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.668479 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      940 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider2.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1341 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider3.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      845 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/connection.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    14094 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/receiver.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      117 2023-03-07 08:29:29.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/apps.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.668880 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.669932 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/commands/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/commands/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    14060 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/commands/_controller.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2943 2020-11-10 08:04:05.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/commands/_sparrow_rabbitmq_consumer.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      643 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/commands/rabbitmq_consumer.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.670234 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/urls.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.672430 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      129 2023-03-07 09:09:03.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/apps.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    21443 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/generators_django_1.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    17804 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/generators_django_2.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.672679 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/management/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/management/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.673233 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/management/commands/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/management/commands/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1614 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/management/commands/_api.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     8069 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/management/commands/register_api_permission.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.673438 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      474 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      855 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      694 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/urls.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      456 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.674800 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      102 2023-03-07 08:30:32.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/apps.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.674977 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      165 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/urls.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      277 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/ping/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.676412 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      121 2023-03-07 08:30:15.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/apps.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      954 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/contributor.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.676702 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/management/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/management/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.676960 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/management/commands/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/management/commands/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1659 2020-10-28 07:54:35.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/management/commands/register_api_schema.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.677159 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/models.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.678809 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      272 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1353 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/compat.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    14532 2023-03-29 03:35:53.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/generators.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      148 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/incompatible_settings.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    17462 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/inspectors.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     7418 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/patch.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1035 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/utils.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.680846 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      143 2023-03-07 09:21:53.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/apps.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.681023 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      268 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      190 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/serializers.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      130 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/urls.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1180 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.681525 sparrowcloud-4.1.0/sparrow_cloud/auth/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/auth/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      467 2021-06-18 03:25:54.000000 sparrowcloud-4.1.0/sparrow_cloud/auth/user.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2149 2021-07-29 06:08:19.000000 sparrowcloud-4.1.0/sparrow_cloud/auth/user_id_authentication.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.681988 sparrowcloud-4.1.0/sparrow_cloud/authorization/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/authorization/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      541 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/sparrow_cloud/authorization/token.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.682308 sparrowcloud-4.1.0/sparrow_cloud/cache/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/cache/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1425 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/cache/cache_manager.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.682946 sparrowcloud-4.1.0/sparrow_cloud/dingtalk/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/dingtalk/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1263 2020-10-28 07:54:06.000000 sparrowcloud-4.1.0/sparrow_cloud/dingtalk/sender.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.683268 sparrowcloud-4.1.0/sparrow_cloud/distributed_lock/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2021-02-07 06:05:50.000000 sparrowcloud-4.1.0/sparrow_cloud/distributed_lock/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2440 2021-02-07 06:05:50.000000 sparrowcloud-4.1.0/sparrow_cloud/distributed_lock/lock_op.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.683967 sparrowcloud-4.1.0/sparrow_cloud/message_service/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/message_service/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     4200 2020-10-28 07:54:22.000000 sparrowcloud-4.1.0/sparrow_cloud/message_service/sender.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2320 2020-10-27 06:12:38.000000 sparrowcloud-4.1.0/sparrow_cloud/message_service/sender_controller.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.685975 sparrowcloud-4.1.0/sparrow_cloud/middleware/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2023-05-08 07:06:50.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1730 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/acl_middleware.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.686279 sparrowcloud-4.1.0/sparrow_cloud/middleware/base/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/base/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      528 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/base/base_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      841 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/exception.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1530 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/jwt_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2432 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/lock_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1031 2023-05-09 02:50:33.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/log_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      651 2020-10-30 09:30:11.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/methodconvert.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3433 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/middleware/tracing_middleware.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.686919 sparrowcloud-4.1.0/sparrow_cloud/registry/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/registry/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2333 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/registry/service_configuration.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3405 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/registry/service_discovery.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.687765 sparrowcloud-4.1.0/sparrow_cloud/restclient/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/restclient/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      593 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/restclient/exception.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3112 2021-07-29 06:08:19.000000 sparrowcloud-4.1.0/sparrow_cloud/restclient/requests_client.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     4190 2021-07-29 06:08:19.000000 sparrowcloud-4.1.0/sparrow_cloud/restclient/rest_client.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.688089 sparrowcloud-4.1.0/sparrow_cloud/service_log/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/service_log/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1010 2020-10-30 06:33:49.000000 sparrowcloud-4.1.0/sparrow_cloud/service_log/sender.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.690997 sparrowcloud-4.1.0/sparrow_cloud/utils/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      181 2023-05-08 07:07:01.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      394 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/build_url.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      283 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/common_exceptions.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      685 2021-06-18 03:25:54.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/decode_jwt.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      341 2021-01-08 06:07:37.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/get_cm_value.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      692 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/get_hash_key.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      700 2020-10-27 08:08:15.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/get_settings_value.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      917 2020-10-27 09:57:27.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/get_user.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      374 2020-10-27 09:57:47.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/normalize_url.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      837 2020-10-27 10:01:08.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/resource_cls_attribute.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2063 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/send_alert.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1240 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/sparrow_cloud/utils/validation_acl.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.692090 sparrowcloud-4.1.0/sparrowcloud.egg-info/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    22393 2023-05-09 06:27:51.000000 sparrowcloud-4.1.0/sparrowcloud.egg-info/PKG-INFO
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     7139 2023-05-09 06:27:51.000000 sparrowcloud-4.1.0/sparrowcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        1 2023-05-09 06:27:51.000000 sparrowcloud-4.1.0/sparrowcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        1 2023-05-09 06:27:51.000000 sparrowcloud-4.1.0/sparrowcloud.egg-info/not-zip-safe
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      155 2023-05-09 06:27:51.000000 sparrowcloud-4.1.0/sparrowcloud.egg-info/requires.txt
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       14 2023-05-09 06:27:51.000000 sparrowcloud-4.1.0/sparrowcloud.egg-info/top_level.txt
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:27:51.698574 sparrowcloud-4.1.0/tests/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2820 2021-07-29 06:08:19.000000 sparrowcloud-4.1.0/tests/test_access_control.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2481 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/tests/test_acl_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     7264 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/tests/test_api_permission.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2332 2023-03-31 03:34:52.000000 sparrowcloud-4.1.0/tests/test_app_message.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3021 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/tests/test_consul_service.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1960 2023-03-31 03:34:52.000000 sparrowcloud-4.1.0/tests/test_ding_talk.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2663 2021-02-07 06:05:50.000000 sparrowcloud-4.1.0/tests/test_distributed_lock.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1663 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/tests/test_exception_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     4670 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/tests/test_get_token_sdk.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      820 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/tests/test_hash_key.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     5470 2023-03-07 09:49:19.000000 sparrowcloud-4.1.0/tests/test_jwtmiddleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3230 2021-06-03 09:44:22.000000 sparrowcloud-4.1.0/tests/test_lock_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      750 2023-05-08 07:07:30.000000 sparrowcloud-4.1.0/tests/test_log_filter.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1773 2020-10-28 05:14:21.000000 sparrowcloud-4.1.0/tests/test_message_client.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     8219 2022-05-30 04:53:46.000000 sparrowcloud-4.1.0/tests/test_rabbitmq_consumer_command.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2178 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/tests/test_register_access_control.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2221 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/tests/test_register_command.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2013 2020-10-28 06:20:10.000000 sparrowcloud-4.1.0/tests/test_register_schema_command.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1344 2023-05-08 07:07:37.000000 sparrowcloud-4.1.0/tests/test_requestid_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3419 2020-10-28 05:11:47.000000 sparrowcloud-4.1.0/tests/test_requests_client.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     5741 2020-10-28 05:12:06.000000 sparrowcloud-4.1.0/tests/test_rest_client.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2182 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/tests/test_service_configuration.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2710 2020-10-30 06:34:59.000000 sparrowcloud-4.1.0/tests/test_service_log.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1450 2020-09-29 03:48:09.000000 sparrowcloud-4.1.0/tests/test_table_api.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1702 2020-10-26 04:41:02.000000 sparrowcloud-4.1.0/tests/test_tracing_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2989 2021-07-29 06:08:19.000000 sparrowcloud-4.1.0/tests/test_user_id_authentication.py
```

### Comparing `sparrowcloud-4.0.1/LICENSE` & `sparrowcloud-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/PKG-INFO` & `sparrowcloud-4.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrowcloud
-Version: 4.0.1
+Version: 4.1.0
 Summary: 基础Django和drf的微服务框架扩展
 Home-page: https://gitee.com/sparrow614/sparrow_cloud
 Author: sparrow
 Author-email: 
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -70,26 +70,29 @@
 [get_user_token](#get_user_token)
 
 [get_app_token](#get_app_token)
 
 [app_message](#app_message)
 
 [distributed_lock](#distributed_lock)
-
+## LogFilter
+[log_filter](#log_filter)
 ## django中间件 ##
 [JWTMiddleware](#jwtmiddleware)
 
 [MethodConvertMiddleware](#method_middleware)
 
 [ExceptionMiddleware](#exceptionmiddleware)
 
 [TracingMiddleware](#tracingmiddleware)
 
 [CheckLockMiddleware](#CheckLockMiddleware)
 
+[LogMiddleware](#LogMiddleware)
+
 ## rest_framework中间件 ##
 [UserID Authentication](#useridauthentication)
 
 
 ## installation ##
 
     pip install sparrowcloud
@@ -517,14 +520,80 @@
     # settings 配置
     MIDDLEWARE = [                 
         "sparrow_cloud.middleware.exception.ExceptionMiddleware"  
     ]
 
 ```
 
+## LogMiddleware
+> 日志中间件（将istio-proxy层的request_id放入线程中，并透传到业务逻辑层，可通过 request.id 获取，与链路追踪中的request_id 一致）
+> 此中间件需要配合log_filter 使用，才能在每条业务逻辑日志中插入request_id, 如单独使用只能透request_id
+``` python
+    # settings 配置
+    MIDDLEWARE = [                 
+        "sparrow_cloud.middleware.log_middleware.RequestIDMiddleware"
+    ]
+
+```
+## log_filter
+> log_filter(自定义logfilter,从线程中获取request_id，从每条日志中打印出来)
+> 需要与LogMiddleware 中间件配合使用，否则不生效
+
+``` python 
+# log_settings 配置
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': False,
+    'filters': {
+        # 新增的配置
+        'request_id': {
+            '()': 'middleware.filters.RequestIDFilter'
+        }
+    },
+    'handlers': {
+        'console': {
+            'level': 'DEBUG',
+            'class': 'logging.StreamHandler',
+            'formatter': 'standard',   # 需要修改的的配置
+            'filters': ['request_id'], # 增加的 log_filter 的配置
+        },
+        # 以访问控制服务的日志举例子
+        'access_control': {
+            'class': 'logging.handlers.RotatingFileHandler',
+            'filters': ['request_id'], # 增加的配置
+            'level': 'DEBUG',
+            'formatter': 'standard', # 修改为新增的formatters 配置
+            'filename': os.path.join(os.path.sep, BASE_DIR_LOG, 'access_control.log'),
+            'mode': 'a',
+            'maxBytes': 1024 * 1024 * 5,
+            'backupCount': 1, # 修改
+        },
+    },
+    'formatters': {
+        # 增加的配置
+        'standard': {
+                    'format': '%(levelname)s %(asctime)s %(request_id)s %(lineno)d %(name)s %(module)s %(funcName)s %(process)d %(thread)d %(message)s'
+                },
+    },
+    # sparrow_cloud 的日志
+    'sparrow_cloud': {
+        'handlers': ['console', 'sparrow_cloud'],
+        'level': 'DEBUG',
+        'propagate': False,
+    },
+    'access_control': {
+        'handlers': ['console', 'access_control'],
+        'level': 'DEBUG',
+        'propagate': False,
+    }
+}
+}
+
+```
+
 ## ACCESS_CONTROL_VERIFY
 > access_control_verify decorators (访问控制验证)
 ``` python
     # settings 配置
     SERVICE_CONF = {
         "NAME": "",  # value为本服务的注册名称
         "SECRET": "",
```

### Comparing `sparrowcloud-4.0.1/README.md` & `sparrowcloud-4.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,26 +53,29 @@
 [get_user_token](#get_user_token)
 
 [get_app_token](#get_app_token)
 
 [app_message](#app_message)
 
 [distributed_lock](#distributed_lock)
-
+## LogFilter
+[log_filter](#log_filter)
 ## django中间件 ##
 [JWTMiddleware](#jwtmiddleware)
 
 [MethodConvertMiddleware](#method_middleware)
 
 [ExceptionMiddleware](#exceptionmiddleware)
 
 [TracingMiddleware](#tracingmiddleware)
 
 [CheckLockMiddleware](#CheckLockMiddleware)
 
+[LogMiddleware](#LogMiddleware)
+
 ## rest_framework中间件 ##
 [UserID Authentication](#useridauthentication)
 
 
 ## installation ##
 
     pip install sparrowcloud
@@ -500,14 +503,80 @@
     # settings 配置
     MIDDLEWARE = [                 
         "sparrow_cloud.middleware.exception.ExceptionMiddleware"  
     ]
 
 ```
 
+## LogMiddleware
+> 日志中间件（将istio-proxy层的request_id放入线程中，并透传到业务逻辑层，可通过 request.id 获取，与链路追踪中的request_id 一致）
+> 此中间件需要配合log_filter 使用，才能在每条业务逻辑日志中插入request_id, 如单独使用只能透request_id
+``` python
+    # settings 配置
+    MIDDLEWARE = [                 
+        "sparrow_cloud.middleware.log_middleware.RequestIDMiddleware"
+    ]
+
+```
+## log_filter
+> log_filter(自定义logfilter,从线程中获取request_id，从每条日志中打印出来)
+> 需要与LogMiddleware 中间件配合使用，否则不生效
+
+``` python 
+# log_settings 配置
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': False,
+    'filters': {
+        # 新增的配置
+        'request_id': {
+            '()': 'middleware.filters.RequestIDFilter'
+        }
+    },
+    'handlers': {
+        'console': {
+            'level': 'DEBUG',
+            'class': 'logging.StreamHandler',
+            'formatter': 'standard',   # 需要修改的的配置
+            'filters': ['request_id'], # 增加的 log_filter 的配置
+        },
+        # 以访问控制服务的日志举例子
+        'access_control': {
+            'class': 'logging.handlers.RotatingFileHandler',
+            'filters': ['request_id'], # 增加的配置
+            'level': 'DEBUG',
+            'formatter': 'standard', # 修改为新增的formatters 配置
+            'filename': os.path.join(os.path.sep, BASE_DIR_LOG, 'access_control.log'),
+            'mode': 'a',
+            'maxBytes': 1024 * 1024 * 5,
+            'backupCount': 1, # 修改
+        },
+    },
+    'formatters': {
+        # 增加的配置
+        'standard': {
+                    'format': '%(levelname)s %(asctime)s %(request_id)s %(lineno)d %(name)s %(module)s %(funcName)s %(process)d %(thread)d %(message)s'
+                },
+    },
+    # sparrow_cloud 的日志
+    'sparrow_cloud': {
+        'handlers': ['console', 'sparrow_cloud'],
+        'level': 'DEBUG',
+        'propagate': False,
+    },
+    'access_control': {
+        'handlers': ['console', 'access_control'],
+        'level': 'DEBUG',
+        'propagate': False,
+    }
+}
+}
+
+```
+
 ## ACCESS_CONTROL_VERIFY
 > access_control_verify decorators (访问控制验证)
 ``` python
     # settings 配置
     SERVICE_CONF = {
         "NAME": "",  # value为本服务的注册名称
         "SECRET": "",
```

### Comparing `sparrowcloud-4.0.1/setup.py` & `sparrowcloud-4.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # import io
 import os
 import sys
 import shutil
 from setuptools import find_packages, setup
 
-version = "v4.0.1"
+version = "v4.1.0"
 
 def read(f):
     return open(f, 'r', encoding='utf-8').read()
 
 
 if sys.argv[-1] == 'publish':
     if os.system("pip freeze | grep twine"):
```

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/access_control/access_verify.py` & `sparrowcloud-4.1.0/sparrow_cloud/access_control/access_verify.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/access_control/decorators.py` & `sparrowcloud-4.1.0/sparrow_cloud/access_control/decorators.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/app_message/sender.py` & `sparrowcloud-4.1.0/sparrow_cloud/app_message/sender.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/example_access_control.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/example_access_control.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/access_control/management/commands/register_access_control.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/access_control/management/commands/register_access_control.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider2.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider2.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider3.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider3.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/connection.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/connection.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/aliyun_amqp/receiver.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/aliyun_amqp/receiver.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/commands/_controller.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/commands/_controller.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/commands/_sparrow_rabbitmq_consumer.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/commands/_sparrow_rabbitmq_consumer.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/message_service/management/commands/rabbitmq_consumer.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/message_service/management/commands/rabbitmq_consumer.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/generators_django_1.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/generators_django_1.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/generators_django_2.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/generators_django_2.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/management/commands/_api.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/management/commands/_api.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/management/commands/register_api_permission.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/management/commands/register_api_permission.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/tests.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/tests.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/permission_command/urls.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/permission_command/urls.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/contributor.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/contributor.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/management/commands/register_api_schema.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/management/commands/register_api_schema.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/compat.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/compat.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/generators.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/generators.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/inspectors.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/inspectors.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/patch.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/patch.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/schema_command/schemas/utils.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/schema_command/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/apps/table_api/views.py` & `sparrowcloud-4.1.0/sparrow_cloud/apps/table_api/views.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/auth/user_id_authentication.py` & `sparrowcloud-4.1.0/sparrow_cloud/auth/user_id_authentication.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/authorization/token.py` & `sparrowcloud-4.1.0/sparrow_cloud/authorization/token.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/cache/cache_manager.py` & `sparrowcloud-4.1.0/sparrow_cloud/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/dingtalk/sender.py` & `sparrowcloud-4.1.0/sparrow_cloud/dingtalk/sender.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/distributed_lock/lock_op.py` & `sparrowcloud-4.1.0/sparrow_cloud/distributed_lock/lock_op.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/message_service/sender.py` & `sparrowcloud-4.1.0/sparrow_cloud/message_service/sender.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/message_service/sender_controller.py` & `sparrowcloud-4.1.0/sparrow_cloud/message_service/sender_controller.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/middleware/acl_middleware.py` & `sparrowcloud-4.1.0/sparrow_cloud/middleware/acl_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/middleware/base/base_middleware.py` & `sparrowcloud-4.1.0/sparrow_cloud/middleware/base/base_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/middleware/exception.py` & `sparrowcloud-4.1.0/sparrow_cloud/middleware/exception.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/middleware/jwt_middleware.py` & `sparrowcloud-4.1.0/sparrow_cloud/middleware/jwt_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/middleware/lock_middleware.py` & `sparrowcloud-4.1.0/sparrow_cloud/middleware/lock_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/middleware/methodconvert.py` & `sparrowcloud-4.1.0/sparrow_cloud/middleware/methodconvert.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/middleware/tracing_middleware.py` & `sparrowcloud-4.1.0/sparrow_cloud/middleware/tracing_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/registry/service_configuration.py` & `sparrowcloud-4.1.0/sparrow_cloud/registry/service_configuration.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/registry/service_discovery.py` & `sparrowcloud-4.1.0/sparrow_cloud/registry/service_discovery.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/restclient/exception.py` & `sparrowcloud-4.1.0/sparrow_cloud/restclient/exception.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/restclient/requests_client.py` & `sparrowcloud-4.1.0/sparrow_cloud/restclient/requests_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/restclient/rest_client.py` & `sparrowcloud-4.1.0/sparrow_cloud/restclient/rest_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/service_log/sender.py` & `sparrowcloud-4.1.0/sparrow_cloud/service_log/sender.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/utils/decode_jwt.py` & `sparrowcloud-4.1.0/sparrow_cloud/utils/decode_jwt.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/utils/get_hash_key.py` & `sparrowcloud-4.1.0/sparrow_cloud/utils/get_hash_key.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/utils/get_settings_value.py` & `sparrowcloud-4.1.0/sparrow_cloud/utils/get_settings_value.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/utils/get_user.py` & `sparrowcloud-4.1.0/sparrow_cloud/utils/get_user.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/utils/resource_cls_attribute.py` & `sparrowcloud-4.1.0/sparrow_cloud/utils/resource_cls_attribute.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/utils/send_alert.py` & `sparrowcloud-4.1.0/sparrow_cloud/utils/send_alert.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrow_cloud/utils/validation_acl.py` & `sparrowcloud-4.1.0/sparrow_cloud/utils/validation_acl.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/sparrowcloud.egg-info/PKG-INFO` & `sparrowcloud-4.1.0/sparrowcloud.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrowcloud
-Version: 4.0.1
+Version: 4.1.0
 Summary: 基础Django和drf的微服务框架扩展
 Home-page: https://gitee.com/sparrow614/sparrow_cloud
 Author: sparrow
 Author-email: 
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -70,26 +70,29 @@
 [get_user_token](#get_user_token)
 
 [get_app_token](#get_app_token)
 
 [app_message](#app_message)
 
 [distributed_lock](#distributed_lock)
-
+## LogFilter
+[log_filter](#log_filter)
 ## django中间件 ##
 [JWTMiddleware](#jwtmiddleware)
 
 [MethodConvertMiddleware](#method_middleware)
 
 [ExceptionMiddleware](#exceptionmiddleware)
 
 [TracingMiddleware](#tracingmiddleware)
 
 [CheckLockMiddleware](#CheckLockMiddleware)
 
+[LogMiddleware](#LogMiddleware)
+
 ## rest_framework中间件 ##
 [UserID Authentication](#useridauthentication)
 
 
 ## installation ##
 
     pip install sparrowcloud
@@ -517,14 +520,80 @@
     # settings 配置
     MIDDLEWARE = [                 
         "sparrow_cloud.middleware.exception.ExceptionMiddleware"  
     ]
 
 ```
 
+## LogMiddleware
+> 日志中间件（将istio-proxy层的request_id放入线程中，并透传到业务逻辑层，可通过 request.id 获取，与链路追踪中的request_id 一致）
+> 此中间件需要配合log_filter 使用，才能在每条业务逻辑日志中插入request_id, 如单独使用只能透request_id
+``` python
+    # settings 配置
+    MIDDLEWARE = [                 
+        "sparrow_cloud.middleware.log_middleware.RequestIDMiddleware"
+    ]
+
+```
+## log_filter
+> log_filter(自定义logfilter,从线程中获取request_id，从每条日志中打印出来)
+> 需要与LogMiddleware 中间件配合使用，否则不生效
+
+``` python 
+# log_settings 配置
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': False,
+    'filters': {
+        # 新增的配置
+        'request_id': {
+            '()': 'middleware.filters.RequestIDFilter'
+        }
+    },
+    'handlers': {
+        'console': {
+            'level': 'DEBUG',
+            'class': 'logging.StreamHandler',
+            'formatter': 'standard',   # 需要修改的的配置
+            'filters': ['request_id'], # 增加的 log_filter 的配置
+        },
+        # 以访问控制服务的日志举例子
+        'access_control': {
+            'class': 'logging.handlers.RotatingFileHandler',
+            'filters': ['request_id'], # 增加的配置
+            'level': 'DEBUG',
+            'formatter': 'standard', # 修改为新增的formatters 配置
+            'filename': os.path.join(os.path.sep, BASE_DIR_LOG, 'access_control.log'),
+            'mode': 'a',
+            'maxBytes': 1024 * 1024 * 5,
+            'backupCount': 1, # 修改
+        },
+    },
+    'formatters': {
+        # 增加的配置
+        'standard': {
+                    'format': '%(levelname)s %(asctime)s %(request_id)s %(lineno)d %(name)s %(module)s %(funcName)s %(process)d %(thread)d %(message)s'
+                },
+    },
+    # sparrow_cloud 的日志
+    'sparrow_cloud': {
+        'handlers': ['console', 'sparrow_cloud'],
+        'level': 'DEBUG',
+        'propagate': False,
+    },
+    'access_control': {
+        'handlers': ['console', 'access_control'],
+        'level': 'DEBUG',
+        'propagate': False,
+    }
+}
+}
+
+```
+
 ## ACCESS_CONTROL_VERIFY
 > access_control_verify decorators (访问控制验证)
 ``` python
     # settings 配置
     SERVICE_CONF = {
         "NAME": "",  # value为本服务的注册名称
         "SECRET": "",
```

### Comparing `sparrowcloud-4.0.1/sparrowcloud.egg-info/SOURCES.txt` & `sparrowcloud-4.1.0/sparrowcloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 sparrow_cloud/message_service/sender.py
 sparrow_cloud/message_service/sender_controller.py
 sparrow_cloud/middleware/__init__.py
 sparrow_cloud/middleware/acl_middleware.py
 sparrow_cloud/middleware/exception.py
 sparrow_cloud/middleware/jwt_middleware.py
 sparrow_cloud/middleware/lock_middleware.py
+sparrow_cloud/middleware/log_middleware.py
 sparrow_cloud/middleware/methodconvert.py
 sparrow_cloud/middleware/tracing_middleware.py
 sparrow_cloud/middleware/base/__init__.py
 sparrow_cloud/middleware/base/base_middleware.py
 sparrow_cloud/registry/__init__.py
 sparrow_cloud/registry/service_configuration.py
 sparrow_cloud/registry/service_discovery.py
@@ -145,19 +146,21 @@
 tests/test_ding_talk.py
 tests/test_distributed_lock.py
 tests/test_exception_middleware.py
 tests/test_get_token_sdk.py
 tests/test_hash_key.py
 tests/test_jwtmiddleware.py
 tests/test_lock_middleware.py
+tests/test_log_filter.py
 tests/test_message_client.py
 tests/test_rabbitmq_consumer_command.py
 tests/test_register_access_control.py
 tests/test_register_command.py
 tests/test_register_schema_command.py
+tests/test_requestid_middleware.py
 tests/test_requests_client.py
 tests/test_rest_client.py
 tests/test_service_configuration.py
 tests/test_service_log.py
 tests/test_table_api.py
 tests/test_tracing_middleware.py
 tests/test_user_id_authentication.py
```

### Comparing `sparrowcloud-4.0.1/tests/test_access_control.py` & `sparrowcloud-4.1.0/tests/test_access_control.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_acl_middleware.py` & `sparrowcloud-4.1.0/tests/test_acl_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_api_permission.py` & `sparrowcloud-4.1.0/tests/test_api_permission.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_app_message.py` & `sparrowcloud-4.1.0/tests/test_app_message.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_consul_service.py` & `sparrowcloud-4.1.0/tests/test_consul_service.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_ding_talk.py` & `sparrowcloud-4.1.0/tests/test_ding_talk.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_distributed_lock.py` & `sparrowcloud-4.1.0/tests/test_distributed_lock.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_exception_middleware.py` & `sparrowcloud-4.1.0/tests/test_exception_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_get_token_sdk.py` & `sparrowcloud-4.1.0/tests/test_get_token_sdk.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_hash_key.py` & `sparrowcloud-4.1.0/tests/test_hash_key.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_jwtmiddleware.py` & `sparrowcloud-4.1.0/tests/test_jwtmiddleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_lock_middleware.py` & `sparrowcloud-4.1.0/tests/test_lock_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_message_client.py` & `sparrowcloud-4.1.0/tests/test_message_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_rabbitmq_consumer_command.py` & `sparrowcloud-4.1.0/tests/test_rabbitmq_consumer_command.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_register_access_control.py` & `sparrowcloud-4.1.0/tests/test_register_access_control.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_register_command.py` & `sparrowcloud-4.1.0/tests/test_register_command.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_register_schema_command.py` & `sparrowcloud-4.1.0/tests/test_register_schema_command.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_requests_client.py` & `sparrowcloud-4.1.0/tests/test_requests_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_rest_client.py` & `sparrowcloud-4.1.0/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_service_configuration.py` & `sparrowcloud-4.1.0/tests/test_service_configuration.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_service_log.py` & `sparrowcloud-4.1.0/tests/test_service_log.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_table_api.py` & `sparrowcloud-4.1.0/tests/test_table_api.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_tracing_middleware.py` & `sparrowcloud-4.1.0/tests/test_tracing_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.0.1/tests/test_user_id_authentication.py` & `sparrowcloud-4.1.0/tests/test_user_id_authentication.py`

 * *Files identical despite different names*

