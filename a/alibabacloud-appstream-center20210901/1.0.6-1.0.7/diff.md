# Comparing `tmp/alibabacloud_appstream-center20210901-1.0.6.tar.gz` & `tmp/alibabacloud_appstream-center20210901-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_appstream-center20210901-1.0.6.tar", last modified: Mon Apr  3 09:43:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_appstream-center20210901-1.0.7.tar", last modified: Tue May  9 09:43:17 2023, max compression
```

## Comparing `alibabacloud_appstream-center20210901-1.0.6.tar` & `alibabacloud_appstream-center20210901-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2406 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1061 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1146 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93812 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901/client.py
--rw-r--r--   0 root         (0) root         (0)   196358 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2406 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      524 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2677 2023-04-03 09:43:23.000000 alibabacloud_appstream-center20210901-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   103790 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901/client.py
+-rw-r--r--   0 root         (0) root         (0)   217328 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-05-09 09:43:17.000000 alibabacloud_appstream-center20210901-1.0.7/setup.py
```

### Comparing `alibabacloud_appstream-center20210901-1.0.6/LICENSE` & `alibabacloud_appstream-center20210901-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210901-1.0.6/PKG-INFO` & `alibabacloud_appstream-center20210901-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_appstream-center20210901
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud appstream-center (20210901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_appstream-center20210901-1.0.6/README-CN.md` & `alibabacloud_appstream-center20210901-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210901-1.0.6/README.md` & `alibabacloud_appstream-center20210901-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901/client.py` & `alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,14 +293,18 @@
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.network):
             request.network_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.network, 'Network', 'json')
         if not UtilClient.is_unset(tmp_req.node_pool):
             request.node_pool_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.node_pool, 'NodePool', 'json')
         if not UtilClient.is_unset(tmp_req.runtime_policy):
             request.runtime_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.runtime_policy, 'RuntimePolicy', 'json')
+        if not UtilClient.is_unset(tmp_req.security_policy):
+            request.security_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.security_policy, 'SecurityPolicy', 'json')
+        if not UtilClient.is_unset(tmp_req.storage_policy):
+            request.storage_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.storage_policy, 'StoragePolicy', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
             request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.app_center_image_id):
             body['AppCenterImageId'] = request.app_center_image_id
         if not UtilClient.is_unset(request.app_instance_group_name):
             body['AppInstanceGroupName'] = request.app_instance_group_name
@@ -326,16 +330,20 @@
             body['PreOpenAppId'] = request.pre_open_app_id
         if not UtilClient.is_unset(request.product_type):
             body['ProductType'] = request.product_type
         if not UtilClient.is_unset(request.promotion_id):
             body['PromotionId'] = request.promotion_id
         if not UtilClient.is_unset(request.runtime_policy_shrink):
             body['RuntimePolicy'] = request.runtime_policy_shrink
+        if not UtilClient.is_unset(request.security_policy_shrink):
+            body['SecurityPolicy'] = request.security_policy_shrink
         if not UtilClient.is_unset(request.session_timeout):
             body['SessionTimeout'] = request.session_timeout
+        if not UtilClient.is_unset(request.storage_policy_shrink):
+            body['StoragePolicy'] = request.storage_policy_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
         if not UtilClient.is_unset(request.users):
             body['Users'] = request.users
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -365,14 +373,18 @@
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.network):
             request.network_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.network, 'Network', 'json')
         if not UtilClient.is_unset(tmp_req.node_pool):
             request.node_pool_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.node_pool, 'NodePool', 'json')
         if not UtilClient.is_unset(tmp_req.runtime_policy):
             request.runtime_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.runtime_policy, 'RuntimePolicy', 'json')
+        if not UtilClient.is_unset(tmp_req.security_policy):
+            request.security_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.security_policy, 'SecurityPolicy', 'json')
+        if not UtilClient.is_unset(tmp_req.storage_policy):
+            request.storage_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.storage_policy, 'StoragePolicy', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
             request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
         body = {}
         if not UtilClient.is_unset(request.app_center_image_id):
             body['AppCenterImageId'] = request.app_center_image_id
         if not UtilClient.is_unset(request.app_instance_group_name):
             body['AppInstanceGroupName'] = request.app_instance_group_name
@@ -398,16 +410,20 @@
             body['PreOpenAppId'] = request.pre_open_app_id
         if not UtilClient.is_unset(request.product_type):
             body['ProductType'] = request.product_type
         if not UtilClient.is_unset(request.promotion_id):
             body['PromotionId'] = request.promotion_id
         if not UtilClient.is_unset(request.runtime_policy_shrink):
             body['RuntimePolicy'] = request.runtime_policy_shrink
+        if not UtilClient.is_unset(request.security_policy_shrink):
+            body['SecurityPolicy'] = request.security_policy_shrink
         if not UtilClient.is_unset(request.session_timeout):
             body['SessionTimeout'] = request.session_timeout
+        if not UtilClient.is_unset(request.storage_policy_shrink):
+            body['StoragePolicy'] = request.storage_policy_shrink
         if not UtilClient.is_unset(request.user_info_shrink):
             body['UserInfo'] = request.user_info_shrink
         if not UtilClient.is_unset(request.users):
             body['Users'] = request.users
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -437,14 +453,92 @@
     async def create_app_instance_group_async(
         self,
         request: appstream_center_20210901_models.CreateAppInstanceGroupRequest,
     ) -> appstream_center_20210901_models.CreateAppInstanceGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_app_instance_group_with_options_async(request, runtime)
 
