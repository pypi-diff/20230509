# Comparing `tmp/ops_channel-0.5.5.tar.gz` & `tmp/ops_channel-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_channel-0.5.5.tar", last modified: Thu Apr 13 03:27:11 2023, max compression
+gzip compressed data, was "ops_channel-0.5.6.tar", last modified: Tue May  9 03:32:38 2023, max compression
```

## Comparing `ops_channel-0.5.5.tar` & `ops_channel-0.5.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-13 03:27:11.984755 ops_channel-0.5.5/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-04-13 03:27:11.984302 ops_channel-0.5.5/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)     2910 2021-11-29 01:44:53.000000 ops_channel-0.5.5/README.md
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-13 03:27:11.980323 ops_channel-0.5.5/ops_channel/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      127 2022-10-20 02:06:16.000000 ops_channel-0.5.5/ops_channel/__init__.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)    97625 2023-04-13 03:19:35.000000 ops_channel-0.5.5/ops_channel/base.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)    25301 2023-04-13 03:10:36.000000 ops_channel-0.5.5/ops_channel/test.py
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-13 03:27:11.983002 ops_channel-0.5.5/ops_channel.egg-info/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-04-13 03:27:11.000000 ops_channel-0.5.5/ops_channel.egg-info/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      222 2023-04-13 03:27:11.000000 ops_channel-0.5.5/ops_channel.egg-info/SOURCES.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-04-13 03:27:11.000000 ops_channel-0.5.5/ops_channel.egg-info/dependency_links.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       12 2023-04-13 03:27:11.000000 ops_channel-0.5.5/ops_channel.egg-info/top_level.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-04-13 03:27:11.984965 ops_channel-0.5.5/setup.cfg
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      675 2023-04-13 03:26:45.000000 ops_channel-0.5.5/setup.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 03:32:38.823518 ops_channel-0.5.6/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-05-09 03:32:38.822990 ops_channel-0.5.6/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)     2910 2021-11-29 01:44:53.000000 ops_channel-0.5.6/README.md
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 03:32:38.819409 ops_channel-0.5.6/ops_channel/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       97 2023-04-17 02:21:10.000000 ops_channel-0.5.6/ops_channel/__init__.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)    97947 2023-05-09 03:29:03.000000 ops_channel-0.5.6/ops_channel/base.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)     5284 2023-04-20 08:22:19.000000 ops_channel-0.5.6/ops_channel/test.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-05-09 03:32:38.822377 ops_channel-0.5.6/ops_channel.egg-info/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      259 2023-05-09 03:32:38.000000 ops_channel-0.5.6/ops_channel.egg-info/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      222 2023-05-09 03:32:38.000000 ops_channel-0.5.6/ops_channel.egg-info/SOURCES.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-05-09 03:32:38.000000 ops_channel-0.5.6/ops_channel.egg-info/dependency_links.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       12 2023-05-09 03:32:38.000000 ops_channel-0.5.6/ops_channel.egg-info/top_level.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-05-09 03:32:38.823682 ops_channel-0.5.6/setup.cfg
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      675 2023-05-09 03:32:31.000000 ops_channel-0.5.6/setup.py
```

### Comparing `ops_channel-0.5.5/README.md` & `ops_channel-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ops_channel-0.5.5/ops_channel/base.py` & `ops_channel-0.5.6/ops_channel/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,26 +201,27 @@
         self.auth_uuid = ''
         self.token = ''
         self.modules = {'zmq': 'pyzmq==19.0.2', 'pymysql': 'PyMySQL==0.9.2', 'kafka': 'kafka==1.3.5',
                         'redis': 'redis==3.5.3', 'yaml': 'PyYAML==5.3.1', 'pyquery': 'pyquery==1.4.0',
                         'elasticsearch': 'elasticsearch==7.17.4', 'flask': 'Flask==1.0.2',
                         'requests': 'requests==2.25.0', 'pymongo': 'pymongo==3.12.3', 'openpyxl': 'openpyxl==2.6.4',
                         'xlrd': 'xlrd==2.0.1', 'jinja2': 'Jinja2==2.11.1', 'dsnparse': 'dsnparse==0.1.15',
-                        'xlsxwriter': 'XlsxWriter==2.0.0', 'pika': 'pika==1.2.0'}
+                        'xlsxwriter': 'XlsxWriter==2.0.0', 'pika': 'pika==1.2.0',' pyjwt':'pyjwt==1.7.1'}
         if PY3:
             self.modules['kafka'] = 'kafka-python==2.0.2'
             self.modules['zmq'] = 'pyzmq==23.2.0'
             self.modules['flask'] = 'Flask==2.0.1'
             self.modules['pymysql'] = 'PyMySQL==1.0.2'
             self.modules['elasticsearch'] = 'elasticsearch==8.3.1'
             self.modules['pymongo'] = 'pymongo==4.2.0'
             self.modules['openpyxl'] = 'openpyxl==3.0.10'
             self.modules['xlrd'] = 'xlrd==2.0.1'
             self.modules['jinja2'] = 'Jinja2==3.1.2'
             self.modules['xlsxwriter'] = 'XlsxWriter==3.0.3'
