# Comparing `tmp/django_pg_simple_hll-0.1.0.tar.gz` & `tmp/django_pg_simple_hll-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pg_simple_hll-0.1.0.tar", max compression
+gzip compressed data, was "django_pg_simple_hll-0.1.1.tar", max compression
```

## Comparing `django_pg_simple_hll-0.1.0.tar` & `django_pg_simple_hll-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/LICENSE
--rw-r--r--   0        0        0    10638 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/__init__.py
--rw-r--r--   0        0        0      688 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/aggregate.py
--rw-r--r--   0        0        0      528 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.py
--rw-r--r--   0        0        0      344 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.reverse.sql
--rw-r--r--   0        0        0     5679 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.sql
--rw-r--r--   0        0        0        0 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/py.typed
--rw-r--r--   0        0        0     2957 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11780 1970-01-01 00:00:00.000000 django_pg_simple_hll-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/LICENSE
+-rw-r--r--   0        0        0    10927 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/aggregate.py
+-rw-r--r--   0        0        0      528 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.py
+-rw-r--r--   0        0        0      344 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.reverse.sql
+-rw-r--r--   0        0        0     5679 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.sql
+-rw-r--r--   0        0        0        0 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/py.typed
+-rw-r--r--   0        0        0     2957 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12069 1970-01-01 00:00:00.000000 django_pg_simple_hll-0.1.1/PKG-INFO
```

### Comparing `django_pg_simple_hll-0.1.0/LICENSE` & `django_pg_simple_hll-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.1.0/README.md` & `django_pg_simple_hll-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -145,27 +145,51 @@
  2023-05-03 00:00:00+00 |              122343
  2023-05-04 00:00:00+00 |              141375
 (7 rows)
 
 Time: 2121.662 ms (00:02.122)
 ```
 
-## SQL implementation
+## How to use
 
-This is a low-privilege implementation of [Hyperloglog](https://www.lix.polytechnique.fr/~fusy/Articles/FlFuGaMe07.pdf) approximate cardinality aggregation written in SQL and some [PL/pgSQL](https://www.postgresql.org/docs/current/plpgsql.html). Read about it [here](http://alejandro.giacometti.me/2023-03-30/hyperloglog-in-sql/),
+Install the package:
+
+```sh
+pip install django-pg-simple-hll
+```
+
+Add it to your Django `INSTALLED_APPS`:
+
+```python
+INSTALLED_APPS = [
+    ...
+    "django_pg_simple_hll",
+    ...
+]
+```
+
+Run migrations
+
+```sh
+django-admin migrate django_pg_simple_hll
+```
 
 ## Should I use this?
 
 If you can use [an optimised version](https://github.com/citusdata/postgresql-hll), you should use that. It will be faster - although I haven't done any benchmarks.
 
 Use this if you can't install extensions on your database, such as on [Amazon RDS](https://aws.amazon.com/rds/).
 
-## Performance
+## Notes on SQL implementation
+
+This is a low-privilege implementation of [Hyperloglog](https://www.lix.polytechnique.fr/~fusy/Articles/FlFuGaMe07.pdf) approximate cardinality aggregation written in SQL and some [PL/pgSQL](https://www.postgresql.org/docs/current/plpgsql.html). Read about it [here](http://alejandro.giacometti.me/2023-03-30/hyperloglog-in-sql/),
+
+## Notes on Performance
 
-This is not a scientific test, but here is an example of performance running on an M1 Macbook Pro, running Postgres 14 in Docker.
+This is not a scientific test, but here is an example of performance running on an M1 MacBook Pro, running Postgres 14 in Docker.
 
 For a dataset of 560k rows and 140k unique values a precision of 6 matches the speed of `COUNT(DISTINCT ...)`:
 
 ```sql
 
 select count(user_uuid) from testapp_session;
  count
```

### Comparing `django_pg_simple_hll-0.1.0/django_pg_simple_hll/aggregate.py` & `django_pg_simple_hll-0.1.1/django_pg_simple_hll/aggregate.py`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.py` & `django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.sql` & `django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.sql`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.1.0/pyproject.toml` & `django_pg_simple_hll-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django_pg_simple_hll"
-version = "0.1.0"
+version = "0.1.1"
 description = "A low-privilege implementation of hyperloglog for django and postgres"
 authors = ["Beauhurst <opensource@beauhurst.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
   "Framework :: Django",
```

### Comparing `django_pg_simple_hll-0.1.0/PKG-INFO` & `django_pg_simple_hll-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pg-simple-hll
-Version: 0.1.0
+Version: 0.1.1
 Summary: A low-privilege implementation of hyperloglog for django and postgres
 License: MIT
 Author: Beauhurst
 Author-email: opensource@beauhurst.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -174,27 +174,51 @@
  2023-05-03 00:00:00+00 |              122343
  2023-05-04 00:00:00+00 |              141375
 (7 rows)
 
 Time: 2121.662 ms (00:02.122)
 ```
 
-## SQL implementation
+## How to use
 
-This is a low-privilege implementation of [Hyperloglog](https://www.lix.polytechnique.fr/~fusy/Articles/FlFuGaMe07.pdf) approximate cardinality aggregation written in SQL and some [PL/pgSQL](https://www.postgresql.org/docs/current/plpgsql.html). Read about it [here](http://alejandro.giacometti.me/2023-03-30/hyperloglog-in-sql/),
+Install the package:
+
+```sh
+pip install django-pg-simple-hll
+```
+
+Add it to your Django `INSTALLED_APPS`:
+
+```python
+INSTALLED_APPS = [
+    ...
+    "django_pg_simple_hll",
+    ...
+]
+```
+
+Run migrations
+
+```sh
+django-admin migrate django_pg_simple_hll
+```
 
 ## Should I use this?
 
 If you can use [an optimised version](https://github.com/citusdata/postgresql-hll), you should use that. It will be faster - although I haven't done any benchmarks.
 
 Use this if you can't install extensions on your database, such as on [Amazon RDS](https://aws.amazon.com/rds/).
 
-## Performance
+## Notes on SQL implementation
+
+This is a low-privilege implementation of [Hyperloglog](https://www.lix.polytechnique.fr/~fusy/Articles/FlFuGaMe07.pdf) approximate cardinality aggregation written in SQL and some [PL/pgSQL](https://www.postgresql.org/docs/current/plpgsql.html). Read about it [here](http://alejandro.giacometti.me/2023-03-30/hyperloglog-in-sql/),
+
+## Notes on Performance
 
-This is not a scientific test, but here is an example of performance running on an M1 Macbook Pro, running Postgres 14 in Docker.
+This is not a scientific test, but here is an example of performance running on an M1 MacBook Pro, running Postgres 14 in Docker.
 
 For a dataset of 560k rows and 140k unique values a precision of 6 matches the speed of `COUNT(DISTINCT ...)`:
 
 ```sql
 
 select count(user_uuid) from testapp_session;
  count
```