+    def create_image_from_app_instance_group_with_options(
+        self,
+        request: appstream_center_20210901_models.CreateImageFromAppInstanceGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> appstream_center_20210901_models.CreateImageFromAppInstanceGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_center_image_name):
+            body['AppCenterImageName'] = request.app_center_image_name
+        if not UtilClient.is_unset(request.app_instance_group_id):
+            body['AppInstanceGroupId'] = request.app_instance_group_id
+        if not UtilClient.is_unset(request.product_type):
+            body['ProductType'] = request.product_type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateImageFromAppInstanceGroup',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            appstream_center_20210901_models.CreateImageFromAppInstanceGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_image_from_app_instance_group_with_options_async(
+        self,
+        request: appstream_center_20210901_models.CreateImageFromAppInstanceGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> appstream_center_20210901_models.CreateImageFromAppInstanceGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_center_image_name):
+            body['AppCenterImageName'] = request.app_center_image_name
+        if not UtilClient.is_unset(request.app_instance_group_id):
+            body['AppInstanceGroupId'] = request.app_instance_group_id
+        if not UtilClient.is_unset(request.product_type):
+            body['ProductType'] = request.product_type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateImageFromAppInstanceGroup',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            appstream_center_20210901_models.CreateImageFromAppInstanceGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_image_from_app_instance_group(
+        self,
+        request: appstream_center_20210901_models.CreateImageFromAppInstanceGroupRequest,
+    ) -> appstream_center_20210901_models.CreateImageFromAppInstanceGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_image_from_app_instance_group_with_options(request, runtime)
+
+    async def create_image_from_app_instance_group_async(
+        self,
+        request: appstream_center_20210901_models.CreateImageFromAppInstanceGroupRequest,
+    ) -> appstream_center_20210901_models.CreateImageFromAppInstanceGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_image_from_app_instance_group_with_options_async(request, runtime)
+
     def delete_app_instance_group_with_options(
         self,
         request: appstream_center_20210901_models.DeleteAppInstanceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> appstream_center_20210901_models.DeleteAppInstanceGroupResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -765,14 +859,88 @@
     async def get_connection_ticket_async(
         self,
         request: appstream_center_20210901_models.GetConnectionTicketRequest,
     ) -> appstream_center_20210901_models.GetConnectionTicketResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_connection_ticket_with_options_async(request, runtime)
 
+    def get_debug_app_instance_with_options(
+        self,
+        request: appstream_center_20210901_models.GetDebugAppInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> appstream_center_20210901_models.GetDebugAppInstanceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_instance_group_id):
+            body['AppInstanceGroupId'] = request.app_instance_group_id
+        if not UtilClient.is_unset(request.product_type):
+            body['ProductType'] = request.product_type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetDebugAppInstance',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            appstream_center_20210901_models.GetDebugAppInstanceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_debug_app_instance_with_options_async(
+        self,
+        request: appstream_center_20210901_models.GetDebugAppInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> appstream_center_20210901_models.GetDebugAppInstanceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_instance_group_id):
+            body['AppInstanceGroupId'] = request.app_instance_group_id
+        if not UtilClient.is_unset(request.product_type):
+            body['ProductType'] = request.product_type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetDebugAppInstance',
+            version='2021-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            appstream_center_20210901_models.GetDebugAppInstanceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_debug_app_instance(
+        self,
+        request: appstream_center_20210901_models.GetDebugAppInstanceRequest,
+    ) -> appstream_center_20210901_models.GetDebugAppInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_debug_app_instance_with_options(request, runtime)
+
+    async def get_debug_app_instance_async(
+        self,
+        request: appstream_center_20210901_models.GetDebugAppInstanceRequest,
+    ) -> appstream_center_20210901_models.GetDebugAppInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_debug_app_instance_with_options_async(request, runtime)
+
     def get_ota_task_by_task_id_with_options(
         self,
         request: appstream_center_20210901_models.GetOtaTaskByTaskIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> appstream_center_20210901_models.GetOtaTaskByTaskIdResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1128,19 +1296,23 @@
     ) -> appstream_center_20210901_models.ListAppInstancesResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_instance_group_id):
             query['AppInstanceGroupId'] = request.app_instance_group_id
         if not UtilClient.is_unset(request.app_instance_id):
             query['AppInstanceId'] = request.app_instance_id
+        if not UtilClient.is_unset(request.include_deleted):
+            query['IncludeDeleted'] = request.include_deleted
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         body = {}
+        if not UtilClient.is_unset(request.app_instance_id_list):
+            body['AppInstanceIdList'] = request.app_instance_id_list
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -1166,19 +1338,23 @@
     ) -> appstream_center_20210901_models.ListAppInstancesResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_instance_group_id):
             query['AppInstanceGroupId'] = request.app_instance_group_id
         if not UtilClient.is_unset(request.app_instance_id):
             query['AppInstanceId'] = request.app_instance_id
+        if not UtilClient.is_unset(request.include_deleted):
+            query['IncludeDeleted'] = request.include_deleted
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         body = {}
+        if not UtilClient.is_unset(request.app_instance_id_list):
+            body['AppInstanceIdList'] = request.app_instance_id_list
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -1567,27 +1743,37 @@
         runtime: util_models.RuntimeOptions,
     ) -> appstream_center_20210901_models.ModifyAppInstanceGroupAttributeResponse:
         UtilClient.validate_model(tmp_req)
         request = appstream_center_20210901_models.ModifyAppInstanceGroupAttributeShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.node_pool):
             request.node_pool_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.node_pool, 'NodePool', 'json')
+        if not UtilClient.is_unset(tmp_req.security_policy):
+            request.security_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.security_policy, 'SecurityPolicy', 'json')
+        if not UtilClient.is_unset(tmp_req.storage_policy):
+            request.storage_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.storage_policy, 'StoragePolicy', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_instance_group_id):
             query['AppInstanceGroupId'] = request.app_instance_group_id
         if not UtilClient.is_unset(request.app_instance_group_name):
             query['AppInstanceGroupName'] = request.app_instance_group_name
         if not UtilClient.is_unset(request.node_pool_shrink):
             query['NodePool'] = request.node_pool_shrink
         if not UtilClient.is_unset(request.product_type):
             query['ProductType'] = request.product_type
         if not UtilClient.is_unset(request.session_timeout):
             query['SessionTimeout'] = request.session_timeout
+        body = {}
+        if not UtilClient.is_unset(request.security_policy_shrink):
+            body['SecurityPolicy'] = request.security_policy_shrink
+        if not UtilClient.is_unset(request.storage_policy_shrink):
+            body['StoragePolicy'] = request.storage_policy_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ModifyAppInstanceGroupAttribute',
             version='2021-09-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1607,27 +1793,37 @@
         runtime: util_models.RuntimeOptions,
     ) -> appstream_center_20210901_models.ModifyAppInstanceGroupAttributeResponse:
         UtilClient.validate_model(tmp_req)
         request = appstream_center_20210901_models.ModifyAppInstanceGroupAttributeShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.node_pool):
             request.node_pool_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.node_pool, 'NodePool', 'json')
