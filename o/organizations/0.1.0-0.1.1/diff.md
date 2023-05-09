# Comparing `tmp/organizations-0.1.0.tar.gz` & `tmp/organizations-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "organizations-0.1.0.tar", last modified: Wed May  3 12:35:01 2023, max compression
+gzip compressed data, was "organizations-0.1.1.tar", last modified: Mon May  8 08:23:24 2023, max compression
```

## Comparing `organizations-0.1.0.tar` & `organizations-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 12:35:01.060121 organizations-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-04-21 11:42:03.000000 organizations-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      434 2023-05-03 12:35:01.059123 organizations-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.0/README.md
--rw-rw-rw-   0        0        0     1083 2023-05-03 12:33:31.000000 organizations-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 12:35:01.061122 organizations-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 12:35:00.949126 organizations-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 12:35:00.993127 organizations-0.1.0/src/organizations/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/__init__.py
--rw-rw-rw-   0        0        0      664 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/abstractions.py
--rw-rw-rw-   0        0        0     5265 2023-05-03 11:22:44.000000 organizations-0.1.0/src/organizations/admin.py
--rw-rw-rw-   0        0        0      234 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:35:01.021122 organizations-0.1.0/src/organizations/did_factory/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/did_factory/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/did_factory/abstractions.py
--rw-rw-rw-   0        0        0      247 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/did_factory/context.py
--rw-rw-rw-   0        0        0      816 2023-04-27 10:52:27.000000 organizations-0.1.0/src/organizations/did_factory/factory.py
--rw-rw-rw-   0        0        0      173 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/did_factory/models.py
--rw-rw-rw-   0        0        0    11061 2023-05-03 09:53:36.000000 organizations-0.1.0/src/organizations/did_factory/strategy.py
--rw-rw-rw-   0        0        0      241 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/enums.py
--rw-rw-rw-   0        0        0      712 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:35:01.056123 organizations-0.1.0/src/organizations/migrations/
--rw-rw-rw-   0        0        0     4963 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      720 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0002_organization_networks.py
--rw-rw-rw-   0        0        0      673 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0003_alter_organization_networks.py
--rw-rw-rw-   0        0        0      867 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0004_alter_organization_email_and_more.py
--rw-rw-rw-   0        0        0     3698 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0005_subject_alter_organization_networks_and_more.py
--rw-rw-rw-   0        0        0     1767 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0006_alter_organization_networks_and_more.py
--rw-rw-rw-   0        0        0      431 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0007_alter_issuer_active.py
--rw-rw-rw-   0        0        0      569 2023-04-27 13:47:50.000000 organizations-0.1.0/src/organizations/migrations/0008_alter_organization_networks.py
--rw-rw-rw-   0        0        0      411 2023-05-02 15:49:34.000000 organizations-0.1.0/src/organizations/migrations/0009_issuer_name.py
--rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/__init__.py
--rw-rw-rw-   0        0        0     3613 2023-05-03 09:45:48.000000 organizations-0.1.0/src/organizations/models.py
--rw-rw-rw-   0        0        0     1104 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/serializers.py
--rw-rw-rw-   0        0        0     2391 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/service.py
--rw-rw-rw-   0        0        0     3293 2023-05-03 12:34:28.000000 organizations-0.1.0/src/organizations/signals.py
--rw-rw-rw-   0        0        0     2643 2023-05-03 12:34:37.000000 organizations-0.1.0/src/organizations/tasks.py
--rw-rw-rw-   0        0        0       63 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/tests.py
--rw-rw-rw-   0        0        0      282 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/urls.py
--rw-rw-rw-   0        0        0     2820 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/views.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:35:01.005121 organizations-0.1.0/src/organizations.egg-info/
--rw-rw-rw-   0        0        0      434 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1493 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      327 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 08:23:24.378190 organizations-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-21 11:42:03.000000 organizations-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      434 2023-05-08 08:23:24.376190 organizations-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1083 2023-05-08 06:41:33.000000 organizations-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 08:23:24.378190 organizations-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 08:23:24.174529 organizations-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 08:23:24.235526 organizations-0.1.1/src/organizations/
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/abstractions.py
+-rw-rw-rw-   0        0        0     5319 2023-05-03 12:36:12.000000 organizations-0.1.1/src/organizations/admin.py
+-rw-rw-rw-   0        0        0      234 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:23:24.271492 organizations-0.1.1/src/organizations/did_factory/
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/did_factory/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/did_factory/abstractions.py
+-rw-rw-rw-   0        0        0      247 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/did_factory/context.py
+-rw-rw-rw-   0        0        0      816 2023-04-27 10:52:27.000000 organizations-0.1.1/src/organizations/did_factory/factory.py
+-rw-rw-rw-   0        0        0      173 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/did_factory/models.py
+-rw-rw-rw-   0        0        0    11063 2023-05-03 12:36:13.000000 organizations-0.1.1/src/organizations/did_factory/strategy.py
+-rw-rw-rw-   0        0        0      241 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/enums.py
+-rw-rw-rw-   0        0        0      712 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:23:24.371195 organizations-0.1.1/src/organizations/migrations/
+-rw-rw-rw-   0        0        0     4963 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      720 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/migrations/0002_organization_networks.py
+-rw-rw-rw-   0        0        0      673 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/migrations/0003_alter_organization_networks.py
+-rw-rw-rw-   0        0        0      867 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/migrations/0004_alter_organization_email_and_more.py
+-rw-rw-rw-   0        0        0     3698 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/migrations/0005_subject_alter_organization_networks_and_more.py
+-rw-rw-rw-   0        0        0     1767 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/migrations/0006_alter_organization_networks_and_more.py
+-rw-rw-rw-   0        0        0      431 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/migrations/0007_alter_issuer_active.py
+-rw-rw-rw-   0        0        0      569 2023-04-27 13:47:50.000000 organizations-0.1.1/src/organizations/migrations/0008_alter_organization_networks.py
+-rw-rw-rw-   0        0        0      411 2023-05-02 15:49:34.000000 organizations-0.1.1/src/organizations/migrations/0009_issuer_name.py
+-rw-rw-rw-   0        0        0      403 2023-05-06 15:29:27.000000 organizations-0.1.1/src/organizations/migrations/0010_alter_organization_name.py
+-rw-rw-rw-   0        0        0      516 2023-05-08 08:22:55.000000 organizations-0.1.1/src/organizations/migrations/0011_issuer_did.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3709 2023-05-08 08:08:33.000000 organizations-0.1.1/src/organizations/models.py
+-rw-rw-rw-   0        0        0     1104 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/serializers.py
+-rw-rw-rw-   0        0        0     2391 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/service.py
+-rw-rw-rw-   0        0        0     3293 2023-05-03 12:34:28.000000 organizations-0.1.1/src/organizations/signals.py
+-rw-rw-rw-   0        0        0     2643 2023-05-03 12:34:37.000000 organizations-0.1.1/src/organizations/tasks.py
+-rw-rw-rw-   0        0        0       63 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/tests.py
+-rw-rw-rw-   0        0        0      282 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/urls.py
+-rw-rw-rw-   0        0        0     2820 2023-04-21 11:42:03.000000 organizations-0.1.1/src/organizations/views.py
+drwxrwxrwx   0        0        0        0 2023-05-08 08:23:24.251533 organizations-0.1.1/src/organizations.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-05-08 08:23:24.000000 organizations-0.1.1/src/organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2023-05-08 08:23:24.000000 organizations-0.1.1/src/organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 08:23:24.000000 organizations-0.1.1/src/organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      327 2023-05-08 08:23:24.000000 organizations-0.1.1/src/organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-08 08:23:24.000000 organizations-0.1.1/src/organizations.egg-info/top_level.txt
```

### Comparing `organizations-0.1.0/LICENSE` & `organizations-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/pyproject.toml` & `organizations-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "organizations"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Alejandro", email="agarrido@izertis.com" },
   { name="Iraia", email="iolabarrieta@izertis.com" },
 ]
 description = "A small organizations handler app for django"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `organizations-0.1.0/src/organizations/abstractions.py` & `organizations-0.1.1/src/organizations/abstractions.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/admin.py` & `organizations-0.1.1/src/organizations/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,30 +76,38 @@
             return {}
 
         return super(IntermediaryAdmin, self).get_model_perms(request)
 
 
 class OrganizationAdmin(admin.ModelAdmin):
     model = Organization
-    list_filter = ['networks']
-    search_fields = ['name', 'email', 'phone',]
-    
+    list_filter = ["networks"]
+    search_fields = [
+        "name",
+        "email",
+        "phone",
+    ]
+
     def get_model_perms(self, request):
 
         if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
             return {}
 
         return super(OrganizationAdmin, self).get_model_perms(request)
 
 
 class OrganizationDIDAdmin(admin.ModelAdmin):
     model = OrganizationDID
-    list_filter = ['network_name', 'organization']
-    search_fields = ['network_name', 'organization', 'did',]
-    
+    list_filter = ["network_name", "organization"]
+    search_fields = [
+        "network_name",
+        "organization",
+        "did",
+    ]
+
     def get_model_perms(self, request):
 
         if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
             return {}
 
         return super(OrganizationDIDAdmin, self).get_model_perms(request)
 
@@ -114,16 +122,15 @@
 
         return super(OrganizationKeysAdmin, self).get_model_perms(request)
 
 
 class IssuerAdmin(admin.ModelAdmin):
     model = Issuer
     readonly_fields = ["active"]
-    list_filter = ['organization']
-
+    list_filter = ["organization"]
 
     def get_model_perms(self, request):
 
         if (
             not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
             or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
             and not waffle.switch_is_active(
@@ -144,16 +151,16 @@
             return {}
 
         return super(UserProxyAdmin, self).get_model_perms(request)
 
 
 class OrganizationOnboardingNotificationAdmin(admin.ModelAdmin):
     model = OrganizationOnboardingNotification
-    list_filter = ['organization']
-    
+    list_filter = ["organization"]
+
     def get_model_perms(self, request):
 
         if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
             return {}
 
         return super(OrganizationOnboardingNotificationAdmin, self).get_model_perms(
             request
```

