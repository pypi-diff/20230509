# Comparing `tmp/ssm-ps-template-1.0.0b1.tar.gz` & `tmp/ssm-ps-template-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-1.0.0b1.tar", last modified: Tue May  9 17:26:34 2023, max compression
+gzip compressed data, was "ssm-ps-template-1.0.0b2.tar", last modified: Tue May  9 17:49:43 2023, max compression
```

## Comparing `ssm-ps-template-1.0.0b1.tar` & `ssm-ps-template-1.0.0b2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7706 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5366 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/README.md
--rw-r--r--   0 root         (0) root         (0)     1602 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:26:34.106467 ssm-ps-template-1.0.0b1/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/discover.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7706 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/tests/
--rw-r--r--   0 root         (0) root         (0)     2244 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/tests/test_discover.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/tests/test_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:49:43.911334 ssm-ps-template-1.0.0b2/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-05-09 17:49:43.911334 ssm-ps-template-1.0.0b2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 17:49:43.911334 ssm-ps-template-1.0.0b2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:49:43.907334 ssm-ps-template-1.0.0b2/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/ssm_ps_template/discover.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:49:43.911334 ssm-ps-template-1.0.0b2/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-05-09 17:49:43.000000 ssm-ps-template-1.0.0b2/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-09 17:49:43.000000 ssm-ps-template-1.0.0b2/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:49:43.000000 ssm-ps-template-1.0.0b2/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-09 17:49:43.000000 ssm-ps-template-1.0.0b2/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-09 17:49:43.000000 ssm-ps-template-1.0.0b2/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-09 17:49:43.000000 ssm-ps-template-1.0.0b2/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:49:43.911334 ssm-ps-template-1.0.0b2/tests/
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/tests/test_discover.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-05-09 17:49:31.000000 ssm-ps-template-1.0.0b2/tests/test_render.py
```

### Comparing `ssm-ps-template-1.0.0b1/LICENSE.txt` & `ssm-ps-template-1.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b1/PKG-INFO` & `ssm-ps-template-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -142,22 +142,22 @@
 settings: {% set values = settings/ %}
 {{ values | toyaml | indent(2, first=True) }}
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--verbose] config
-
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix] [--verbose] config
 Templating for SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
+  --prefix              Default SSM Key Prefix
   --verbose
 ```
```

### Comparing `ssm-ps-template-1.0.0b1/README.md` & `ssm-ps-template-1.0.0b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,22 +100,22 @@
 settings: {% set values = settings/ %}
 {{ values | toyaml | indent(2, first=True) }}
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--verbose] config
-
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix] [--verbose] config
 Templating for SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
+  --prefix              Default SSM Key Prefix
   --verbose
 ```
```

### Comparing `ssm-ps-template-1.0.0b1/pyproject.toml` & `ssm-ps-template-1.0.0b2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ssm-ps-template-1.0.0b1/ssm_ps_template/__main__.py` & `ssm-ps-template-1.0.0b2/ssm_ps_template/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 
 def parse_cli_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description='Templating for SSM Parameter Store')
     parser.add_argument('--aws-profile', action='store', help='AWS Profile')
     parser.add_argument('--aws-region', action='store', help='AWS Region')
+    parser.add_argument('--prefix', action='store_true',
+                        help='Default SSM Key Prefix')
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('config', type=config.configuration_file, nargs=1)
     return parser.parse_args()
 
 
 def render_templates(args: argparse.Namespace) -> typing.NoReturn:
     parameter_store = ssm.ParameterStore(
```

### Comparing `ssm-ps-template-1.0.0b1/ssm_ps_template/config.py` & `ssm-ps-template-1.0.0b2/ssm_ps_template/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,34 @@
     profile: typing.Optional[str]
     region: typing.Optional[str]
     verbose: bool
 
 
 def _load_configuration(value: dict) -> Configuration:
     try:
-        return Configuration(templates=[_entry_to_template(**template)
-                                        for template in value['templates']],
-                             profile=value.get('profile'),
-                             region=value.get('region'),
-                             verbose=value.get('verbose', False))
+        return Configuration(
+            templates=[
+                _entry_to_template(prefix=value.get('prefix'), **template)
+                for template in value['templates']],
+            profile=value.get('profile'),
+            region=value.get('region'),
+            verbose=value.get('verbose', False))
     except KeyError as error:
         raise argparse.ArgumentTypeError(
             f'Failed to load configuration due to invalid key: {error}')
 
 
-def _entry_to_template(**kwargs) -> Template:
+def _entry_to_template(prefix: typing.Optional[str], **kwargs) -> Template:
     source = pathlib.Path(kwargs['source'])
     if not source.exists():
         raise argparse.ArgumentTypeError(
             f'Specified template {source} does not exist')
     return Template(source=source,
                     destination=pathlib.Path(kwargs['destination']),
-                    prefix=kwargs.get('prefix', None))
+                    prefix=kwargs.get('prefix', prefix))
 
 
 def configuration_file(value: str) -> Configuration:
     """Load the configuration from the specified path"""
     path = pathlib.Path(value)
     if not path.exists():
         raise argparse.ArgumentTypeError(f'{value} does not exist')
```

### Comparing `ssm-ps-template-1.0.0b1/ssm_ps_template/discover.py` & `ssm-ps-template-1.0.0b2/ssm_ps_template/discover.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b1/ssm_ps_template/render.py` & `ssm-ps-template-1.0.0b2/ssm_ps_template/render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b1/ssm_ps_template/ssm.py` & `ssm-ps-template-1.0.0b2/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-1.0.0b2/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -142,22 +142,22 @@
 settings: {% set values = settings/ %}
 {{ values | toyaml | indent(2, first=True) }}
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--verbose] config
-
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix] [--verbose] config
 Templating for SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
+  --prefix              Default SSM Key Prefix
   --verbose
 ```
```

### Comparing `ssm-ps-template-1.0.0b1/tests/test_config.py` & `ssm-ps-template-1.0.0b2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b1/tests/test_render.py` & `ssm-ps-template-1.0.0b2/tests/test_render.py`

 * *Files identical despite different names*

