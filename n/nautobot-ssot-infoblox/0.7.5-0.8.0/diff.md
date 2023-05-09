# Comparing `tmp/nautobot_ssot_infoblox-0.7.5.tar.gz` & `tmp/nautobot_ssot_infoblox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_ssot_infoblox-0.7.5.tar", max compression
+gzip compressed data, was "nautobot_ssot_infoblox-0.8.0.tar", max compression
```

## Comparing `nautobot_ssot_infoblox-0.7.5.tar` & `nautobot_ssot_infoblox-0.8.0.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0      591 2022-12-01 15:23:35.239800 nautobot_ssot_infoblox-0.7.5/LICENSE
--rw-r--r--   0        0        0    11632 2022-12-01 15:23:35.239800 nautobot_ssot_infoblox-0.7.5/README.md
--rw-r--r--   0        0        0     1340 2022-12-01 15:23:35.247800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/__init__.py
--rw-r--r--   0        0        0      218 2022-12-01 15:23:35.247800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/constant.py
--rw-r--r--   0        0        0       65 2022-12-01 15:23:35.247800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/__init__.py
--rw-r--r--   0        0        0       86 2022-12-01 15:23:35.247800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/adapters/__init__.py
--rw-r--r--   0        0        0     7464 2022-12-01 15:23:35.247800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/adapters/infoblox.py
--rw-r--r--   0        0        0    13101 2022-12-01 15:23:35.247800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/adapters/nautobot.py
--rw-r--r--   0        0        0      519 2022-12-01 15:23:35.247800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/models/__init__.py
--rw-r--r--   0        0        0     1911 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/models/base.py
--rw-r--r--   0        0        0     4312 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/models/infoblox.py
--rw-r--r--   0        0        0    17080 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/models/nautobot.py
--rw-r--r--   0        0        0     5977 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/jobs.py
--rw-r--r--   0        0        0     2430 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/signals.py
--rw-r--r--   0        0        0     9530 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/static/nautobot_ssot_infoblox/infoblox_logo.png
--rw-r--r--   0        0        0       52 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/__init__.py
--rw-r--r--   0        0        0      190 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/create_a_record.json
--rw-r--r--   0        0        0      155 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/create_host_record.json
--rw-r--r--   0        0        0      254 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/create_ptr_record.json
--rw-r--r--   0        0        0      168 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/find_network_reference.json
--rw-r--r--   0        0        0       43 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/find_next_available_ip.json
--rw-r--r--   0        0        0      305 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_a_record_by_ip.json
--rw-r--r--   0        0        0      306 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_a_record_by_name.json
--rw-r--r--   0        0        0      378 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_dns_views.json
--rw-r--r--   0        0        0     1050 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks.json
--rw-r--r--   0        0        0      505 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_bulk.json
--rw-r--r--   0        0        0   500490 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_large.json
--rw-r--r--   0        0        0     4274 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_medium.json
--rw-r--r--   0        0        0      447 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_subnets.json
--rw-r--r--   0        0        0     1281 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_authoritative_zone.json
--rw-r--r--   0        0        0      257 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_dhcp_lease_from_hostname.json
--rw-r--r--   0        0        0      283 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_dhcp_lease_from_ipv4.json
--rw-r--r--   0        0        0      716 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_host_by_ip.json
--rw-r--r--   0        0        0      716 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_host_record_by_name.json
--rw-r--r--   0        0        0      256 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_ptr_record_by_name.json
--rw-r--r--   0        0        0      891 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/search_ipv4_address.json
--rw-r--r--   0        0        0     3748 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures_infoblox.py
--rw-r--r--   0        0        0    25365 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/test_client.py
--rw-r--r--   0        0        0      994 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/test_utils.py
--rw-r--r--   0        0        0      121 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/urls.py
--rw-r--r--   0        0        0       64 2022-12-01 15:23:35.251800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/utils/__init__.py
--rw-r--r--   0        0        0    43765 2022-12-01 15:23:35.255800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/utils/client.py
--rw-r--r--   0        0        0     2813 2022-12-01 15:23:35.255800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/utils/diffsync.py
--rw-r--r--   0        0        0     1157 2022-12-01 15:23:35.255800 nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/utils/nautobot.py
--rw-r--r--   0        0        0     3053 2022-12-01 15:23:49.724058 nautobot_ssot_infoblox-0.7.5/pyproject.toml
--rw-r--r--   0        0        0    12924 1970-01-01 00:00:00.000000 nautobot_ssot_infoblox-0.7.5/setup.py
--rw-r--r--   0        0        0    12566 1970-01-01 00:00:00.000000 nautobot_ssot_infoblox-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-09 15:31:04.357519 nautobot_ssot_infoblox-0.8.0/LICENSE
+-rw-r--r--   0        0        0    12478 2023-05-09 15:31:04.357519 nautobot_ssot_infoblox-0.8.0/README.md
+-rw-r--r--   0        0        0     1338 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/__init__.py
+-rw-r--r--   0        0        0      218 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/constant.py
+-rw-r--r--   0        0        0       65 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/__init__.py
+-rw-r--r--   0        0        0       86 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/adapters/__init__.py
+-rw-r--r--   0        0        0     8102 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/adapters/infoblox.py
+-rw-r--r--   0        0        0    13101 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/adapters/nautobot.py
+-rw-r--r--   0        0        0      519 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/models/__init__.py
+-rw-r--r--   0        0        0     1911 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/models/base.py
+-rw-r--r--   0        0        0     4312 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/models/infoblox.py
+-rw-r--r--   0        0        0    17110 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/models/nautobot.py
+-rw-r--r--   0        0        0     5977 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/jobs.py
+-rw-r--r--   0        0        0     2430 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/signals.py
+-rw-r--r--   0        0        0     9530 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/static/nautobot_ssot_infoblox/infoblox_logo.png
+-rw-r--r--   0        0        0       52 2023-05-09 15:31:04.365519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/create_a_record.json
+-rw-r--r--   0        0        0      155 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/create_host_record.json
+-rw-r--r--   0        0        0      254 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/create_ptr_record.json
+-rw-r--r--   0        0        0      168 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/find_network_reference.json
+-rw-r--r--   0        0        0       43 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/find_next_available_ip.json
+-rw-r--r--   0        0        0      305 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_a_record_by_ip.json
+-rw-r--r--   0        0        0      306 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_a_record_by_name.json
+-rw-r--r--   0        0        0      378 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_dns_views.json
+-rw-r--r--   0        0        0     1050 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks.json
+-rw-r--r--   0        0        0      505 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_bulk.json
+-rw-r--r--   0        0        0   500490 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_large.json
+-rw-r--r--   0        0        0     4274 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_medium.json
+-rw-r--r--   0        0        0      447 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_subnets.json
+-rw-r--r--   0        0        0     1281 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_authoritative_zone.json
+-rw-r--r--   0        0        0      257 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_dhcp_lease_from_hostname.json
+-rw-r--r--   0        0        0      283 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_dhcp_lease_from_ipv4.json
+-rw-r--r--   0        0        0      716 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_host_by_ip.json
+-rw-r--r--   0        0        0      716 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_host_record_by_name.json
+-rw-r--r--   0        0        0      256 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_ptr_record_by_name.json
+-rw-r--r--   0        0        0      891 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/search_ipv4_address.json
+-rw-r--r--   0        0        0     3748 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures_infoblox.py
+-rw-r--r--   0        0        0    25362 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/test_client.py
+-rw-r--r--   0        0        0      994 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/test_utils.py
+-rw-r--r--   0        0        0      121 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/urls.py
+-rw-r--r--   0        0        0       64 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/utils/__init__.py
+-rw-r--r--   0        0        0    43765 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/utils/client.py
+-rw-r--r--   0        0        0     2813 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/utils/diffsync.py
+-rw-r--r--   0        0        0     1157 2023-05-09 15:31:04.369519 nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/utils/nautobot.py
+-rw-r--r--   0        0        0     3268 2023-05-09 15:31:18.193499 nautobot_ssot_infoblox-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13429 1970-01-01 00:00:00.000000 nautobot_ssot_infoblox-0.8.0/PKG-INFO
```

### Comparing `nautobot_ssot_infoblox-0.7.5/LICENSE` & `nautobot_ssot_infoblox-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/README.md` & `nautobot_ssot_infoblox-0.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 | NAUTOBOT_INFOBLOX_URL             | N/A     | URL of the Infoblox instance to sync with.                             |
 | NAUTOBOT_INFOBLOX_USERNAME        | N/A     | The username to authenticate against Infoblox with.                    |
 | NAUTOBOT_INFOBLOX_PASSWORD        | N/A     | The password to authenticate against Infblox with.                     |
 | NAUTOBOT_INFOBLOX_VERIFY_SSL      | True    | Toggle SSL verification when syncing data with Infoblox.               |
 | NAUTOBOT_INFOBLOX_WAPI_VERSION    | v2.12   | The version of the Infoblox API.                                       |
 | enable_sync_to_infoblox           | False   | Add job to sync data from Nautobot into Infoblox.                      |
 | enable_rfc1918_network_containers | False   | Add job to sync network containers to Nautobot (top level aggregates). |
