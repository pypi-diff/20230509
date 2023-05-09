# Comparing `tmp/nbdbsession-0.2.5.tar.gz` & `tmp/nbdbsession-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdbsession-0.2.5.tar", last modified: Mon Mar 20 10:19:36 2023, max compression
+gzip compressed data, was "nbdbsession-0.2.7.tar", last modified: Tue May  9 07:50:16 2023, max compression
```

## Comparing `nbdbsession-0.2.5.tar` & `nbdbsession-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-03-20 10:19:36.737273 nbdbsession-0.2.5/
--rw-r--r--   0 david      (501) staff       (20)     1067 2023-02-07 21:02:35.000000 nbdbsession-0.2.5/LICENSE
--rw-r--r--   0 david      (501) staff       (20)     2904 2023-03-20 10:19:36.736577 nbdbsession-0.2.5/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     2626 2023-03-20 10:19:15.000000 nbdbsession-0.2.5/README.md
--rw-r--r--   0 david      (501) staff       (20)       38 2023-03-20 10:19:36.737503 nbdbsession-0.2.5/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      633 2023-03-20 10:11:47.000000 nbdbsession-0.2.5/setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-03-20 10:19:36.716946 nbdbsession-0.2.5/src/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-03-20 10:19:36.728707 nbdbsession-0.2.5/src/nbdbsession/
--rw-r--r--   0 david      (501) staff       (20)        0 2023-02-07 21:02:35.000000 nbdbsession-0.2.5/src/nbdbsession/__init__.py
--rw-r--r--   0 david      (501) staff       (20)      556 2023-02-07 21:02:35.000000 nbdbsession-0.2.5/src/nbdbsession/connection_string.py
--rw-r--r--   0 david      (501) staff       (20)       56 2023-02-07 21:02:35.000000 nbdbsession-0.2.5/src/nbdbsession/exceptions.py
--rw-r--r--   0 david      (501) staff       (20)      337 2023-03-20 10:14:08.000000 nbdbsession-0.2.5/src/nbdbsession/ipython_magic.py
--rw-r--r--   0 david      (501) staff       (20)     2050 2023-02-24 10:47:58.000000 nbdbsession-0.2.5/src/nbdbsession/settings.py
--rw-r--r--   0 david      (501) staff       (20)     1379 2023-03-20 10:13:24.000000 nbdbsession-0.2.5/src/nbdbsession/sqlconn.py
--rw-r--r--   0 david      (501) staff       (20)     1281 2023-02-07 21:02:35.000000 nbdbsession-0.2.5/src/nbdbsession/ssh_tunnel.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-03-20 10:19:36.735480 nbdbsession-0.2.5/src/nbdbsession.egg-info/
--rw-r--r--   0 david      (501) staff       (20)     2904 2023-03-20 10:19:36.000000 nbdbsession-0.2.5/src/nbdbsession.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      395 2023-03-20 10:19:36.000000 nbdbsession-0.2.5/src/nbdbsession.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-03-20 10:19:36.000000 nbdbsession-0.2.5/src/nbdbsession.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)       12 2023-03-20 10:19:36.000000 nbdbsession-0.2.5/src/nbdbsession.egg-info/top_level.txt
+drwxr-xr-x   0 davidkuda   (502) staff       (20)        0 2023-05-09 07:50:16.178354 nbdbsession-0.2.7/
+-rw-r--r--   0 davidkuda   (502) staff       (20)     1067 2023-03-27 18:42:51.000000 nbdbsession-0.2.7/LICENSE
+-rw-r--r--   0 davidkuda   (502) staff       (20)     3583 2023-05-09 07:50:16.178243 nbdbsession-0.2.7/PKG-INFO
+-rw-r--r--   0 davidkuda   (502) staff       (20)     3305 2023-05-09 07:50:00.000000 nbdbsession-0.2.7/README.md
+-rw-r--r--   0 davidkuda   (502) staff       (20)       38 2023-05-09 07:50:16.178388 nbdbsession-0.2.7/setup.cfg
+-rw-r--r--   0 davidkuda   (502) staff       (20)      633 2023-05-08 14:55:44.000000 nbdbsession-0.2.7/setup.py
+drwxr-xr-x   0 davidkuda   (502) staff       (20)        0 2023-05-09 07:50:16.176085 nbdbsession-0.2.7/src/
+drwxr-xr-x   0 davidkuda   (502) staff       (20)        0 2023-05-09 07:50:16.177427 nbdbsession-0.2.7/src/nbdbsession/
+-rw-r--r--   0 davidkuda   (502) staff       (20)        0 2023-03-27 18:42:51.000000 nbdbsession-0.2.7/src/nbdbsession/__init__.py
+-rw-r--r--   0 davidkuda   (502) staff       (20)      556 2023-03-27 18:42:51.000000 nbdbsession-0.2.7/src/nbdbsession/connection_string.py
+-rw-r--r--   0 davidkuda   (502) staff       (20)      106 2023-05-08 13:22:19.000000 nbdbsession-0.2.7/src/nbdbsession/exceptions.py
+-rw-r--r--   0 davidkuda   (502) staff       (20)      557 2023-03-27 18:42:51.000000 nbdbsession-0.2.7/src/nbdbsession/ipython_magic.py
+-rw-r--r--   0 davidkuda   (502) staff       (20)     3036 2023-05-08 14:42:48.000000 nbdbsession-0.2.7/src/nbdbsession/settings.py
+-rw-r--r--   0 davidkuda   (502) staff       (20)     1379 2023-05-08 14:56:01.000000 nbdbsession-0.2.7/src/nbdbsession/sqlconn.py
+-rw-r--r--   0 davidkuda   (502) staff       (20)     1281 2023-03-27 18:42:51.000000 nbdbsession-0.2.7/src/nbdbsession/ssh_tunnel.py
+drwxr-xr-x   0 davidkuda   (502) staff       (20)        0 2023-05-09 07:50:16.177852 nbdbsession-0.2.7/src/nbdbsession.egg-info/
+-rw-r--r--   0 davidkuda   (502) staff       (20)     3583 2023-05-09 07:50:16.000000 nbdbsession-0.2.7/src/nbdbsession.egg-info/PKG-INFO
+-rw-r--r--   0 davidkuda   (502) staff       (20)      429 2023-05-09 07:50:16.000000 nbdbsession-0.2.7/src/nbdbsession.egg-info/SOURCES.txt
+-rw-r--r--   0 davidkuda   (502) staff       (20)        1 2023-05-09 07:50:16.000000 nbdbsession-0.2.7/src/nbdbsession.egg-info/dependency_links.txt
+-rw-r--r--   0 davidkuda   (502) staff       (20)       12 2023-05-09 07:50:16.000000 nbdbsession-0.2.7/src/nbdbsession.egg-info/top_level.txt
+drwxr-xr-x   0 davidkuda   (502) staff       (20)        0 2023-05-09 07:50:16.177974 nbdbsession-0.2.7/tests/
+-rw-r--r--   0 davidkuda   (502) staff       (20)      933 2023-05-08 14:45:11.000000 nbdbsession-0.2.7/tests/test_parse_toml_settings.py
```

### Comparing `nbdbsession-0.2.5/LICENSE` & `nbdbsession-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdbsession-0.2.5/PKG-INFO` & `nbdbsession-0.2.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,52 @@
-Metadata-Version: 2.1
-Name: nbdbsession
-Version: 0.2.5
-Summary: Config mgt to connect to databases from jupyter notebooks.
-Home-page: https://github.com/davidkuda/jupyter_database_io
-Author: David Kuda
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nbdbsession
 
 __This code helps you to manage connections to sql databases in jupyter notebooks.__
 
 `nbdbsession` stands for "notebook database session".
 