+        if not UtilClient.is_unset(tmp_req.security_policy):
+            request.security_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.security_policy, 'SecurityPolicy', 'json')
+        if not UtilClient.is_unset(tmp_req.storage_policy):
+            request.storage_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.storage_policy, 'StoragePolicy', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_instance_group_id):
             query['AppInstanceGroupId'] = request.app_instance_group_id
         if not UtilClient.is_unset(request.app_instance_group_name):
             query['AppInstanceGroupName'] = request.app_instance_group_name
         if not UtilClient.is_unset(request.node_pool_shrink):
             query['NodePool'] = request.node_pool_shrink
         if not UtilClient.is_unset(request.product_type):
             query['ProductType'] = request.product_type
         if not UtilClient.is_unset(request.session_timeout):
             query['SessionTimeout'] = request.session_timeout
+        body = {}
+        if not UtilClient.is_unset(request.security_policy_shrink):
+            body['SecurityPolicy'] = request.security_policy_shrink
+        if not UtilClient.is_unset(request.storage_policy_shrink):
+            body['StoragePolicy'] = request.storage_policy_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ModifyAppInstanceGroupAttribute',
             version='2021-09-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
```

### Comparing `alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901/models.py` & `alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,17 +402,19 @@
             self.mode = m.get('Mode')
         return self
 
 
 class CreateAppInstanceGroupRequestNetwork(TeaModel):
     def __init__(
         self,
+        ip_expire_minutes: int = None,
         routes: List[CreateAppInstanceGroupRequestNetworkRoutes] = None,
         strategy_type: str = None,
     ):
+        self.ip_expire_minutes = ip_expire_minutes
         self.routes = routes
         self.strategy_type = strategy_type
 
     def validate(self):
         if self.routes:
             for k in self.routes:
                 if k:
@@ -420,24 +422,28 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.ip_expire_minutes is not None:
+            result['IpExpireMinutes'] = self.ip_expire_minutes
         result['Routes'] = []
         if self.routes is not None:
             for k in self.routes:
                 result['Routes'].append(k.to_map() if k else None)
         if self.strategy_type is not None:
             result['StrategyType'] = self.strategy_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('IpExpireMinutes') is not None:
+            self.ip_expire_minutes = m.get('IpExpireMinutes')
         self.routes = []
         if m.get('Routes') is not None:
             for k in m.get('Routes'):
                 temp_model = CreateAppInstanceGroupRequestNetworkRoutes()
                 self.routes.append(temp_model.from_map(k))
         if m.get('StrategyType') is not None:
             self.strategy_type = m.get('StrategyType')
@@ -630,38 +636,105 @@
             self.warm_up = m.get('WarmUp')
         return self
 
 
 class CreateAppInstanceGroupRequestRuntimePolicy(TeaModel):
     def __init__(
         self,
+        debug_mode: str = None,
         session_type: str = None,
     ):
+        self.debug_mode = debug_mode
+        # 会话类型。
         self.session_type = session_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.debug_mode is not None:
+            result['DebugMode'] = self.debug_mode
         if self.session_type is not None:
             result['SessionType'] = self.session_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('DebugMode') is not None:
+            self.debug_mode = m.get('DebugMode')
         if m.get('SessionType') is not None:
             self.session_type = m.get('SessionType')
         return self
 
 
+class CreateAppInstanceGroupRequestSecurityPolicy(TeaModel):
+    def __init__(
+        self,
+        reset_after_unbind: bool = None,
+        skip_user_auth_check: bool = None,
+    ):
+        self.reset_after_unbind = reset_after_unbind
+        self.skip_user_auth_check = skip_user_auth_check
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.reset_after_unbind is not None:
+            result['ResetAfterUnbind'] = self.reset_after_unbind
+        if self.skip_user_auth_check is not None:
+            result['SkipUserAuthCheck'] = self.skip_user_auth_check
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ResetAfterUnbind') is not None:
+            self.reset_after_unbind = m.get('ResetAfterUnbind')
+        if m.get('SkipUserAuthCheck') is not None:
+            self.skip_user_auth_check = m.get('SkipUserAuthCheck')
+        return self
+
+
+class CreateAppInstanceGroupRequestStoragePolicy(TeaModel):
+    def __init__(
+        self,
+        storage_type_list: List[str] = None,
+    ):
+        self.storage_type_list = storage_type_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.storage_type_list is not None:
+            result['StorageTypeList'] = self.storage_type_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('StorageTypeList') is not None:
+            self.storage_type_list = m.get('StorageTypeList')
+        return self
+
+
 class CreateAppInstanceGroupRequestUserInfo(TeaModel):
     def __init__(
         self,
         type: str = None,
     ):
         self.type = type
 
@@ -699,15 +772,17 @@
         node_pool: CreateAppInstanceGroupRequestNodePool = None,
         period: int = None,
         period_unit: str = None,
         pre_open_app_id: str = None,
         product_type: str = None,
         promotion_id: str = None,
         runtime_policy: CreateAppInstanceGroupRequestRuntimePolicy = None,
+        security_policy: CreateAppInstanceGroupRequestSecurityPolicy = None,
         session_timeout: int = None,
+        storage_policy: CreateAppInstanceGroupRequestStoragePolicy = None,
         user_info: CreateAppInstanceGroupRequestUserInfo = None,
         users: List[str] = None,
     ):
         self.app_center_image_id = app_center_image_id
         self.app_instance_group_name = app_instance_group_name
         self.auto_pay = auto_pay
         self.auto_renew = auto_renew
@@ -718,25 +793,31 @@
         self.node_pool = node_pool
         self.period = period
         self.period_unit = period_unit
         self.pre_open_app_id = pre_open_app_id
         self.product_type = product_type
         self.promotion_id = promotion_id
         self.runtime_policy = runtime_policy
+        self.security_policy = security_policy
         self.session_timeout = session_timeout
+        self.storage_policy = storage_policy
         self.user_info = user_info
         self.users = users
 
     def validate(self):
         if self.network:
             self.network.validate()
         if self.node_pool:
             self.node_pool.validate()
         if self.runtime_policy:
             self.runtime_policy.validate()
