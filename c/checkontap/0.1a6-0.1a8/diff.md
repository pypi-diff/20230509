# Comparing `tmp/checkontap-0.1a6.tar.gz` & `tmp/checkontap-0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkontap-0.1a6.tar", last modified: Tue May  2 15:04:01 2023, max compression
+gzip compressed data, was "checkontap-0.1a8.tar", last modified: Tue May  9 10:50:31 2023, max compression
```

## Comparing `checkontap-0.1a6.tar` & `checkontap-0.1a8.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a6/README.md
--rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a6/checkontap/__init__.py
--rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a6/checkontap/cli.py
--rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a6/checkontap/ontapcmd/__init__.py
--rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a6/checkontap/ontapcmd/about.py
--rw-r--r--   0        0        0     7033 2023-04-28 13:18:56.743322 checkontap-0.1a6/checkontap/ontapcmd/aggregateusage.py
--rw-r--r--   0        0        0     4641 2023-04-27 15:24:18.383341 checkontap-0.1a6/checkontap/ontapcmd/clusterhealth.py
--rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a6/checkontap/ontapcmd/diskhealth.py
--rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a6/checkontap/ontapcmd/hardwarehealth.py
--rw-r--r--   0        0        0     3878 2023-04-27 14:42:48.878279 checkontap-0.1a6/checkontap/ontapcmd/interfacehealth.py
--rw-r--r--   0        0        0     4994 2023-04-21 14:49:47.394778 checkontap-0.1a6/checkontap/ontapcmd/lunusage.py
--rw-r--r--   0        0        0     4298 2023-05-02 15:00:56.886969 checkontap-0.1a6/checkontap/ontapcmd/porthealth.py
--rw-r--r--   0        0        0     7239 2023-04-28 14:49:04.694080 checkontap-0.1a6/checkontap/ontapcmd/ports.py
--rw-r--r--   0        0        0     5079 2023-04-21 14:49:57.522947 checkontap-0.1a6/checkontap/ontapcmd/volumehealth.py
--rw-r--r--   0        0        0     8463 2023-04-26 12:55:43.724726 checkontap-0.1a6/checkontap/ontapcmd/volumeusage.py
--rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a6/checkontap/tools/__init__.py
--rw-r--r--   0        0        0    10030 2023-04-28 13:08:45.930194 checkontap-0.1a6/checkontap/tools/cli.py
--rw-r--r--   0        0        0     3918 2023-04-28 12:56:43.397643 checkontap-0.1a6/checkontap/tools/helper.py
--rw-r--r--   0        0        0      857 2023-05-02 15:01:41.029050 checkontap-0.1a6/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a6/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a8/README.md
+-rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a8/checkontap/__init__.py
+-rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a8/checkontap/cli.py
+-rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a8/checkontap/ontapcmd/__init__.py
+-rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a8/checkontap/ontapcmd/about.py
+-rw-r--r--   0        0        0     7058 2023-05-03 11:57:10.637337 checkontap-0.1a8/checkontap/ontapcmd/aggregateusage.py
+-rw-r--r--   0        0        0     4641 2023-04-27 15:24:18.383341 checkontap-0.1a8/checkontap/ontapcmd/clusterhealth.py
+-rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a8/checkontap/ontapcmd/diskhealth.py
+-rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a8/checkontap/ontapcmd/hardwarehealth.py
+-rw-r--r--   0        0        0     3878 2023-04-27 14:42:48.878279 checkontap-0.1a8/checkontap/ontapcmd/interfacehealth.py
+-rw-r--r--   0        0        0     4842 2023-05-09 07:55:59.466057 checkontap-0.1a8/checkontap/ontapcmd/lunusage.py
+-rw-r--r--   0        0        0     4298 2023-05-02 15:00:56.886969 checkontap-0.1a8/checkontap/ontapcmd/porthealth.py
+-rw-r--r--   0        0        0     5533 2023-05-09 10:47:17.544800 checkontap-0.1a8/checkontap/ontapcmd/volumehealth.py
+-rw-r--r--   0        0        0     9699 2023-05-08 12:58:13.829491 checkontap-0.1a8/checkontap/ontapcmd/volumeusage.py
+-rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a8/checkontap/tools/__init__.py
+-rw-r--r--   0        0        0    10030 2023-04-28 13:08:45.930194 checkontap-0.1a8/checkontap/tools/cli.py
+-rw-r--r--   0        0        0     3927 2023-05-02 15:41:17.067310 checkontap-0.1a8/checkontap/tools/helper.py
+-rw-r--r--   0        0        0      857 2023-05-09 10:50:23.207374 checkontap-0.1a8/pyproject.toml
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a8/PKG-INFO
```

### Comparing `checkontap-0.1a6/checkontap/__init__.py` & `checkontap-0.1a8/checkontap/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/cli.py` & `checkontap-0.1a8/checkontap/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/__init__.py` & `checkontap-0.1a8/checkontap/ontapcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/about.py` & `checkontap-0.1a8/checkontap/ontapcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/aggregateusage.py` & `checkontap-0.1a8/checkontap/ontapcmd/aggregateusage.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,25 +86,26 @@
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
     check = Check(threshold = Threshold(args.warning or None, args.critical or None))
     setup_connection(args.host, args.api_user, args.api_pass)
 
     try:
         aggr_count = Aggregate.count_collection()
