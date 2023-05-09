# Comparing `tmp/qload-1.0.0.tar.gz` & `tmp/qload-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qload-1.0.0.tar", max compression
+gzip compressed data, was "qload-1.0.1.tar", max compression
```

## Comparing `qload-1.0.0.tar` & `qload-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1343 2022-12-21 19:35:12.542300 qload-1.0.0/README.md
--rw-r--r--   0        0        0      753 2022-12-21 18:36:11.492418 qload-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2967 2022-12-21 18:53:34.198324 qload-1.0.0/src/qload/__init__.py
--rw-r--r--   0        0        0     2761 2022-12-21 18:20:27.645795 qload-1.0.0/src/qload/base.py
--rw-r--r--   0        0        0     5592 2022-12-21 18:54:17.130445 qload-1.0.0/src/qload/driver.py
--rw-r--r--   0        0        0      141 2022-12-21 14:10:10.173856 qload-1.0.0/src/qload/exception.py
--rw-r--r--   0        0        0      893 2022-12-21 18:14:41.052458 qload-1.0.0/src/qload/expression.py
--rw-r--r--   0        0        0     2186 1970-01-01 00:00:00.000000 qload-1.0.0/setup.py
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 qload-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1867 2023-05-09 12:17:31.714775 qload-1.0.1/README.md
+-rw-r--r--   0        0        0      884 2023-05-09 12:18:23.418934 qload-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3492 2023-05-09 12:17:31.718775 qload-1.0.1/src/qload/__init__.py
+-rw-r--r--   0        0        0     3315 2023-05-09 12:17:31.718775 qload-1.0.1/src/qload/base.py
+-rw-r--r--   0        0        0     6660 2023-05-09 12:16:43.234626 qload-1.0.1/src/qload/driver.py
+-rw-r--r--   0        0        0      141 2022-12-21 14:10:10.173856 qload-1.0.1/src/qload/exception.py
+-rw-r--r--   0        0        0      893 2022-12-21 18:14:41.052458 qload-1.0.1/src/qload/expression.py
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 qload-1.0.1/setup.py
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 qload-1.0.1/PKG-INFO
```

### Comparing `qload-1.0.0/README.md` & `qload-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # qload : better assertion on files
 
-qload is a library to load or extract content of a file to perform assertion in automatic tests wihtout
+qload is a library to load or extract content of a file to perform assertion in automatic tests without
 boilerplate. It support file from filesystem, ftp, s3, ...
 
 ## Benefits
 
 * oneliner to assert on the content of a file