+        if self.security_policy:
+            self.security_policy.validate()
+        if self.storage_policy:
+            self.storage_policy.validate()
         if self.user_info:
             self.user_info.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -768,16 +849,20 @@
             result['PreOpenAppId'] = self.pre_open_app_id
         if self.product_type is not None:
             result['ProductType'] = self.product_type
         if self.promotion_id is not None:
             result['PromotionId'] = self.promotion_id
         if self.runtime_policy is not None:
             result['RuntimePolicy'] = self.runtime_policy.to_map()
+        if self.security_policy is not None:
+            result['SecurityPolicy'] = self.security_policy.to_map()
         if self.session_timeout is not None:
             result['SessionTimeout'] = self.session_timeout
+        if self.storage_policy is not None:
+            result['StoragePolicy'] = self.storage_policy.to_map()
         if self.user_info is not None:
             result['UserInfo'] = self.user_info.to_map()
         if self.users is not None:
             result['Users'] = self.users
         return result
 
     def from_map(self, m: dict = None):
@@ -811,16 +896,22 @@
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
         if m.get('PromotionId') is not None:
             self.promotion_id = m.get('PromotionId')
         if m.get('RuntimePolicy') is not None:
             temp_model = CreateAppInstanceGroupRequestRuntimePolicy()
             self.runtime_policy = temp_model.from_map(m['RuntimePolicy'])
+        if m.get('SecurityPolicy') is not None:
+            temp_model = CreateAppInstanceGroupRequestSecurityPolicy()
+            self.security_policy = temp_model.from_map(m['SecurityPolicy'])
         if m.get('SessionTimeout') is not None:
             self.session_timeout = m.get('SessionTimeout')
+        if m.get('StoragePolicy') is not None:
+            temp_model = CreateAppInstanceGroupRequestStoragePolicy()
+            self.storage_policy = temp_model.from_map(m['StoragePolicy'])
         if m.get('UserInfo') is not None:
             temp_model = CreateAppInstanceGroupRequestUserInfo()
             self.user_info = temp_model.from_map(m['UserInfo'])
         if m.get('Users') is not None:
             self.users = m.get('Users')
         return self
 
@@ -839,15 +930,17 @@
         node_pool_shrink: str = None,
         period: int = None,
         period_unit: str = None,
         pre_open_app_id: str = None,
         product_type: str = None,
         promotion_id: str = None,
         runtime_policy_shrink: str = None,
+        security_policy_shrink: str = None,
         session_timeout: int = None,
+        storage_policy_shrink: str = None,
         user_info_shrink: str = None,
         users: List[str] = None,
     ):
         self.app_center_image_id = app_center_image_id
         self.app_instance_group_name = app_instance_group_name
         self.auto_pay = auto_pay
         self.auto_renew = auto_renew
@@ -858,15 +951,17 @@
         self.node_pool_shrink = node_pool_shrink
         self.period = period
         self.period_unit = period_unit
         self.pre_open_app_id = pre_open_app_id
         self.product_type = product_type
         self.promotion_id = promotion_id
         self.runtime_policy_shrink = runtime_policy_shrink
+        self.security_policy_shrink = security_policy_shrink
         self.session_timeout = session_timeout
+        self.storage_policy_shrink = storage_policy_shrink
         self.user_info_shrink = user_info_shrink
         self.users = users
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -901,16 +996,20 @@
             result['PreOpenAppId'] = self.pre_open_app_id
         if self.product_type is not None:
             result['ProductType'] = self.product_type
         if self.promotion_id is not None:
             result['PromotionId'] = self.promotion_id
         if self.runtime_policy_shrink is not None:
             result['RuntimePolicy'] = self.runtime_policy_shrink
+        if self.security_policy_shrink is not None:
+            result['SecurityPolicy'] = self.security_policy_shrink
         if self.session_timeout is not None:
             result['SessionTimeout'] = self.session_timeout
+        if self.storage_policy_shrink is not None:
+            result['StoragePolicy'] = self.storage_policy_shrink
         if self.user_info_shrink is not None:
             result['UserInfo'] = self.user_info_shrink
         if self.users is not None:
             result['Users'] = self.users
         return result
 
     def from_map(self, m: dict = None):
@@ -941,16 +1040,20 @@
             self.pre_open_app_id = m.get('PreOpenAppId')
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
         if m.get('PromotionId') is not None:
             self.promotion_id = m.get('PromotionId')
         if m.get('RuntimePolicy') is not None:
             self.runtime_policy_shrink = m.get('RuntimePolicy')
+        if m.get('SecurityPolicy') is not None:
+            self.security_policy_shrink = m.get('SecurityPolicy')
         if m.get('SessionTimeout') is not None:
             self.session_timeout = m.get('SessionTimeout')
+        if m.get('StoragePolicy') is not None:
+            self.storage_policy_shrink = m.get('StoragePolicy')
         if m.get('UserInfo') is not None:
             self.user_info_shrink = m.get('UserInfo')
         if m.get('Users') is not None:
             self.users = m.get('Users')
         return self
 
 
@@ -1068,14 +1171,130 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateAppInstanceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateImageFromAppInstanceGroupRequest(TeaModel):
+    def __init__(
+        self,
+        app_center_image_name: str = None,
+        app_instance_group_id: str = None,
+        product_type: str = None,
+    ):
+        self.app_center_image_name = app_center_image_name
+        self.app_instance_group_id = app_instance_group_id
+        self.product_type = product_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_center_image_name is not None:
+            result['AppCenterImageName'] = self.app_center_image_name
+        if self.app_instance_group_id is not None:
+            result['AppInstanceGroupId'] = self.app_instance_group_id
+        if self.product_type is not None:
+            result['ProductType'] = self.product_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppCenterImageName') is not None:
+            self.app_center_image_name = m.get('AppCenterImageName')
+        if m.get('AppInstanceGroupId') is not None:
+            self.app_instance_group_id = m.get('AppInstanceGroupId')
+        if m.get('ProductType') is not None:
+            self.product_type = m.get('ProductType')
+        return self
+
+
+class CreateImageFromAppInstanceGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        image_id: str = None,
+        request_id: str = None,
+    ):
+        self.image_id = image_id
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_id is not None:
+            result['ImageId'] = self.image_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ImageId') is not None:
+            self.image_id = m.get('ImageId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateImageFromAppInstanceGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateImageFromAppInstanceGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateImageFromAppInstanceGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteAppInstanceGroupRequest(TeaModel):
     def __init__(
         self,
         app_instance_group_id: str = None,
         product_type: str = None,
     ):
         self.app_instance_group_id = app_instance_group_id
@@ -1690,14 +1909,15 @@
         node_pool: List[GetAppInstanceGroupResponseBodyAppInstanceGroupModelsNodePool] = None,
         os_type: str = None,
         ota_info: GetAppInstanceGroupResponseBodyAppInstanceGroupModelsOtaInfo = None,
         product_type: str = None,
         region_id: str = None,
         resource_status: str = None,
         session_timeout: str = None,
+        skip_user_auth_check: bool = None,
         spec_id: str = None,
         status: str = None,
     ):
         self.amount = amount
         self.app_center_image_id = app_center_image_id
         self.app_center_image_name = app_center_image_name
         self.app_instance_group_id = app_instance_group_id
