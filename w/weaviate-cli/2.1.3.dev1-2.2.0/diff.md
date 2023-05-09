# Comparing `tmp/weaviate-cli-2.1.3.dev1.tar.gz` & `tmp/weaviate-cli-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/weaviate-cli-2.1.3.dev1.tar", last modified: Mon Oct 25 13:57:21 2021, max compression
+gzip compressed data, was "weaviate-cli-2.2.0.tar", last modified: Tue May  9 14:32:52 2023, max compression
```

## Comparing `weaviate-cli-2.1.3.dev1.tar` & `weaviate-cli-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     2915 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/PKG-INFO
-drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/semi/
--rw-r--r--   0 stefanbogdan   (501) staff       (20)       62 2021-10-25 13:47:48.000000 weaviate-cli-2.1.3.dev1/semi/version.py
-drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/semi/config/
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     2611 2021-10-25 13:34:29.000000 weaviate-cli-2.1.3.dev1/semi/config/configuration.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)        0 2021-01-12 14:42:39.000000 weaviate-cli-2.1.3.dev1/semi/config/__init__.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)      117 2021-01-12 14:42:39.000000 weaviate-cli-2.1.3.dev1/semi/config/config_values.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     1330 2021-01-12 14:42:39.000000 weaviate-cli-2.1.3.dev1/semi/config/manage.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)        0 2021-01-12 14:42:39.000000 weaviate-cli-2.1.3.dev1/semi/__init__.py
-drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/semi/commands/
--rw-r--r--   0 stefanbogdan   (501) staff       (20)      481 2021-08-02 06:57:26.000000 weaviate-cli-2.1.3.dev1/semi/commands/misc.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)        0 2021-01-12 14:42:39.000000 weaviate-cli-2.1.3.dev1/semi/commands/__init__.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     8639 2021-10-25 13:47:37.000000 weaviate-cli-2.1.3.dev1/semi/commands/data.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     2049 2021-08-02 06:54:14.000000 weaviate-cli-2.1.3.dev1/semi/commands/schema.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     1133 2021-08-02 06:52:29.000000 weaviate-cli-2.1.3.dev1/semi/prompt.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)      865 2021-08-02 06:38:51.000000 weaviate-cli-2.1.3.dev1/setup.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     3556 2021-10-25 13:31:11.000000 weaviate-cli-2.1.3.dev1/cli.py
--rw-r--r--   0 stefanbogdan   (501) staff       (20)       38 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/setup.cfg
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     2215 2021-04-16 14:03:40.000000 weaviate-cli-2.1.3.dev1/README.rst
-drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/weaviate_cli.egg-info/
--rw-r--r--   0 stefanbogdan   (501) staff       (20)     2915 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/weaviate_cli.egg-info/PKG-INFO
--rw-r--r--   0 stefanbogdan   (501) staff       (20)      490 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/weaviate_cli.egg-info/SOURCES.txt
--rw-r--r--   0 stefanbogdan   (501) staff       (20)       49 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/weaviate_cli.egg-info/entry_points.txt
--rw-r--r--   0 stefanbogdan   (501) staff       (20)       36 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/weaviate_cli.egg-info/requires.txt
--rw-r--r--   0 stefanbogdan   (501) staff       (20)        9 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/weaviate_cli.egg-info/top_level.txt
--rw-r--r--   0 stefanbogdan   (501) staff       (20)        1 2021-10-25 13:57:21.000000 weaviate-cli-2.1.3.dev1/weaviate_cli.egg-info/dependency_links.txt
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:32:52.958742 weaviate-cli-2.2.0/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1508 2021-01-12 14:42:39.000000 weaviate-cli-2.2.0/LICENSE
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2465 2023-05-09 14:32:52.957545 weaviate-cli-2.2.0/PKG-INFO
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2207 2022-03-14 12:08:38.000000 weaviate-cli-2.2.0/README.rst
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      854 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/cli.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:32:52.945299 weaviate-cli-2.2.0/semi/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        0 2021-01-12 14:42:39.000000 weaviate-cli-2.2.0/semi/__init__.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:32:52.946138 weaviate-cli-2.2.0/semi/classification/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/classification/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     4770 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/classification/commands.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:32:52.948866 weaviate-cli-2.2.0/semi/config/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        0 2021-01-12 14:42:39.000000 weaviate-cli-2.2.0/semi/config/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     6353 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/config/commands.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      117 2021-01-12 14:42:39.000000 weaviate-cli-2.2.0/semi/config/config_values.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:32:52.950057 weaviate-cli-2.2.0/semi/data/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/data/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     9387 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/data/commands.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1660 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/misc.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1200 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/prompt.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:32:52.951348 weaviate-cli-2.2.0/semi/schema/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/schema/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     3287 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/schema/commands.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1233 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/utils.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       57 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/semi/version.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       38 2023-05-09 14:32:52.958935 weaviate-cli-2.2.0/setup.cfg
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1071 2023-05-09 14:31:21.000000 weaviate-cli-2.2.0/setup.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2023-05-09 14:32:52.955795 weaviate-cli-2.2.0/weaviate_cli.egg-info/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2465 2023-05-09 14:32:52.000000 weaviate-cli-2.2.0/weaviate_cli.egg-info/PKG-INFO
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      560 2023-05-09 14:32:52.000000 weaviate-cli-2.2.0/weaviate_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        1 2023-05-09 14:32:52.000000 weaviate-cli-2.2.0/weaviate_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       38 2023-05-09 14:32:52.000000 weaviate-cli-2.2.0/weaviate_cli.egg-info/entry_points.txt
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       56 2023-05-09 14:32:52.000000 weaviate-cli-2.2.0/weaviate_cli.egg-info/requires.txt
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        9 2023-05-09 14:32:52.000000 weaviate-cli-2.2.0/weaviate_cli.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `weaviate-cli-2.1.3.dev1/PKG-INFO` & `weaviate-cli-2.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 Metadata-Version: 2.1
 Name: weaviate-cli
-Version: 2.1.3.dev1
+Version: 2.2.0
 Summary: Comand line interface to interact with weaviate
-Home-page: UNKNOWN
 Author: SeMI Technologies
 Author-email: hello@semi.technology
-License: UNKNOWN
-Description: Weaviate CLI
-        ============
-        .. image:: https://raw.githubusercontent.com/semi-technologies/weaviate/19de0956c69b66c5552447e84d016f4fe29d12c9/docs/assets/weaviate-logo.png
-            :width: 180
-            :align: right
-            :alt: Weaviate logo
-        
-        .. image:: https://travis-ci.com/semi-technologies/weaviate-cli.svg?branch=master
-            :target: https://travis-ci.com/semi-technologies/weaviate-cli
-            :alt: Build Status (Travis CI)
-        
-        .. image:: https://badge.fury.io/py/weaviate-cli.svg
-            :target: https://badge.fury.io/py/weaviate-cli
-            :alt: PyPI version
-        
-        
-        **Command Line Interface (CLI) tool for interacting with a Weaviate instance directly from your Terminal**
-        
-        Visit the official `SeMi Technology <https://www.semi.technology/>`_ website for more information about the Weaviate and how to use it in production.
-        
-        Check out our `weaviate-client <https://pypi.org/project/weaviate-client/>`_ library for interacting with a Weaviate instance using python.
-        
-        Installation
-        ------------
-        
-        | Install using: ``pip install weaviate-cli``
-        | Run using: ``weaviate --help``
-        
-        Articles
-        --------
-        
-        Here are some articles on weaviate: 
-        
-        - `Semantic Search Queries Return More Informed Results <https://hackernoon.com/semantic-search-queries-return-more-informed-results-nr5335nw>`_
-        - `Getting Started with Weaviate Python Library <https://towardsdatascience.com/getting-started-with-weaviate-python-client-e85d14f19e4f>`_
-        - `A sub-50ms neural search with DistilBERT and Weaviate <https://towardsdatascience.com/a-sub-50ms-neural-search-with-distilbert-and-weaviate-4857ae390154>`_
-        - `SeMI Technology Medium blogs <https://medium.com/semi-technologies>`_
-        
-        Support
-        -------
-        
-        - Use our `Slack Channel <https://join.slack.com/t/weaviate/shared_invite/zt-goaoifjr-o8FuVz9b1HLzhlUfyfddhw>`_ for support or any other question.
-        - Use the ``weaviate`` tag on `Stackoverflow <https://stackoverflow.com/questions/tagged/weaviate>`_  for questions.
-        - For bugs and/or problems with the package submit a Github `issue <https://github.com/semi-technologies/weaviate-python-client/issues>`_.
-        
-        Contributing
-        ------------
-        
-        - Do you want to contribute to `Weaviate`, read `How to Contribute <https://github.com/semi-technologies/weaviate/blob/master/CONTRIBUTE.md>`_.
-        
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Weaviate CLI
+============
+.. image:: https://raw.githubusercontent.com/semi-technologies/weaviate/19de0956c69b66c5552447e84d016f4fe29d12c9/docs/assets/weaviate-logo.png
+    :width: 180
+    :align: right
+    :alt: Weaviate logo
+
+.. image:: https://travis-ci.com/semi-technologies/weaviate-cli.svg?branch=master
+    :target: https://travis-ci.com/semi-technologies/weaviate-cli
+    :alt: Build Status (Travis CI)
+
+.. image:: https://badge.fury.io/py/weaviate-cli.svg
+    :target: https://badge.fury.io/py/weaviate-cli
+    :alt: PyPI version
+
+
+**Command Line Interface (CLI) tool for interacting with a Weaviate instance directly from your Terminal**
+
+Visit the official `SeMi Technology <https://weaviate.io/>`_ website for more information about the Weaviate and how to use it in production.
+
+Check out our `weaviate-client <https://pypi.org/project/weaviate-client/>`_ library for interacting with a Weaviate instance using python.
+
+Installation
+------------
+
+| Install using: ``pip install weaviate-cli``
+| Run using: ``weaviate --help``
+
+Articles
+--------
+
+Here are some articles on weaviate: 
+
+- `Semantic Search Queries Return More Informed Results <https://hackernoon.com/semantic-search-queries-return-more-informed-results-nr5335nw>`_
+- `Getting Started with Weaviate Python Library <https://towardsdatascience.com/getting-started-with-weaviate-python-client-e85d14f19e4f>`_
+- `A sub-50ms neural search with DistilBERT and Weaviate <https://towardsdatascience.com/a-sub-50ms-neural-search-with-distilbert-and-weaviate-4857ae390154>`_
+- `SeMI Technology Medium blogs <https://medium.com/semi-technologies>`_
+
+Support
+-------
+
+- Use our `Slack Channel <https://join.slack.com/t/weaviate/shared_invite/zt-goaoifjr-o8FuVz9b1HLzhlUfyfddhw>`_ for support or any other question.
+- Use the ``weaviate`` tag on `Stackoverflow <https://stackoverflow.com/questions/tagged/weaviate>`_  for questions.
+- For bugs and/or problems with the package submit a Github `issue <https://github.com/semi-technologies/weaviate-python-client/issues>`_.
+
+Contributing
+------------
+
+- Do you want to contribute to `Weaviate`, read `How to Contribute <https://github.com/semi-technologies/weaviate/blob/master/CONTRIBUTE.md>`_.
```

### Comparing `weaviate-cli-2.1.3.dev1/semi/commands/data.py` & `weaviate-cli-2.2.0/semi/data/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,63 @@
-import json
+"""
+Weaviate CLI data group functions.
+"""
+
 import sys
