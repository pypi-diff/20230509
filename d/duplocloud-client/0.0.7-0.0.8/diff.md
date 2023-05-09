# Comparing `tmp/duplocloud-client-0.0.7.tar.gz` & `tmp/duplocloud-client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplocloud-client-0.0.7.tar", last modified: Wed Apr 26 23:16:31 2023, max compression
+gzip compressed data, was "duplocloud-client-0.0.8.tar", last modified: Tue May  9 17:24:38 2023, max compression
```

## Comparing `duplocloud-client-0.0.7.tar` & `duplocloud-client-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.751641 duplocloud-client-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-26 23:16:31.751641 duplocloud-client-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-26 23:16:31.751641 duplocloud-client-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/src/duplo_resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplo_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplo_resource/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplo_resource/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplo_resource/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/src/duplocloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.751641 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.238013 duplocloud-client-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.238013 duplocloud-client-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/src/duplo_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplo_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplo_resource/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplo_resource/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplo_resource/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/src/duplocloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/top_level.txt
```

### Comparing `duplocloud-client-0.0.7/.github/workflows/publish.yaml` & `duplocloud-client-0.0.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.7/.github/workflows/test.yml` & `duplocloud-client-0.0.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.7/CONTRIBUTING.md` & `duplocloud-client-0.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.7/PKG-INFO` & `duplocloud-client-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generic DuploClient for Python apps.
 Home-page: https://github.com/duplocloud/py-client
 Author: Kelly Ferrone
 Author-email: kelly@duplocloud.net
 Project-URL: Bug Tracker, https://github.com/duplocloud/py-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplocloud-client-0.0.7/setup.cfg` & `duplocloud-client-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.7/src/duplo_resource/service.py` & `duplocloud-client-0.0.8/src/duplo_resource/service.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.7/src/duplo_resource/tenant.py` & `duplocloud-client-0.0.8/src/duplo_resource/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-import datetime
 from duplocloud.client import DuploClient
 from duplocloud.resource import DuploResource
 from duplocloud.errors import DuploError
 
-class DuploTenant(DuploResource):
+class DuploUser(DuploResource):
   def __init__(self, duplo: DuploClient):
     super().__init__(duplo)
+    self.tenent_svc = duplo.service('tenant')
   
-  def list(self):
-    """Retrieve a list of all tenants in the Duplo system."""
-    return self.duplo.get("adminproxy/GetTenantNames")
+  def add_tenant(self, username, tenant):
+    """Retrieve a list of all users in the Duplo system."""
+    tenant_id = self.tenent_svc.find(tenant)["TenantId"]
+    res = self.duplo.post("admin/UpdateUserAccess", {
+      "Policy": { "IsReadOnly": None },
+      "Username": username,
+      "TenantId": tenant_id
+    })
+    # check http response is 204
+    if res.status_code != 204:
+      raise DuploError(f"Failed to add user '{username}' to tenant '{tenant}'", res["status_code"])
+    else:
+      return f"User '{username}' added to tenant '{tenant}'"
 
-  def find(self, tenant_name):
-    """Find a tenant by name."""
+  def find(self, username):
+    """Find a User by their username."""
     try:
-      return [t for t in self.list() if t["AccountName"] == tenant_name][0]
+      return [u for u in self.list() if u["Username"] == username][0]
     except IndexError:
-      raise DuploError(f"Tenant '{tenant_name}' not found", 404)
+      raise DuploError(f"User '{username}' not found", 404)
     
-  def shutdown(self, tenant_name, schedule=None):
-    """Expire a tenant."""
-    tenant = self.find(tenant_name)
-    tenant_id = tenant["TenantId"]
-
-    # if the schedule not specified then set the date 5 minute from now
-    if schedule is None:
-      now = datetime.datetime.now() + datetime.timedelta(minutes=5)
-      schedule = now.strftime("%a, %d %b %Y %H:%M:%S GMT")
-
-    res = self.duplo.post("adminproxy/UpdateTenantCleanupTimers", {
-      "TenantId": tenant_id,
-      "PauseTime": schedule
-    })
-
-    if res.status_code == 200:
-      return f"Tenant '{tenant_name}' will shutdown on {schedule}"
-    else:
-      raise DuploError(f"Failed to expire tenant '{tenant_name}'", res.status_code)
+  def list(self):
+    """Retrieve a list of all users in the Duplo system."""
+    return self.duplo.get("admin/GetAllUserRoles")
```

### Comparing `duplocloud-client-0.0.7/src/duplocloud/cli.py` & `duplocloud-client-0.0.8/src/duplocloud/cli.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.7/src/duplocloud/client.py` & `duplocloud-client-0.0.8/src/duplocloud/client.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.7/src/duplocloud/resource.py` & `duplocloud-client-0.0.8/src/duplocloud/resource.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.7/src/duplocloud_client.egg-info/PKG-INFO` & `duplocloud-client-0.0.8/src/duplocloud_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generic DuploClient for Python apps.
 Home-page: https://github.com/duplocloud/py-client
 Author: Kelly Ferrone
 Author-email: kelly@duplocloud.net
 Project-URL: Bug Tracker, https://github.com/duplocloud/py-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplocloud-client-0.0.7/src/duplocloud_client.egg-info/SOURCES.txt` & `duplocloud-client-0.0.8/src/duplocloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