@@ -1711,14 +1931,15 @@
         self.node_pool = node_pool
         self.os_type = os_type
         self.ota_info = ota_info
         self.product_type = product_type
         self.region_id = region_id
         self.resource_status = resource_status
         self.session_timeout = session_timeout
+        self.skip_user_auth_check = skip_user_auth_check
         self.spec_id = spec_id
         self.status = status
 
     def validate(self):
         if self.apps:
             for k in self.apps:
                 if k:
@@ -1772,14 +1993,16 @@
             result['ProductType'] = self.product_type
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_status is not None:
             result['ResourceStatus'] = self.resource_status
         if self.session_timeout is not None:
             result['SessionTimeout'] = self.session_timeout
+        if self.skip_user_auth_check is not None:
+            result['SkipUserAuthCheck'] = self.skip_user_auth_check
         if self.spec_id is not None:
             result['SpecId'] = self.spec_id
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
@@ -1823,14 +2046,16 @@
             self.product_type = m.get('ProductType')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceStatus') is not None:
             self.resource_status = m.get('ResourceStatus')
         if m.get('SessionTimeout') is not None:
             self.session_timeout = m.get('SessionTimeout')
+        if m.get('SkipUserAuthCheck') is not None:
+            self.skip_user_auth_check = m.get('SkipUserAuthCheck')
         if m.get('SpecId') is not None:
             self.spec_id = m.get('SpecId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
@@ -2098,14 +2323,154 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetConnectionTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetDebugAppInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        app_instance_group_id: str = None,
+        product_type: str = None,
+    ):
+        self.app_instance_group_id = app_instance_group_id
+        self.product_type = product_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_instance_group_id is not None:
+            result['AppInstanceGroupId'] = self.app_instance_group_id
+        if self.product_type is not None:
+            result['ProductType'] = self.product_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppInstanceGroupId') is not None:
+            self.app_instance_group_id = m.get('AppInstanceGroupId')
+        if m.get('ProductType') is not None:
+            self.product_type = m.get('ProductType')
+        return self
+
+
+class GetDebugAppInstanceResponseBody(TeaModel):
+    def __init__(
+        self,
+        app_id: str = None,
+        app_instance_group_id: str = None,
+        app_instance_id: str = None,
+        app_version: str = None,
+        auth_code: str = None,
+        request_id: str = None,
+        user_id: str = None,
+    ):
+        self.app_id = app_id
+        self.app_instance_group_id = app_instance_group_id
+        self.app_instance_id = app_instance_id
+        self.app_version = app_version
+        self.auth_code = auth_code
+        self.request_id = request_id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_id is not None:
+            result['AppId'] = self.app_id
+        if self.app_instance_group_id is not None:
+            result['AppInstanceGroupId'] = self.app_instance_group_id
+        if self.app_instance_id is not None:
+            result['AppInstanceId'] = self.app_instance_id
+        if self.app_version is not None:
+            result['AppVersion'] = self.app_version
+        if self.auth_code is not None:
+            result['AuthCode'] = self.auth_code
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppId') is not None:
+            self.app_id = m.get('AppId')
+        if m.get('AppInstanceGroupId') is not None:
+            self.app_instance_group_id = m.get('AppInstanceGroupId')
+        if m.get('AppInstanceId') is not None:
+            self.app_instance_id = m.get('AppInstanceId')
+        if m.get('AppVersion') is not None:
+            self.app_version = m.get('AppVersion')
+        if m.get('AuthCode') is not None:
+            self.auth_code = m.get('AuthCode')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class GetDebugAppInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDebugAppInstanceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDebugAppInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetOtaTaskByTaskIdRequest(TeaModel):
     def __init__(
         self,
         task_id: str = None,
     ):
         self.task_id = task_id
 
@@ -2962,18 +3327,21 @@
         self,
         app_icon: str = None,
         app_id: str = None,
         app_name: str = None,
         app_version: str = None,
         app_version_name: str = None,
     ):
+        # 应用图标。
         self.app_icon = app_icon
         self.app_id = app_id
         self.app_name = app_name
+        # 应用版本。
         self.app_version = app_version
+        # 应用版本名称。
         self.app_version_name = app_version_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3287,35 +3655,39 @@
         node_pool: List[ListAppInstanceGroupResponseBodyAppInstanceGroupModelsNodePool] = None,
         os_type: str = None,
         ota_info: ListAppInstanceGroupResponseBodyAppInstanceGroupModelsOtaInfo = None,
         product_type: str = None,
         region_id: str = None,
         resource_status: str = None,
         session_timeout: str = None,
+        skip_user_auth_check: bool = None,
         spec_id: str = None,
         status: str = None,
     ):
         self.amount = amount
         self.app_center_image_id = app_center_image_id
         self.app_instance_group_id = app_instance_group_id
         self.app_instance_group_name = app_instance_group_name
         self.app_instance_type = app_instance_type
+        # 策略ID。
         self.app_policy_id = app_policy_id
         self.apps = apps
+        # 售卖模式。
         self.charge_resource_mode = charge_resource_mode
         self.charge_type = charge_type
         self.expired_time = expired_time
         self.gmt_create = gmt_create
         self.node_pool = node_pool
         self.os_type = os_type
         self.ota_info = ota_info
         self.product_type = product_type
         self.region_id = region_id
         self.resource_status = resource_status
         self.session_timeout = session_timeout
