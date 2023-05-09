# Comparing `tmp/ssm-ps-template-1.0.0a0.tar.gz` & `tmp/ssm-ps-template-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-1.0.0a0.tar", last modified: Fri May  5 21:14:48 2023, max compression
+gzip compressed data, was "ssm-ps-template-1.0.0b1.tar", last modified: Tue May  9 17:26:34 2023, max compression
```

## Comparing `ssm-ps-template-1.0.0a0.tar` & `ssm-ps-template-1.0.0b1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 21:14:48.969203 ssm-ps-template-1.0.0a0/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     5159 2023-05-05 21:14:48.965203 ssm-ps-template-1.0.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2819 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)     1592 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 21:14:48.969203 ssm-ps-template-1.0.0a0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 21:14:48.965203 ssm-ps-template-1.0.0a0/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 21:14:48.965203 ssm-ps-template-1.0.0a0/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5159 2023-05-05 21:14:48.000000 ssm-ps-template-1.0.0a0/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-05 21:14:48.000000 ssm-ps-template-1.0.0a0/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 21:14:48.000000 ssm-ps-template-1.0.0a0/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-05 21:14:48.000000 ssm-ps-template-1.0.0a0/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-05-05 21:14:48.000000 ssm-ps-template-1.0.0a0/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-05 21:14:48.000000 ssm-ps-template-1.0.0a0/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 21:14:48.965203 ssm-ps-template-1.0.0a0/tests/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-05-05 21:14:34.000000 ssm-ps-template-1.0.0a0/tests/test_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7706 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:26:34.106467 ssm-ps-template-1.0.0b1/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/discover.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7706 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-09 17:26:34.000000 ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:26:34.110467 ssm-ps-template-1.0.0b1/tests/
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/tests/test_discover.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-05-09 17:26:24.000000 ssm-ps-template-1.0.0b1/tests/test_render.py
```

### Comparing `ssm-ps-template-1.0.0a0/LICENSE.txt` & `ssm-ps-template-1.0.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0a0/PKG-INFO` & `ssm-ps-template-1.0.0b1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0a0
+Version: 1.0.0b1
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -69,36 +69,84 @@
 | `region`    | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
 | `verbose`   | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
 The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
 
-| Directive     | Description                                            |
-|---------------|--------------------------------------------------------|
-| `source`      | The source file of the template                        |
-| `destination` | The destination path to write the rendered template to |
+| Directive     | Description                                                                          |
+|---------------|--------------------------------------------------------------------------------------|
+| `source`      | The source file of the template                                                      |
+| `destination` | The destination path to write the rendered template to                               |
+| `prefix`      | The prefix to prepend variables with if they do not start with a forward-slash (`/`) |
+
+### Extended Templating Functionality
+
+In addition to the base functionality exposed by Jinja2, the following Python functions have been added:
+
+| Function   | Definition                                                                                                                                          |
+|------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
+| `urlparse` | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
+| `parse_qs` | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
+| `unquote`  | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
+
+The following filters are added:
+
+| Filter   | Description                         |
+|----------|-------------------------------------|
+| `toyaml` | Converts a dictionary value to YAML |
+
+The following variables are exposed:
+
+| Variable  | Definition                                                                                                              |
+|-----------|-------------------------------------------------------------------------------------------------------------------------|
+| `environ` | The [`os.environ`](https://docs.python.org/3/library/os.html#os.environ) dictionary for accessing environment variables |
 
 ### Configuration File Format
 
 The application supports JSON, TOML, or YAML for configuration. The following example is in YAML:
 
 ### Example Configuration File
 
 ```yaml
 templates:
   - source: /etc/ssm-templates/nginx-example
     destination: /etc/nginx/sites-available/example
+    prefix: /namespaced/application/nginx/
   - source: /etc/ssm-templates/postgres-example
     destination: /etc/postgresql/14/main/postgresql.conf
+    prefix: /namespaced/application/postgres/
 profile: default
 region: us-east-1
 verbose: false
 ```
 
+## Path Based Dictionaries
+
+In more complex templates it's possible to need a dictionary of values from SSM instead of straight key/value usage.
+
+This is achieved by setting a variable to a key with a trailing slash (`/`).
+
+The following pattern will retrieve all keys under a path and return them as a nested dictionary with a `/` delimiter,
+and then iterate over the key/value pairs:
+
+```
+{% set values = settings/ %}
+{% for key, value in settings.items() %}
+  {{ key }}: {{ value }}
+{% endfor %}
+```
+
+Or to convert them to YAML:
+
+```
+settings: {% set values = settings/ %}
+{{ values | toyaml | indent(2, first=True) }}
+```
+
 ## Command Line Usage
 
 ```
 usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--verbose] config
 
 Templating for SSM Parameter Store
```

### Comparing `ssm-ps-template-1.0.0a0/pyproject.toml` & `ssm-ps-template-1.0.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "ssm-ps-template"
-version = "1.0.0a0"
+version = "1.0.0b1"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3"
 ]
 dependencies = [
     "boto3>=1.26.127,<2",
+    "flatdict>=4,<5",
     "jinja2>=3,<4",
     "pyyaml>=6,<7",
     "toml>=0.10,<1"
 ]
 keywords = ["aws", "ssm", "parameter store", "templating"]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
