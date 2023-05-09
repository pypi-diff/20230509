# Comparing `tmp/braincube-aws-core-alpha-0.0.22.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.22.tar", last modified: Mon May  8 14:19:41 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.23.tar", last modified: Tue May  9 09:48:46 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.22.tar` & `braincube-aws-core-alpha-0.0.23.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.910251 braincube-aws-core-alpha-0.0.22/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.22/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 14:19:41.910528 braincube-aws-core-alpha-0.0.22/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.22/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.22/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-08 14:19:41.912641 braincube-aws-core-alpha-0.0.22/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.22/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.895884 braincube-aws-core-alpha-0.0.22/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.901380 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.901767 braincube-aws-core-alpha-0.0.22/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.904018 braincube-aws-core-alpha-0.0.22/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1243 2023-05-08 14:04:48.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      248 2023-05-08 13:56:23.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2434 2023-05-08 10:25:13.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    30110 2023-05-08 12:48:30.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.905482 braincube-aws-core-alpha-0.0.22/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      575 2023-05-08 13:58:47.000000 braincube-aws-core-alpha-0.0.22/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4059 2023-05-08 14:00:15.000000 braincube-aws-core-alpha-0.0.22/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.907900 braincube-aws-core-alpha-0.0.22/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2835 2023-05-08 12:13:01.000000 braincube-aws-core-alpha-0.0.22/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3700 2023-05-08 14:01:38.000000 braincube-aws-core-alpha-0.0.22/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3597 2023-05-08 14:02:55.000000 braincube-aws-core-alpha-0.0.22/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.909738 braincube-aws-core-alpha-0.0.22/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-07 19:45:48.000000 braincube-aws-core-alpha-0.0.22/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1391 2023-05-08 14:03:54.000000 braincube-aws-core-alpha-0.0.22/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.636150 braincube-aws-core-alpha-0.0.23/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.23/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-09 09:48:46.636482 braincube-aws-core-alpha-0.0.23/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.23/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.23/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-09 09:48:46.637814 braincube-aws-core-alpha-0.0.23/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.23/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.618811 braincube-aws-core-alpha-0.0.23/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.622977 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.623454 braincube-aws-core-alpha-0.0.23/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.626951 braincube-aws-core-alpha-0.0.23/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1243 2023-05-08 14:04:48.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      248 2023-05-08 13:56:23.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3354 2023-05-09 09:28:51.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    30491 2023-05-09 08:33:33.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.629611 braincube-aws-core-alpha-0.0.23/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      575 2023-05-08 13:58:47.000000 braincube-aws-core-alpha-0.0.23/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4178 2023-05-08 17:05:17.000000 braincube-aws-core-alpha-0.0.23/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.633000 braincube-aws-core-alpha-0.0.23/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2835 2023-05-08 12:13:01.000000 braincube-aws-core-alpha-0.0.23/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3736 2023-05-08 16:38:53.000000 braincube-aws-core-alpha-0.0.23/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3597 2023-05-08 14:02:55.000000 braincube-aws-core-alpha-0.0.23/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.635296 braincube-aws-core-alpha-0.0.23/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-07 19:45:48.000000 braincube-aws-core-alpha-0.0.23/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1391 2023-05-08 14:03:54.000000 braincube-aws-core-alpha-0.0.23/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.22/LICENSE` & `braincube-aws-core-alpha-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.22/PKG-INFO` & `braincube-aws-core-alpha-0.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.22
+Version: 0.0.23
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.22/README.md` & `braincube-aws-core-alpha-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.22/setup.cfg` & `braincube-aws-core-alpha-0.0.23/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.22
+version = 0.0.23
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.22
+Version: 0.0.23
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.23/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.23/src/core/dal/postgres_connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
 import json
-from asyncpg import create_pool, connect, Connection
+from contextlib import asynccontextmanager
+
 from asyncpg.pool import Pool