-        logger.debug(f"found {aggr_count} Aggregates")
+        logger.info(f"found {aggr_count} Aggregates")
         if aggr_count == 0:
             check.exit(Status.UNKNOWN, "no aggregates found")
 
         for aggr in Aggregate.get_collection():
             aggr.get(fields="space,uuid")
             if (args.exclude or args.include) and item_filter(args,aggr.name):
-                logger.debug(f"{aggr.name} filtered out and removed from check")
+                logger.info(f"{aggr.name} filtered out and removed from check")
                 aggr_count -= 1
                 continue
-            logger.debug(f"Aggregate {aggr.name}\n{aggr.__dict__}")
+            logger.info(f"Aggregate {aggr.name}")
+            logger.debug(f"{aggr.__dict__}")
             
             plex_count = Plex.count_collection(aggr.uuid)
             if plex_count != 0:
                 for plex in Plex.get_collection(aggr.uuid):
                     plex.get(fields="raid_groups")
                     logging.debug(f"Plex {plex.name}\n{plex.__dict__}")
                     for rg in plex.raid_groups:
```

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/clusterhealth.py` & `checkontap-0.1a8/checkontap/ontapcmd/clusterhealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/diskhealth.py` & `checkontap-0.1a8/checkontap/ontapcmd/diskhealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/hardwarehealth.py` & `checkontap-0.1a8/checkontap/ontapcmd/hardwarehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/interfacehealth.py` & `checkontap-0.1a8/checkontap/ontapcmd/interfacehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/porthealth.py` & `checkontap-0.1a8/checkontap/ontapcmd/porthealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/ontapcmd/volumehealth.py` & `checkontap-0.1a8/checkontap/ontapcmd/volumehealth.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,49 +19,51 @@
 from monplugin import Check,Status
 from netapp_ontap.resources import Volume
 from netapp_ontap import NetAppRestError
 from ..tools import cli
 from ..tools.helper import setup_connection,severity,item_filter
 
 __cmd__ = "volume-health"
+description = "Check state of volumes online,offline,error or mixed"
 """
 Volume({
-    'snapshot_policy': {'name': 'none'}, 
-    'analytics': {'state': 'off'}, 
-    'space': {'size': 27487790694400, 'available': 13976673030144, 'used': 13511117664256}, 
-    'type': 'rw', 
-    'size': 27487790694400, 
-    'cloud_retrieval_policy': 'default', 
-    'name': 'eald_p', 
+    'snapshot_policy': {'name': 'none'},
+    'analytics': {'state': 'off'},
+    'space': {'size': 27487790694400, 'available': 13976673030144, 'used': 13511117664256},
+    'type': 'rw',
+    'size': 27487790694400,
+    'cloud_retrieval_policy': 'default',
+    'name': 'eald_p',
     'svm': {
-        'name': 'acme01', 
-        'uuid': '21a63386-5483-11ea-8c65-00a098ef551e', 
-        '_links': {'self': {'href': '/api/svm/svms/21a63386-5483-11ea-8c65-00a098ef551e'}}}, 
-    'aggregates': [{'uuid': '01d71c4b-88d8-43c3-ae33-afa2b64a629d', 'name': 'acme01_data'}], 
-    'snapmirror': {'is_protected': True}, 
-    'style': 'flexvol', 
-    'uuid': '42b7ee25-a342-11eb-b488-00a098c53056', 
-    '_links': {'self': {'href': '/api/storage/volumes/42b7ee25-a342-11eb-b488-00a098c53056'}}, 
-    'state': 'online', 
-    'nas': {'export_policy': {'name': 'default'}}, 
-    'tiering': {'policy': 'none'}, 
-    'clone': {'is_flexclone': False}, 
-    'language': 'c.utf_8', 
+        'name': 'acme01',
+        'uuid': '21a63386-5483-11ea-8c65-00a098ef551e',
+        '_links': {'self': {'href': '/api/svm/svms/21a63386-5483-11ea-8c65-00a098ef551e'}}},
+    'aggregates': [{'uuid': '01d71c4b-88d8-43c3-ae33-afa2b64a629d', 'name': 'acme01_data'}],
+    'snapmirror': {'is_protected': True},
+    'style': 'flexvol',
+    'uuid': '42b7ee25-a342-11eb-b488-00a098c53056',
+    '_links': {'self': {'href': '/api/storage/volumes/42b7ee25-a342-11eb-b488-00a098c53056'}},
+    'state': 'online',
+    'nas': {'export_policy': {'name': 'default'}},
+    'tiering': {'policy': 'none'},
+    'clone': {'is_flexclone': False},
+    'language': 'c.utf_8',
     'metric': {
-        'status': 'ok', 
-        'timestamp': '2022-08-03T11:22:00+00:00', 
-        'latency': {'other': 214, 'write': 259, 'read': 173, 'total': 205}, 
-        'duration': 'PT15S', 
-        'iops': {'other': 7, 'write': 2, 'read': 5, 'total': 15}, 
-        'throughput': {'other': 0, 'write': 6967, 'read': 25478, 'total': 32445}}, 
-    'comment': '', 
+        'status': 'ok',
+        'timestamp': '2022-08-03T11:22:00+00:00',
+        'latency': {'other': 214, 'write': 259, 'read': 173, 'total': 205},
+        'duration': 'PT15S',
+        'iops': {'other': 7, 'write': 2, 'read': 5, 'total': 15},
+        'throughput': {'other': 0, 'write': 6967, 'read': 25478, 'total': 32445}},
+    'comment': '',
     'create_time': '2021-04-22T10:10:54+02:00'})
 """
 def run():
     parser = cli.Parser()
+    parser.set_description(description)
     parser.set_epilog("")
     parser.add_optional_arguments(cli.Argument.WARNING,
                                   cli.Argument.CRITICAL,
                                   cli.Argument.EXCLUDE,
                                   cli.Argument.INCLUDE,
                                   cli.Argument.NAME)
     args = parser.get_args()
@@ -82,35 +84,44 @@
         logger.info(f"found {volumes_count} volumes")
         if volumes_count == 0:
             check.exit(Status.UNKNOWN, "no vols found")
 
         if args.name:
             for n in args.name[0]:
                 vol = Volume.find(name=n)
+                logger.info(f"find volume {n}")
+                logger.debug(f"{vol}")
                 if args.warning and vol.state in args.warning:
                     check.add_message(Status.WARNING, f"Vol: {vol.name} has state {vol.state}")
                 elif args.critical and vol.state in args.critical:
                     check.add_message(Status.CRITICAL, f"Vol: {vol.name} has state {vol.state}")
                 else:
                     check.add_message(Status.OK, f"Vol: {vol.name} has state {vol.state}")
         else:
             for vol in Volume.get_collection():
+                logger.info(f"get volume {vol.name}")
                 vol.get(fields="name,state,style,comment")
+                logger.debug(f"{vol}")
                 if not hasattr(vol,'state'):
+                    volumes_count -= 1
                     continue
                 if (args.exclude or args.include) and item_filter(args,vol.name):
+                    volumes_count -= 1
                     continue
                 logger.info(f"state: {vol.state}\tname: {vol.name}\tstyle: {vol.style}\tcomment: {vol.comment}")
                 if args.warning and vol.state in args.warning:
                     check.add_message(Status.WARNING, f"Vol: {vol.name} has state {vol.state}")
                 elif args.critical and vol.state in args.critical:
                     check.add_message(Status.CRITICAL, f"Vol: {vol.name} has state {vol.state}")
                 else:
                     check.add_message(Status.OK, f"Vol: {vol.name} has state {vol.state}")
-        (code, message) = check.check_messages(separator='\n ')
-        check.exit(code=code,message=message)
-        
+        short = f"checked {volumes_count} volumes"
+        (code, message) = check.check_messages(separator='\n')
+        check.exit(code=code,message=f"{short}\n{message}")
+
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error.http_err_response.http_response.text))
-    
+    except Exception as error:
+        logger.exception(error)
+
 if __name__ == "__main__":
-    run()
+    run()
```