+import json
+import click
 import weaviate
-# import Batcher for weaviate-client version < 3.0.0
-VERSION_2 = (int(weaviate.__version__.split('.')[0]) < 3)
-if VERSION_2:
-    from weaviate.tools import Batcher
-from semi.config.configuration import Configuration
+
+from semi.utils import get_client_from_context
 from semi.prompt import is_question_answer_yes
 
 
-def delete_all_data(cfg: Configuration, force: bool) -> None:
+@click.group("data", help="Data object manipulation in weaviate.")
+def data_group():
+    pass
+
+
+@data_group.command("import", help="Import data from json file.")
+@click.pass_context
+@click.argument('file')
+@click.option('--fail-on-error', required=False, default=False, is_flag=True, help="Fail if entity loading throws an error")
+def concept_import(ctx, file, fail_on_error):
+    import_data_from_file(get_client_from_context(ctx), file, fail_on_error)
+
+
+@data_group.command("delete", help="Delete all data objects in weaviate.")
+@click.pass_context
+@click.option('--force', required=False, default=False, is_flag=True)
+def data_empty(ctx, force):
+    delete_all_data(get_client_from_context(ctx), force)
+
+
+####################################################################################################
+# Helper functions
+####################################################################################################
+
+
+def delete_all_data(client: weaviate.Client, force: bool) -> None:
     """
     Delete all weaviate objects.
 
     Parameters
     ----------
     cfg : Configuration
         A CLI configuration.
     force : bool
         If True force delete all objects, if False ask for permission.
     """
 
     if force:
-        _delete_all(cfg.client)
+        _delete_all(client)
         sys.exit(0)
     if not is_question_answer_yes("Do you really want to delete all data?"):
         sys.exit(0)
-    _delete_all(cfg.client)
+    _delete_all(client)
 
 
 def _delete_all(client: weaviate.Client):
     """
     Delete all weaviate data.
 
     Parameters
@@ -40,32 +67,37 @@
     """
 
     schema = client.schema.get()
     client.schema.delete_all()
     client.schema.create(schema)
 
 
-def import_data_from_file(cfg: Configuration, file: str, fail_on_error: bool) -> None:
+def import_data_from_file(client: weaviate.Client, file: str, fail_on_error: bool) -> None:
     """
     Import data from a file.
 
     Parameters
     ----------
     cfg : Configuration
         A CLI configuration.
     file : str
         The data file path.
     fail_on_error : bool
         If True exits at the first error, if False prints the error only.
     """
 
-    importer = DataFileImporter(cfg.client, file, fail_on_error)
+    importer = DataFileImporter(client, file, fail_on_error)
     importer.load()
 
 
+####################################################################################################
+# DataFileImporter
+####################################################################################################
+
+
 class DataFileImporter:
 
     def __init__(self, client: weaviate.Client, data_path: str, fail_on_error: bool):
         """
         Initialize a DataFileImporter.
 
         Parameters
@@ -76,25 +108,20 @@
             The data file path.
         fail_on_error : bool
             If True exits at the first error, if False prints the error only.
         """
 
         self.client = client
         self.fail_on_error = fail_on_error
