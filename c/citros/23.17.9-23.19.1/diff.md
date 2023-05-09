# Comparing `tmp/citros-23.17.9.tar.gz` & `tmp/citros-23.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.17.9.tar", last modified: Wed May  3 06:51:18 2023, max compression
+gzip compressed data, was "citros-23.19.1.tar", last modified: Tue May  9 11:03:27 2023, max compression
```

## Comparing `citros-23.17.9.tar` & `citros-23.19.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:18.005273 citros-23.17.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 06:50:53.000000 citros-23.17.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-03 06:51:18.001273 citros-23.17.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-03 06:50:53.000000 citros-23.17.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:17.997274 citros-23.17.9/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-03 06:50:53.000000 citros-23.17.9/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:17.997274 citros-23.17.9/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 06:50:53.000000 citros-23.17.9/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-03 06:50:53.000000 citros-23.17.9/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-05-03 06:50:53.000000 citros-23.17.9/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 06:50:53.000000 citros-23.17.9/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-03 06:50:53.000000 citros-23.17.9/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-03 06:50:53.000000 citros-23.17.9/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-03 06:50:53.000000 citros-23.17.9/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-03 06:50:53.000000 citros-23.17.9/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:18.001273 citros-23.17.9/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-03 06:50:53.000000 citros-23.17.9/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-03 06:50:53.000000 citros-23.17.9/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:18.001273 citros-23.17.9/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-03 06:50:53.000000 citros-23.17.9/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-03 06:50:53.000000 citros-23.17.9/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-03 06:50:53.000000 citros-23.17.9/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:18.001273 citros-23.17.9/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 06:50:53.000000 citros-23.17.9/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 06:50:53.000000 citros-23.17.9/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-03 06:50:53.000000 citros-23.17.9/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:18.001273 citros-23.17.9/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-03 06:50:53.000000 citros-23.17.9/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-03 06:50:53.000000 citros-23.17.9/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-03 06:50:53.000000 citros-23.17.9/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-03 06:50:53.000000 citros-23.17.9/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:17.997274 citros-23.17.9/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-03 06:51:17.000000 citros-23.17.9/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 06:51:17.000000 citros-23.17.9/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:51:17.000000 citros-23.17.9/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 06:51:17.000000 citros-23.17.9/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 06:51:17.000000 citros-23.17.9/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 06:50:53.000000 citros-23.17.9/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:51:18.005273 citros-23.17.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 06:50:53.000000 citros-23.17.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:18.001273 citros-23.17.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:50:53.000000 citros-23.17.9/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:50:53.000000 citros-23.17.9/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 11:03:09.000000 citros-23.19.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-09 11:03:27.239459 citros-23.19.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-09 11:03:09.000000 citros-23.19.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.235459 citros-23.19.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-05-09 11:03:09.000000 citros-23.19.1/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.235459 citros-23.19.1/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-09 11:03:09.000000 citros-23.19.1/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-09 11:03:09.000000 citros-23.19.1/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-09 11:03:09.000000 citros-23.19.1/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-09 11:03:09.000000 citros-23.19.1/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-09 11:03:09.000000 citros-23.19.1/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-09 11:03:09.000000 citros-23.19.1/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-09 11:03:09.000000 citros-23.19.1/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 11:03:09.000000 citros-23.19.1/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-09 11:03:09.000000 citros-23.19.1/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-09 11:03:09.000000 citros-23.19.1/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-09 11:03:09.000000 citros-23.19.1/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-09 11:03:09.000000 citros-23.19.1/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-09 11:03:09.000000 citros-23.19.1/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-09 11:03:09.000000 citros-23.19.1/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:03:27.239459 citros-23.19.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-09 11:03:09.000000 citros-23.19.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:09.000000 citros-23.19.1/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:09.000000 citros-23.19.1/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.17.9/LICENSE` & `citros-23.19.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/PKG-INFO` & `citros-23.19.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.9
+Version: 23.19.1
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.9/README.md` & `citros-23.19.1/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/bin/citros` & `citros-23.19.1/bin/citros`

 * *Files 5% similar despite different names*

```diff
@@ -52,18 +52,31 @@
     if not citros.isAuthenticated():
         print("sync_project: please log in first!")
         return
     project_data = citros.parser_ros2.parse(args.dir, args.name, args.ws)
     # print("sync_project:project: ", json.dumps(project_data, indent=2))
     citros.integration.sync_project(project_data)
 
-def run_simulation(simulation_id, repeats):    
-    # TODO: create new batch for this simulation
-    # run the batch 
-    pass
+def run_simulation(args, argv):    
+    print_citros()       
+        
+    citros = Citros()   
+    if args.key:
+        loggedin = citros.authenticate_with_key(args.key)
+        if not loggedin:
+            sys.exit("run_ros2_project.authenticate_with_key: please log in first!") 
+    
+    if not citros.isAuthenticated():
+        sys.exit("run_simulation: please log in first!")      
+        
+    # create new batch for this simulation
+    batch_run_id = citros.batch.create_manual_batch(args.simulation_id, args.completions)
+    print(f"created new batch_run_id: {batch_run_id}")
+    run_batch(batch_run_id, 10*60)
+    sys.exit(0)
     
 def run_batch(batch_run_id, timeout):
     batch = Citros().batch.get_batch(batch_run_id)
     
     completions = 1
     try:
         completions = int(batch["batchRun"]["completions"]) + 1