+from asyncpg import create_pool, connect, Connection
+
+from .database_errors import DatabaseError
 
 
 async def get(user: str = os.environ["PG_USER"], password: str = os.environ["PG_PASSWORD"],
               database: str = os.environ["PG_DATABASE"], host: str = os.environ["PG_HOST"],
               port: int = os.environ["PG_PORT"]) -> Connection:
     """Retrieve a database connection.
     :param user: Database user.
@@ -41,11 +45,31 @@
 
     return await create_pool(user=user, password=password, database=database, host=host, port=port,
                              min_size=min_size, max_size=max_size,
                              max_inactive_connection_lifetime=max_inactive_connection_lifetime,
                              init=__init)
 
 
+@asynccontextmanager
+async def transactional(pool: Pool = None, connection: Connection = None):
+    """Create a database transaction. If connection is provided then a transaction is created immediately, if not then
+    a transaction established using a connection acquired from provided connection pool.
+    :param pool: (asyncpg) Connection pool.
+    :param connection: (asyncpg) Connection.
+    :raise DatabaseError: If nor connection neither connection pool are specified.
+    :return: Transactional connection.
+    """
+
+    if connection:
+        async with connection.transaction():
+            yield connection
+    elif pool:
+        async with pool.acquire() as connection, connection.transaction():
+            yield connection
+    else:
+        raise DatabaseError("nor connection neither connection pool are specified")
+
+
 async def __init(conn: Connection):
     await conn.set_type_codec("uuid", encoder=str, decoder=str, schema="pg_catalog")
     await conn.set_type_codec("numeric", encoder=str, decoder=float, schema="pg_catalog")
     await conn.set_type_codec("jsonb", encoder=json.dumps, decoder=json.loads, schema="pg_catalog")
```

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.23/src/core/dal/postgres_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,23 +294,34 @@
                         order: list[Order] | None = None,
                         connection: Connection | None = None) -> list[dict[str, any]]:
 
         q, _ = self._init_select_query(aliases, criterion, order)
 
         return await self._fetch(q, connection=connection)
 
-    # TODO: Optional connection
-    async def _find_many(self, connection: Connection,
-                         aliases: list[str] | None = None,
+    async def _find_many(self, aliases: list[str] | None = None,
                          criterion: Criterion | None = None,
                          page: Pageable = Pageable(),
-                         order: list[Order] | None = None) -> Page | Top | list[dict[str, any]]:
+                         order: list[Order] | None = None,
+                         connection: Connection | None = None) -> Page | Top:
+
+        if connection:
+            return await self.__find_many(connection, aliases, criterion, page, order)
+        async with self._pool.acquire() as connection_:
+            return await self.__find_many(connection_, aliases, criterion, page, order)
+
+    async def __find_many(self, connection: Connection,
+                          aliases: list[str] | None = None,
+                          criterion: Criterion | None = None,
+                          page: Pageable = Pageable(),
+                          order: list[Order] | None = None) -> Page | Top:
 
         if page.top_size < 0:
-            return await self._find_all(aliases, criterion, order, connection)
+            data = await self._find_all(aliases, criterion, order, connection)
+            return Top(data, page.top_size, False)
 
         start = time.time()
 
         calc_top = page.top_size > 0
         q, cq = self._init_select_query(aliases, criterion, order, count_query=not calc_top)
 
         # top implementation
@@ -453,30 +464,27 @@
 
         return await self._find_all(aliases, criterion, order, connection)
 
     async def find_many(self, aliases: list[str] | None = None,
                         conditions: list[Condition] | None = None,
                         page: Pageable = Pageable(),
                         order: list[Order] | None = None,
-                        connection: Connection | None = None) -> Page | Top | list[dict[str, any]]:
+                        connection: Connection | None = None) -> Page | Top:
         """Find records from passed filters using paging.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param page: Limit and offset of the query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records wrapped by Page or Top dataclass.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
