# Comparing `tmp/redis_elastic-1.0.0.tar.gz` & `tmp/redis_elastic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_elastic-1.0.0.tar", last modified: Thu May  4 22:58:52 2023, max compression
+gzip compressed data, was "redis_elastic-1.0.1.tar", last modified: Mon May  8 23:11:50 2023, max compression
```

## Comparing `redis_elastic-1.0.0.tar` & `redis_elastic-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/Develop/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-04 19:00:06.000000 redis_elastic-1.0.0/Develop/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2682 2023-04-27 18:32:13.000000 redis_elastic-1.0.0/Develop/extract.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1323 2023-05-04 22:53:19.000000 redis_elastic-1.0.0/Develop/tools.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3120 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2697 2023-05-04 22:51:13.000000 redis_elastic-1.0.0/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/Warehouse/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-1.0.0/Warehouse/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4988 2023-05-04 22:48:21.000000 redis_elastic-1.0.0/Warehouse/redis_elastic.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/redis_elastic.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3120 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      307 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       71 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       18 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-04 22:58:52.387008 redis_elastic-1.0.0/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      876 2023-05-04 22:54:12.000000 redis_elastic-1.0.0/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 23:11:50.741869 redis_elastic-1.0.1/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 23:11:50.737869 redis_elastic-1.0.1/Develop/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-04 19:00:06.000000 redis_elastic-1.0.1/Develop/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2682 2023-04-27 18:32:13.000000 redis_elastic-1.0.1/Develop/extract.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1323 2023-05-04 22:53:19.000000 redis_elastic-1.0.1/Develop/tools.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3082 2023-05-08 23:11:50.741869 redis_elastic-1.0.1/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2659 2023-05-08 23:10:51.000000 redis_elastic-1.0.1/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 23:11:50.737869 redis_elastic-1.0.1/Warehouse/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-1.0.1/Warehouse/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5089 2023-05-08 22:42:24.000000 redis_elastic-1.0.1/Warehouse/redis_elastic.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 23:11:50.741869 redis_elastic-1.0.1/redis_elastic.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3082 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      307 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       71 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       18 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-08 23:11:50.741869 redis_elastic-1.0.1/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      876 2023-05-08 23:10:51.000000 redis_elastic-1.0.1/setup.py
```

### Comparing `redis_elastic-1.0.0/Develop/extract.py` & `redis_elastic-1.0.1/Develop/extract.py`

 * *Files identical despite different names*

### Comparing `redis_elastic-1.0.0/Develop/tools.py` & `redis_elastic-1.0.1/Develop/tools.py`

 * *Files identical despite different names*

### Comparing `redis_elastic-1.0.0/PKG-INFO` & `redis_elastic-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: redis_elastic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 1.0.0 (Stable release)
+version 1.0.1 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -44,16 +44,14 @@
     "host": "127.0.0.1",
     "port": "5432",
     "user": "etl",
     "password": "123",
     "database": "customer"
 }
 
-list_fields = ['id', 'name', 'code']
-
 query = """Select rp.id,rp.name,rp.code from res_partner rp"""
 
 my_object = Settings_redis_elastic("localhost", "6379", "http://localhost:9200")
 my_object.fusion(query, "_test", "test", 10, 20, postgres)
 ``` 
 
 ## Documentation
```

### Comparing `redis_elastic-1.0.0/README.md` & `redis_elastic-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 1.0.0 (Stable release)
+version 1.0.1 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -33,16 +33,14 @@
     "host": "127.0.0.1",
     "port": "5432",
     "user": "etl",
     "password": "123",
     "database": "customer"
 }
 
-list_fields = ['id', 'name', 'code']
-
 query = """Select rp.id,rp.name,rp.code from res_partner rp"""
 
 my_object = Settings_redis_elastic("localhost", "6379", "http://localhost:9200")
 my_object.fusion(query, "_test", "test", 10, 20, postgres)
 ``` 
 
 ## Documentation
```

### Comparing `redis_elastic-1.0.0/Warehouse/redis_elastic.py` & `redis_elastic-1.0.1/Warehouse/redis_elastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         @cache_function_results
         def cached_query_dates():
             return query_dates()
 
         def update_cache():
             while True:
                 # Obtener la versión actual del caché
-                cached_version = redis_client.get(f"query_version{redis_name}").decode("utf8")
+                cached_version = redis_client.get(f"query_version{redis_name}")
 
                 # Obtener la versión actual de la consulta en la base de datos
                 db_version = str(query_dates().values)
 
                 # Si la versión en la base de datos es diferente a la versión en caché,
                 # actualizar el caché y la versión en caché
                 if cached_version != db_version:
@@ -93,17 +93,19 @@
             # convertir los datos de bytes a una cadena de caracteres y luego a un diccionario
             # En caso de no realizar el ast, lo parse a un json
             try:
                 cached_query_odoo = ast.literal_eval(cached_query_redis.decode())
                 df = pd.DataFrame(cached_query_odoo)
 
             except Exception:
-                data = json.loads(cached_query_redis)
-                df = pd.DataFrame.from_dict(data)
-
+                if cached_query_redis is None:
+                    df = pd.DataFrame()
+                else:
+                    data = json.loads(cached_query_redis)
+                    df = pd.DataFrame.from_dict(data)
             return df
 
         def elastic_indexation():
             client = Elasticsearch(self.url_elasticsearch)
 
             # Obtiene la variable de columnas de la función query dates
             get_list_columns = query_dates().columns.tolist()
```

### Comparing `redis_elastic-1.0.0/redis_elastic.egg-info/PKG-INFO` & `redis_elastic-1.0.1/redis_elastic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: redis-elastic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 1.0.0 (Stable release)
+version 1.0.1 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -44,16 +44,14 @@
     "host": "127.0.0.1",
     "port": "5432",
     "user": "etl",
     "password": "123",
     "database": "customer"
 }
 
-list_fields = ['id', 'name', 'code']
-
 query = """Select rp.id,rp.name,rp.code from res_partner rp"""
 
 my_object = Settings_redis_elastic("localhost", "6379", "http://localhost:9200")
 my_object.fusion(query, "_test", "test", 10, 20, postgres)
 ``` 
 
 ## Documentation
```

### Comparing `redis_elastic-1.0.0/setup.py` & `redis_elastic-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 
 setup(
     name="redis_elastic",
-    version="1.0.0",
+    version="1.0.1",
     description="Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch",
     install_requires=[
         "setuptools",
         "psycopg2",
         "psycopg2-binary",
         "redis",
         "elasticsearch==7.13.4",
```

