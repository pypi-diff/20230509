# Comparing `tmp/neulabs-cdk-constructs-0.3.0.tar.gz` & `tmp/neulabs-cdk-constructs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.3.0.tar", last modified: Tue May  2 15:15:24 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.3.1.tar", last modified: Tue May  9 15:00:35 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.3.0.tar` & `neulabs-cdk-constructs-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.047906 neulabs-cdk-constructs-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   325919 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40775 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    38906 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.865791 neulabs-cdk-constructs-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.865791 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   326301 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    40775 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    41596 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-09 15:00:21.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:00:35.869792 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-09 15:00:35.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-09 15:00:35.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:00:35.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-09 15:00:35.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 15:00:35.000000 neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.3.0/LICENSE` & `neulabs-cdk-constructs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.0/PKG-INFO` & `neulabs-cdk-constructs-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.3.0
+Version: 0.3.1
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.3.0 Summary:
+Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.3.1 Summary:
 neulabs-cdk-constructs Home-page: https://github.com/neulabscom/neulabs-cdk-
 constructs.git Author: Neulabs
 neulabs.com> License: Apache-2.0 Project-URL: Source, https://github.com/
 neulabscom/neulabs-cdk-constructs.git Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: JavaScript Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `neulabs-cdk-constructs-0.3.0/README.md` & `neulabs-cdk-constructs-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.0/setup.py` & `neulabs-cdk-constructs-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.3.0",
+    "version": "0.3.1",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.3.0.jsii.tgz"
+            "neulabs-cdk-constructs@0.3.1.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.3.0",
+    "0.3.1",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.3.0.jsii.tgz",
+    "neulabs-cdk-constructs@0.3.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         github_repository: builtins.str,
         github_user: builtins.str,
         token_action: "TokenActions",
+        cdk_deploy_role_aws_managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
         cdk_deploy_role_managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
         cdk_deploy_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         token_action_custom: typing.Optional[builtins.str] = None,
         stage: builtins.str,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
@@ -49,14 +50,15 @@
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param github_repository: 
         :param github_user: 
         :param token_action: 
+        :param cdk_deploy_role_aws_managed_policies: 
         :param cdk_deploy_role_managed_policies: 
         :param cdk_deploy_role_policy_statements: 
         :param token_action_custom: 
         :param stage: 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
@@ -71,14 +73,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__71fabbd315f27662df384897235533205fa1984af573f69ade1128bc72da169d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = GithubOIDCStackStackProps(
             github_repository=github_repository,
             github_user=github_user,
             token_action=token_action,
+            cdk_deploy_role_aws_managed_policies=cdk_deploy_role_aws_managed_policies,
             cdk_deploy_role_managed_policies=cdk_deploy_role_managed_policies,
             cdk_deploy_role_policy_statements=cdk_deploy_role_policy_statements,
             token_action_custom=token_action_custom,
             stage=stage,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
@@ -96,25 +99,28 @@
     def create_cdk_bootstrap_role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
         return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.invoke(self, "createCdkBootstrapRole", []))
 
     @jsii.member(jsii_name="createCdkDeployRole")
     def create_cdk_deploy_role(
         self,
         managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
+        aws_managed_policy: typing.Optional[typing.Sequence[builtins.str]] = None,
         policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     ) -> _aws_cdk_aws_iam_ceddda9d.IRole:
         '''
         :param managed_policies: -
+        :param aws_managed_policy: -
         :param policy_statements: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__38a804dad69a7e88a361d5bccc16731b0a29b939ca83b1a6ef43cd272245e971)
             check_type(argname="argument managed_policies", value=managed_policies, expected_type=type_hints["managed_policies"])
+            check_type(argname="argument aws_managed_policy", value=aws_managed_policy, expected_type=type_hints["aws_managed_policy"])
             check_type(argname="argument policy_statements", value=policy_statements, expected_type=type_hints["policy_statements"])
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.invoke(self, "createCdkDeployRole", [managed_policies, policy_statements]))
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.invoke(self, "createCdkDeployRole", [managed_policies, aws_managed_policy, policy_statements]))
 
     @jsii.member(jsii_name="createOidcRole")
     def create_oidc_role(
         self,
         provider_url: builtins.str,
         token: builtins.str,
     ) -> _aws_cdk_aws_iam_ceddda9d.IRole:
@@ -219,14 +225,31 @@
     def token_action(self, value: "TokenActions") -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4bd4e27b23fafc5b18640f9f3bcb5f8d377178e9ee818017fc064e45c9ffe9cb)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tokenAction", value)
 
     @builtins.property
+    @jsii.member(jsii_name="cdkDeployRoleAwsManagedPolicies")
+    def cdk_deploy_role_aws_managed_policies(
+        self,
+    ) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "cdkDeployRoleAwsManagedPolicies"))
+
+    @cdk_deploy_role_aws_managed_policies.setter
+    def cdk_deploy_role_aws_managed_policies(
+        self,
+        value: typing.Optional[typing.List[builtins.str]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__118110011a00e54769ad26aae3f4147ce2a03b30a6a1767adf34ab290769ae94)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "cdkDeployRoleAwsManagedPolicies", value)
+
+    @builtins.property
     @jsii.member(jsii_name="cdkDeployRoleManagedPolicies")
     def cdk_deploy_role_managed_policies(
         self,
     ) -> typing.Optional[typing.List[builtins.str]]:
         return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "cdkDeployRoleManagedPolicies"))
 
     @cdk_deploy_role_managed_policies.setter
@@ -270,14 +293,15 @@
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "stage": "stage",
         "github_repository": "githubRepository",
         "github_user": "githubUser",
         "token_action": "tokenAction",
+        "cdk_deploy_role_aws_managed_policies": "cdkDeployRoleAwsManagedPolicies",
         "cdk_deploy_role_managed_policies": "cdkDeployRoleManagedPolicies",
         "cdk_deploy_role_policy_statements": "cdkDeployRolePolicyStatements",
         "token_action_custom": "tokenActionCustom",
     },
 )
 class GithubOIDCStackStackProps(_BaseStackProps_bfec638c):
     def __init__(
@@ -292,14 +316,15 @@
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         stage: builtins.str,
         github_repository: builtins.str,
         github_user: builtins.str,
         token_action: "TokenActions",
+        cdk_deploy_role_aws_managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
         cdk_deploy_role_managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
         cdk_deploy_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         token_action_custom: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
@@ -310,14 +335,15 @@
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param stage: 
         :param github_repository: 
         :param github_user: 
         :param token_action: 
+        :param cdk_deploy_role_aws_managed_policies: 
         :param cdk_deploy_role_managed_policies: 
         :param cdk_deploy_role_policy_statements: 
         :param token_action_custom: 
         '''
         if isinstance(env, dict):
             env = _aws_cdk_ceddda9d.Environment(**env)
         if __debug__:
@@ -331,14 +357,15 @@
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
             check_type(argname="argument github_repository", value=github_repository, expected_type=type_hints["github_repository"])
             check_type(argname="argument github_user", value=github_user, expected_type=type_hints["github_user"])
             check_type(argname="argument token_action", value=token_action, expected_type=type_hints["token_action"])
+            check_type(argname="argument cdk_deploy_role_aws_managed_policies", value=cdk_deploy_role_aws_managed_policies, expected_type=type_hints["cdk_deploy_role_aws_managed_policies"])
             check_type(argname="argument cdk_deploy_role_managed_policies", value=cdk_deploy_role_managed_policies, expected_type=type_hints["cdk_deploy_role_managed_policies"])
             check_type(argname="argument cdk_deploy_role_policy_statements", value=cdk_deploy_role_policy_statements, expected_type=type_hints["cdk_deploy_role_policy_statements"])
             check_type(argname="argument token_action_custom", value=token_action_custom, expected_type=type_hints["token_action_custom"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "stage": stage,
             "github_repository": github_repository,
             "github_user": github_user,
@@ -358,14 +385,16 @@
             self._values["stack_name"] = stack_name
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
+        if cdk_deploy_role_aws_managed_policies is not None:
+            self._values["cdk_deploy_role_aws_managed_policies"] = cdk_deploy_role_aws_managed_policies
         if cdk_deploy_role_managed_policies is not None:
             self._values["cdk_deploy_role_managed_policies"] = cdk_deploy_role_managed_policies
         if cdk_deploy_role_policy_statements is not None:
             self._values["cdk_deploy_role_policy_statements"] = cdk_deploy_role_policy_statements
         if token_action_custom is not None:
             self._values["token_action_custom"] = token_action_custom
 
@@ -552,14 +581,21 @@
     @builtins.property
     def token_action(self) -> "TokenActions":
         result = self._values.get("token_action")
         assert result is not None, "Required property 'token_action' is missing"
         return typing.cast("TokenActions", result)
 
     @builtins.property
+    def cdk_deploy_role_aws_managed_policies(
+        self,
+    ) -> typing.Optional[typing.List[builtins.str]]:
+        result = self._values.get("cdk_deploy_role_aws_managed_policies")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
     def cdk_deploy_role_managed_policies(
         self,
     ) -> typing.Optional[typing.List[builtins.str]]:
         result = self._values.get("cdk_deploy_role_managed_policies")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
@@ -611,14 +647,15 @@
 def _typecheckingstub__71fabbd315f27662df384897235533205fa1984af573f69ade1128bc72da169d(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     github_repository: builtins.str,
     github_user: builtins.str,
     token_action: TokenActions,
+    cdk_deploy_role_aws_managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
     cdk_deploy_role_managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
     cdk_deploy_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     token_action_custom: typing.Optional[builtins.str] = None,
     stage: builtins.str,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
@@ -630,14 +667,15 @@
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__38a804dad69a7e88a361d5bccc16731b0a29b939ca83b1a6ef43cd272245e971(
     managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
+    aws_managed_policy: typing.Optional[typing.Sequence[builtins.str]] = None,
     policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f3ff2f52a754bcc8ac66171d89cb70ca23ceedd5d32cd487bb12f17483fa9054(
     provider_url: builtins.str,
@@ -687,14 +725,20 @@
 
 def _typecheckingstub__4bd4e27b23fafc5b18640f9f3bcb5f8d377178e9ee818017fc064e45c9ffe9cb(
     value: TokenActions,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__118110011a00e54769ad26aae3f4147ce2a03b30a6a1767adf34ab290769ae94(
+    value: typing.Optional[typing.List[builtins.str]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__fb7c5799447871d7244ed8f819a93a50ee2bdf4efa6b5632a166e6328dcb9e42(
     value: typing.Optional[typing.List[builtins.str]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ee7947bb0d3c0b596daf1087e748fb7729130cd41bc163bb8d67823f75c6a075(
@@ -714,13 +758,14 @@
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
     stage: builtins.str,
     github_repository: builtins.str,
     github_user: builtins.str,
     token_action: TokenActions,
+    cdk_deploy_role_aws_managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
     cdk_deploy_role_managed_policies: typing.Optional[typing.Sequence[builtins.str]] = None,
     cdk_deploy_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     token_action_custom: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.3.0
+Version: 0.3.1
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.3.0 Summary:
+Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.3.1 Summary:
 neulabs-cdk-constructs Home-page: https://github.com/neulabscom/neulabs-cdk-
 constructs.git Author: Neulabs
 neulabs.com> License: Apache-2.0 Project-URL: Source, https://github.com/
 neulabscom/neulabs-cdk-constructs.git Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: JavaScript Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.3.1/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.0.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.1.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