+        self.skip_user_auth_check = skip_user_auth_check
         self.spec_id = spec_id
         self.status = status
 
     def validate(self):
         if self.apps:
             for k in self.apps:
                 if k:
@@ -3369,14 +3741,16 @@
             result['ProductType'] = self.product_type
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_status is not None:
             result['ResourceStatus'] = self.resource_status
         if self.session_timeout is not None:
             result['SessionTimeout'] = self.session_timeout
+        if self.skip_user_auth_check is not None:
+            result['SkipUserAuthCheck'] = self.skip_user_auth_check
         if self.spec_id is not None:
             result['SpecId'] = self.spec_id
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
@@ -3420,14 +3794,16 @@
             self.product_type = m.get('ProductType')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceStatus') is not None:
             self.resource_status = m.get('ResourceStatus')
         if m.get('SessionTimeout') is not None:
             self.session_timeout = m.get('SessionTimeout')
+        if m.get('SkipUserAuthCheck') is not None:
+            self.skip_user_auth_check = m.get('SkipUserAuthCheck')
         if m.get('SpecId') is not None:
             self.spec_id = m.get('SpecId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
@@ -3535,20 +3911,24 @@
 
 
 class ListAppInstancesRequest(TeaModel):
     def __init__(
         self,
         app_instance_group_id: str = None,
         app_instance_id: str = None,
+        app_instance_id_list: List[str] = None,
+        include_deleted: bool = None,
         page_number: int = None,
         page_size: int = None,
         status: List[str] = None,
     ):
         self.app_instance_group_id = app_instance_group_id
         self.app_instance_id = app_instance_id
+        self.app_instance_id_list = app_instance_id_list
+        self.include_deleted = include_deleted
         self.page_number = page_number
         self.page_size = page_size
         self.status = status
 
     def validate(self):
         pass
 
@@ -3558,69 +3938,115 @@
             return _map
 
         result = dict()
         if self.app_instance_group_id is not None:
             result['AppInstanceGroupId'] = self.app_instance_group_id
         if self.app_instance_id is not None:
             result['AppInstanceId'] = self.app_instance_id
+        if self.app_instance_id_list is not None:
+            result['AppInstanceIdList'] = self.app_instance_id_list
+        if self.include_deleted is not None:
+            result['IncludeDeleted'] = self.include_deleted
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AppInstanceGroupId') is not None:
             self.app_instance_group_id = m.get('AppInstanceGroupId')
         if m.get('AppInstanceId') is not None:
             self.app_instance_id = m.get('AppInstanceId')
+        if m.get('AppInstanceIdList') is not None:
+            self.app_instance_id_list = m.get('AppInstanceIdList')
+        if m.get('IncludeDeleted') is not None:
+            self.include_deleted = m.get('IncludeDeleted')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
+class ListAppInstancesResponseBodyAppInstanceModelsBindInfo(TeaModel):
+    def __init__(
+        self,
+        end_user_id: str = None,
+        usage_duration: int = None,
+    ):
+        self.end_user_id = end_user_id
+        self.usage_duration = usage_duration
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_user_id is not None:
+            result['EndUserId'] = self.end_user_id
+        if self.usage_duration is not None:
+            result['UsageDuration'] = self.usage_duration
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndUserId') is not None:
+            self.end_user_id = m.get('EndUserId')
+        if m.get('UsageDuration') is not None:
+            self.usage_duration = m.get('UsageDuration')
+        return self
+
+
 class ListAppInstancesResponseBodyAppInstanceModels(TeaModel):
     def __init__(
         self,
         app_instance_group_id: str = None,
         app_instance_id: str = None,
+        bind_info: ListAppInstancesResponseBodyAppInstanceModelsBindInfo = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         main_eth_public_ip: str = None,
         session_status: str = None,
         status: str = None,
     ):
         self.app_instance_group_id = app_instance_group_id
         self.app_instance_id = app_instance_id
+        self.bind_info = bind_info
         self.gmt_create = gmt_create
         self.gmt_modified = gmt_modified
         self.main_eth_public_ip = main_eth_public_ip
         self.session_status = session_status
         self.status = status
 
     def validate(self):
-        pass
+        if self.bind_info:
+            self.bind_info.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.app_instance_group_id is not None:
             result['AppInstanceGroupId'] = self.app_instance_group_id
         if self.app_instance_id is not None:
             result['AppInstanceId'] = self.app_instance_id
+        if self.bind_info is not None:
+            result['BindInfo'] = self.bind_info.to_map()
         if self.gmt_create is not None:
             result['GmtCreate'] = self.gmt_create
         if self.gmt_modified is not None:
             result['GmtModified'] = self.gmt_modified
         if self.main_eth_public_ip is not None:
             result['MainEthPublicIp'] = self.main_eth_public_ip
         if self.session_status is not None:
@@ -3631,14 +4057,17 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AppInstanceGroupId') is not None:
             self.app_instance_group_id = m.get('AppInstanceGroupId')
         if m.get('AppInstanceId') is not None:
             self.app_instance_id = m.get('AppInstanceId')
+        if m.get('BindInfo') is not None:
+            temp_model = ListAppInstancesResponseBodyAppInstanceModelsBindInfo()
+            self.bind_info = temp_model.from_map(m['BindInfo'])
         if m.get('GmtCreate') is not None:
             self.gmt_create = m.get('GmtCreate')
         if m.get('GmtModified') is not None:
             self.gmt_modified = m.get('GmtModified')
         if m.get('MainEthPublicIp') is not None:
             self.main_eth_public_ip = m.get('MainEthPublicIp')
         if m.get('SessionStatus') is not None:
@@ -3758,17 +4187,20 @@
         language: str = None,
         node_instance_type: str = None,
         os_type: str = None,
         page_number: int = None,
         page_size: int = None,
         product_type: str = None,
     ):
+        # 资源所属的地域ID。关于支持的地域详情，请参见[使用限制](~~426036~~)。
         self.biz_region_id = biz_region_id
+        # 语言类型。
         self.language = language
         self.node_instance_type = node_instance_type
+        # 支持的操作系统类型。
         self.os_type = os_type
         self.page_number = page_number
         self.page_size = page_size
         self.product_type = product_type
 
     def validate(self):
         pass