@@ -36,16 +37,15 @@
     "flake8-comprehensions",
     "flake8-deprecated",
     "flake8-import-order",
     "flake8-print",
     "flake8-pyproject",
     "flake8-quotes",
     "flake8-rst-docstrings",
-    "flake8-tuple",
-    "yapf"
+    "flake8-tuple"
 ]
 
 [tool.coverage.run]
 branch = true
 command_line = "-m unittest discover tests --verbose"
 data_file = "build/.coverage"
```

### Comparing `ssm-ps-template-1.0.0a0/ssm_ps_template/__main__.py` & `ssm-ps-template-1.0.0b1/ssm_ps_template/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 import argparse
 from importlib import metadata
 import logging
+import sys
 import time
+import typing
 
-from ssm_ps_template import config, render, ssm
+from botocore import exceptions
+
+from ssm_ps_template import config, discover, render, ssm
 
 LOGGER = logging.getLogger(__name__)
 
 
 def parse_cli_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description='Templating for SSM Parameter Store')
     parser.add_argument('--aws-profile', action='store', help='AWS Profile')
     parser.add_argument('--aws-region', action='store', help='AWS Region')
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('config', type=config.configuration_file, nargs=1)
     return parser.parse_args()
 
 
-def main():
-    args = parse_cli_arguments()
-    verbose = args.config[0].verbose or args.verbose
-    logging.basicConfig(level=logging.DEBUG if verbose else logging.INFO)
-    LOGGER.info('ssm-ps-template v%s', metadata.version('ssm-ps-template'))
+def render_templates(args: argparse.Namespace) -> typing.NoReturn:
     parameter_store = ssm.ParameterStore(
         profile=args.aws_profile or args.config[0].profile,
         region=args.aws_region or args.config[0].region)
+
     start_time = time.time()
     for template in args.config[0].templates:
-        renderer = render.Renderer(
-            source=template.source)
-        variables = renderer.discover_variables()
-        LOGGER.debug('Variables: %r', variables)
-        values = parameter_store.fetch_variables(variables)
+        variable_discovery = discover.Variables(template.source)
+        variables = sorted(variable_discovery.discover())
+
+        try:
+            values = parameter_store.fetch_variables(variables,
+                                                     template.prefix)
+        except (exceptions.ClientError, exceptions.UnauthorizedSSOTokenError):
+            sys.exit(1)
+
+        renderer = render.Renderer(source=template.source, variables=variables)
         with template.destination.open('w') as handle:
             handle.write(renderer.render(values))
-        LOGGER.info('Rendered %s in %0.2f seconds',
-                    template.destination, time.time() - start_time)
+
+        LOGGER.info('Rendered %s in %0.2f seconds', template.destination,
+                    time.time() - start_time)
+
+
+def main():
+    args = parse_cli_arguments()
+
+    verbose = args.config[0].verbose or args.verbose
+    logging.basicConfig(level=logging.DEBUG if verbose else logging.INFO)
+    for logger in ['boto3', 'botocore', 'urllib3']:
+        logging.getLogger(logger).setLevel(logging.INFO)
+
+    LOGGER.info('ssm-ps-template v%s', metadata.version('ssm-ps-template'))
+    render_templates(args)
```

### Comparing `ssm-ps-template-1.0.0a0/ssm_ps_template/config.py` & `ssm-ps-template-1.0.0b1/ssm_ps_template/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,45 +8,45 @@
 import yaml
 
 
 @dataclasses.dataclass
 class Template:
     source: pathlib.Path
     destination: pathlib.Path
+    prefix: typing.Optional[str]
 
 
 @dataclasses.dataclass
 class Configuration:
     templates: list[Template]
     profile: typing.Optional[str]
     region: typing.Optional[str]
     verbose: bool
 
 
 def _load_configuration(value: dict) -> Configuration:
     try:
-        return Configuration(
-            templates=[_entry_to_template(**template)
-                       for template in value['templates']],
-            profile=value.get('profile'),
-            region=value.get('region'),
-            verbose=value.get('verbose', False))
+        return Configuration(templates=[_entry_to_template(**template)
+                                        for template in value['templates']],
+                             profile=value.get('profile'),
+                             region=value.get('region'),
+                             verbose=value.get('verbose', False))
     except KeyError as error:
         raise argparse.ArgumentTypeError(
             f'Failed to load configuration due to invalid key: {error}')
 
 
 def _entry_to_template(**kwargs) -> Template:
     source = pathlib.Path(kwargs['source'])
     if not source.exists():
         raise argparse.ArgumentTypeError(
             f'Specified template {source} does not exist')
