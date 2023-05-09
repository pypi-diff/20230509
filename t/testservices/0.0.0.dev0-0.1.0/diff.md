# Comparing `tmp/testservices-0.0.0.dev0.tar.gz` & `tmp/testservices-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testservices-0.0.0.dev0.tar", last modified: Sat Feb 25 20:04:34 2023, max compression
+gzip compressed data, was "testservices-0.1.0.tar", last modified: Tue May  9 07:12:50 2023, max compression
```

## Comparing `testservices-0.0.0.dev0.tar` & `testservices-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,49 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-25 20:04:34.955742 testservices-0.0.0.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/.carthorse.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-25 20:04:34.951741 testservices-0.0.0.dev0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/.readthedocs.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/LICENSE.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2023-02-25 20:04:34.955742 testservices-0.0.0.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      421 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-25 20:04:34.955742 testservices-0.0.0.dev0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2575 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/docs/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/docs/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/docs/changes.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1739 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/docs/development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/docs/license.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/docs/use.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-02-25 20:04:34.955742 testservices-0.0.0.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-25 20:04:34.955742 testservices-0.0.0.dev0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/tests/test_imports.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-25 20:04:34.955742 testservices-0.0.0.dev0/testservices/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/testservices/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/testservices/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/testservices/provider.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/testservices/service.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-02-25 20:04:23.000000 testservices-0.0.0.dev0/testservices/supplier.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-25 20:04:34.955742 testservices-0.0.0.dev0/testservices.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2023-02-25 20:04:34.000000 testservices-0.0.0.dev0/testservices.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      624 2023-02-25 20:04:34.000000 testservices-0.0.0.dev0/testservices.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-25 20:04:34.000000 testservices-0.0.0.dev0/testservices.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-25 20:04:30.000000 testservices-0.0.0.dev0/testservices.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-02-25 20:04:34.000000 testservices-0.0.0.dev0/testservices.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-02-25 20:04:34.000000 testservices-0.0.0.dev0/testservices.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2023-05-09 07:12:38.000000 testservices-0.1.0/.carthorse.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1839 2023-05-09 07:12:38.000000 testservices-0.1.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-09 07:12:38.000000 testservices-0.1.0/.coveragerc
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-05-09 07:12:38.000000 testservices-0.1.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-05-09 07:12:38.000000 testservices-0.1.0/.readthedocs.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-05-09 07:12:38.000000 testservices-0.1.0/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-05-09 07:12:38.000000 testservices-0.1.0/LICENSE.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-09 07:12:50.887726 testservices-0.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-05-09 07:12:38.000000 testservices-0.1.0/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/changes.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1739 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/license.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/use.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-09 07:12:38.000000 testservices-0.1.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-09 07:12:50.887726 testservices-0.1.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2023-05-09 07:12:38.000000 testservices-0.1.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1699 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/test_containers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3254 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/test_databases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/test_imports.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/test_service.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/testservices/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/service.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/testservices/services/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/services/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.883726 testservices-0.1.0/testservices/services/config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/testservices/services/config/clickhouse/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/services/config/clickhouse/docker_related_config.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/services/containers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4661 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/services/databases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/supplier.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/testservices.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 07:12:46.000000 testservices-0.1.0/testservices.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/top_level.txt
```

### Comparing `testservices-0.0.0.dev0/LICENSE.rst` & `testservices-0.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `testservices-0.0.0.dev0/PKG-INFO` & `testservices-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: testservices
-Version: 0.0.0.dev0
+Version: 0.1.0
 Summary: Orchestrating services for testing and development.
 Home-page: https://github.com/simplistix/testservices
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: build
 License-File: LICENSE.rst
 
-
 testservices
 ============
 
 |CircleCI|_  |Docs|_
 
 .. |CircleCI| image:: https://circleci.com/gh/simplistix/testservices/tree/master.svg?style=shield
 .. _CircleCI: https://circleci.com/gh/simplistix/testservices/tree/master
 
 .. |Docs| image:: https://readthedocs.org/projects/testservices/badge/?version=latest
 .. _Docs: http://testservices.readthedocs.org/en/latest/
 
- Orchestrating services for testing and development.
+Orchestrating services for testing and development.
```

### Comparing `testservices-0.0.0.dev0/docs/Makefile` & `testservices-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `testservices-0.0.0.dev0/docs/conf.py` & `testservices-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `testservices-0.0.0.dev0/docs/development.rst` & `testservices-0.1.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `testservices-0.0.0.dev0/setup.py` & `testservices-0.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,35 +5,51 @@
 
 from setuptools import setup, find_packages
 
 base_dir = os.path.dirname(__file__)
 
 setup(
     name='testservices',
-    version='0.0.0.dev0',
+    version='0.1.0',
     author='Chris Withers',
     author_email='chris@withers.org',
     license='MIT',
     description=(
         "Orchestrating services for testing and development."
     ),
     long_description=open('README.rst').read(),
     url='https://github.com/simplistix/testservices',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.11',
     ],
     packages=find_packages(exclude=["tests"]),
     zip_safe=False,
     include_package_data=True,
+    python_requires=">=3.8",
     extras_require=dict(
         test=[
+            'PyMySQL',
+            'clickhouse-driver',
+            'docker',
             'pytest',
             'pytest-cov',
             'sybil',
             'testfixtures',
+            'psycopg',
+            'sqlalchemy',
+            # https://github.com/docker/docker-py/issues/3113
+            'urllib3<2',
         ],
-        build=['furo', 'sphinx', 'setuptools-git', 'twine', 'wheel']
+        build=[
+            'furo',
+            'sphinx',
+            'setuptools-git',
+            'twine',
+            # https://github.com/docker/docker-py/issues/3113
+            'urllib3<2',
+            'wheel'
+        ]
     ),
 )
```

### Comparing `testservices-0.0.0.dev0/testservices.egg-info/PKG-INFO` & `testservices-0.1.0/testservices.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: testservices
-Version: 0.0.0.dev0
+Version: 0.1.0
 Summary: Orchestrating services for testing and development.
 Home-page: https://github.com/simplistix/testservices
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: build
 License-File: LICENSE.rst
 
-
 testservices
 ============
 
 |CircleCI|_  |Docs|_
 
 .. |CircleCI| image:: https://circleci.com/gh/simplistix/testservices/tree/master.svg?style=shield
 .. _CircleCI: https://circleci.com/gh/simplistix/testservices/tree/master
 
 .. |Docs| image:: https://readthedocs.org/projects/testservices/badge/?version=latest
 .. _Docs: http://testservices.readthedocs.org/en/latest/
 
- Orchestrating services for testing and development.
+Orchestrating services for testing and development.
```

