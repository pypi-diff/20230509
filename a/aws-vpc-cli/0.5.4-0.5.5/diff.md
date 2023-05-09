# Comparing `tmp/aws-vpc-cli-0.5.4.tar.gz` & `tmp/aws-vpc-cli-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-vpc-cli-0.5.4.tar", last modified: Sat Apr  1 00:45:44 2023, max compression
+gzip compressed data, was "aws-vpc-cli-0.5.5.tar", last modified: Tue May  9 06:37:01 2023, max compression
```

## Comparing `aws-vpc-cli-0.5.4.tar` & `aws-vpc-cli-0.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 00:45:44.092421 aws-vpc-cli-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-01 00:45:44.092421 aws-vpc-cli-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 00:45:44.092421 aws-vpc-cli-0.5.4/aws_vpc_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-01 00:45:44.000000 aws-vpc-cli-0.5.4/aws_vpc_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-01 00:45:44.000000 aws-vpc-cli-0.5.4/aws_vpc_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 00:45:44.000000 aws-vpc-cli-0.5.4/aws_vpc_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-01 00:45:44.000000 aws-vpc-cli-0.5.4/aws_vpc_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-01 00:45:44.000000 aws-vpc-cli-0.5.4/aws_vpc_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-01 00:45:44.000000 aws-vpc-cli-0.5.4/aws_vpc_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-01 00:45:44.092421 aws-vpc-cli-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 00:45:44.092421 aws-vpc-cli-0.5.4/vpc_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/vpc_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/vpc_cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    15985 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/vpc_cli/create_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/vpc_cli/deploy_cfn.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/vpc_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/vpc_cli/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/vpc_cli/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-01 00:45:28.000000 aws-vpc-cli-0.5.4/vpc_cli/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:37:01.923454 aws-vpc-cli-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 06:37:01.923454 aws-vpc-cli-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:37:01.919454 aws-vpc-cli-0.5.5/aws_vpc_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 06:37:01.000000 aws-vpc-cli-0.5.5/aws_vpc_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-09 06:37:01.000000 aws-vpc-cli-0.5.5/aws_vpc_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:37:01.000000 aws-vpc-cli-0.5.5/aws_vpc_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 06:37:01.000000 aws-vpc-cli-0.5.5/aws_vpc_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-09 06:37:01.000000 aws-vpc-cli-0.5.5/aws_vpc_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 06:37:01.000000 aws-vpc-cli-0.5.5/aws_vpc_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-09 06:37:01.923454 aws-vpc-cli-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:37:01.923454 aws-vpc-cli-0.5.5/vpc_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/vpc_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/vpc_cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15985 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/vpc_cli/create_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/vpc_cli/deploy_cfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/vpc_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/vpc_cli/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/vpc_cli/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-09 06:36:41.000000 aws-vpc-cli-0.5.5/vpc_cli/validators.py
```

### Comparing `aws-vpc-cli-0.5.4/LICENSE` & `aws-vpc-cli-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-vpc-cli-0.5.4/README.md` & `aws-vpc-cli-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `aws-vpc-cli-0.5.4/setup.py` & `aws-vpc-cli-0.5.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from setuptools import setup, find_packages
 
 requires = [
-    'ansicon==1.89.0',
-    'aws-cloudformation-visualizer==0.0.2',
-    'blessed==1.20.0',
-    'boto3==1.26.104',
-    'botocore==1.29.104',
-    'inquirer==3.1.3',
-    'ipaddr==2.2.0',
-    'jinxed==1.2.0',
-    'jmespath==1.0.1',
-    'prettytable==3.6.0',
-    'pyfiglet==0.8.post1',
-    'python-dateutil==2.8.2',
-    'python-editor==1.0.4',
-    'PyYAML==6.0',
+    'ansicon>=1.89.0',
+    'aws-cloudformation-visualizer>=0.0.2',
+    'blessed>=1.20.0',
+    'boto3>=1.26.81',
+    'botocore>=1.29.81',
+    'inquirer>=3.1.2',
+    'ipaddr>=2.2.0',
+    'jinxed>=1.2.0',
+    'jmespath>=1.0.1',
+    'prettytable>=3.6.0',
+    'pyfiglet>=0.8.post1',
+    'python-dateutil>=2.8.2',
+    'python-editor>=1.0.4',
+    'PyYAML>=6.0',
     'readchar==4.0.3',
-    's3transfer==0.6.0',
-    'six==1.16.0',
-    'urllib3==1.26.14',
-    'wcwidth==0.2.6',
+    's3transfer>=0.6.0',
+    'six>=1.16.0',
+    'urllib3>=1.26.14',
+    'wcwidth>=0.2.6',
 ]
 
 setup(
     name='aws-vpc-cli',
-    version='0.5.4',
+    version='0.5.5',
     author='marcus16-kang',
     description='AWS VPC CloudFormation Stack Generator',
     author_email='marcus16-kang@outlook.com',
     license='MIT',
     entry_points={
         'console_scripts': [
             'vpc-cli=vpc_cli.main:main'
```

### Comparing `aws-vpc-cli-0.5.4/vpc_cli/command.py` & `aws-vpc-cli-0.5.5/vpc_cli/command.py`

 * *Files identical despite different names*

### Comparing `aws-vpc-cli-0.5.4/vpc_cli/create_yaml.py` & `aws-vpc-cli-0.5.5/vpc_cli/create_yaml.py`

 * *Files identical despite different names*

### Comparing `aws-vpc-cli-0.5.4/vpc_cli/deploy_cfn.py` & `aws-vpc-cli-0.5.5/vpc_cli/deploy_cfn.py`

 * *Files identical despite different names*

### Comparing `aws-vpc-cli-0.5.4/vpc_cli/main.py` & `aws-vpc-cli-0.5.5/vpc_cli/main.py`

 * *Files identical despite different names*

### Comparing `aws-vpc-cli-0.5.4/vpc_cli/print_table.py` & `aws-vpc-cli-0.5.5/vpc_cli/print_table.py`

 * *Files identical despite different names*

### Comparing `aws-vpc-cli-0.5.4/vpc_cli/tools.py` & `aws-vpc-cli-0.5.5/vpc_cli/tools.py`

 * *Files identical despite different names*

### Comparing `aws-vpc-cli-0.5.4/vpc_cli/validators.py` & `aws-vpc-cli-0.5.5/vpc_cli/validators.py`

 * *Files identical despite different names*