-        if VERSION_2:
-            self.batcher = Batcher(
-                client,
-                batch_size=512,
-                return_values_callback=self._exit_on_error,
-            )
-        else:
-            self.batcher = client.batch(
-                batch_size=512,
-                callback=self._exit_on_error,
-            )
+
+        self.batcher = client.batch(
+            batch_size=512,
+            callback=self._exit_on_error,
+        )
+
         with open(data_path, 'r') as data_io:
             self.data = json.load(data_io)
 
     def _exit_on_error(self, batch_results: list):
         """
         Exit if an error occurred.
 
@@ -122,18 +149,15 @@
         vasd = ValidateAndSplitData(self.data, schema)
         vasd.validate_and_split()
         print("Importing data")
         for obj in vasd.data_objects:
             self.batcher.add_data_object(**obj)
         for ref in vasd.data_references:
             self.batcher.add_reference(**ref)
-        if VERSION_2:
-            self.batcher.close()
-        else:
-            self.batcher.flush()
+        self.batcher.flush()
 
 class ValidateAndSplitData:
 
     def __init__(self, data: dict, schema: dict):
         """
         Initialize a ValidateAndSplitData class instance.
 
@@ -147,17 +171,17 @@
 
         self.data = data
         self.schema = dissect_schema(schema)
         self.data_objects = []
         self.data_references = []
 
     def validate_and_split(self) -> None:
-        """ 
+        """
         Go through the entire data and validate it against a schema
-        if not valid exit with error, if valid split it into the 
+        if not valid exit with error, if valid split it into the
         primitive object and the references.
         """
 
         for obj in self.data.get("classes", []):
             self._validate_obj(obj)
 
     def _validate_obj(self, obj):
@@ -212,15 +236,15 @@
     Dissect a reference list into the parametes required for a batch request.
 
     Parameters
     ----------
     refs : list
         A list of references to be dissected.
     from_class : str
-        The object's class name. 
+        The object's class name.
     from_id : str
         The id of the object.
     from_prop : str
         The property name.
 
     Returns
     -------
@@ -238,15 +262,15 @@
             "to_object_uuid": beacon_split[-1]
         }
         result.append(ref_batch_parameters)
     return result
 
 
 def dissect_schema(schema: dict) -> dict:
-    """ 
+    """
     Dissect the schema into a dict listing all classes with their name as key to have faster
     validation access.
 
     Parameters
     ----------
     schema : dict
         The schema as exported from weaviate
```

### Comparing `weaviate-cli-2.1.3.dev1/semi/prompt.py` & `weaviate-cli-2.2.0/semi/prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,38 +15,41 @@
     -------
     bool
         True if the user answers "yes", False otherwise.
     """
 
     answer = input(question + " [y/N] ")
     answer = answer.lower()