@@ -3824,19 +4256,28 @@
         memory: int = None,
         node_instance_type: str = None,
         node_instance_type_family: str = None,
         node_type_name: str = None,
     ):
         self.cpu = cpu
         self.gpu = gpu
+        # 显卡内存大小，单位为MB。
         self.gpu_memory = gpu_memory
+        # 最大并发会话数，即单个资源可同时连接的会话数。如果同时连接的会话数过多，可能导致应用的使用体验下降。取值范围因资源规格不同而不同。各资源规格对应的取值范围分别是：
+        # 
+        # - appstreaming.general.4c8g：1\~2；
+        # - appstreaming.general.8c16g：1\~4；
+        # - appstreaming.vgpu.8c16g.4g：1\~4；
+        # - appstreaming.vgpu.8c31g.16g：1\~4；
+        # - appstreaming.vgpu.14c93g.12g：1\~6；
         self.max_capacity = max_capacity
         self.memory = memory
         self.node_instance_type = node_instance_type
         self.node_instance_type_family = node_instance_type_family
+        # 资源规格名称。
         self.node_type_name = node_type_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4542,32 +4983,100 @@
         if m.get('NodeCapacity') is not None:
             self.node_capacity = m.get('NodeCapacity')
         if m.get('NodePoolId') is not None:
             self.node_pool_id = m.get('NodePoolId')
         return self
 
 
+class ModifyAppInstanceGroupAttributeRequestSecurityPolicy(TeaModel):
+    def __init__(
+        self,
+        reset_after_unbind: bool = None,
+        skip_user_auth_check: bool = None,
+    ):
+        self.reset_after_unbind = reset_after_unbind
+        self.skip_user_auth_check = skip_user_auth_check
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.reset_after_unbind is not None:
+            result['ResetAfterUnbind'] = self.reset_after_unbind
+        if self.skip_user_auth_check is not None:
+            result['SkipUserAuthCheck'] = self.skip_user_auth_check
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ResetAfterUnbind') is not None:
+            self.reset_after_unbind = m.get('ResetAfterUnbind')
+        if m.get('SkipUserAuthCheck') is not None:
+            self.skip_user_auth_check = m.get('SkipUserAuthCheck')
+        return self
+
+
+class ModifyAppInstanceGroupAttributeRequestStoragePolicy(TeaModel):
+    def __init__(
+        self,
+        storage_type_list: List[str] = None,
+    ):
+        self.storage_type_list = storage_type_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.storage_type_list is not None:
+            result['StorageTypeList'] = self.storage_type_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('StorageTypeList') is not None:
+            self.storage_type_list = m.get('StorageTypeList')
+        return self
+
+
 class ModifyAppInstanceGroupAttributeRequest(TeaModel):
     def __init__(
         self,
         app_instance_group_id: str = None,
         app_instance_group_name: str = None,
         node_pool: ModifyAppInstanceGroupAttributeRequestNodePool = None,
         product_type: str = None,
+        security_policy: ModifyAppInstanceGroupAttributeRequestSecurityPolicy = None,
         session_timeout: int = None,
+        storage_policy: ModifyAppInstanceGroupAttributeRequestStoragePolicy = None,
     ):
         self.app_instance_group_id = app_instance_group_id
         self.app_instance_group_name = app_instance_group_name
         self.node_pool = node_pool
         self.product_type = product_type
+        self.security_policy = security_policy
         self.session_timeout = session_timeout
+        self.storage_policy = storage_policy
 
     def validate(self):
         if self.node_pool:
             self.node_pool.validate()
+        if self.security_policy:
+            self.security_policy.validate()
+        if self.storage_policy:
+            self.storage_policy.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -4575,48 +5084,62 @@
             result['AppInstanceGroupId'] = self.app_instance_group_id
         if self.app_instance_group_name is not None:
             result['AppInstanceGroupName'] = self.app_instance_group_name
         if self.node_pool is not None:
             result['NodePool'] = self.node_pool.to_map()
         if self.product_type is not None:
             result['ProductType'] = self.product_type
+        if self.security_policy is not None:
+            result['SecurityPolicy'] = self.security_policy.to_map()
         if self.session_timeout is not None:
             result['SessionTimeout'] = self.session_timeout
+        if self.storage_policy is not None:
+            result['StoragePolicy'] = self.storage_policy.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AppInstanceGroupId') is not None:
             self.app_instance_group_id = m.get('AppInstanceGroupId')
         if m.get('AppInstanceGroupName') is not None:
             self.app_instance_group_name = m.get('AppInstanceGroupName')
         if m.get('NodePool') is not None:
             temp_model = ModifyAppInstanceGroupAttributeRequestNodePool()
             self.node_pool = temp_model.from_map(m['NodePool'])
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
+        if m.get('SecurityPolicy') is not None:
+            temp_model = ModifyAppInstanceGroupAttributeRequestSecurityPolicy()
+            self.security_policy = temp_model.from_map(m['SecurityPolicy'])
         if m.get('SessionTimeout') is not None:
             self.session_timeout = m.get('SessionTimeout')
+        if m.get('StoragePolicy') is not None:
+            temp_model = ModifyAppInstanceGroupAttributeRequestStoragePolicy()
+            self.storage_policy = temp_model.from_map(m['StoragePolicy'])
         return self
 
 
 class ModifyAppInstanceGroupAttributeShrinkRequest(TeaModel):
     def __init__(
         self,
         app_instance_group_id: str = None,
         app_instance_group_name: str = None,
         node_pool_shrink: str = None,
         product_type: str = None,
+        security_policy_shrink: str = None,
         session_timeout: int = None,
+        storage_policy_shrink: str = None,
     ):
         self.app_instance_group_id = app_instance_group_id
         self.app_instance_group_name = app_instance_group_name
         self.node_pool_shrink = node_pool_shrink
         self.product_type = product_type
+        self.security_policy_shrink = security_policy_shrink
         self.session_timeout = session_timeout
+        self.storage_policy_shrink = storage_policy_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -4627,30 +5150,38 @@
             result['AppInstanceGroupId'] = self.app_instance_group_id
         if self.app_instance_group_name is not None:
             result['AppInstanceGroupName'] = self.app_instance_group_name
         if self.node_pool_shrink is not None:
             result['NodePool'] = self.node_pool_shrink
         if self.product_type is not None:
             result['ProductType'] = self.product_type