### Comparing `checkontap-0.1a6/checkontap/tools/__init__.py` & `checkontap-0.1a8/checkontap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/tools/cli.py` & `checkontap-0.1a8/checkontap/tools/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a6/checkontap/tools/helper.py` & `checkontap-0.1a8/checkontap/tools/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return err
     return(r)
 
 def bytes_to_uom(value, uom, maximum=None, bsize=1024) -> None:
     a = {'kB' : 1, 'MB': 2, 'GB' : 3, 'TB' : 4, 'PB' : 5, 'EB' : 6 }
     try:
         if '%' in uom and maximum:
-            r = (float(value) / int(maximum) ) * 100
+            r = round((float(value) / int(maximum) ) * 100,2)
         else:
             r = round(float(value) / (bsize ** a[uom]),3)
     except Exception as err:
         return err
     return(r)
 
 # Percent returned with 2 decimals
```

### Comparing `checkontap-0.1a6/pyproject.toml` & `checkontap-0.1a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkontap"
 readme = "README.md"
 description = "check_ontap monitoring plugin"
-version = "0.1a6"
+version = "0.1a8"
 requires-python = ">= 3.6"
 authors = [
     { name = "Matthias Gallinger", email = "matthias.gallinger@consol.de" }
 ]
 dependencies = [
     "netapp-ontap >= 9.11.1.0",
     "monplugin >= 0.5",
```

### Comparing `checkontap-0.1a6/PKG-INFO` & `checkontap-0.1a8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkontap
-Version: 0.1a6
+Version: 0.1a8
 Summary: check_ontap monitoring plugin
 Author-email: Matthias Gallinger <matthias.gallinger@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