-    if answer == "y" or answer == "yes":
+    if answer in ("y", "yes"):
         return True
     return False
 
 
-def let_user_pick(options: list) -> int:
+def let_user_pick(options: list, query: str) -> int:
     """
     Present a list of options to the user for selection.
 
     Parameters
     ----------
     options : list
         A list of options to be printed and user to choose from.
 
+    query : str
+        Query string to present to user.
+
     Returns
     -------
     int
         The index of the users selection.
     """
 
-    print("Please choose:")
+    print(query)
     for idx, element in enumerate(options):
         print(f"{idx + 1}) {element}")
     choice = input("Enter number: ")
     try:
         if 0 < int(choice) <= len(options):
             return int(choice) - 1
-    except:
+    except TypeError:
         pass
     print("Not a valid choice choose again!")
-    return let_user_pick(options)
+    return let_user_pick(options, query)
```

### Comparing `weaviate-cli-2.1.3.dev1/setup.py` & `weaviate-cli-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+from sys import version_info, exit
+#check python version
+if version_info.major < 3:
+    exit("Python 3.x is required to run this program")
+
 from os import path
 from builtins import open
 from setuptools import setup
 from semi.version import __version__
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
@@ -12,18 +17,19 @@
     name="weaviate-cli",
     version=__version__,
     description="Comand line interface to interact with weaviate",
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author="SeMI Technologies",
     author_email="hello@semi.technology",
-    packages=["semi", "semi.config", "semi.commands"],
+    packages=["semi", "semi.config",  "semi.data", "semi.schema", "semi.classification"],
     py_modules=['cli'],
     python_requires='>=3.6',
     install_requires=[
-        "weaviate-client>=2.1.0",
-        "click==7.1.2"],
+        "weaviate-client>=3.7.0",
+        "click==7.1.2",
+        "click-params==0.3.0"],
     entry_points='''
     [console_scripts]
     weaviate=cli:main
     '''
 )
```

### Comparing `weaviate-cli-2.1.3.dev1/README.rst` & `weaviate-cli-2.2.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 .. image:: https://badge.fury.io/py/weaviate-cli.svg
     :target: https://badge.fury.io/py/weaviate-cli
     :alt: PyPI version
 
 
 **Command Line Interface (CLI) tool for interacting with a Weaviate instance directly from your Terminal**
 
-Visit the official `SeMi Technology <https://www.semi.technology/>`_ website for more information about the Weaviate and how to use it in production.
+Visit the official `SeMi Technology <https://weaviate.io/>`_ website for more information about the Weaviate and how to use it in production.
 
 Check out our `weaviate-client <https://pypi.org/project/weaviate-client/>`_ library for interacting with a Weaviate instance using python.
 
 Installation
 ------------
 
 | Install using: ``pip install weaviate-cli``
```

### Comparing `weaviate-cli-2.1.3.dev1/weaviate_cli.egg-info/PKG-INFO` & `weaviate-cli-2.2.0/weaviate_cli.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 Metadata-Version: 2.1
 Name: weaviate-cli
-Version: 2.1.3.dev1
+Version: 2.2.0
 Summary: Comand line interface to interact with weaviate
-Home-page: UNKNOWN
 Author: SeMI Technologies
 Author-email: hello@semi.technology
