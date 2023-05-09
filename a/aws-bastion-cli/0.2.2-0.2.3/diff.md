# Comparing `tmp/aws-bastion-cli-0.2.2.tar.gz` & `tmp/aws-bastion-cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-bastion-cli-0.2.2.tar", last modified: Fri Apr  7 11:30:22 2023, max compression
+gzip compressed data, was "aws-bastion-cli-0.2.3.tar", last modified: Tue May  9 06:40:16 2023, max compression
```

## Comparing `aws-bastion-cli-0.2.2.tar` & `aws-bastion-cli-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:30:22.022451 aws-bastion-cli-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-07 11:30:22.022451 aws-bastion-cli-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:30:22.022451 aws-bastion-cli-0.2.2/aws_bastion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-07 11:30:22.000000 aws-bastion-cli-0.2.2/aws_bastion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-07 11:30:22.000000 aws-bastion-cli-0.2.2/aws_bastion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 11:30:22.000000 aws-bastion-cli-0.2.2/aws_bastion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-07 11:30:22.000000 aws-bastion-cli-0.2.2/aws_bastion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-07 11:30:22.000000 aws-bastion-cli-0.2.2/aws_bastion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 11:30:22.000000 aws-bastion-cli-0.2.2/aws_bastion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:30:22.022451 aws-bastion-cli-0.2.2/bastion_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/bastion_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/bastion_cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/bastion_cli/create_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/bastion_cli/deploy_cfn.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/bastion_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/bastion_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/bastion_cli/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-07 11:30:22.026451 aws-bastion-cli-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-07 11:30:07.000000 aws-bastion-cli-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:40:16.655913 aws-bastion-cli-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 06:40:16.655913 aws-bastion-cli-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:40:16.651914 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:40:16.655913 aws-bastion-cli-0.2.3/bastion_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/create_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/deploy_cfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-09 06:40:16.655913 aws-bastion-cli-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/setup.py
```

### Comparing `aws-bastion-cli-0.2.2/LICENSE` & `aws-bastion-cli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.2/README.md` & `aws-bastion-cli-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.2/bastion_cli/command.py` & `aws-bastion-cli-0.2.3/bastion_cli/command.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.2/bastion_cli/create_yaml.py` & `aws-bastion-cli-0.2.3/bastion_cli/create_yaml.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.2/bastion_cli/deploy_cfn.py` & `aws-bastion-cli-0.2.3/bastion_cli/deploy_cfn.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.2/bastion_cli/main.py` & `aws-bastion-cli-0.2.3/bastion_cli/main.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.2/bastion_cli/utils.py` & `aws-bastion-cli-0.2.3/bastion_cli/utils.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.2/bastion_cli/validators.py` & `aws-bastion-cli-0.2.3/bastion_cli/validators.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.2/setup.py` & `aws-bastion-cli-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 
 requires = [
-    'ansicon==1.89.0',
-    'aws-cloudformation-visualizer==0.0.2',
-    'blessed==1.20.0',
-    'boto3==1.26.104',
-    'botocore==1.29.104',
-    'inquirer==3.1.3',
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
+    'boto3>=1.26.104',
+    'botocore>=1.29.104',
+    'inquirer>=3.1.3',
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
     name='aws-bastion-cli',
-    version='0.2.2',
+    version='0.2.3',
     author='marcus16-kang',
     description='AWS Bastion EC2 Server Stack Generator',
     author_email='marcus16-kang@outlook.com',
     license='MIT',
     entry_points={
         'console_scripts': [
             'bastion-cli=bastion_cli.main:main'
```

