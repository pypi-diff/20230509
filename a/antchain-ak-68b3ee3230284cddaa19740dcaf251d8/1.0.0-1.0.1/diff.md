# Comparing `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0.tar.gz` & `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0.tar", last modified: Tue May  9 10:06:36 2023, max compression
+gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1.tar", last modified: Thu Feb  9 02:54:43 2023, max compression
```

## Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0.tar` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-09 10:06:35.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-09 10:06:35.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-09 10:06:35.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-09 10:06:35.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-09 10:06:35.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20374 2023-05-09 10:06:35.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
--rw-r--r--   0 root         (0) root         (0)    13930 2023-05-09 10:06:35.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-09 10:06:36.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-09 10:06:35.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22810 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
+-rw-r--r--   0 root         (0) root         (0)    16218 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/setup.py
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/LICENSE` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/README-CN.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/README.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDuration': self._keep_alive_duration_millis,
+            'keepAliveDurationMillis': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -130,17 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
-                    '_prod_code': 'ak_68b3ee3230284cddaa19740dcaf251d8',
-                    '_prod_channel': 'saas'
+                    'sdk_version': '1.0.1'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -197,15 +195,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDuration': self._keep_alive_duration_millis,
+            'keepAliveDurationMillis': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -233,17 +231,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
-                    '_prod_code': 'ak_68b3ee3230284cddaa19740dcaf251d8',
-                    '_prod_channel': 'saas'
+                    'sdk_version': '1.0.1'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -275,41 +271,41 @@
 
     def bind_demo_aaa_bbb_ccc(
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccRequest,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccResponse:
         """
         Description: 自动化测试创建test
-        Summary: 自动化测试创建test1
+        Summary: 自动化测试创建test
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.bind_demo_aaa_bbb_ccc_ex(request, headers, runtime)
 
     async def bind_demo_aaa_bbb_ccc_async(
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccRequest,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccResponse:
         """
         Description: 自动化测试创建test
-        Summary: 自动化测试创建test1
+        Summary: 自动化测试创建test
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.bind_demo_aaa_bbb_ccc_ex_async(request, headers, runtime)
 
     def bind_demo_aaa_bbb_ccc_ex(
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccResponse:
         """
         Description: 自动化测试创建test
-        Summary: 自动化测试创建test1
+        Summary: 自动化测试创建test
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccResponse(),
             self.do_request('1.0', 'demo.aaa.bbb.ccc.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
@@ -317,15 +313,15 @@
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccResponse:
         """
         Description: 自动化测试创建test
-        Summary: 自动化测试创建test1
+        Summary: 自动化测试创建test
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAaaBbbCccResponse(),
             await self.do_request_async('1.0', 'demo.aaa.bbb.ccc.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
@@ -436,7 +432,63 @@
         Summary: 能力中心九期测试
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse(),
             await self.do_request_async('1.0', 'demo.center.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def bind_demo_more_ability_testabc(
+        self,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse:
+        """
+        Description: 测试API绑定多个标签时的情况
+        Summary: API绑定多个标签
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.bind_demo_more_ability_testabc_ex(request, headers, runtime)
+
+    async def bind_demo_more_ability_testabc_async(
+        self,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse:
+        """
+        Description: 测试API绑定多个标签时的情况
+        Summary: API绑定多个标签
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.bind_demo_more_ability_testabc_ex_async(request, headers, runtime)
+
+    def bind_demo_more_ability_testabc_ex(
+        self,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse:
+        """
+        Description: 测试API绑定多个标签时的情况
+        Summary: API绑定多个标签
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse(),
+            self.do_request('1.0', 'demo.more.ability.testabc.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def bind_demo_more_ability_testabc_ex_async(
+        self,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse:
+        """
+        Description: 测试API绑定多个标签时的情况
+        Summary: API绑定多个标签
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse(),
+            await self.do_request_async('1.0', 'demo.more.ability.testabc.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -406,7 +406,83 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class BindDemoMoreAbilityTestabcRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class BindDemoMoreAbilityTestabcResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.0/setup.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_68b3ee3230284cddaa19740dcaf251d8.
 
-Created on 09/05/2023
+Created on 09/02/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8"
 NAME = "antchain_ak_68b3ee3230284cddaa19740dcaf251d8" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python"
```

