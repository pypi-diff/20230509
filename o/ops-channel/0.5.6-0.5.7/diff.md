# Comparing `tmp/ops_channel-0.5.6.tar.gz` & `tmp/ops_channel-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_channel-0.5.6.tar", last modified: Tue May  9 03:32:38 2023, max compression
+gzip compressed data, was "ops_channel-0.5.7.tar", last modified: Tue May  9 06:42:02 2023, max compression
```

## Comparing `ops_channel-0.5.6.tar` & `ops_channel-0.5.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 03:32:38.823518 ops_channel-0.5.6/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-05-09 03:32:38.822990 ops_channel-0.5.6/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)     2910 2021-11-29 01:44:53.000000 ops_channel-0.5.6/README.md
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 03:32:38.819409 ops_channel-0.5.6/ops_channel/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       97 2023-04-17 02:21:10.000000 ops_channel-0.5.6/ops_channel/__init__.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)    97947 2023-05-09 03:29:03.000000 ops_channel-0.5.6/ops_channel/base.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)     5284 2023-04-20 08:22:19.000000 ops_channel-0.5.6/ops_channel/test.py
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 03:32:38.822377 ops_channel-0.5.6/ops_channel.egg-info/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-05-09 03:32:38.000000 ops_channel-0.5.6/ops_channel.egg-info/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      222 2023-05-09 03:32:38.000000 ops_channel-0.5.6/ops_channel.egg-info/SOURCES.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-05-09 03:32:38.000000 ops_channel-0.5.6/ops_channel.egg-info/dependency_links.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       12 2023-05-09 03:32:38.000000 ops_channel-0.5.6/ops_channel.egg-info/top_level.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-05-09 03:32:38.823682 ops_channel-0.5.6/setup.cfg
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      675 2023-05-09 03:32:31.000000 ops_channel-0.5.6/setup.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 06:42:02.167414 ops_channel-0.5.7/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-05-09 06:42:02.166849 ops_channel-0.5.7/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)     2910 2021-11-29 01:44:53.000000 ops_channel-0.5.7/README.md
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 06:42:02.160720 ops_channel-0.5.7/ops_channel/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       97 2023-04-17 02:21:10.000000 ops_channel-0.5.7/ops_channel/__init__.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)    99265 2023-05-09 06:40:14.000000 ops_channel-0.5.7/ops_channel/base.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)     5284 2023-04-20 08:22:19.000000 ops_channel-0.5.7/ops_channel/test.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 06:42:02.165926 ops_channel-0.5.7/ops_channel.egg-info/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-05-09 06:42:02.000000 ops_channel-0.5.7/ops_channel.egg-info/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      222 2023-05-09 06:42:02.000000 ops_channel-0.5.7/ops_channel.egg-info/SOURCES.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-05-09 06:42:02.000000 ops_channel-0.5.7/ops_channel.egg-info/dependency_links.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       12 2023-05-09 06:42:02.000000 ops_channel-0.5.7/ops_channel.egg-info/top_level.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-05-09 06:42:02.167596 ops_channel-0.5.7/setup.cfg
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      675 2023-05-09 06:41:23.000000 ops_channel-0.5.7/setup.py
```

### Comparing `ops_channel-0.5.6/README.md` & `ops_channel-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `ops_channel-0.5.6/ops_channel/base.py` & `ops_channel-0.5.7/ops_channel/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1682,40 +1682,55 @@
                 results.append(line)
             else:
                 results.append(line)
 
         return "\n".join(results)
 
 
-    def dump_sqlite_data(self, conn, dir='', limit=10, tables=[], overwrite=False):
+    def dump_sqlite_data(self, conn, dir='', limit=10, tables=[], overwrite=False,db_type='sqlite',all_in_one=False):
         # conn = self.get_mysql_connection(dsn)
         data_map = {}
         if len(tables) == 0:
             tables = self.get_sqlite_tables(conn)
         for table in tables:
             if limit > 0:
                 sql = 'select * from `{table}` limit {limit}'.format(table=table, limit=limit)
             else:
                 sql = 'select * from `{table}`'.format(table=table, limit=limit)
             table_data = self.sqlite_query(conn, sql)
             if len(table_data) == 0:
                 continue
             fpath = '{dir}/{table}.sql'.format(dir=dir, table=table)
-            sql_str = self.gen_insert_sql(table, table_data, db_type='sqlite')
-            if dir == '':
+            sql_str = self.gen_insert_sql(table, table_data, db_type=db_type)
+            if dir == '' or all_in_one:
                 data_map[table] = sql_str
             if dir != '':
                 if not os.path.exists(fpath) or overwrite:
                     with open(fpath, 'w+') as fp:
                         fp.write(sql_str)
                         self.log.info('gen table {table}'.format(table=table))
                 else:
                     self.log.warn('skip table {table}'.format(table=table))
             else:
                 self.log.error('dir is null')
+
+        if all_in_one:
+            fpath = '{dir}/all.sql'.format(dir=dir)
+            sql_str = ''
+            for table in data_map:
+                sql_str += data_map[table]+"\n\n"
+                if os.path.exists('{dir}/{table}.sql'.format(dir=dir, table=table)):
+                    os.remove('{dir}/{table}.sql'.format(dir=dir, table=table))
+            if not os.path.exists(fpath) or overwrite:
+                with open(fpath, 'w+') as fp:
+                    fp.write(sql_str)
+                    self.log.info('gen all sql')
+            else:
+                self.log.warn('skip all sql')
+
         return data_map
 
     # dump mysql data by table keys map
     def dump_mysql_data_by_keys(self, conn, dir='',table_keys_map={}, overwrite=False):
         data_map = {}
         for table in table_keys_map:
             keys=table_keys_map[table]
@@ -1741,40 +1756,54 @@
                     self.log.warn('skip table {table}'.format(table=table))
             else:
                 self.log.error('dir is null')
         return data_map
 
 
     # dump_mysql_data
-    def dump_mysql_data(self, conn, dir='', limit=10, tables=[], overwrite=False):
+    def dump_mysql_data(self, conn, dir='', limit=10, tables=[], overwrite=False,db_type='mysql',all_in_one=False):
         # conn = self.get_mysql_connection(dsn)
         data_map = {}
         if len(tables) == 0:
             tables = self.get_mysql_tables(conn)
         for table in tables:
             if limit > 0:
                 sql = 'select * from `{table}` limit {limit}'.format(table=table, limit=limit)
             else:
                 sql = 'select * from `{table}`'.format(table=table, limit=limit)
             table_data = self.mysql_query(conn, sql)
             if len(table_data) == 0:
                 continue
             fpath = '{dir}/{table}.sql'.format(dir=dir, table=table)
-            sql_str = self.gen_insert_sql(table, table_data)
-            if dir == '':
+            sql_str = self.gen_insert_sql(table, table_data, db_type=db_type)
+            if dir == '' or all_in_one:
                 data_map[table] = sql_str
             if dir != '':
                 if not os.path.exists(fpath) or overwrite:
                     with open(fpath, 'w+') as fp:
                         fp.write(sql_str)
                         self.log.info('gen table {table}'.format(table=table))
                 else:
                     self.log.warn('skip table {table}'.format(table=table))
             else:
                 self.log.error('dir is null')
+
+        if all_in_one:
+            fpath = '{dir}/all.sql'.format(dir=dir)
+            sql_str = ''
+            for table in data_map:
+                sql_str += data_map[table]+"\n\n"
+                if os.path.exists('{dir}/{table}.sql'.format(dir=dir, table=table)):
+                    os.remove('{dir}/{table}.sql'.format(dir=dir, table=table))
+            if not os.path.exists(fpath) or overwrite:
+                with open(fpath, 'w+') as fp:
+                    fp.write(sql_str)
+                    self.log.info('gen all sql')
+            else:
+                self.log.warn('skip all sql')
         return data_map
 
     def get_uuid(self):
         return str(uuid.uuid4())
 
     def uuid(self):
         return self.get_uuid()
```

### Comparing `ops_channel-0.5.6/ops_channel/test.py` & `ops_channel-0.5.7/ops_channel/test.py`

 * *Files identical despite different names*

### Comparing `ops_channel-0.5.6/setup.py` & `ops_channel-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time:  2018-11-27 19:17:34
 #############################################
 
 from setuptools import setup, find_packages
 
 setup(
     name="ops_channel",
-    version="0.5.6",
+    version="0.5.7",
     keywords=("pip", "ops_channel"),
     description="ops_channel util",
     long_description="ops_channel util",
     license="MIT Licence",
     packages=find_packages(),
     url="https://github.com/sjqzhang/ops_channel",
     author="jqzhang",
```