### Comparing `organizations-0.1.0/src/organizations/did_factory/abstractions.py` & `organizations-0.1.1/src/organizations/did_factory/abstractions.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/did_factory/factory.py` & `organizations-0.1.1/src/organizations/did_factory/factory.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/did_factory/strategy.py` & `organizations-0.1.1/src/organizations/did_factory/strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     AddKeyValidator,
     AddIdentityIssuerValidator,
     EidasLevelEnum,
 )
 from django.conf import settings
 from multiformats import multibase
 
+
 class AlastriaNetworkStrategy(ANetworkStrategy):
     def __init__(self, props: FactoryArgsModel):
         self.alastria_service_client: AlastriaAClinet = AlastriaClient(
             service_host=settings.ALASTRIA_SERVICE_HOST
         )
         self.props = props
         network_data = self.props.net
```

### Comparing `organizations-0.1.0/src/organizations/forms.py` & `organizations-0.1.1/src/organizations/forms.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/migrations/0001_initial.py` & `organizations-0.1.1/src/organizations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/migrations/0002_organization_networks.py` & `organizations-0.1.1/src/organizations/migrations/0002_organization_networks.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/migrations/0003_alter_organization_networks.py` & `organizations-0.1.1/src/organizations/migrations/0003_alter_organization_networks.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/migrations/0004_alter_organization_email_and_more.py` & `organizations-0.1.1/src/organizations/migrations/0004_alter_organization_email_and_more.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/migrations/0005_subject_alter_organization_networks_and_more.py` & `organizations-0.1.1/src/organizations/migrations/0005_subject_alter_organization_networks_and_more.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/migrations/0006_alter_organization_networks_and_more.py` & `organizations-0.1.1/src/organizations/migrations/0006_alter_organization_networks_and_more.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/migrations/0008_alter_organization_networks.py` & `organizations-0.1.1/src/organizations/migrations/0008_alter_organization_networks.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/models.py` & `organizations-0.1.1/src/organizations/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     def __str__(self) -> str:
         return f"{self.network_name} - {self.organization.name}"
 
 
 class Issuer(models.Model):
     name = models.CharField(max_length=2500, null=False, blank=True)
     organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