+            self.modules['pyjwt'] = 'pyjwt==2.6.0'
 
         if len(sys.argv) == 2 and len(sys.argv[1]) == 36:
             self.get_param('')
 
     def gen_requirements(self, path=''):
         mods = []
         install_mods = []
@@ -1075,29 +1076,32 @@
     def get_mysql_connection(self, dsn_str):
         '''
         :param dsn_str='mysql://root:root@localhost:3306/ferry':
         :return:
         '''
         import dsnparse
         dsn = dsnparse.parse(dsn_str)
+        charset=dsn.query.get('charset')
+        if charset is None or charset=='':
+            charset='utf8mb4'
         import pymysql
         from pymysql.constants import CLIENT
         try:
             from collections import OrderedDict
             from pymysql.cursors import DictCursorMixin, Cursor
             class OrderedDictCursor(DictCursorMixin, Cursor):
                 dict_type = OrderedDict
         except Exception as er:
             OrderedDictCursor = pymysql.cursors.DictCursor
         connection = pymysql.connect(host=dsn.host,
                                      user=dsn.user,
                                      port=dsn.port,
                                      password=dsn.password,
                                      database=dsn.database,
-                                     charset='utf8mb4',
+                                     charset=charset,
                                      cursorclass=OrderedDictCursor,
                                      # local_infile=True,
                                      client_flag=CLIENT.MULTI_STATEMENTS,
                                      max_allowed_packet=1024 * 1024 * 1024)
         connection.autocommit(True)
         # try:
         #     self.mysql_query(connection, 'set  global max_allowed_packet=1073741824;')
@@ -1274,15 +1278,15 @@
                 if row[fn] is None:
                     data.append('NULL')
                 elif type(row[fn]) == int or type(row[fn]) == float:
                     data.append(str(row[fn]))
                 else:
                     if db_type == 'sqlite3' or db_type == 'sqlite':
                         s = str(row[fn]).replace('\\', '\\\\').replace("'", "''")
-                        s = s.replace("\n", "\\n").replace('"', '\\"')
+                        s = s.replace("\n", "\\n")#.replace('"', '\\"')
                         data.append("'%s'" % (s))
                     else:
                         s = str(row[fn]).replace('\\', '\\\\').replace("'", "\\'")
                         s = s.replace("\n", "\\n").replace('"', '\\"')
                         data.append("'%s'" % (s))
             rows.append("\t(" + ','.join(data) + ')')
             if i % batch_row_max == 0:
@@ -1790,14 +1794,23 @@
 
     @property
     def pymongo(self):
         import pymongo
         return pymongo
 
     @property
+    def jwt(self):
+        import jwt
+        return jwt
+
+    @property
+    def pyjwt(self):
+        return self.jwt
+
+    @property
     def flask(self):
         import flask
         return flask
 
     @property
     def pyquery(self):
         import pyquery
@@ -2493,15 +2506,15 @@
             except Exception as err:
                 if PY3:
                     logger.warning('No module named: pip3 install %s' % (cli.modules[m]))
                 else:
                     logger.warning('No module named: pip install %s' % (cli.modules[m]))
 
 
-__check_module()
+# __check_module()
 
 
 class CAS(object):
     def __init__(self, objname=''):
         self.objname = objname
         self.id_key = '_id'
         self.version_key = '_version'
```

### Comparing `ops_channel-0.5.5/setup.py` & `ops_channel-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time:  2018-11-27 19:17:34
 #############################################
 
 from setuptools import setup, find_packages
 
 setup(
     name="ops_channel",
-    version="0.5.5",
+    version="0.5.6",
     keywords=("pip", "ops_channel"),
     description="ops_channel util",
     long_description="ops_channel util",
     license="MIT Licence",
     packages=find_packages(),
     url="https://github.com/sjqzhang/ops_channel",
     author="jqzhang",
```