@@ -249,26 +262,32 @@
     # experimental
     # -----------------------------------------
     build_parser = subparsers.add_parser("params", help="generating parameters to the project")
     build_parser.add_argument("batch_run_id", help="Batch run id")
     build_parser.add_argument("sid", help="simulation run id")    
     build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")
     build_parser.set_defaults(func=load_params)
-    
-    # experimental
+        
     # -----------------------------------------
     # runs the [batch_run, simulation_run]
     build_parser = subparsers.add_parser("run", help="run ros2 project")
     build_parser.add_argument("batch_run_id", help="Batch run id")
     build_parser.add_argument("sid", nargs='?', default='', help="simulation run id")    
     build_parser.add_argument("-timeout", default=60*60, help="simulation timeout")    
     build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")
     build_parser.add_argument("--key", help="jwt ket of the user")
-    
     build_parser.set_defaults(func=run_ros2_project)
+    
+    # -----------------------------------------
+    build_parser = subparsers.add_parser("run_simulation", help="create new batch and run it")
+    build_parser.add_argument("simulation_id", help="Simulation run id")
+    build_parser.add_argument("completions", default=1, help="how many tiumes to run the simulation")
+    build_parser.add_argument("-timeout", default=60*60, help="simulation timeout")
+    build_parser.add_argument("--key", help="jwt ket of the user")
+    build_parser.set_defaults(func=run_simulation)
      
     # experimental
     # -----------------------------------------
     # runs the [batch_run, simulation_run]
     build_parser = subparsers.add_parser("upload_bag", help="upload bag to citros")
     build_parser.add_argument("bag", help="bag file")
     build_parser.add_argument("batch_run_id", help="Batch run id")
```

### Comparing `citros-23.17.9/citros/__init__.py` & `citros-23.19.1/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/citros.py` & `citros-23.19.1/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/citros_bag.py` & `citros-23.19.1/citros/citros_bag.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         self.log.debug("------------------------------------------------------------------------------------")
         self.log.debug("uploading bag to google bucket")
         if not self.citros.isAuthenticated():
             self.log.debug("not authenticated. please login first.")
             return False, "not authenticated. please login first." , None       
         
         user = self.citros.getUser()
-        tenant =  user["organization"]["domain_prefix"]
+        tenant =  user["organization"]["domainPrefix"]
         
         bag_file_name = path_to_bag.split('/')[-1]            
         data_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={tenant + "/" + batch_run_id + "/sid-" + simulation_run_id + "/" + bag_file_name}'        
         
         metadata_name = path_to_metadata.split('/')[-1]  
         metadata_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={tenant + "/" + batch_run_id + "/sid-" + simulation_run_id + "/" + metadata_name}'
```

### Comparing `citros-23.17.9/citros/citros_batch.py` & `citros-23.19.1/citros/citros_batch.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,10 +23,31 @@
                     }
                 }
             }            
         }
         """
         result = self.citros.gql_execute(query, variable_values={"batchRunId": batch_run_id})
         return result
+    
+    def create_manual_batch(self, simulation_id, completions):
+        query = """
+        mutation createBatch($simulationId: UUID!, $completions: Int) {
+        createBatchRun(input: {             
+            batchRun: {
+                simulationId: $simulationId,
+                completions: $completions,
+                parallelism: 0,
+                trigger: MANUAL,
+                isManual: true
+                }
+            }){
+                batchRun {
+                id
+                }
+            } 
+        }
+        """ 
+        result = self.citros.gql_execute(query, variable_values={"simulationId": simulation_id, "completions": int(completions)})        
+        return result["createBatchRun"]["batchRun"]["id"]
```

### Comparing `citros-23.17.9/citros/citros_events.py` & `citros-23.19.1/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/citros_integration.py` & `citros-23.19.1/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/citros_params.py` & `citros-23.19.1/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/citros_utils.py` & `citros-23.19.1/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/launches/__init__.py` & `citros-23.19.1/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/launches/launch.py` & `citros-23.19.1/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/logger/__init__.py` & `citros-23.19.1/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/logger/logger.py` & `citros-23.19.1/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/logger/logger_pg_handler.py` & `citros-23.19.1/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/parsers/__init__.py` & `citros-23.19.1/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/parsers/parser_ros2.py` & `citros-23.19.1/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/rosbag/__init__.py` & `citros-23.19.1/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/rosbag/reader_base.py` & `citros-23.19.1/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/rosbag/reader_mcap.py` & `citros-23.19.1/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros/rosbag/reader_sqlite.py` & `citros-23.19.1/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/citros.egg-info/PKG-INFO` & `citros-23.19.1/citros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.9
+Version: 23.19.1
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.9/citros.egg-info/SOURCES.txt` & `citros-23.19.1/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.17.9/setup.py` & `citros-23.19.1/setup.py`

 * *Files identical despite different names*