+    did = models.ForeignKey(OrganizationDID, on_delete=models.SET_NULL, blank=True, null=True)
     active = models.BooleanField(default=False)
 
     def __str__(self) -> str:
         return f"{self.name} - {self.organization.name}"
 
 
 class Intermediary(models.Model):
```

### Comparing `organizations-0.1.0/src/organizations/serializers.py` & `organizations-0.1.1/src/organizations/serializers.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/service.py` & `organizations-0.1.1/src/organizations/service.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/signals.py` & `organizations-0.1.1/src/organizations/signals.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/tasks.py` & `organizations-0.1.1/src/organizations/tasks.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations/views.py` & `organizations-0.1.1/src/organizations/views.py`

 * *Files identical despite different names*

### Comparing `organizations-0.1.0/src/organizations.egg-info/SOURCES.txt` & `organizations-0.1.1/src/organizations.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 src/organizations/migrations/0003_alter_organization_networks.py
 src/organizations/migrations/0004_alter_organization_email_and_more.py
 src/organizations/migrations/0005_subject_alter_organization_networks_and_more.py
 src/organizations/migrations/0006_alter_organization_networks_and_more.py
 src/organizations/migrations/0007_alter_issuer_active.py
 src/organizations/migrations/0008_alter_organization_networks.py
 src/organizations/migrations/0009_issuer_name.py
+src/organizations/migrations/0010_alter_organization_name.py
+src/organizations/migrations/0011_issuer_did.py
 src/organizations/migrations/__init__.py
```

