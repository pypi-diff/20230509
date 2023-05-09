# Comparing `tmp/refractio-1.0.2.tar.gz` & `tmp/refractio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-1.0.2.tar", last modified: Fri Apr 28 11:15:32 2023, max compression
+gzip compressed data, was "refractio-1.0.3.tar", last modified: Tue May  9 10:20:07 2023, max compression
```

## Comparing `refractio-1.0.2.tar` & `refractio-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-28 11:15:32.462608 refractio-1.0.2/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1054 2023-04-28 11:15:32.461609 refractio-1.0.2/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      525 2023-04-28 11:13:39.000000 refractio-1.0.2/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-28 11:15:32.460609 refractio-1.0.2/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-28 10:17:05.000000 refractio-1.0.2/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13016 2023-04-28 10:17:05.000000 refractio-1.0.2/refractio/refractio.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-04-28 11:15:32.461609 refractio-1.0.2/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1054 2023-04-28 11:15:32.000000 refractio-1.0.2/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      227 2023-04-28 11:15:32.000000 refractio-1.0.2/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-04-28 11:15:32.000000 refractio-1.0.2/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      335 2023-04-28 11:15:32.000000 refractio-1.0.2/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-04-28 11:15:32.000000 refractio-1.0.2/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-04-28 11:15:32.462608 refractio-1.0.2/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1819 2023-04-28 11:15:11.000000 refractio-1.0.2/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-09 10:20:07.309095 refractio-1.0.3/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1124 2023-05-09 10:20:07.309095 refractio-1.0.3/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      564 2023-05-09 10:18:35.000000 refractio-1.0.3/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-09 10:20:07.308096 refractio-1.0.3/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-09 10:18:23.000000 refractio-1.0.3/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13351 2023-05-09 10:18:35.000000 refractio-1.0.3/refractio/refractio.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-09 10:20:07.308096 refractio-1.0.3/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1124 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      227 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-09 10:20:07.309095 refractio-1.0.3/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     2125 2023-05-09 10:18:35.000000 refractio-1.0.3/setup.py
```

### Comparing `refractio-1.0.2/PKG-INFO` & `refractio-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 1.0.2
+Version: 1.0.3
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -14,22 +14,34 @@
 Provides-Extra: all
 Provides-Extra: snowflake
 Provides-Extra: s3
 Provides-Extra: azureblob
 Provides-Extra: local
 Provides-Extra: sftp
 Provides-Extra: mysql
+Provides-Extra: hive
 
 
 Usage:
+
 without any dependencies: pip install refractio
+
 with all dependencies: pip install refractio[all]
+
 with snowflake: pip install refractio[snowflake]
+
 with s3: pip install refractio[s3]
+
 with azureblob: pip install refractio[azureblob]
+
 with local: pip install refractio[local]
+
 with sftp: pip install refractio[sftp]
+
 with mysql: pip install refractio[mysql]
 
+with hive: pip install refractio[hive]
+
+
 Source code is also available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git
```

### Comparing `refractio-1.0.2/README.md` & `refractio-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 with all dependencies: pip install refractio[all]
 with snowflake: pip install refractio[snowflake]
 with s3: pip install refractio[s3]
 with azureblob: pip install refractio[azureblob]
 with local: pip install refractio[local]
 with sftp: pip install refractio[sftp]
 with mysql: pip install refractio[mysql]
+with hive: pip install refractio[hive]
 
 Source code is also available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git
```

### Comparing `refractio-1.0.2/refractio/refractio.py` & `refractio-1.0.3/refractio/refractio.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 """Library to read and write dataframes"""
 
 import os
 import requests
 import pandas as pd
 
 
-def get_dataframe(ds_name, user_id=os.getenv("user_id"), project_id=os.getenv("project_id"),
-                  row_count=-1, strategy="top"):
+def get_dataframe(ds_name, project_id=os.getenv("project_id"), row_count=-1, strategy="top", user_id="1001"):
     """
     Param:
         ds_name,
-        user_id=os.getenv("user_id"),
         project_id=os.getenv("project_id"),
         row_count=-1,
         strategy="top"
+        user_id="1001"
     To get pandas dataframe.
     Need to install mosaic-connector-python for reading dataframe using connector backend,
     git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git@1.0.29.3
     """
     try:
-        print(f'user_id: {user_id}\nproject_id: {project_id}')
         url = f"http://connection-manager:80/connections/api/External/v1/external/getConnConfig/" \
-              f"{ds_name}/{user_id}/{project_id}"
+              f"{ds_name}/refract_user/{project_id}"    # user id hard coded, as it's not being used in API code.
         connection_details = requests.get(url, verify=False).json()
 
         if connection_details["params"]["READER"]["type"] == "RDBMS":
             if connection_details["params"]["READER"]["sub_type"] == "SNOWFLAKE":
                 data_frame = get_snowflake_df(connection_details, row_count, strategy)
             elif connection_details["params"]["READER"]["sub_type"] == "MYSQL":
                 data_frame = get_mysql_df(connection_details, row_count, strategy)
+            elif connection_details["params"]["READER"]["sub_type"] == "HIVE":
+                data_frame = get_hive_df(connection_details, row_count, strategy, user_id)
             else:
                 print("Reading dataframe using connector backend")
                 # Need to install, git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git
                 from connector.mosaicio import MosaicioConnector
                 connector = MosaicioConnector()
                 data_frame = connector.getPandasDataFrame(
                     param=connection_details["params"],
@@ -45,14 +45,15 @@
                 data_frame = get_s3_df(connection_details, row_count, strategy)
             elif connection_details["params"]["READER_STORAGE"]["type"] == "AZURE":
                 data_frame = get_azureblob_df(connection_details, row_count, strategy)
             elif connection_details["params"]["READER_STORAGE"]["type"] == "SFTP":
                 data_frame = get_sftp_df(connection_details, row_count, strategy)
         return data_frame
     except Exception as ex:
+        print(f'project_id: {project_id}')
         print(f"Connection details fetched: {connection_details}")
         print(f"Exception occurred in get_dataframe: {ex}")
 
 
 def get_local_dataframe(local_file_path, row_count=-1):
     """
     Param:
@@ -110,47 +111,51 @@
     )
     # Create cursor
     cur = con.cursor()
     if int(row_count) > 0:
         # Execute query
         cur.execute(f"SELECT * FROM {connection_details['params']['READER']['tables']} LIMIT {int(row_count)}")
     else:
-        cur.execute(f"SELECT * FROM {connection_details['params']['READER']['tables']};")
+        cur.execute(f"SELECT * FROM {connection_details['params']['READER']['tables']}")
 
     # Read results into a pandas DataFrame
     data_frame = cur.fetch_pandas_all()
 
     # Close cursor and connection
     cur.close()
     con.close()
     return data_frame
 
 
-def get_hive_df(connection_details, row_count, strategy):
+def get_hive_df(connection_details, row_count, strategy, user_id):
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
+        user_id: template image user id
     To read data frame form hive connection
     """
-    import pyhive
+    print("Reading dataframe from hive native connector")
 
-    # Establish connection to the Hive Server
-    conn = pyhive.hive.Connection(host=connection_details["params"]["READER"]["host"],
-                                  port=connection_details["params"]["READER"]["port"],
-                                  username=connection_details["params"]["READER"]["user"],
-                                  password=connection_details["params"]["READER"]["password"],
-                                  database=connection_details["params"]["READER"]["database"])
+    # Non Kerberos Connection
+    from impala.dbapi import connect
+    os.environ['USER'] = user_id
+    conn = connect(host=connection_details["params"]["READER"]["host"],
+                   port=int(connection_details["params"]["READER"]["port"]),
+                   auth_mechanism='PLAIN',
+                   user=connection_details["params"]["READER"]["user"],
+                   password=connection_details["params"]["READER"]["password"],
+                   database=connection_details["params"]["READER"]["database"])
 
     if int(row_count) > 0:
         # Generate query
         query = f"SELECT * FROM {connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
     else:
-        query = f"SELECT * FROM {connection_details['params']['READER']['tables']};"
+        query = f"SELECT * FROM {connection_details['params']['READER']['tables']}"
 
     # Read data from Hive
     data_frame = pd.read_sql(query, conn)
 
     # Close the connection
     conn.close()
     return data_frame
@@ -160,27 +165,28 @@
     """
     Param:
         connection_details: connection details dict
         row_count: number of rows to be fetched
         strategy: top/bottom
     To read data frame form mysql connection
     """
+    print("Reading dataframe from mysql native connector")
     import pymysql
 
     conn = pymysql.connect(host=connection_details["params"]["READER"]["host"],
                            port=int(connection_details["params"]["READER"]["port"]),
                            user=connection_details["params"]["READER"]["user"],
                            passwd=connection_details["params"]["READER"]["password"],
                            db=connection_details["params"]["READER"]["database"])
 
     if int(row_count) > 0:
         # Generate query
         query = f"SELECT * FROM {connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
     else:
-        query = f"SELECT * FROM {connection_details['params']['READER']['tables']};"
+        query = f"SELECT * FROM {connection_details['params']['READER']['tables']}"
     # Read data fromm mysql
     data_frame = pd.read_sql(query, con=conn)
     # Close connection
     conn.close()
     return data_frame
```

### Comparing `refractio-1.0.2/refractio.egg-info/PKG-INFO` & `refractio-1.0.3/refractio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 1.0.2
+Version: 1.0.3
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -14,22 +14,34 @@
 Provides-Extra: all
 Provides-Extra: snowflake
 Provides-Extra: s3
 Provides-Extra: azureblob
 Provides-Extra: local
 Provides-Extra: sftp
 Provides-Extra: mysql
+Provides-Extra: hive
 
 
 Usage:
+
 without any dependencies: pip install refractio
+
 with all dependencies: pip install refractio[all]
+
 with snowflake: pip install refractio[snowflake]
+
 with s3: pip install refractio[s3]
+
 with azureblob: pip install refractio[azureblob]
+
 with local: pip install refractio[local]
+
 with sftp: pip install refractio[sftp]
+
 with mysql: pip install refractio[mysql]
 
+with hive: pip install refractio[hive]
+
+
 Source code is also available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git
```

### Comparing `refractio-1.0.2/setup.py` & `refractio-1.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 LONG_DESCRIPTION = '''
-Usage:
-without any dependencies: pip install refractio
-with all dependencies: pip install refractio[all]
-with snowflake: pip install refractio[snowflake]
-with s3: pip install refractio[s3]
-with azureblob: pip install refractio[azureblob]
-with local: pip install refractio[local]
-with sftp: pip install refractio[sftp]
-with mysql: pip install refractio[mysql]
+Usage:\n
+without any dependencies: pip install refractio\n
+with all dependencies: pip install refractio[all]\n
+with snowflake: pip install refractio[snowflake]\n
+with s3: pip install refractio[s3]\n
+with azureblob: pip install refractio[azureblob]\n
+with local: pip install refractio[local]\n
+with sftp: pip install refractio[sftp]\n
+with mysql: pip install refractio[mysql]\n
+with hive: pip install refractio[hive]\n
 
 Source code is also available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git
 '''
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
         "openpyxl==3.1.2",
         "xlrd==2.0.1",
         "pysftp==0.2.9",
-        "pymysql==1.0.3"
+        "pymysql==1.0.3",
+        "impyla==0.16.2",
+        "thrift-sasl==0.4.3",
+        "pure-sasl==0.6.2",
+        "PyHive==0.6.3.dev0"
     ],
     "snowflake": [
         "snowflake-connector-python[pandas]==3.0.2"
     ],
     "s3": [
         "boto3==1.26.116"
     ],
@@ -40,14 +45,20 @@
         "xlrd==2.0.1",
     ],
     "sftp": [
         "pysftp==0.2.9"
     ],
     "mysql": [
         "pymysql==1.0.3"
+    ],
+    "hive": [
+        "impyla==0.16.2",
+        "thrift-sasl==0.4.3",
+        "pure-sasl==0.6.2",
+        "PyHive==0.6.3.dev0"
     ]
 }
 
 # Setting up
 setup(
     name="refractio",
     version=VERSION,
@@ -66,8 +77,7 @@
     ],
     extras_require=extras_require,
     project_urls={
         "Product": "https://www.fosfor.com/refract/",
         "Source": "https://git.lti-aiq.in/refract-sdk/refract-sdk",
     }
 )
-
```