-        if connection:
-            return await self._find_many(connection, aliases, criterion, page, order)
-        async with self._pool.acquire() as connection_:
-            return await self._find_many(connection_, aliases, criterion, page, order)
+        return await self._find_many(aliases, criterion, page, order, connection)
 
     async def insert(self, data: BaseModel | dict[str, any],
                      returning_aliases: list[str] | None = None,
                      connection: Connection | None = None) -> dict[str, any]:
         """Insert one record from dictionary.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
```

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.23/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.23/src/core/di/injector.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 class _Injector:
     """Module that used in order to resolve dependencies from components or route functions."""
 
     dependencies: list[Dependency] = list()
 
     @staticmethod
+    def init_config():
+        _Injector.dependencies.append(Dependency(Scope.singleton, Pool, factory=get_pool))
+        # here put any other dependency you want to provide out of the box
+
+    @staticmethod
     def inject(name: str | None = None, scope: Scope = Scope.singleton, qualifier: str | None = None):
         def _inject(component):
             data = qualifier_to_data(qualifier) if qualifier else dict()
             if isfunction(component):
                 cls = component.__annotations__.get("return")
                 if not cls:
                     raise ValueError(f"injected function '{component.__name__}' must specify return type.")
@@ -33,19 +38,14 @@
 
     @staticmethod
     async def provide(cls: Type[T], name: str | None = None) -> T:
 
         matched = list(filter(lambda d: (d.cls is cls or issubclass(d.cls, cls)) and
                                         (d.name == name if name else d.name is None), _Injector.dependencies))
 
-        if not matched and cls is Pool:
-            instance = await get_pool()
-            _Injector.dependencies.append(Dependency(Scope.singleton, Pool, instance=instance))
-            return instance
-
         if not matched:
             raise ValueError(f"component name:'{name}', class:'{cls}' not found.")
         if len(matched) > 1:
             raise ValueError(f"multiple matching components have been found for class: '{cls}'")
         if not matched[0].instance:
             nested = list()
             if matched[0].params:
@@ -62,14 +62,20 @@
         return matched[0].instance
 
     @staticmethod
     def register_instance(cls: Type[T], instance: T, name: str | None = None):
         _Injector.dependencies.append(Dependency(Scope.singleton, cls, name=name, instance=instance))
 
 
+def init_config():
+    """Dependencies configuration using environment variables."""
+
+    _Injector.init_config()
+
+
 def inject(name: str | None = None, scope: Scope = Scope.singleton, qualifier: str | None = None):
     """Inject a class or function.
     :param name: Component name.
     :param scope: Class of the Scope in which to resolve.
     :param qualifier: Comma separated string, used to specify components by name in case of multiple implementations.
     """
```

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.23/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.23/src/core/rest/app_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inspect import signature
 from dataclasses import dataclass
 from typing import get_args, get_origin
 
 from ..utils.convert import JSONEncoder
 from ..utils.data import import_modules, import_directories
 from ..di.data import qualifier_to_data
-from ..di.injector import provide
+from ..di.injector import init_config, provide
 from .data import HTTPRequest, HTTPResponse, http_event_to_request
 from .app_controller import AppController
 
 
 @dataclass()
 class _Route:
     func: callable
@@ -40,14 +40,16 @@
         root = os.environ["ROOT_DIRECTORY"] if os.environ.get("ROOT_DIRECTORY") else "/var/task/"
 
         if directories:
             import_directories(root, directories)
         elif os.environ.get("IMPORT_DIRECTORIES"):
             import_directories(root, os.environ["IMPORT_DIRECTORIES"].split(","))
 
+        init_config()
+
         routes = dict()
 
         for c in controllers:
             routes.update(c.routes)
 
         for resource, methods in routes.items():
             for method, handler in methods.items():
```

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.23/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.23/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.22/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.23/src/core/utils/data.py`

 * *Files identical despite different names*