-    return Template(
-        source=source,
-        destination=pathlib.Path(kwargs['destination']))
+    return Template(source=source,
+                    destination=pathlib.Path(kwargs['destination']),
+                    prefix=kwargs.get('prefix', None))
 
 
 def configuration_file(value: str) -> Configuration:
     """Load the configuration from the specified path"""
     path = pathlib.Path(value)
     if not path.exists():
         raise argparse.ArgumentTypeError(f'{value} does not exist')
```

### Comparing `ssm-ps-template-1.0.0a0/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-1.0.0b1/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0a0
+Version: 1.0.0b1
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -69,36 +69,84 @@
 | `region`    | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
 | `verbose`   | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
 The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
 
-| Directive     | Description                                            |
-|---------------|--------------------------------------------------------|
-| `source`      | The source file of the template                        |
-| `destination` | The destination path to write the rendered template to |
+| Directive     | Description                                                                          |
+|---------------|--------------------------------------------------------------------------------------|
+| `source`      | The source file of the template                                                      |
+| `destination` | The destination path to write the rendered template to                               |
+| `prefix`      | The prefix to prepend variables with if they do not start with a forward-slash (`/`) |
+
+### Extended Templating Functionality
+
+In addition to the base functionality exposed by Jinja2, the following Python functions have been added:
+
+| Function   | Definition                                                                                                                                          |
+|------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
+| `urlparse` | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
+| `parse_qs` | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
+| `unquote`  | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
+
+The following filters are added:
+
+| Filter   | Description                         |
+|----------|-------------------------------------|
+| `toyaml` | Converts a dictionary value to YAML |
+
+The following variables are exposed:
+
+| Variable  | Definition                                                                                                              |
+|-----------|-------------------------------------------------------------------------------------------------------------------------|
+| `environ` | The [`os.environ`](https://docs.python.org/3/library/os.html#os.environ) dictionary for accessing environment variables |
 
 ### Configuration File Format
 
 The application supports JSON, TOML, or YAML for configuration. The following example is in YAML:
 
 ### Example Configuration File
 
 ```yaml
 templates:
   - source: /etc/ssm-templates/nginx-example
     destination: /etc/nginx/sites-available/example
+    prefix: /namespaced/application/nginx/
   - source: /etc/ssm-templates/postgres-example
     destination: /etc/postgresql/14/main/postgresql.conf
+    prefix: /namespaced/application/postgres/
 profile: default
 region: us-east-1
 verbose: false
 ```
 
+## Path Based Dictionaries
+
+In more complex templates it's possible to need a dictionary of values from SSM instead of straight key/value usage.
+
+This is achieved by setting a variable to a key with a trailing slash (`/`).
+
+The following pattern will retrieve all keys under a path and return them as a nested dictionary with a `/` delimiter,
+and then iterate over the key/value pairs:
+
+```
+{% set values = settings/ %}
+{% for key, value in settings.items() %}
+  {{ key }}: {{ value }}
+{% endfor %}
+```
+
+Or to convert them to YAML:
+
+```
+settings: {% set values = settings/ %}
+{{ values | toyaml | indent(2, first=True) }}
+```
+
 ## Command Line Usage
 
 ```
 usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--verbose] config
 
 Templating for SSM Parameter Store
```

### Comparing `ssm-ps-template-1.0.0a0/tests/test_config.py` & `ssm-ps-template-1.0.0b1/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,37 +8,35 @@
 class TestCase1(unittest.TestCase):
 
     def setUp(self) -> None:
         self.expectation = config.Configuration(
             templates=[
                 config.Template(
                     source=pathlib.Path('tests/templates/case1a.tmpl'),
-                    destination=pathlib.Path('build/case1a.out')),
+                    destination=pathlib.Path('build/case1a.out'),
+                    prefix=None),
                 config.Template(
                     source=pathlib.Path('tests/templates/case1b.tmpl'),
-                    destination=pathlib.Path('build/case1b.out')),
-            ],
+                    destination=pathlib.Path('build/case1b.out'),
+                    prefix=None)],
             profile=None,
             region=None,
             verbose=False)
 
     def test_load_json_file(self):
-        self.assertEqual(
-            config.configuration_file('tests/config/case1.json'),
-            self.expectation)
+        self.assertEqual(config.configuration_file('tests/config/case1.json'),
+                         self.expectation)
 
     def test_load_toml_file(self):
-        self.assertEqual(
-            config.configuration_file('tests/config/case1.toml'),
-            self.expectation)
+        self.assertEqual(config.configuration_file('tests/config/case1.toml'),
+                         self.expectation)
 
     def test_load_yaml_file(self):
-        self.assertEqual(
-            config.configuration_file('tests/config/case1.yaml'),
-            self.expectation)
+        self.assertEqual(config.configuration_file('tests/config/case1.yaml'),
+                         self.expectation)
 
 
 class TestCase2(unittest.TestCase):
 
     def test_invalid_file_type(self):
         with self.assertRaises(argparse.ArgumentTypeError):
             config.configuration_file('tests/config/case2d.ini')
```