-License: UNKNOWN
-Description: Weaviate CLI
-        ============
-        .. image:: https://raw.githubusercontent.com/semi-technologies/weaviate/19de0956c69b66c5552447e84d016f4fe29d12c9/docs/assets/weaviate-logo.png
-            :width: 180
-            :align: right
-            :alt: Weaviate logo
-        
-        .. image:: https://travis-ci.com/semi-technologies/weaviate-cli.svg?branch=master
-            :target: https://travis-ci.com/semi-technologies/weaviate-cli
-            :alt: Build Status (Travis CI)
-        
-        .. image:: https://badge.fury.io/py/weaviate-cli.svg
-            :target: https://badge.fury.io/py/weaviate-cli
-            :alt: PyPI version
-        
-        
-        **Command Line Interface (CLI) tool for interacting with a Weaviate instance directly from your Terminal**
-        
-        Visit the official `SeMi Technology <https://www.semi.technology/>`_ website for more information about the Weaviate and how to use it in production.
-        
-        Check out our `weaviate-client <https://pypi.org/project/weaviate-client/>`_ library for interacting with a Weaviate instance using python.
-        
-        Installation
-        ------------
-        
-        | Install using: ``pip install weaviate-cli``
-        | Run using: ``weaviate --help``
-        
-        Articles
-        --------
-        
-        Here are some articles on weaviate: 
-        
-        - `Semantic Search Queries Return More Informed Results <https://hackernoon.com/semantic-search-queries-return-more-informed-results-nr5335nw>`_
-        - `Getting Started with Weaviate Python Library <https://towardsdatascience.com/getting-started-with-weaviate-python-client-e85d14f19e4f>`_
-        - `A sub-50ms neural search with DistilBERT and Weaviate <https://towardsdatascience.com/a-sub-50ms-neural-search-with-distilbert-and-weaviate-4857ae390154>`_
-        - `SeMI Technology Medium blogs <https://medium.com/semi-technologies>`_
-        
-        Support
-        -------
-        
-        - Use our `Slack Channel <https://join.slack.com/t/weaviate/shared_invite/zt-goaoifjr-o8FuVz9b1HLzhlUfyfddhw>`_ for support or any other question.
-        - Use the ``weaviate`` tag on `Stackoverflow <https://stackoverflow.com/questions/tagged/weaviate>`_  for questions.
-        - For bugs and/or problems with the package submit a Github `issue <https://github.com/semi-technologies/weaviate-python-client/issues>`_.
-        
-        Contributing
-        ------------
-        
-        - Do you want to contribute to `Weaviate`, read `How to Contribute <https://github.com/semi-technologies/weaviate/blob/master/CONTRIBUTE.md>`_.
-        
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Weaviate CLI
+============
+.. image:: https://raw.githubusercontent.com/semi-technologies/weaviate/19de0956c69b66c5552447e84d016f4fe29d12c9/docs/assets/weaviate-logo.png
+    :width: 180
+    :align: right
+    :alt: Weaviate logo
+
+.. image:: https://travis-ci.com/semi-technologies/weaviate-cli.svg?branch=master
+    :target: https://travis-ci.com/semi-technologies/weaviate-cli
+    :alt: Build Status (Travis CI)
+
+.. image:: https://badge.fury.io/py/weaviate-cli.svg
+    :target: https://badge.fury.io/py/weaviate-cli
+    :alt: PyPI version
+
+
+**Command Line Interface (CLI) tool for interacting with a Weaviate instance directly from your Terminal**
+
+Visit the official `SeMi Technology <https://weaviate.io/>`_ website for more information about the Weaviate and how to use it in production.
+
+Check out our `weaviate-client <https://pypi.org/project/weaviate-client/>`_ library for interacting with a Weaviate instance using python.
+
+Installation
+------------
+
+| Install using: ``pip install weaviate-cli``
+| Run using: ``weaviate --help``
+
+Articles
+--------
+
+Here are some articles on weaviate: 
+
+- `Semantic Search Queries Return More Informed Results <https://hackernoon.com/semantic-search-queries-return-more-informed-results-nr5335nw>`_
+- `Getting Started with Weaviate Python Library <https://towardsdatascience.com/getting-started-with-weaviate-python-client-e85d14f19e4f>`_
+- `A sub-50ms neural search with DistilBERT and Weaviate <https://towardsdatascience.com/a-sub-50ms-neural-search-with-distilbert-and-weaviate-4857ae390154>`_
+- `SeMI Technology Medium blogs <https://medium.com/semi-technologies>`_
+
+Support
+-------
+
+- Use our `Slack Channel <https://join.slack.com/t/weaviate/shared_invite/zt-goaoifjr-o8FuVz9b1HLzhlUfyfddhw>`_ for support or any other question.
+- Use the ``weaviate`` tag on `Stackoverflow <https://stackoverflow.com/questions/tagged/weaviate>`_  for questions.
+- For bugs and/or problems with the package submit a Github `issue <https://github.com/semi-technologies/weaviate-python-client/issues>`_.
+
+Contributing
+------------
+
+- Do you want to contribute to `Weaviate`, read `How to Contribute <https://github.com/semi-technologies/weaviate/blob/master/CONTRIBUTE.md>`_.
```