-I use notebooks all the time to connect to databases like postgres. With the notebook sessions, I often work on PoCs (proof of concept), on presentations or on debugging.
+I use notebooks very often to connect to databases like postgres. With the notebook sessions, I often work on PoCs (proof of concept), on presentations or on debugging.
 
-[`catherinedevlin`](https://github.com/catherinedevlin) has created open source software that I love: [`ipython-sql`](https://pypi.org/project/ipython-sql/).
+[`catherinedevlin`](https://github.com/catherinedevlin) has created open source software that I love: [`ipython-sql`](https://pypi.org/project/ipython-sql/).  (Note: There was a fork of this project: [`jupy-sql`](https://jupysql.ploomber.io/en/latest/quick-start.html). The original version is not actively maintained, and does not work with sqlalchemy version 2 that was [released in January 2023](https://docs.sqlalchemy.org/en/20/changelog/changelog_20.html#change-2.0.0))
 
 This code -- `nbdbsession` -- lets you connect to sql databases from your notebook, and run queries.
 
-### How to publish a pkg to PyPI
-
-```sh
-# package code
-python setup.py sdist
-
-# upload code to PyPI
-twine upload dist/*
-
-# update pkg
-pip install nbdbsession --upgrade
-```
-
 ### How To Use `nbdbsession`
 
 First, install it:
 
 ```
 pip install nbdbsession
 ```
 
 Then, in your git repository where you start your notebook, create a `.settings.toml` file with your database login credentials:
 
+You need to define your database credentials in a toml file. The toml file should look like this:
+
 ```toml
-# .settings.toml on top level of your git repo
+# either: .settings.toml on top level of your git repo
+# or:     $HOME/.nbdbsession.creds.toml
+
 [davidkuda]
 db_driver = "postgresql"
 database = "dev"
 user = "davidkuda"
 password = "${DB_PASSWORD}" # you can use environment variables
 db_url = "localhost"
 port = 5439
 # the ssh command is optional:
 ssh_cmd = "ssh -fL 5432:db.kuda.ai:5432"
 ```
 
+nbdbsession will scan three places for a toml file and will choose the first hit in this order:
+
+- env var `$SETTINGS_FILE_PATH`
+- (root directory of a git project)/.settings.toml
+- `$HOME/.nbdbsession.creds.toml`
+
 Finally, you can connect to your database in your notebook by running the following code in a cell:
 
 ```python
 from nbdbsession.sqlconn import connect
 
 connect("davidkuda") # note: this is the name as defined in .settings.toml
 ```
@@ -80,14 +67,27 @@
     *
 FROM
     table
 LIMIT
     10;
 ```
 
+### How to publish a pkg to PyPI
+
+```sh
+# package code
+python setup.py sdist
+
+# upload code to PyPI
+twine upload dist/*
+
+# update pkg
+pip install nbdbsession --upgrade
+```
+
 ### Managing the conn without this repo
 
 In the usual way, you would create a connection string, something like this:
 
 ```python
 %load_ext sql
```

### Comparing `nbdbsession-0.2.5/README.md` & `nbdbsession-0.2.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,62 @@
+Metadata-Version: 2.1
+Name: nbdbsession
+Version: 0.2.7
+Summary: Config mgt to connect to databases from jupyter notebooks.
+Home-page: https://github.com/davidkuda/jupyter_database_io
+Author: David Kuda
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nbdbsession
 
 __This code helps you to manage connections to sql databases in jupyter notebooks.__
 
 `nbdbsession` stands for "notebook database session".
 
-I use notebooks all the time to connect to databases like postgres. With the notebook sessions, I often work on PoCs (proof of concept), on presentations or on debugging.
+I use notebooks very often to connect to databases like postgres. With the notebook sessions, I often work on PoCs (proof of concept), on presentations or on debugging.
 
-[`catherinedevlin`](https://github.com/catherinedevlin) has created open source software that I love: [`ipython-sql`](https://pypi.org/project/ipython-sql/).
+[`catherinedevlin`](https://github.com/catherinedevlin) has created open source software that I love: [`ipython-sql`](https://pypi.org/project/ipython-sql/).  (Note: There was a fork of this project: [`jupy-sql`](https://jupysql.ploomber.io/en/latest/quick-start.html). The original version is not actively maintained, and does not work with sqlalchemy version 2 that was [released in January 2023](https://docs.sqlalchemy.org/en/20/changelog/changelog_20.html#change-2.0.0))
 
 This code -- `nbdbsession` -- lets you connect to sql databases from your notebook, and run queries.
 
-### How to publish a pkg to PyPI
-
-```sh
-# package code
-python setup.py sdist
-
-# upload code to PyPI
-twine upload dist/*
-
-# update pkg
-pip install nbdbsession --upgrade
-```
-
 ### How To Use `nbdbsession`
 
 First, install it:
 
 ```
 pip install nbdbsession
 ```
 
 Then, in your git repository where you start your notebook, create a `.settings.toml` file with your database login credentials:
 
+You need to define your database credentials in a toml file. The toml file should look like this:
+
 ```toml
-# .settings.toml on top level of your git repo
+# either: .settings.toml on top level of your git repo
+# or:     $HOME/.nbdbsession.creds.toml
+
 [davidkuda]
 db_driver = "postgresql"
 database = "dev"
 user = "davidkuda"
 password = "${DB_PASSWORD}" # you can use environment variables
 db_url = "localhost"
 port = 5439
 # the ssh command is optional:
 ssh_cmd = "ssh -fL 5432:db.kuda.ai:5432"
 ```
 
+nbdbsession will scan three places for a toml file and will choose the first hit in this order:
+
+- env var `$SETTINGS_FILE_PATH`
+- (root directory of a git project)/.settings.toml
+- `$HOME/.nbdbsession.creds.toml`
+
 Finally, you can connect to your database in your notebook by running the following code in a cell:
 
 ```python
 from nbdbsession.sqlconn import connect
 
 connect("davidkuda") # note: this is the name as defined in .settings.toml
 ```
@@ -70,14 +77,27 @@
     *
 FROM
     table
 LIMIT
     10;
 ```
 
+### How to publish a pkg to PyPI
+
+```sh
+# package code
+python setup.py sdist
+
+# upload code to PyPI
+twine upload dist/*
+
+# update pkg
+pip install nbdbsession --upgrade
+```
+
 ### Managing the conn without this repo
 
 In the usual way, you would create a connection string, something like this:
 
 ```python
 %load_ext sql
```

### Comparing `nbdbsession-0.2.5/setup.py` & `nbdbsession-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 # nbdbsession := notebook_database_session
 setup(
     name="nbdbsession",
-    version="0.2.5",
+    version="0.2.7",
     description="Config mgt to connect to databases from jupyter notebooks.",
     author="David Kuda",
     license="MIT",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/davidkuda/jupyter_database_io",
     long_description=long_description,
```

### Comparing `nbdbsession-0.2.5/src/nbdbsession/connection_string.py` & `nbdbsession-0.2.7/src/nbdbsession/connection_string.py`

 * *Files identical despite different names*

### Comparing `nbdbsession-0.2.5/src/nbdbsession/sqlconn.py` & `nbdbsession-0.2.7/src/nbdbsession/sqlconn.py`

 * *Files identical despite different names*

### Comparing `nbdbsession-0.2.5/src/nbdbsession/ssh_tunnel.py` & `nbdbsession-0.2.7/src/nbdbsession/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `nbdbsession-0.2.5/src/nbdbsession.egg-info/PKG-INFO` & `nbdbsession-0.2.7/src/nbdbsession.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,62 @@
 Metadata-Version: 2.1
 Name: nbdbsession
-Version: 0.2.5
+Version: 0.2.7
 Summary: Config mgt to connect to databases from jupyter notebooks.
 Home-page: https://github.com/davidkuda/jupyter_database_io
 Author: David Kuda
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nbdbsession
 
 __This code helps you to manage connections to sql databases in jupyter notebooks.__
 
 `nbdbsession` stands for "notebook database session".
 
-I use notebooks all the time to connect to databases like postgres. With the notebook sessions, I often work on PoCs (proof of concept), on presentations or on debugging.
+I use notebooks very often to connect to databases like postgres. With the notebook sessions, I often work on PoCs (proof of concept), on presentations or on debugging.
 
-[`catherinedevlin`](https://github.com/catherinedevlin) has created open source software that I love: [`ipython-sql`](https://pypi.org/project/ipython-sql/).
+[`catherinedevlin`](https://github.com/catherinedevlin) has created open source software that I love: [`ipython-sql`](https://pypi.org/project/ipython-sql/).  (Note: There was a fork of this project: [`jupy-sql`](https://jupysql.ploomber.io/en/latest/quick-start.html). The original version is not actively maintained, and does not work with sqlalchemy version 2 that was [released in January 2023](https://docs.sqlalchemy.org/en/20/changelog/changelog_20.html#change-2.0.0))
 
 This code -- `nbdbsession` -- lets you connect to sql databases from your notebook, and run queries.
 
-### How to publish a pkg to PyPI
-
-```sh
-# package code
-python setup.py sdist
-
-# upload code to PyPI
-twine upload dist/*
-
-# update pkg
-pip install nbdbsession --upgrade
-```
-
 ### How To Use `nbdbsession`
 
 First, install it:
 
 ```
 pip install nbdbsession
 ```
 
 Then, in your git repository where you start your notebook, create a `.settings.toml` file with your database login credentials:
 
+You need to define your database credentials in a toml file. The toml file should look like this:
+
 ```toml
-# .settings.toml on top level of your git repo
+# either: .settings.toml on top level of your git repo
+# or:     $HOME/.nbdbsession.creds.toml
+
 [davidkuda]
 db_driver = "postgresql"
 database = "dev"
 user = "davidkuda"
 password = "${DB_PASSWORD}" # you can use environment variables
 db_url = "localhost"
 port = 5439
 # the ssh command is optional:
 ssh_cmd = "ssh -fL 5432:db.kuda.ai:5432"
 ```
 
+nbdbsession will scan three places for a toml file and will choose the first hit in this order:
+
+- env var `$SETTINGS_FILE_PATH`
+- (root directory of a git project)/.settings.toml
+- `$HOME/.nbdbsession.creds.toml`
+
 Finally, you can connect to your database in your notebook by running the following code in a cell:
 
 ```python
 from nbdbsession.sqlconn import connect
 
 connect("davidkuda") # note: this is the name as defined in .settings.toml
 ```
@@ -80,14 +77,27 @@
     *
 FROM
     table
 LIMIT
     10;
 ```
 
+### How to publish a pkg to PyPI
+
+```sh
+# package code
+python setup.py sdist
+
+# upload code to PyPI
+twine upload dist/*
+
+# update pkg
+pip install nbdbsession --upgrade
+```
+
 ### Managing the conn without this repo
 
 In the usual way, you would create a connection string, something like this:
 
 ```python
 %load_ext sql
```

