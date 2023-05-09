# Comparing `tmp/komora_syncer-2.2.tar.gz` & `tmp/komora_syncer-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komora_syncer-2.2.tar", last modified: Wed Sep  7 09:42:27 2022, max compression
+gzip compressed data, was "komora_syncer-2.3.tar", last modified: Tue May  9 06:50:22 2023, max compression
```

## Comparing `komora_syncer-2.2.tar` & `komora_syncer-2.3.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2022-09-07 09:42:27.252185 komora_syncer-2.2/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1378 2022-09-07 09:42:27.252185 komora_syncer-2.2/PKG-INFO
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      529 2022-04-28 10:08:08.000000 komora_syncer-2.2/README.md
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2022-09-07 09:42:27.252185 komora_syncer-2.2/komora_syncer/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       28 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/__init__.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     2664 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/__main__.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3162 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/config.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2022-09-07 09:42:27.252185 komora_syncer-2.2/komora_syncer/connections/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      713 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/connections/NetboxConnection.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/connections/__init__.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2022-09-07 09:42:27.252185 komora_syncer-2.2/komora_syncer/helpers/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/helpers/__init__.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      221 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/helpers/utils.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2022-09-07 09:42:27.252185 komora_syncer-2.2/komora_syncer/models/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     5827 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/Synchronizer.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/__init__.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2022-09-07 09:42:27.252185 komora_syncer-2.2/komora_syncer/models/komora/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     8194 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/KomoraApi.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/__init__.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      747 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/address.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     4500 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/contact.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1048 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/device.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      271 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/district.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      520 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/location.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      381 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/municipality.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1304 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/organization.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      171 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/region.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     2042 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/site.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      230 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/komora/site_contact.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2022-09-07 09:42:27.252185 komora_syncer-2.2/komora_syncer/models/netbox/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     4949 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/netbox/NbDevice.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3386 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/netbox/NbLocation.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3770 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/netbox/NbRegion.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     6052 2022-07-13 11:09:12.000000 komora_syncer-2.2/komora_syncer/models/netbox/NbSite.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3854 2022-07-13 11:09:12.000000 komora_syncer-2.2/komora_syncer/models/netbox/NbTenant.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      235 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/netbox/NetboxBase.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.2/komora_syncer/models/netbox/__init__.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2022-09-07 09:42:27.252185 komora_syncer-2.2/komora_syncer.egg-info/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1378 2022-09-07 09:42:27.000000 komora_syncer-2.2/komora_syncer.egg-info/PKG-INFO
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1338 2022-09-07 09:42:27.000000 komora_syncer-2.2/komora_syncer.egg-info/SOURCES.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        1 2022-09-07 09:42:27.000000 komora_syncer-2.2/komora_syncer.egg-info/dependency_links.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       62 2022-09-07 09:42:27.000000 komora_syncer-2.2/komora_syncer.egg-info/entry_points.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        1 2022-07-13 11:11:13.000000 komora_syncer-2.2/komora_syncer.egg-info/not-zip-safe
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       81 2022-09-07 09:42:27.000000 komora_syncer-2.2/komora_syncer.egg-info/requires.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       14 2022-09-07 09:42:27.000000 komora_syncer-2.2/komora_syncer.egg-info/top_level.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       38 2022-09-07 09:42:27.252185 komora_syncer-2.2/setup.cfg
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1853 2022-09-07 09:42:17.000000 komora_syncer-2.2/setup.py
+drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-09 06:50:22.161746 komora_syncer-2.3/
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1378 2023-05-09 06:50:22.161746 komora_syncer-2.3/PKG-INFO
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      529 2022-04-28 10:08:08.000000 komora_syncer-2.3/README.md
+drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-09 06:50:22.131746 komora_syncer-2.3/komora_syncer/
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       28 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/__init__.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     2664 2023-05-09 06:49:52.000000 komora_syncer-2.3/komora_syncer/__main__.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3162 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/config.py
+drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-09 06:50:22.131746 komora_syncer-2.3/komora_syncer/connections/
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      713 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/connections/NetboxConnection.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/connections/__init__.py
+drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-09 06:50:22.131746 komora_syncer-2.3/komora_syncer/helpers/
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/helpers/__init__.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      221 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/helpers/utils.py
+drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-09 06:50:22.131746 komora_syncer-2.3/komora_syncer/models/
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     5827 2023-05-09 06:49:52.000000 komora_syncer-2.3/komora_syncer/models/Synchronizer.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/__init__.py
+drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-09 06:50:22.151746 komora_syncer-2.3/komora_syncer/models/komora/
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     8478 2023-05-09 06:50:01.000000 komora_syncer-2.3/komora_syncer/models/komora/KomoraApi.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/__init__.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      747 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/address.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     4500 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/contact.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1048 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/device.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      271 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/district.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1329 2023-02-21 12:57:34.000000 komora_syncer-2.3/komora_syncer/models/komora/inventory.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      520 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/location.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      381 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/municipality.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1304 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/organization.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      171 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/region.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     2042 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/site.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      230 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/komora/site_contact.py
+drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-09 06:50:22.161746 komora_syncer-2.3/komora_syncer/models/netbox/
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     4949 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/netbox/NbDevice.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     6538 2023-05-03 12:57:12.000000 komora_syncer-2.3/komora_syncer/models/netbox/NbInventoryItem.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3386 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/netbox/NbLocation.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3770 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/netbox/NbRegion.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     6052 2022-07-13 11:09:12.000000 komora_syncer-2.3/komora_syncer/models/netbox/NbSite.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3854 2023-05-09 06:49:52.000000 komora_syncer-2.3/komora_syncer/models/netbox/NbTenant.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      235 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/netbox/NetboxBase.py
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.3/komora_syncer/models/netbox/__init__.py
+drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-09 06:50:22.131746 komora_syncer-2.3/komora_syncer.egg-info/
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1378 2023-05-09 06:50:22.000000 komora_syncer-2.3/komora_syncer.egg-info/PKG-INFO
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1426 2023-05-09 06:50:22.000000 komora_syncer-2.3/komora_syncer.egg-info/SOURCES.txt
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        1 2023-05-09 06:50:22.000000 komora_syncer-2.3/komora_syncer.egg-info/dependency_links.txt
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       62 2023-05-09 06:50:22.000000 komora_syncer-2.3/komora_syncer.egg-info/entry_points.txt
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        1 2022-07-13 11:11:13.000000 komora_syncer-2.3/komora_syncer.egg-info/not-zip-safe
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       81 2023-05-09 06:50:22.000000 komora_syncer-2.3/komora_syncer.egg-info/requires.txt
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       14 2023-05-09 06:50:22.000000 komora_syncer-2.3/komora_syncer.egg-info/top_level.txt
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       38 2023-05-09 06:50:22.161746 komora_syncer-2.3/setup.cfg
+-rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1853 2023-05-09 06:50:01.000000 komora_syncer-2.3/setup.py
```

### Comparing `komora_syncer-2.2/PKG-INFO` & `komora_syncer-2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komora_syncer
-Version: 2.2
+Version: 2.3
 Summary: Synchronize data between Komora and Netbox applications
 Home-page: https://gitlab.cesnet.cz/701/done/netbox_komora_syncer
 Author: Jan Krupa
 Author-email: jan.krupa@cesnet.cz
 License: UNKNOWN
 Keywords: netbox,komora
 Platform: UNKNOWN
