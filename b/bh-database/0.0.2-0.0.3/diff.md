# Comparing `tmp/bh-database-0.0.2.tar.gz` & `tmp/bh-database-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bh-database-0.0.2.tar", last modified: Sun May  7 00:59:16 2023, max compression
+gzip compressed data, was "bh-database-0.0.3.tar", last modified: Tue May  9 00:06:04 2023, max compression
```

## Comparing `bh-database-0.0.2.tar` & `bh-database-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.832926 bh-database-0.0.2/
--rw-rw-rw-   0        0        0     2484 2023-05-07 00:59:16.832926 bh-database-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1858 2023-01-25 03:51:11.000000 bh-database-0.0.2/README.md
--rw-rw-rw-   0        0        0     1026 2023-05-07 00:55:04.000000 bh-database-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 00:59:16.832926 bh-database-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.788928 bh-database-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.796929 bh-database-0.0.2/src/bh_database/
--rw-rw-rw-   0        0        0       90 2023-01-25 04:17:39.000000 bh-database-0.0.2/src/bh_database/__init__.py
--rw-rw-rw-   0        0        0    22724 2023-05-06 02:18:13.000000 bh-database-0.0.2/src/bh_database/base_table.py
--rw-rw-rw-   0        0        0     2239 2023-01-25 03:51:11.000000 bh-database-0.0.2/src/bh_database/constant.py
--rw-rw-rw-   0        0        0    17779 2023-04-08 05:23:07.000000 bh-database-0.0.2/src/bh_database/core.py
--rw-rw-rw-   0        0        0     5120 2023-01-25 03:51:11.000000 bh-database-0.0.2/src/bh_database/paginator.py
-drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.816957 bh-database-0.0.2/src/bh_database.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-07 00:59:16.000000 bh-database-0.0.2/src/bh_database.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 00:59:16.831928 bh-database-0.0.2/tests/
--rw-rw-rw-   0        0        0     5782 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_01_core_database_postgresql.py
--rw-rw-rw-   0        0        0     5682 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_02_core_database_mysql.py
--rw-rw-rw-   0        0        0     3956 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_05_core_basesqlalchemy_postgresql.py
--rw-rw-rw-   0        0        0     3634 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_06_core_basesqlalchemy_mysql.py
--rw-rw-rw-   0        0        0     3394 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_11_paginator_postgresql.py
--rw-rw-rw-   0        0        0     3309 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_12_paginator_mysql.py
--rw-rw-rw-   0        0        0     6937 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_15_base_table_postgresql.py
--rw-rw-rw-   0        0        0     6413 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_16_base_table_mysql.py
--rw-rw-rw-   0        0        0     1651 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_17_base_table_methods.py
--rw-rw-rw-   0        0        0     1616 2023-01-25 03:51:11.000000 bh-database-0.0.2/tests/test_20_base_table_dunder.py
--rw-rw-rw-   0        0        0    19258 2023-04-08 12:11:15.000000 bh-database-0.0.2/tests/test_25_base_table_crud_methods_postgresql.py
--rw-rw-rw-   0        0        0    19133 2023-04-08 12:10:59.000000 bh-database-0.0.2/tests/test_26_base_table_crud_methods_mysql.py
--rw-rw-rw-   0        0        0     4335 2023-04-08 08:41:22.000000 bh-database-0.0.2/tests/test_30_base_table_exception_postgresql.py
--rw-rw-rw-   0        0        0     4270 2023-04-08 08:43:50.000000 bh-database-0.0.2/tests/test_31_base_table_exception_mysql.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.372944 bh-database-0.0.3/
+-rw-rw-rw-   0        0        0     2484 2023-05-09 00:06:04.370936 bh-database-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1858 2023-01-25 03:51:11.000000 bh-database-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1033 2023-05-08 23:24:08.000000 bh-database-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 00:06:04.372944 bh-database-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.310927 bh-database-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.317931 bh-database-0.0.3/src/bh_database/
+-rw-rw-rw-   0        0        0       90 2023-01-25 04:17:39.000000 bh-database-0.0.3/src/bh_database/__init__.py
+-rw-rw-rw-   0        0        0    22724 2023-05-06 02:18:13.000000 bh-database-0.0.3/src/bh_database/base_table.py
+-rw-rw-rw-   0        0        0     2239 2023-01-25 03:51:11.000000 bh-database-0.0.3/src/bh_database/constant.py
+-rw-rw-rw-   0        0        0    17779 2023-04-08 05:23:07.000000 bh-database-0.0.3/src/bh_database/core.py
+-rw-rw-rw-   0        0        0     5120 2023-01-25 03:51:11.000000 bh-database-0.0.3/src/bh_database/paginator.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.332926 bh-database-0.0.3/src/bh_database.egg-info/
+-rw-rw-rw-   0        0        0     2484 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.366935 bh-database-0.0.3/tests/
+-rw-rw-rw-   0        0        0     5782 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_01_core_database_postgresql.py
+-rw-rw-rw-   0        0        0     5682 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_02_core_database_mysql.py
+-rw-rw-rw-   0        0        0     3956 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_05_core_basesqlalchemy_postgresql.py
+-rw-rw-rw-   0        0        0     3634 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_06_core_basesqlalchemy_mysql.py
+-rw-rw-rw-   0        0        0     3423 2023-05-08 23:54:52.000000 bh-database-0.0.3/tests/test_11_paginator_postgresql.py
+-rw-rw-rw-   0        0        0     3336 2023-05-08 23:56:42.000000 bh-database-0.0.3/tests/test_12_paginator_mysql.py
+-rw-rw-rw-   0        0        0     6937 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_15_base_table_postgresql.py
+-rw-rw-rw-   0        0        0     6413 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_16_base_table_mysql.py
+-rw-rw-rw-   0        0        0     1651 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_17_base_table_methods.py
+-rw-rw-rw-   0        0        0     1616 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_20_base_table_dunder.py
+-rw-rw-rw-   0        0        0    19258 2023-04-08 12:11:15.000000 bh-database-0.0.3/tests/test_25_base_table_crud_methods_postgresql.py
+-rw-rw-rw-   0        0        0    19133 2023-04-08 12:10:59.000000 bh-database-0.0.3/tests/test_26_base_table_crud_methods_mysql.py
+-rw-rw-rw-   0        0        0     4335 2023-04-08 08:41:22.000000 bh-database-0.0.3/tests/test_30_base_table_exception_postgresql.py
+-rw-rw-rw-   0        0        0     4270 2023-04-08 08:43:50.000000 bh-database-0.0.3/tests/test_31_base_table_exception_mysql.py
```

### Comparing `bh-database-0.0.2/PKG-INFO` & `bh-database-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bh-database
-Version: 0.0.2
+Version: 0.0.3
 Summary: Database wrapper classes for SQLAlchemy.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_database
 Project-URL: documentation, https://bh-database.readthedocs.io/
 Keywords: SQLAlchemy,database,wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bh-database-0.0.2/README.md` & `bh-database-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/pyproject.toml` & `bh-database-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bh-database"