+| default_status                    | active  | Default Status to be assigned to imported objects.                     |
+| infoblox_import_objects           | True    | Dictionary with keys for each import object and the value define import.|
+| infoblox_import_subnets           | N/A     | List of Subnets in CIDR string notation to filter import to.           |
 
 ### Configuration Example
 
 ```python
 PLUGINS_CONFIG = {
     "nautobot_ssot": {
         "hide_example_jobs": True,  # defaults to False if unspecified
@@ -50,14 +53,22 @@
         "NAUTOBOT_INFOBLOX_URL": os.getenv("NAUTOBOT_INFOBLOX_URL", ""),
         "NAUTOBOT_INFOBLOX_USERNAME": os.getenv("NAUTOBOT_INFOBLOX_USERNAME", ""),
         "NAUTOBOT_INFOBLOX_PASSWORD": os.getenv("NAUTOBOT_INFOBLOX_PASSWORD", ""),
         "NAUTOBOT_INFOBLOX_VERIFY_SSL": os.getenv("NAUTOBOT_INFOBLOX_VERIFY_SSL", "true"),
         "NAUTOBOT_INFOBLOX_WAPI_VERSION": os.getenv("NAUTOBOT_INFOBLOX_WAPI_VERSION", "v2.12"),
         "enable_sync_to_infoblox": False,
         "enable_rfc1918_network_containers": False,
+        "default_status": "active",
+        "infoblox_import_objects": {
+            "vlan_views": os.getenv("NAUTOBOT_INFOBLOX_IMPORT_VLAN_VIEWS", True),
+            "vlans": os.getenv("NAUTOBOT_INFOBLOX_IMPORT_VLANS", True),
+            "subnets": os.getenv("NAUTOBOT_INFOBLOX_INFOBLOX_IMPORT_SUBNETS", True),
+            "ip_addresses": os.getenv("NAUTOBOT_INFOBLOX_IMPORT_IP_ADDRESSES", True),
+        },
+        "infoblox_import_subnets": ["10.46.128.0/18", "192.168.1.0/24"],
     }
 }
 ```
 
 ## DiffSync Models
 
 Below are the data mappings between objects within Infoblox and the corresponding objects within Nautobot:
```

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/__init__.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """Plugin declaration for nautobot_ssot_infoblox."""
 # Metadata is inherited from Nautobot. If not including Nautobot in the environment, this should be added
 try:
     from importlib import metadata
 except ImportError:
     # Python version < 3.8
     import importlib_metadata as metadata
-
-__version__ = metadata.version(__name__)
-
 from nautobot.core.signals import nautobot_database_ready
 from nautobot.extras.plugins import PluginConfig
-
 from nautobot_ssot_infoblox.signals import nautobot_database_ready_callback
 
+__version__ = metadata.version(__name__)
+
 
 class NautobotSSoTInfobloxConfig(PluginConfig):
     """Plugin configuration for the nautobot_ssot_infoblox plugin."""
 
     name = "nautobot_ssot_infoblox"
     verbose_name = "Nautobot SSoT Infoblox"
     version = __version__
     author = "Network to Code, LLC"
     description = "Nautobot SSoT Infoblox."
     base_url = "ssot-infoblox"
     required_settings = []
-    min_version = "1.2.0"
+    min_version = "1.4.0"
     max_version = "1.9999"
     default_settings = {
         "enable_sync_to_infoblox": False,
         "enable_rfc1918_network_containers": False,
     }
     caching_config = {}
```

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/adapters/infoblox.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/adapters/infoblox.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Infoblox Adapter for Infoblox integration with SSoT plugin."""
 import ipaddress
 import re
 
 from diffsync import DiffSync
 from diffsync.enum import DiffSyncFlags
 from nautobot.extras.plugins.exceptions import PluginImproperlyConfigured
+from nautobot_ssot_infoblox.constant import PLUGIN_CFG
 from nautobot_ssot_infoblox.utils.client import get_default_ext_attrs, get_dns_name
 from nautobot_ssot_infoblox.utils.diffsync import get_ext_attr_dict, build_vlan_map
 from nautobot_ssot_infoblox.diffsync.models.infoblox import (
     InfobloxAggregate,
     InfobloxIPAddress,
     InfobloxNetwork,
     InfobloxVLANView,
@@ -44,19 +45,25 @@
             self.job.log_failure(
                 message="Improperly configured settings for communicating to Infoblox. Please validate accuracy."
             )
             raise PluginImproperlyConfigured
 
     def load_prefixes(self):
         """Load InfobloxNetwork DiffSync model."""
-        # Need to load containers here to prevent duplicates when syncing back to Infoblox
-        containers = self.conn.get_network_containers()
-        subnets = self.conn.get_all_subnets()
+        if PLUGIN_CFG.get("import_subnets"):
+            subnets = []
+            for prefix in PLUGIN_CFG["import_subnets"]:
+                subnets.extend(self.conn.get_all_subnets(prefix=prefix))
+            all_networks = subnets
+        else:
+            # Need to load containers here to prevent duplicates when syncing back to Infoblox
+            containers = self.conn.get_network_containers()
+            subnets = self.conn.get_all_subnets()
+            all_networks = containers + subnets
         self.subnets = [(x["network"], x["network_view"]) for x in subnets]
-        all_networks = containers + subnets
         default_ext_attrs = get_default_ext_attrs(review_list=all_networks)
         for _pf in all_networks:
             pf_ext_attrs = get_ext_attr_dict(extattrs=_pf.get("extattrs", {}))
             new_pf = self.prefix(
                 network=_pf["network"],
                 description=_pf.get("comment", ""),
                 status=_pf.get("status", "active"),
@@ -114,26 +121,34 @@
                 description=_vlan["comment"] if _vlan.get("comment") else "",
                 ext_attrs={**default_ext_attrs, **vlan_ext_attrs},
             )
             self.add(new_vlan)
 
     def load(self):
         """Load all models by calling other methods."""
-        self.load_prefixes()
-        if "prefix" in self.dict():
-            self.job.log(message=f"Loaded {len(self.dict()['prefix'])} prefixes from Infoblox.")
-        self.load_ipaddresses()
-        if "ipaddress" in self.dict():
-            self.job.log(message=f"Loaded {len(self.dict()['ipaddress'])} IP addresses from Infoblox.")
-        self.load_vlanviews()
-        if "vlangroup" in self.dict():
-            self.job.log(message=f"Loaded {len(self.dict()['vlangroup'])} VLAN views from Infoblox.")
-        self.load_vlans()
-        if "vlan" in self.dict():
-            self.job.log(message=f"Loaded {len(self.dict()['vlan'])} VLANs from Infoblox.")
+        if "infoblox_import_objects" in PLUGIN_CFG:
+            if PLUGIN_CFG["infoblox_import_objects"].get("subnets"):
+                self.load_prefixes()
+            if PLUGIN_CFG["infoblox_import_objects"].get("ip_addresses"):
+                self.load_ipaddresses()
+            if PLUGIN_CFG["infoblox_import_objects"].get("vlan_views"):
+                self.load_vlanviews()
+            if PLUGIN_CFG["infoblox_import_objects"].get("vlans"):
+                self.load_vlans()
+        else:
+            self.job.log_info(
+                message="The `infoblox_import_objects` setting was not found so all objects will be imported."
+            )
+            self.load_prefixes()
+            self.load_ipaddresses()
+            self.load_vlanviews()
+            self.load_vlans()
+        for obj in ["prefix", "ipaddress", "vlangroup", "vlan"]:
+            if obj in self.dict():
+                self.job.log(message=f"Loaded {len(self.dict()[obj])} {obj} from Infoblox.")
 
     def sync_complete(self, source, diff, flags=DiffSyncFlags.NONE, logger=None):
         """Add tags and custom fields to synced objects."""
         source.tag_involved_objects(target=self)
 
 
 class InfobloxAggregateAdapter(DiffSync):
```

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/adapters/nautobot.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/adapters/nautobot.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/models/__init__.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/models/base.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/models/base.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/models/infoblox.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/models/infoblox.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/diffsync/models/nautobot.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/diffsync/models/nautobot.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,16 @@
                 try:
                     obj.tenant = diffsync.tenant_map[attr_value]
                 except KeyError as err:
                     diffsync.job.log_warning(
                         message=f"Unable to find Tenant {attr_value} for {obj} found in Extensibility Attributes '{attr}'. {err}"
                     )
             _cf_dict = {
-                "name": slugify(attr),
+                "name": attr,
+                "slug": slugify(attr),
                 "type": CustomFieldTypeChoices.TYPE_TEXT,
                 "label": attr,
             }
             field, _ = OrmCF.objects.get_or_create(name=_cf_dict["name"], defaults=_cf_dict)
             field.content_types.add(ContentType.objects.get_for_model(type(obj)).id)
             obj.custom_field_data.update({_cf_dict["name"]: str(attr_value)})
```

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/jobs.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/signals.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/static/nautobot_ssot_infoblox/infoblox_logo.png` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/static/nautobot_ssot_infoblox/infoblox_logo.png`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks.json` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_large.json` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_large.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_medium.json` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_all_ipv4address_networks_medium.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_authoritative_zone.json` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_authoritative_zone.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_host_by_ip.json` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_host_by_ip.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/get_host_record_by_name.json` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/get_host_record_by_name.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures/search_ipv4_address.json` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures/search_ipv4_address.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/fixtures_infoblox.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/fixtures_infoblox.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/test_client.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,14 @@
             req.get(f"{LOCALHOST}/{mock_uri}", json=mock_response, status_code=404)
             with pytest.raises(HTTPError) as err:
                 self.infoblox_client.get_authoritative_zone()
 
         self.assertEqual(err.value.response.status_code, 404)
 
     def test_create_ptr_record_success(self):
-
         mock_uri = "record:ptr"
         mock_fqdn = "test-device.test-site"
         mock_ip_address = "10.1.1.1"
 
         mock_response = create_ptr_record()
         with requests_mock.Mocker() as req:
             req.post(f"{LOCALHOST}/{mock_uri}", json=mock_response, status_code=200)
@@ -430,15 +429,14 @@
 
             with pytest.raises(HTTPError) as err:
                 self.infoblox_client.create_ptr_record(mock_fqdn, mock_ip_address)
 
         self.assertEqual(err.value.response.status_code, 404)
 
     def test_create_a_record_success(self):
-
         mock_uri = "record:a"
         mock_fqdn = "test-device.test-site"
         mock_ip_address = "10.1.1.1"
 
         mock_response = create_a_record()
         with requests_mock.Mocker() as req:
             req.post(f"{LOCALHOST}/{mock_uri}", json=mock_response, status_code=200)
@@ -457,15 +455,14 @@
 
             with pytest.raises(HTTPError) as err:
                 self.infoblox_client.create_a_record(mock_fqdn, mock_ip_address)
 
         self.assertEqual(err.value.response.status_code, 404)
 
     def test_create_host_record_success(self):
-
         mock_uri = "record:host"
         mock_fqdn = "test-device.test-site"
         mock_ip_address = "10.1.1.1"
 
         mock_response = create_host_record()
         with requests_mock.Mocker() as req:
             req.post(f"{LOCALHOST}/{mock_uri}", json=mock_response, status_code=200)
```

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/tests/test_utils.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/utils/client.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/utils/client.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/utils/diffsync.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/utils/diffsync.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/nautobot_ssot_infoblox/utils/nautobot.py` & `nautobot_ssot_infoblox-0.8.0/nautobot_ssot_infoblox/utils/nautobot.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_infoblox-0.7.5/pyproject.toml` & `nautobot_ssot_infoblox-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-ssot-infoblox"
-version = "v0.7.5"
+version = "v0.8.0"
 description = "Nautobot SSoT Infoblox"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/networktocode-llc/nautobot-plugin-ssot-infoblox"
 repository = "https://github.com/networktocode-llc/nautobot-plugin-ssot-infoblox"
 keywords = ["nautobot", "nautobot-plugin"]
@@ -14,25 +14,27 @@
 ]
 packages = [
     { include = "nautobot_ssot_infoblox" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-nautobot = "*"
 dnspython = "^2.1.0"
 nautobot-ssot = "^1.1.0"
+nautobot = "^1.4.0"
 
 [tool.poetry.dev-dependencies]
 bandit = "*"
 black = "*"
 coverage = "*"
 django-debug-toolbar = "*"
 django-extensions = "*"
-flake8 = "*"
+# we need to pin flake8 because of package dependencies that cause it to downgrade and
+# therefore cause issues with linting since older versions do not take .flake8 as config
+flake8 = "^3.9.2"
 invoke = "*"
 ipython = "*"
 mkdocs = "*"
 pydocstyle = "*"
 pylint = "*"
 pylint-django = "*"
 pytest = "*"
@@ -118,7 +120,8 @@
 major_on_zero = true
 branch = "main"
 upload_to_repository = false
 upload_to_release = false
 changelog_file = "CHANGELOG.md"
 build_command = false
 version_source = "tag"
+commit_version_number = true
```

### Comparing `nautobot_ssot_infoblox-0.7.5/setup.py` & `nautobot_ssot_infoblox-0.8.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,264 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nautobot-ssot-infoblox
+Version: 0.8.0
+Summary: Nautobot SSoT Infoblox
+Home-page: https://github.com/networktocode-llc/nautobot-plugin-ssot-infoblox
+License: Apache-2.0
+Keywords: nautobot,nautobot-plugin
+Author: Network to Code, LLC
+Author-email: info@networktocode.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dnspython (>=2.1.0,<3.0.0)
+Requires-Dist: nautobot (>=1.4.0,<2.0.0)
+Requires-Dist: nautobot-ssot (>=1.1.0,<2.0.0)
+Project-URL: Repository, https://github.com/networktocode-llc/nautobot-plugin-ssot-infoblox
+Description-Content-Type: text/markdown
 
-packages = \
-['nautobot_ssot_infoblox',
- 'nautobot_ssot_infoblox.diffsync',
- 'nautobot_ssot_infoblox.diffsync.adapters',
- 'nautobot_ssot_infoblox.diffsync.models',
- 'nautobot_ssot_infoblox.tests',
- 'nautobot_ssot_infoblox.utils']
-
-package_data = \
-{'': ['*'],
- 'nautobot_ssot_infoblox': ['static/nautobot_ssot_infoblox/*'],
- 'nautobot_ssot_infoblox.tests': ['fixtures/*']}
-
-install_requires = \
-['dnspython>=2.1.0,<3.0.0', 'nautobot', 'nautobot-ssot>=1.1.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'nautobot-ssot-infoblox',
-    'version': '0.7.5',
-    'description': 'Nautobot SSoT Infoblox',
-    'long_description': '# Nautobot SSoT Infoblox\n\nUsing the [Nautobot SSoT](https://github.com/nautobot/nautobot-plugin-ssot) framework, the SSoT plugin for Infoblox allows for synchronizing of IP network and VLAN data between [Infoblox](https://infoblox.com/) and [Nautobot](https://github.com/nautobot/nautobot).\n\n## Installation\n\nThe plugin is available as a Python package in PyPi and can be installed with pip.\n\n```shell\npip install nautobot-ssot-infoblox\n```\n\n> The plugin is compatible with Nautobot 1.2.0 and higher\n\nTo ensure Nautobot SSoT Infoblox is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the Nautobot root directory (alongside `requirements.txt`) and list the `nautobot-ssot-infoblox` package:\n\n```no-highlight\n# echo nautobot-ssot-infoblox >> local_requirements.txt\n```\n\nOnce installed, the plugin needs to be enabled in your `nautobot_config.py`\n\n```python\n# In your nautobot_config.py\nPLUGINS = ["nautobot_ssot", "nautobot_ssot_infoblox"]\n```\n\nSee the section below for configuration settings.\n\n## Configuration\n\n| Setting                           | Default | Description                                                            |\n| --------------------------------- | ------- | ---------------------------------------------------------------------- |\n| NAUTOBOT_INFOBLOX_URL             | N/A     | URL of the Infoblox instance to sync with.                             |\n| NAUTOBOT_INFOBLOX_USERNAME        | N/A     | The username to authenticate against Infoblox with.                    |\n| NAUTOBOT_INFOBLOX_PASSWORD        | N/A     | The password to authenticate against Infblox with.                     |\n| NAUTOBOT_INFOBLOX_VERIFY_SSL      | True    | Toggle SSL verification when syncing data with Infoblox.               |\n| NAUTOBOT_INFOBLOX_WAPI_VERSION    | v2.12   | The version of the Infoblox API.                                       |\n| enable_sync_to_infoblox           | False   | Add job to sync data from Nautobot into Infoblox.                      |\n| enable_rfc1918_network_containers | False   | Add job to sync network containers to Nautobot (top level aggregates). |\n\n### Configuration Example\n\n```python\nPLUGINS_CONFIG = {\n    "nautobot_ssot": {\n        "hide_example_jobs": True,  # defaults to False if unspecified\n    }\n    "nautobot_ssot_infoblox": {\n        "NAUTOBOT_INFOBLOX_URL": os.getenv("NAUTOBOT_INFOBLOX_URL", ""),\n        "NAUTOBOT_INFOBLOX_USERNAME": os.getenv("NAUTOBOT_INFOBLOX_USERNAME", ""),\n        "NAUTOBOT_INFOBLOX_PASSWORD": os.getenv("NAUTOBOT_INFOBLOX_PASSWORD", ""),\n        "NAUTOBOT_INFOBLOX_VERIFY_SSL": os.getenv("NAUTOBOT_INFOBLOX_VERIFY_SSL", "true"),\n        "NAUTOBOT_INFOBLOX_WAPI_VERSION": os.getenv("NAUTOBOT_INFOBLOX_WAPI_VERSION", "v2.12"),\n        "enable_sync_to_infoblox": False,\n        "enable_rfc1918_network_containers": False,\n    }\n}\n```\n\n## DiffSync Models\n\nBelow are the data mappings between objects within Infoblox and the corresponding objects within Nautobot:\n\n| Infoblox          | Nautobot       |\n| ----------------- | -------------- |\n| Network           | Prefix         |\n| IP Address        | IP Address     |\n| VLAN              | VLAN           |\n| VLAN view         | VLAN Group     |\n| Network container | Aggregate      |\n| Extensibility Attrs | Custom Fields |\n\nNOTE - More information about Extensibility Attributes can be found in the [project documentation](#project-documentation).\n\n### DiffSyncModel - Network\n\n![Diffsync Model - Network](./docs/static/diffsyncmodel-network.png)\n\n### DiffSyncModel - IPAddress\n\n![Diffsync Model - IPAddress](./docs/static/diffsyncmodel-ipaddress.png)\n\n### DiffSyncModel - Aggregate\n\n![Diffsync Model - Aggregate](./docs/static/diffsyncmodel-aggregate.png)\n\n## Contributing\n\nPull requests are welcomed and automatically built and tested against multiple version of Python and multiple version of Nautobot through GitHub Actions.\n\nThe project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within GitHub Actions.\n\nThe project is following Network to Code software development guideline and is leveraging:\n\n- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.\n- Django unit test to ensure the plugin is working properly.\n\n### Development Environment\n\nThe development environment can be used in 2 ways. First, with a local poetry environment if you wish to develop outside of Docker with the caveat of using external services provided by Docker for PostgresQL and Redis. Second, all services are spun up using Docker and a local mount so you can develop locally, but Nautobot is spun up within the Docker container.\n\nBelow is a quick start guide if you\'re already familiar with the development environment provided, but if you\'re not familiar, please read the [Getting Started Guide](GETTING_STARTED.md).\n\n#### Invoke\n\nThe [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters which can be passed to PyInvoke to override the default configuration:\n\n- `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: 1.1.4)\n- `project_name`: the default docker compose project name (default: nautobot_ssot_infoblox)\n- `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.6)\n- `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)\n- `compose_dir`: the full path to a directory containing the project compose files\n- `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)\n\nUsing **PyInvoke** these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_NAUTOBOT_SSOT_INFOBLOX_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a yaml file.  There is an example `invoke.yml` (`invoke.example.yml`) in this directory which can be used as a starting point.\n\n#### Local Poetry Development Environment\n\n1. Copy `development/creds.example.env` to `development/creds.env` (This file will be ignored by Git and Docker)\n2. Uncomment the `POSTGRES_HOST`, `REDIS_HOST`, and `NAUTOBOT_ROOT` variables in `development/creds.env`\n3. Create an `invoke.yml` file with the following contents at the root of the repo (you can also `cp invoke.example.yml invoke.yml` and edit as necessary):\n\n```yaml\n---\nnautobot_ssot_infoblox:\n  local: true\n  compose_files:\n    - "docker-compose.requirements.yml"\n```\n\n3. Run the following commands:\n\n```shell\npoetry shell\npoetry install --extras nautobot\nexport $(cat development/dev.env | xargs)\nexport $(cat development/creds.env | xargs) \ninvoke start && sleep 5\nnautobot-server migrate\n```\n\n> If you want to develop on the latest develop branch of Nautobot, run the following command: `poetry add --optional git+https://github.com/nautobot/nautobot@develop`. After the `@` symbol must match either a branch or a tag.\n\n4. You can now run nautobot-server commands as you would from the [Nautobot documentation](https://nautobot.readthedocs.io/en/latest/) for example to start the development server:\n\n```shell\nnautobot-server runserver 0.0.0.0:8080 --insecure\n```\n\nNautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).\n\nIt is typically recommended to launch the Nautobot **runserver** command in a separate shell so you can keep developing and manage the webserver separately.\n\n#### Docker Development Environment\n\nThis project is managed by [Python Poetry](https://python-poetry.org/) and has a few requirements to setup your development environment:\n\n1. Install Poetry, see the [Poetry Documentation](https://python-poetry.org/docs/#installation) for your operating system.\n2. Install Docker, see the [Docker documentation](https://docs.docker.com/get-docker/) for your operating system.\n\nOnce you have Poetry and Docker installed you can run the following commands to install all other development dependencies in an isolated python virtual environment:\n\n```shell\npoetry shell\npoetry install\ninvoke start\n```\n\nNautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).\n\nTo either stop or destroy the development environment use the following options.\n\n- **invoke stop** - Stop the containers, but keep all underlying systems intact\n- **invoke destroy** - Stop and remove all containers, volumes, etc. (This results in data loss due to the volume being deleted)\n\n### CLI Helper Commands\n\nThe project is coming with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help setup the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.\n\nEach command can be executed with `invoke <command>`. Environment variables `INVOKE_NAUTOBOT_SSOT_INFOBLOX_PYTHON_VER` and `INVOKE_NAUTOBOT_SSOT_INFOBLOX_NAUTOBOT_VER` may be specified to override the default versions. Each command also has its own help `invoke <command> --help`\n\n#### Docker dev environment\n\n```no-highlight\n  build            Build all docker images.\n  debug            Start Nautobot and its dependencies in debug mode.\n  destroy          Destroy all containers and volumes.\n  restart          Restart Nautobot and its dependencies.\n  start            Start Nautobot and its dependencies in detached mode.\n  stop             Stop Nautobot and its dependencies.\n```\n\n#### Utility\n\n```no-highlight\n  cli              Launch a bash shell inside the running Nautobot container.\n  create-user      Create a new user in django (default: admin), will prompt for password.\n  makemigrations   Run Make Migration in Django.\n  nbshell          Launch a nbshell session.\n  shell-plus       Launch a shell_plus session, which uses iPython and automatically imports all models.\n```\n\n#### Testing\n\n```no-highlight\n  bandit           Run bandit to validate basic static code security analysis.\n  black            Run black to check that Python files adhere to its style standards.\n  flake8           This will run flake8 for the specified name and Python version.\n  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.\n  pylint           Run pylint code analysis.\n  tests            Run all tests for this plugin.\n  unittest         Run Django unit tests for the plugin.\n```\n\n### Project Documentation\n\nProject documentation is generated by [mkdocs](https://www.mkdocs.org/) from the documentation located in the docs folder.  You can configure [readthedocs.io](https://readthedocs.io/) to point at this folder in your repo.  A container hosting the docs will be started using the invoke commands on [http://localhost:8001](http://localhost:8001), as changes are saved the docs will be automatically reloaded.\n\n## Questions\n\nFor any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code slack channel](https://networktocode.slack.com/) (channel #networktocode).\nSign up [here](http://slack.networktocode.com/)\n\n## Screenshots\n\n![Infoblox SSoT Status](./docs/static/ssot-status.png)\n\n![Infoblox SSoT Logs](./docs/static/ssot-logs.png)\n',
-    'author': 'Network to Code, LLC',
-    'author_email': 'info@networktocode.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/networktocode-llc/nautobot-plugin-ssot-infoblox',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+# Nautobot SSoT Infoblox
+
+Using the [Nautobot SSoT](https://github.com/nautobot/nautobot-plugin-ssot) framework, the SSoT plugin for Infoblox allows for synchronizing of IP network and VLAN data between [Infoblox](https://infoblox.com/) and [Nautobot](https://github.com/nautobot/nautobot).
+
+## Installation
+
+The plugin is available as a Python package in PyPi and can be installed with pip.
+
+```shell
+pip install nautobot-ssot-infoblox
+```
+
+> The plugin is compatible with Nautobot 1.2.0 and higher
+
+To ensure Nautobot SSoT Infoblox is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the Nautobot root directory (alongside `requirements.txt`) and list the `nautobot-ssot-infoblox` package:
+
+```no-highlight
+# echo nautobot-ssot-infoblox >> local_requirements.txt
+```
+
+Once installed, the plugin needs to be enabled in your `nautobot_config.py`
+
+```python
+# In your nautobot_config.py
+PLUGINS = ["nautobot_ssot", "nautobot_ssot_infoblox"]
+```
+
+See the section below for configuration settings.
+
+## Configuration
+
+| Setting                           | Default | Description                                                            |
+| --------------------------------- | ------- | ---------------------------------------------------------------------- |
+| NAUTOBOT_INFOBLOX_URL             | N/A     | URL of the Infoblox instance to sync with.                             |
+| NAUTOBOT_INFOBLOX_USERNAME        | N/A     | The username to authenticate against Infoblox with.                    |
+| NAUTOBOT_INFOBLOX_PASSWORD        | N/A     | The password to authenticate against Infblox with.                     |
+| NAUTOBOT_INFOBLOX_VERIFY_SSL      | True    | Toggle SSL verification when syncing data with Infoblox.               |
+| NAUTOBOT_INFOBLOX_WAPI_VERSION    | v2.12   | The version of the Infoblox API.                                       |
+| enable_sync_to_infoblox           | False   | Add job to sync data from Nautobot into Infoblox.                      |
+| enable_rfc1918_network_containers | False   | Add job to sync network containers to Nautobot (top level aggregates). |
+| default_status                    | active  | Default Status to be assigned to imported objects.                     |
+| infoblox_import_objects           | True    | Dictionary with keys for each import object and the value define import.|
+| infoblox_import_subnets           | N/A     | List of Subnets in CIDR string notation to filter import to.           |
+
+### Configuration Example
+
+```python
+PLUGINS_CONFIG = {
+    "nautobot_ssot": {
+        "hide_example_jobs": True,  # defaults to False if unspecified
+    }
+    "nautobot_ssot_infoblox": {
+        "NAUTOBOT_INFOBLOX_URL": os.getenv("NAUTOBOT_INFOBLOX_URL", ""),
+        "NAUTOBOT_INFOBLOX_USERNAME": os.getenv("NAUTOBOT_INFOBLOX_USERNAME", ""),
+        "NAUTOBOT_INFOBLOX_PASSWORD": os.getenv("NAUTOBOT_INFOBLOX_PASSWORD", ""),
+        "NAUTOBOT_INFOBLOX_VERIFY_SSL": os.getenv("NAUTOBOT_INFOBLOX_VERIFY_SSL", "true"),
+        "NAUTOBOT_INFOBLOX_WAPI_VERSION": os.getenv("NAUTOBOT_INFOBLOX_WAPI_VERSION", "v2.12"),
+        "enable_sync_to_infoblox": False,
+        "enable_rfc1918_network_containers": False,
+        "default_status": "active",
+        "infoblox_import_objects": {
+            "vlan_views": os.getenv("NAUTOBOT_INFOBLOX_IMPORT_VLAN_VIEWS", True),
+            "vlans": os.getenv("NAUTOBOT_INFOBLOX_IMPORT_VLANS", True),
+            "subnets": os.getenv("NAUTOBOT_INFOBLOX_INFOBLOX_IMPORT_SUBNETS", True),
+            "ip_addresses": os.getenv("NAUTOBOT_INFOBLOX_IMPORT_IP_ADDRESSES", True),
+        },
+        "infoblox_import_subnets": ["10.46.128.0/18", "192.168.1.0/24"],
+    }
 }
+```
+
+## DiffSync Models
+
+Below are the data mappings between objects within Infoblox and the corresponding objects within Nautobot:
+
+| Infoblox          | Nautobot       |
+| ----------------- | -------------- |
+| Network           | Prefix         |
+| IP Address        | IP Address     |
+| VLAN              | VLAN           |
+| VLAN view         | VLAN Group     |
+| Network container | Aggregate      |
+| Extensibility Attrs | Custom Fields |
+
+NOTE - More information about Extensibility Attributes can be found in the [project documentation](#project-documentation).
+
+### DiffSyncModel - Network
+
+![Diffsync Model - Network](./docs/static/diffsyncmodel-network.png)
+
+### DiffSyncModel - IPAddress
+
+![Diffsync Model - IPAddress](./docs/static/diffsyncmodel-ipaddress.png)
+
+### DiffSyncModel - Aggregate
+
+![Diffsync Model - Aggregate](./docs/static/diffsyncmodel-aggregate.png)
+
+## Contributing
+
+Pull requests are welcomed and automatically built and tested against multiple version of Python and multiple version of Nautobot through GitHub Actions.
+
+The project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within GitHub Actions.
+
+The project is following Network to Code software development guideline and is leveraging:
+
+- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.
+- Django unit test to ensure the plugin is working properly.
+
+### Development Environment
+
+The development environment can be used in 2 ways. First, with a local poetry environment if you wish to develop outside of Docker with the caveat of using external services provided by Docker for PostgresQL and Redis. Second, all services are spun up using Docker and a local mount so you can develop locally, but Nautobot is spun up within the Docker container.
+
+Below is a quick start guide if you're already familiar with the development environment provided, but if you're not familiar, please read the [Getting Started Guide](GETTING_STARTED.md).
+
+#### Invoke
+
+The [PyInvoke](http://www.pyinvoke.org/) library is used to provide some helper commands based on the environment.  There are a few configuration parameters which can be passed to PyInvoke to override the default configuration:
+
+- `nautobot_ver`: the version of Nautobot to use as a base for any built docker containers (default: 1.1.4)
+- `project_name`: the default docker compose project name (default: nautobot_ssot_infoblox)
+- `python_ver`: the version of Python to use as a base for any built docker containers (default: 3.6)
+- `local`: a boolean flag indicating if invoke tasks should be run on the host or inside the docker containers (default: False, commands will be run in docker containers)
+- `compose_dir`: the full path to a directory containing the project compose files
+- `compose_files`: a list of compose files applied in order (see [Multiple Compose files](https://docs.docker.com/compose/extends/#multiple-compose-files) for more information)
+
+Using **PyInvoke** these configuration options can be overridden using [several methods](http://docs.pyinvoke.org/en/stable/concepts/configuration.html).  Perhaps the simplest is simply setting an environment variable `INVOKE_NAUTOBOT_SSOT_INFOBLOX_VARIABLE_NAME` where `VARIABLE_NAME` is the variable you are trying to override.  The only exception is `compose_files`, because it is a list it must be overridden in a yaml file.  There is an example `invoke.yml` (`invoke.example.yml`) in this directory which can be used as a starting point.
+
+#### Local Poetry Development Environment
+
+1. Copy `development/creds.example.env` to `development/creds.env` (This file will be ignored by Git and Docker)
+2. Uncomment the `POSTGRES_HOST`, `REDIS_HOST`, and `NAUTOBOT_ROOT` variables in `development/creds.env`
+3. Create an `invoke.yml` file with the following contents at the root of the repo (you can also `cp invoke.example.yml invoke.yml` and edit as necessary):
+
+```yaml
+---
+nautobot_ssot_infoblox:
+  local: true
+  compose_files:
+    - "docker-compose.requirements.yml"
+```
+
+3. Run the following commands:
+
+```shell
+poetry shell
+poetry install --extras nautobot
+export $(cat development/dev.env | xargs)
+export $(cat development/creds.env | xargs) 
+invoke start && sleep 5
+nautobot-server migrate
+```
+
+> If you want to develop on the latest develop branch of Nautobot, run the following command: `poetry add --optional git+https://github.com/nautobot/nautobot@develop`. After the `@` symbol must match either a branch or a tag.
+
+4. You can now run nautobot-server commands as you would from the [Nautobot documentation](https://nautobot.readthedocs.io/en/latest/) for example to start the development server:
+
+```shell
+nautobot-server runserver 0.0.0.0:8080 --insecure
+```
+
+Nautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).
+
+It is typically recommended to launch the Nautobot **runserver** command in a separate shell so you can keep developing and manage the webserver separately.
+
+#### Docker Development Environment
+
+This project is managed by [Python Poetry](https://python-poetry.org/) and has a few requirements to setup your development environment:
+
+1. Install Poetry, see the [Poetry Documentation](https://python-poetry.org/docs/#installation) for your operating system.
+2. Install Docker, see the [Docker documentation](https://docs.docker.com/get-docker/) for your operating system.
+
+Once you have Poetry and Docker installed you can run the following commands to install all other development dependencies in an isolated python virtual environment:
+
+```shell
+poetry shell
+poetry install
+invoke start
+```
+
+Nautobot server can now be accessed at [http://localhost:8080](http://localhost:8080).
+
+To either stop or destroy the development environment use the following options.
+
+- **invoke stop** - Stop the containers, but keep all underlying systems intact
+- **invoke destroy** - Stop and remove all containers, volumes, etc. (This results in data loss due to the volume being deleted)
+
+### CLI Helper Commands
+
+The project is coming with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help setup the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.
+
+Each command can be executed with `invoke <command>`. Environment variables `INVOKE_NAUTOBOT_SSOT_INFOBLOX_PYTHON_VER` and `INVOKE_NAUTOBOT_SSOT_INFOBLOX_NAUTOBOT_VER` may be specified to override the default versions. Each command also has its own help `invoke <command> --help`
+
+#### Docker dev environment
+
+```no-highlight
+  build            Build all docker images.
+  debug            Start Nautobot and its dependencies in debug mode.
+  destroy          Destroy all containers and volumes.
+  restart          Restart Nautobot and its dependencies.
+  start            Start Nautobot and its dependencies in detached mode.
+  stop             Stop Nautobot and its dependencies.
+```
+
+#### Utility
+
+```no-highlight
+  cli              Launch a bash shell inside the running Nautobot container.
+  create-user      Create a new user in django (default: admin), will prompt for password.
+  makemigrations   Run Make Migration in Django.
+  nbshell          Launch a nbshell session.
+  shell-plus       Launch a shell_plus session, which uses iPython and automatically imports all models.
+```
+
+#### Testing
+
+```no-highlight
+  bandit           Run bandit to validate basic static code security analysis.
+  black            Run black to check that Python files adhere to its style standards.
+  flake8           This will run flake8 for the specified name and Python version.
+  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.
+  pylint           Run pylint code analysis.
+  tests            Run all tests for this plugin.
+  unittest         Run Django unit tests for the plugin.
+```
+
+### Project Documentation
+
+Project documentation is generated by [mkdocs](https://www.mkdocs.org/) from the documentation located in the docs folder.  You can configure [readthedocs.io](https://readthedocs.io/) to point at this folder in your repo.  A container hosting the docs will be started using the invoke commands on [http://localhost:8001](http://localhost:8001), as changes are saved the docs will be automatically reloaded.
+
+## Questions
+
+For any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code slack channel](https://networktocode.slack.com/) (channel #networktocode).
+Sign up [here](http://slack.networktocode.com/)
+
+## Screenshots
+
+![Infoblox SSoT Status](./docs/static/ssot-status.png)
 
+![Infoblox SSoT Logs](./docs/static/ssot-logs.png)
 
-setup(**setup_kwargs)
```