```

### Comparing `komora_syncer-2.2/README.md` & `komora_syncer-2.3/README.md`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/__main__.py` & `komora_syncer-2.3/komora_syncer/__main__.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/config.py` & `komora_syncer-2.3/komora_syncer/config.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/connections/NetboxConnection.py` & `komora_syncer-2.3/komora_syncer/connections/NetboxConnection.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/Synchronizer.py` & `komora_syncer-2.3/komora_syncer/models/Synchronizer.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/komora/KomoraApi.py` & `komora_syncer-2.3/komora_syncer/models/komora/KomoraApi.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,15 +95,22 @@
         except Exception as e:
             logger.exception("Unable to poll organizations from Komora")
             logger.debug(f"URL: {url}")
             raise e
         else:
             response = response.json()
 
+        # TODO: unique cids
+        unique_cids = []
         for organization in response.get("data", []):
+            if organization['clientId'] not in unique_cids:
+                unique_cids.append(organization['clientId'])
+            else:
+                logger.critical(f"Duplicated CID: {organization}")
+                continue
             self.organizations.append(Organization(**organization))
 
         return self.organizations
 
     def get_regions(self):
         if self.regions:
             return self.regions
```

### Comparing `komora_syncer-2.2/komora_syncer/models/komora/address.py` & `komora_syncer-2.3/komora_syncer/models/komora/address.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/komora/contact.py` & `komora_syncer-2.3/komora_syncer/models/komora/contact.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/komora/device.py` & `komora_syncer-2.3/komora_syncer/models/komora/device.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/komora/location.py` & `komora_syncer-2.3/komora_syncer/models/komora/location.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/komora/organization.py` & `komora_syncer-2.3/komora_syncer/models/komora/organization.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/komora/site.py` & `komora_syncer-2.3/komora_syncer/models/komora/site.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/netbox/NbDevice.py` & `komora_syncer-2.3/komora_syncer/models/netbox/NbDevice.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/netbox/NbLocation.py` & `komora_syncer-2.3/komora_syncer/models/netbox/NbLocation.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/netbox/NbRegion.py` & `komora_syncer-2.3/komora_syncer/models/netbox/NbRegion.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/netbox/NbSite.py` & `komora_syncer-2.3/komora_syncer/models/netbox/NbSite.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer/models/netbox/NbTenant.py` & `komora_syncer-2.3/komora_syncer/models/netbox/NbTenant.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.2/komora_syncer.egg-info/PKG-INFO` & `komora_syncer-2.3/komora_syncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komora-syncer
-Version: 2.2
+Version: 2.3
 Summary: Synchronize data between Komora and Netbox applications
 Home-page: https://gitlab.cesnet.cz/701/done/netbox_komora_syncer
 Author: Jan Krupa
 Author-email: jan.krupa@cesnet.cz
 License: UNKNOWN
 Keywords: netbox,komora
 Platform: UNKNOWN