-version = "0.0.2"
+version = "0.0.3"
 description = "Database wrapper classes for SQLAlchemy."
 
 readme = "README.md"
 authors = [{ name = "Van Be Hai Nguyen", email = "behai_nguyen@hotmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
 ]
 keywords = ["SQLAlchemy", "database", "wrapper"]
 
 dependencies = [
     'tomli; python_version >= "3.10"',
     'SQLAlchemy', 
-    'psycopg2',
+    'psycopg2-binary',
     'mysql-connector-python',
     'bh_apistatus',
     'bh_utils'
 ]
 
 requires-python = ">=3.7"
```

### Comparing `bh-database-0.0.2/src/bh_database/base_table.py` & `bh-database-0.0.3/src/bh_database/base_table.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/src/bh_database/constant.py` & `bh-database-0.0.3/src/bh_database/constant.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/src/bh_database/core.py` & `bh-database-0.0.3/src/bh_database/core.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/src/bh_database/paginator.py` & `bh-database-0.0.3/src/bh_database/paginator.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/src/bh_database.egg-info/PKG-INFO` & `bh-database-0.0.3/src/bh_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bh-database
-Version: 0.0.2
+Version: 0.0.3
 Summary: Database wrapper classes for SQLAlchemy.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_database
 Project-URL: documentation, https://bh-database.readthedocs.io/
 Keywords: SQLAlchemy,database,wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bh-database-0.0.2/src/bh_database.egg-info/SOURCES.txt` & `bh-database-0.0.3/src/bh_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_01_core_database_postgresql.py` & `bh-database-0.0.3/tests/test_01_core_database_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_02_core_database_mysql.py` & `bh-database-0.0.3/tests/test_02_core_database_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_05_core_basesqlalchemy_postgresql.py` & `bh-database-0.0.3/tests/test_05_core_basesqlalchemy_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_06_core_basesqlalchemy_mysql.py` & `bh-database-0.0.3/tests/test_06_core_basesqlalchemy_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_11_paginator_postgresql.py` & `bh-database-0.0.3/tests/test_12_paginator_mysql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""Test the paginating functionality of BaseQuery class with PostgreSQL database.
+"""Test the paginating functionality of BaseQuery class with MySQL database.
 
-To run only tests in this module: pytest -m paginator_postgresql
+To run only tests in this module: pytest -m paginator_mysql
 
-To run all tests with PostgreSQL database: pytest -k _postgresql_ -v
+To run all tests with MySQL database: pytest -k _mysql_ -v
 
-On postgresql() fixture:
-------------------------
+On mysql() fixture:
+-------------------
 
 To ensure each test module can run independently and does not inadvertently produce
-any side effects on later tests, or tests in other modules, the postgresql() fixture
-needs to be called only once for this module.
+any side effects on later tests, or tests in other modules, the mysql() fixture needs 
+to be called only once for this module.
 
-The postgresql() fixture establishes a connection to the underlying PostgreSQL 
-Employees Sample Database. This call is similar to applications establish database
-connection on starting up.
+The mysql() fixture establishes a connection to the underlying MySQL Employees Sample 
+Database. This call is similar to applications establish database connection on starting up.
 """
 
 import pytest
 
 from bh_database import core
 
 from tests.employees import Employees
 
-@pytest.mark.paginator_postgresql
-def test_postgresql_prepare(postgresql):
+# @pytest.mark.paginator_mysql
+@pytest.mark.behai_only
+def test_mysql_prepare(mysql):
     """Database connection management.
 
     The purpose of this method is to establish the connection to the database.
-    The postgresql() method need to run FIRST and ONCE to establish the connection.
+    The mysql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
     # BaseSQLAlchemy is abstract, with no table name.
     assert core.BaseSQLAlchemy.query == None
 
     assert Employees.query != None
 
-@pytest.mark.paginator_postgresql
-def test_postgresql_paginator_01():
+@pytest.mark.paginator_mysql
+def test_mysql_paginator_01():
     """
     First page.
     """
     paginator = Employees.query.filter(Employees.last_name.ilike('%NAS%')).\
         order_by(Employees.emp_no).paginate(page=1, per_page=10)
 
     assert paginator != None
@@ -66,16 +66,16 @@
     assert employee['last_name'] == 'Nastansky'
 
     employee = paginator.items[9].as_dict()
     assert employee['emp_no'] == 15174
     assert employee['first_name'] == 'Otilia'
     assert employee['last_name'] == 'Salinas'
 
-@pytest.mark.paginator_postgresql
-def test_postgresql_paginator_02():
+@pytest.mark.paginator_mysql
+def test_mysql_paginator_02():
     """
     Last page.
     """
     paginator = Employees.query.filter(Employees.last_name.ilike('%NAS%')).\
         order_by(Employees.emp_no).paginate(page=58, per_page=10)
 
     assert paginator != None
```

### Comparing `bh-database-0.0.2/tests/test_12_paginator_mysql.py` & `bh-database-0.0.3/tests/test_11_paginator_postgresql.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-"""Test the paginating functionality of BaseQuery class with MySQL database.
+"""Test the paginating functionality of BaseQuery class with PostgreSQL database.
 
-To run only tests in this module: pytest -m paginator_mysql
+To run only tests in this module: pytest -m paginator_postgresql
 
-To run all tests with MySQL database: pytest -k _mysql_ -v
+To run all tests with PostgreSQL database: pytest -k _postgresql_ -v
 
-On mysql() fixture:
--------------------
+On postgresql() fixture:
+------------------------
 
 To ensure each test module can run independently and does not inadvertently produce
-any side effects on later tests, or tests in other modules, the mysql() fixture needs 
-to be called only once for this module.
+any side effects on later tests, or tests in other modules, the postgresql() fixture
+needs to be called only once for this module.
 
-The mysql() fixture establishes a connection to the underlying MySQL Employees Sample 
-Database. This call is similar to applications establish database connection on starting up.
+The postgresql() fixture establishes a connection to the underlying PostgreSQL 
+Employees Sample Database. This call is similar to applications establish database
+connection on starting up.
 """
 
 import pytest
 
 from bh_database import core
 
 from tests.employees import Employees
 
-@pytest.mark.paginator_mysql
-def test_mysql_prepare(mysql):
+# @pytest.mark.paginator_postgresql
+# @pytest.mark.behai_only
+def test_postgresql_prepare(postgresql):
     """Database connection management.
 
     The purpose of this method is to establish the connection to the database.
-    The mysql() method need to run FIRST and ONCE to establish the connection.
+    The postgresql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
     # BaseSQLAlchemy is abstract, with no table name.
     assert core.BaseSQLAlchemy.query == None
 
     assert Employees.query != None
 
-@pytest.mark.paginator_mysql
-def test_mysql_paginator_01():
+@pytest.mark.paginator_postgresql
+def test_postgresql_paginator_01():
     """
     First page.
     """
     paginator = Employees.query.filter(Employees.last_name.ilike('%NAS%')).\
         order_by(Employees.emp_no).paginate(page=1, per_page=10)
 
     assert paginator != None
@@ -65,16 +67,16 @@
     assert employee['last_name'] == 'Nastansky'
 
     employee = paginator.items[9].as_dict()
     assert employee['emp_no'] == 15174
     assert employee['first_name'] == 'Otilia'
     assert employee['last_name'] == 'Salinas'
 
-@pytest.mark.paginator_mysql
-def test_mysql_paginator_02():
+@pytest.mark.paginator_postgresql
+def test_postgresql_paginator_02():
     """
     Last page.
     """
     paginator = Employees.query.filter(Employees.last_name.ilike('%NAS%')).\
         order_by(Employees.emp_no).paginate(page=58, per_page=10)
 
     assert paginator != None
```

### Comparing `bh-database-0.0.2/tests/test_15_base_table_postgresql.py` & `bh-database-0.0.3/tests/test_15_base_table_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_16_base_table_mysql.py` & `bh-database-0.0.3/tests/test_16_base_table_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_17_base_table_methods.py` & `bh-database-0.0.3/tests/test_17_base_table_methods.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_20_base_table_dunder.py` & `bh-database-0.0.3/tests/test_20_base_table_dunder.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_25_base_table_crud_methods_postgresql.py` & `bh-database-0.0.3/tests/test_25_base_table_crud_methods_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_26_base_table_crud_methods_mysql.py` & `bh-database-0.0.3/tests/test_26_base_table_crud_methods_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_30_base_table_exception_postgresql.py` & `bh-database-0.0.3/tests/test_30_base_table_exception_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.2/tests/test_31_base_table_exception_mysql.py` & `bh-database-0.0.3/tests/test_31_base_table_exception_mysql.py`

 * *Files identical despite different names*