+        if self.security_policy_shrink is not None:
+            result['SecurityPolicy'] = self.security_policy_shrink
         if self.session_timeout is not None:
             result['SessionTimeout'] = self.session_timeout
+        if self.storage_policy_shrink is not None:
+            result['StoragePolicy'] = self.storage_policy_shrink
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AppInstanceGroupId') is not None:
             self.app_instance_group_id = m.get('AppInstanceGroupId')
         if m.get('AppInstanceGroupName') is not None:
             self.app_instance_group_name = m.get('AppInstanceGroupName')
         if m.get('NodePool') is not None:
             self.node_pool_shrink = m.get('NodePool')
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
+        if m.get('SecurityPolicy') is not None:
+            self.security_policy_shrink = m.get('SecurityPolicy')
         if m.get('SessionTimeout') is not None:
             self.session_timeout = m.get('SessionTimeout')
+        if m.get('StoragePolicy') is not None:
+            self.storage_policy_shrink = m.get('StoragePolicy')
         return self
 
 
 class ModifyAppInstanceGroupAttributeResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -4736,16 +5267,19 @@
 class ModifyNodePoolAttributeRequestNodePoolStrategyRecurrenceSchedulesTimerPeriods(TeaModel):
     def __init__(
         self,
         amount: int = None,
         end_time: str = None,
         start_time: str = None,
     ):
+        # 资源数量。
         self.amount = amount
+        # 结束时间。格式为HH:mm。
         self.end_time = end_time
+        # 开始时间。格式为HH:mm。
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4775,16 +5309,25 @@
 class ModifyNodePoolAttributeRequestNodePoolStrategyRecurrenceSchedules(TeaModel):
     def __init__(
         self,
         recurrence_type: str = None,
         recurrence_values: List[int] = None,
         timer_periods: List[ModifyNodePoolAttributeRequestNodePoolStrategyRecurrenceSchedulesTimerPeriods] = None,
     ):
+        # 策略执行周期的类型。必须同时指定`RecurrenceType`和`RecurrenceValues`。
         self.recurrence_type = recurrence_type
+        # 策略执行周期的数值列表。
         self.recurrence_values = recurrence_values
+        # 策略执行周期的时间段列表。时间段设置要求：
+        # 
+        # - 最多可添加3个时间段。
+        # - 时间段之间不重叠。
+        # - 时间段之间的间隔大于或等于5分钟。
+        # - 单个时间段的时长大于或等于15分钟。
+        # - 所有时间段累计不跨天。
         self.timer_periods = timer_periods
 
     def validate(self):
         if self.timer_periods:
             for k in self.timer_periods:
                 if k:
                     k.validate()
@@ -4830,22 +5373,31 @@
         scaling_usage_threshold: str = None,
         strategy_disable_date: str = None,
         strategy_enable_date: str = None,
         strategy_type: str = None,
         warm_up: bool = None,
     ):
         self.max_scaling_amount = max_scaling_amount
+        # 购买资源的数量。取值范围：1~100。
+        # 
+        # > 
+        # - 若为包年包月资源，则该参数不可修改。
+        # - 若为按量付费资源，则当弹性模式（`StrategyType`）为固定数量（`NODE_FIXED`）或自动扩缩容（`NODE_SCALING_BY_USAGE`）时该参数可修改。
         self.node_amount = node_amount
+        # 策略执行周期列表。`StrategyType`（弹性模式）设为`NODE_SCALING_BY_SCHEDULE`（定时扩缩容）时，该字段必填。
         self.recurrence_schedules = recurrence_schedules
         self.scaling_down_after_idle_minutes = scaling_down_after_idle_minutes
         self.scaling_step = scaling_step
         self.scaling_usage_threshold = scaling_usage_threshold
+        # 策略失效日期。格式为：yyyy-MM-dd。失效日期与生效日期的间隔必须介于7天到1年之间（含7天和1年）。`StrategyType`（弹性模式）设为`NODE_SCALING_BY_SCHEDULE`（定时扩缩容）时，该字段必填。
         self.strategy_disable_date = strategy_disable_date
+        # 策略生效日期。格式为：yyyy-MM-dd。该日期必须大于或等于当前日期。`StrategyType`（弹性模式）设为`NODE_SCALING_BY_SCHEDULE`（定时扩缩容）时，该字段必填。
         self.strategy_enable_date = strategy_enable_date
         self.strategy_type = strategy_type
+        # 是否开启资源预热策略。`StrategyType`（弹性模式）设为`NODE_SCALING_BY_SCHEDULE`（定时扩缩容）时，该字段必填。
         self.warm_up = warm_up
 
     def validate(self):
         if self.recurrence_schedules:
             for k in self.recurrence_schedules:
                 if k:
                     k.validate()
@@ -4917,14 +5469,15 @@
         pool_id: str = None,
         product_type: str = None,
     ):
         self.biz_region_id = biz_region_id
         self.node_capacity = node_capacity
         self.node_pool_strategy = node_pool_strategy
         self.pool_id = pool_id
+        # 产品类型。
         self.product_type = product_type
 
     def validate(self):
         if self.node_pool_strategy:
             self.node_pool_strategy.validate()
 
     def to_map(self):
@@ -4970,14 +5523,15 @@
         pool_id: str = None,
         product_type: str = None,
     ):
         self.biz_region_id = biz_region_id
         self.node_capacity = node_capacity
         self.node_pool_strategy_shrink = node_pool_strategy_shrink
         self.pool_id = pool_id
+        # 产品类型。
         self.product_type = product_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901.egg-info/PKG-INFO` & `alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-appstream-center20210901
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud appstream-center (20210901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_appstream-center20210901-1.0.6/alibabacloud_appstream_center20210901.egg-info/SOURCES.txt` & `alibabacloud_appstream-center20210901-1.0.7/alibabacloud_appstream_center20210901.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_appstream-center20210901-1.0.6/setup.py` & `alibabacloud_appstream-center20210901-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_appstream-center20210901.
 
-Created on 03/04/2023
+Created on 09/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_appstream_center20210901"
 NAME = "alibabacloud_appstream-center20210901" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud appstream-center (20210901) SDK Library for Python"
```