-* useful differential when the test fails
-* support for the most common formats (yaml, csv, json, txt, ...)
-* support for multiple file systems and protocols (local, ftp, s3, ...)
+* useful differential when the test fails thanks to subpart extraction
+* support for the most common formats (yaml, csv, json, txt)
+* support for multiple file systems and protocols (local, ftp, s3)
+* rich expression engine to extract part of a file ([regexp](https://docs.python.org/3/library/re.html#regular-expression-syntax) for `text` and [jmespath](https://jmespath.org) for `csv`, `json` and `yaml` to improve differential) 
 
 ## Gettings started
 
 ```bash
 pip install qload
 ```
 
@@ -28,13 +29,19 @@
 assert qload.json('s3://mybucket/file1.json') == {}
 assert qload.json('file.json', expression='$.id') == ''
 assert len(qload.json('file.json', expression='$.id')) == 4
 
 assert qload.yaml('file.yml')  == {}
 assert qload.yaml('file.yml', expression='$.id')  == ''
 
-assert qload.csv('file.csv', expression='$.id') == ''
+assert qload.csv('file.csv', expression='[*].Account') == ['ALK', 'BTL', 'CKL']
+assert qload.csv('file.csv', expression='[*].Account')[0] == 'ALK'
+
+assert qload.parquet('file.parquet', expression='[*].Account')[0] == 'ALK'
 
 assert qload.ftp(host='localhost', port=21, login='admin', password='admin').csv(path='dir/file.csv', expression='') == []
 assert qload.s3(bucket='bucket', aws_access_key_id='', aws_secret_access_key='', region_name='eu-west-1', endpoint_url='http://localhost:9090').json(path='dir/file.csv') == {}
 
+
+assert qload.isfile('file.json') is True
+assert qload.s3(bucket='bucket').isfile('file.json') is True
 ```
```

### Comparing `qload-1.0.0/pyproject.toml` & `qload-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 [tool.poetry]
 name = "qload"
-version = "1.0.0"
+version = "1.0.1"
 description = "python library to perform assertion on files"
 authors = ["Fabien Arcellier <fabien.arcellier@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "qload", from = "src" },
 ]
 
+[tool.poetry.urls]
+"Source" = "https://github.com/FabienArcellier/qload"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 jsonpath-ng = "^1.5.3"
 jmespath = "^1.0.1"
 pyyaml = "^6.0"
 ftputil = "^5.0.4"
 boto3 = "^1.26.34"
+pandas = "^2.0.1"
+pyarrow = "^12.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 alfred-cli = "^1.2.0"
 fixtup = "^0.1.4"
 pytest = "^7.2.0"
 sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.1.1"
+boto3 = "^1.26.130"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tools.fixtup]
 fixtures = "tests/fixtures/fixtup"
```

### Comparing `qload-1.0.0/src/qload/__init__.py` & `qload-1.0.1/src/qload/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from typing import Optional, List, Union, Callable
 
 from qload.driver import file, ftp, s3
 
 
+def isfile(path: str, **kwargs) -> bool:
+    return file().isfile(path=path, **kwargs)
+
+
 def csv(path: str, expression: Optional[str] = None, **kwargs) ->  Union[None, str, list, dict]:
     """
     loads the content of a csv file and can filter it using jmespath expression to
     to make error display more explicit on the assertion.
 
     csv uses the csv.DictReader reader to parse and read the contents of the csv file
     into a dictionary list.
@@ -36,14 +40,25 @@
     :param path:
     :param expression: jmespath expression
     :return:
     """
     return file().json(path=path, expression=expression)
 
 
+def parquet(path:str, expression: Optional[str] = None) -> Union[None, str, list, dict]:
+    """
+    loads the content of a parquet file and can filter it using jmespath expression to
+    to make error display more explicit on the assertion.
+
+    pandas uses the pandas reader & pyarrow to parse and read the contents of the parquet file
+    into a dictionary list.
+    """
+    return file().parquet(path=path, expression=expression)
+
+
 def text(path: str, expression: Optional[str] = None, flags: int = 0) -> Union[str, List[str]]:
     """
     loads text from a file and can filter it through a regular expression
     to make the error displayed by an assertion more explicit.
 
     >>> import qload
     >>> assert qload.text('/home/fabien/file.txt') == "content"
```

### Comparing `qload-1.0.0/src/qload/base.py` & `qload-1.0.1/src/qload/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     This engine takes the file on disk or which has been moved to disk, reads its content and
     applies an expression according to the format requested by the user.
     """
 
     def __init__(self, driver: 'QloadDriver' = None):
         self.driver = driver
 
+    def isfile(self, path: str, **kwargs) -> bool:
+        isfile = self.driver.isfile(path=path)
+        return isfile
+
     def csv(self, path: str, expression: Optional[str] = None, **kwargs) ->  Union[None, str, list, dict]:
         local_path = self.driver.download(path=path)
         content = []
         with io.open(local_path) as fp:
             reader = csv.DictReader(fp, **kwargs)
             for item in reader:
                 content.append(item)
@@ -43,14 +47,26 @@
 
             if expression is None:
                 return content
 
             result = _expression.jmespath_find_all(content, expression)
             return result
 
+    def parquet(self, path: str, expression: Optional[str] = None, **kwargs) ->  Union[None, str, list, dict]:
+        local_path = self.driver.download(path=path)
+        from pandas import read_parquet
+
+        df = read_parquet(local_path)
+        content = df.to_dict('records')
+        if expression is None:
+            return content
+
+        result = _expression.jmespath_find_all(content, expression)
+        return result
+
     def text(self, path: str, expression: Optional[str] = None, flags: int = 0) -> str:
         """
 
         :param path:
         :param expression: regular expression in re.findall format
         :param flags: the regular expression’s behaviour can be modified by specifying a flags value (view https://docs.python.org/3/library/re.html#flags)
         :return:
```

### Comparing `qload-1.0.0/src/qload/driver.py` & `qload-1.0.1/src/qload/driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os.path
 import tempfile
 from typing import Optional
 
 import boto3
 import ftputil
 
 from qload.base import QloadEngine
@@ -42,38 +43,47 @@
 
 
 class QloadDriver:
     """
     the driver is an interface to download a remote file locally. A driver corresponds to a storage system.
     """
 
+
     def download(self, path: str) -> str:
         """
         primitive pour télécharger le fichier en local. Une fois téléchargée, le chemin est retourné.
 
         :param path: remote file path to download
         :return: path of the file that was downloaded locally
         """
         raise NotImplementedError
 
 
+    def isfile(self, path: str) -> bool:
+        """
+        primitive to check if a file exists
+        """
+        raise NotImplementedError
+
 class QloadDriverFile(QloadDriver):
 
+
     def download(self, path: str) -> str:
         """
         the driver which dialogues with the local filesystem does not need to download the file in order to be able to read its content.
-
-        :param path:
-        :return:
         """
         return path
 
+    def isfile(self, path: str) -> bool:
+        return os.path.isfile(path)
+
 
 class QloadDriverFtp(QloadDriver):
 
+
     def __init__(self, host: str = 'localhost', user: Optional[str] = None, passwd: Optional[str] = None, **kwargs):
         """
         Les arguments du driver correspond aux arguments de `ftplib.FTP`
 
         :param host:
         :param port:
         :param user:
@@ -98,17 +108,27 @@
         with ftputil.FTPHost(self.host, self.user, self.passwd, session_factory=my_session_factory) as host:
             if host.path.isfile(path):
                 host.download(path, filepath)
                 return filepath
 
         raise InvalidRemoteFile(path)
 
+    def isfile(self, path: str) -> bool:
+        """
+        Checks if a file exists on the ftp server
+
+        """
+        my_session_factory = ftputil.session.session_factory(**self.kwargs)
+
+        with ftputil.FTPHost(self.host, self.user, self.passwd, session_factory=my_session_factory) as host:
+            return host.path.isfile(path)
 
 class QloadDriverS3(QloadDriver):
 
+
     def __init__(self, bucket: str, endpoint_url: Optional[str] = None, region_name: Optional[str] = None, aws_access_key_id: Optional[str] = None, aws_secret_access_key: Optional[str] =  None, **kwargs):
         """
 
         :param bucket:
         :param endpoint_url: The complete URL to use for the constructed client. Normally, botocore will automatically construct the appropriate URL to use when communicating with a service.
         :param region_name: The name of the region associated with the client. A client is associated with a single region.
         :param aws_access_key_id: The access key to use when creating the client. This is entirely optional, and if not provided, the credentials configured for the session will automatically be used. You only need to provide this argument if you want to override the credentials used for this specific client.
@@ -128,15 +148,15 @@
         if aws_secret_access_key is not None:
             kwargs['aws_secret_access_key'] = aws_secret_access_key
 
         self.kwargs = kwargs
 
     def download(self, path: str) -> Optional[str]:
         """
-        QloadDriver3 loads a file from a s3 bucket into the system temporary files and
+        QloadDriverS3 loads a file from a s3 bucket into the system temporary files and
         returns the path to the downloaded file.
 
         :param path: s3 key of the file on the s3 bucket
         :return:
         """
         from botocore.errorfactory import ClientError
 
@@ -146,7 +166,24 @@
             client.head_object(Bucket=self.bucket, Key=path)
         except ClientError:
             raise InvalidRemoteFile(path)
 
         client.download_file(Bucket=self.bucket, Key=path, Filename=filepath)
         return filepath
 
+
+    def isfile(self, path: str) -> bool:
+        """
+        QloadDriverS3 checks if a file exists on the s3 bucket
+
+        >>> driver = QloadDriverS3(bucket='mybucket')
+        >>> driver.isfile(path='mykey')
+        """
+        from botocore.errorfactory import ClientError
+
+        client = boto3.client('s3', **self.kwargs)
+        _, filepath = tempfile.mkstemp()
+        try:
+            client.head_object(Bucket=self.bucket, Key=path)
+            return True
+        except ClientError:
+            return False
```

### Comparing `qload-1.0.0/src/qload/expression.py` & `qload-1.0.1/src/qload/expression.py`

 * *Files identical despite different names*

### Comparing `qload-1.0.0/setup.py` & `qload-1.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.26.34,<2.0.0',
  'ftputil>=5.0.4,<6.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'jsonpath-ng>=1.5.3,<2.0.0',
+ 'pandas>=2.0.1,<3.0.0',
+ 'pyarrow>=12.0.0,<13.0.0',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'qload',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'python library to perform assertion on files',
-    'long_description': "# qload : better assertion on files\n\nqload is a library to load or extract content of a file to perform assertion in automatic tests wihtout\nboilerplate. It support file from filesystem, ftp, s3, ...\n\n## Benefits\n\n* oneliner to assert on the content of a file\n* useful differential when the test fails\n* support for the most common formats (yaml, csv, json, txt, ...)\n* support for multiple file systems and protocols (local, ftp, s3, ...)\n\n## Gettings started\n\n```bash\npip install qload\n```\n\n## Usage\n\n```python\nimport qload\n\nassert 'database_url: postgresql://127.0.0.1:5432/postgres' in qload.text('file.txt')\nassert qload.text('file.txt', expression='Hello .*') == 'Hello Fabien'\n\nassert qload.json('file.json') == {}\nassert qload.json('s3://mybucket/file1.json') == {}\nassert qload.json('file.json', expression='$.id') == ''\nassert len(qload.json('file.json', expression='$.id')) == 4\n\nassert qload.yaml('file.yml')  == {}\nassert qload.yaml('file.yml', expression='$.id')  == ''\n\nassert qload.csv('file.csv', expression='$.id') == ''\n\nassert qload.ftp(host='localhost', port=21, login='admin', password='admin').csv(path='dir/file.csv', expression='') == []\nassert qload.s3(bucket='bucket', aws_access_key_id='', aws_secret_access_key='', region_name='eu-west-1', endpoint_url='http://localhost:9090').json(path='dir/file.csv') == {}\n\n```",
+    'long_description': "# qload : better assertion on files\n\nqload is a library to load or extract content of a file to perform assertion in automatic tests without\nboilerplate. It support file from filesystem, ftp, s3, ...\n\n## Benefits\n\n* oneliner to assert on the content of a file\n* useful differential when the test fails thanks to subpart extraction\n* support for the most common formats (yaml, csv, json, txt)\n* support for multiple file systems and protocols (local, ftp, s3)\n* rich expression engine to extract part of a file ([regexp](https://docs.python.org/3/library/re.html#regular-expression-syntax) for `text` and [jmespath](https://jmespath.org) for `csv`, `json` and `yaml` to improve differential) \n\n## Gettings started\n\n```bash\npip install qload\n```\n\n## Usage\n\n```python\nimport qload\n\nassert 'database_url: postgresql://127.0.0.1:5432/postgres' in qload.text('file.txt')\nassert qload.text('file.txt', expression='Hello .*') == 'Hello Fabien'\n\nassert qload.json('file.json') == {}\nassert qload.json('s3://mybucket/file1.json') == {}\nassert qload.json('file.json', expression='$.id') == ''\nassert len(qload.json('file.json', expression='$.id')) == 4\n\nassert qload.yaml('file.yml')  == {}\nassert qload.yaml('file.yml', expression='$.id')  == ''\n\nassert qload.csv('file.csv', expression='[*].Account') == ['ALK', 'BTL', 'CKL']\nassert qload.csv('file.csv', expression='[*].Account')[0] == 'ALK'\n\nassert qload.parquet('file.parquet', expression='[*].Account')[0] == 'ALK'\n\nassert qload.ftp(host='localhost', port=21, login='admin', password='admin').csv(path='dir/file.csv', expression='') == []\nassert qload.s3(bucket='bucket', aws_access_key_id='', aws_secret_access_key='', region_name='eu-west-1', endpoint_url='http://localhost:9090').json(path='dir/file.csv') == {}\n\n\nassert qload.isfile('file.json') is True\nassert qload.s3(bucket='bucket').isfile('file.json') is True\n```",
     'author': 'Fabien Arcellier',
     'author_email': 'fabien.arcellier@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `qload-1.0.0/PKG-INFO` & `qload-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qload
-Version: 1.0.0
+Version: 1.0.1
 Summary: python library to perform assertion on files
 License: MIT
 Author: Fabien Arcellier
 Author-email: fabien.arcellier@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,28 +12,32 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.34,<2.0.0)
 Requires-Dist: ftputil (>=5.0.4,<6.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Source, https://github.com/FabienArcellier/qload
 Description-Content-Type: text/markdown
 
 # qload : better assertion on files
 
-qload is a library to load or extract content of a file to perform assertion in automatic tests wihtout
+qload is a library to load or extract content of a file to perform assertion in automatic tests without
 boilerplate. It support file from filesystem, ftp, s3, ...
 
 ## Benefits
 
 * oneliner to assert on the content of a file
-* useful differential when the test fails
-* support for the most common formats (yaml, csv, json, txt, ...)
-* support for multiple file systems and protocols (local, ftp, s3, ...)
+* useful differential when the test fails thanks to subpart extraction
+* support for the most common formats (yaml, csv, json, txt)
+* support for multiple file systems and protocols (local, ftp, s3)
+* rich expression engine to extract part of a file ([regexp](https://docs.python.org/3/library/re.html#regular-expression-syntax) for `text` and [jmespath](https://jmespath.org) for `csv`, `json` and `yaml` to improve differential) 
 
 ## Gettings started
 
 ```bash
 pip install qload
 ```
 
@@ -49,13 +53,19 @@
 assert qload.json('s3://mybucket/file1.json') == {}
 assert qload.json('file.json', expression='$.id') == ''
 assert len(qload.json('file.json', expression='$.id')) == 4
 
 assert qload.yaml('file.yml')  == {}
 assert qload.yaml('file.yml', expression='$.id')  == ''
 
-assert qload.csv('file.csv', expression='$.id') == ''
+assert qload.csv('file.csv', expression='[*].Account') == ['ALK', 'BTL', 'CKL']
+assert qload.csv('file.csv', expression='[*].Account')[0] == 'ALK'
+
+assert qload.parquet('file.parquet', expression='[*].Account')[0] == 'ALK'
 
 assert qload.ftp(host='localhost', port=21, login='admin', password='admin').csv(path='dir/file.csv', expression='') == []
 assert qload.s3(bucket='bucket', aws_access_key_id='', aws_secret_access_key='', region_name='eu-west-1', endpoint_url='http://localhost:9090').json(path='dir/file.csv') == {}
 
+
+assert qload.isfile('file.json') is True
+assert qload.s3(bucket='bucket').isfile('file.json') is True
 ```
```