```

### Comparing `komora_syncer-2.2/komora_syncer.egg-info/SOURCES.txt` & `komora_syncer-2.3/komora_syncer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 komora_syncer/models/__init__.py
 komora_syncer/models/komora/KomoraApi.py
 komora_syncer/models/komora/__init__.py
 komora_syncer/models/komora/address.py
 komora_syncer/models/komora/contact.py
 komora_syncer/models/komora/device.py
 komora_syncer/models/komora/district.py
+komora_syncer/models/komora/inventory.py
 komora_syncer/models/komora/location.py
 komora_syncer/models/komora/municipality.py
 komora_syncer/models/komora/organization.py
 komora_syncer/models/komora/region.py
 komora_syncer/models/komora/site.py
 komora_syncer/models/komora/site_contact.py
 komora_syncer/models/netbox/NbDevice.py
+komora_syncer/models/netbox/NbInventoryItem.py
 komora_syncer/models/netbox/NbLocation.py
 komora_syncer/models/netbox/NbRegion.py
 komora_syncer/models/netbox/NbSite.py
 komora_syncer/models/netbox/NbTenant.py
 komora_syncer/models/netbox/NetboxBase.py
 komora_syncer/models/netbox/__init__.py
```

### Comparing `komora_syncer-2.2/setup.py` & `komora_syncer-2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
       include_package_data=True,
       keywords="netbox,komora",
       packages=find_packages(),
       setup_requires=setup_requirements,
       test_suite="tests",
       tests_require=test_requirements,
       url="https://gitlab.cesnet.cz/701/done/netbox_komora_syncer",
-      version='2.2',
+      version='2.3',
       zip_safe=False,
       python_requires='>=3.6, <4',
       entry_points={
           'console_scripts': [
             'komora_syncer=komora_syncer.__main__:cli',
             ]
       },
```

