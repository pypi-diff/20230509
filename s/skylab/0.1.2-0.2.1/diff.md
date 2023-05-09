# Comparing `tmp/skylab-0.1.2.tar.gz` & `tmp/skylab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skylab-0.1.2.tar", max compression
+gzip compressed data, was "skylab-0.2.1.tar", max compression
```

## Comparing `skylab-0.1.2.tar` & `skylab-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,18 @@
--rw-r--r--   0        0        0     1090 2023-04-23 21:28:56.735383 skylab-0.1.2/LICENSE
--rw-r--r--   0        0        0      831 2023-05-03 21:42:11.409035 skylab-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      857 2023-05-03 19:11:19.310742 skylab-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-21 22:27:55.460381 skylab-0.1.2/skylab/__init__.py
--rw-r--r--   0        0        0      236 2023-04-23 22:12:51.429163 skylab-0.1.2/skylab/__main__.py
--rw-r--r--   0        0        0     1471 2023-05-03 21:07:31.551740 skylab-0.1.2/skylab/api.py
--rw-r--r--   0        0        0      424 2023-04-24 13:45:07.205633 skylab-0.1.2/skylab/css/styles.css
--rw-r--r--   0        0        0     1668 2023-04-25 20:23:37.949077 skylab-0.1.2/skylab/models.py
--rw-r--r--   0        0        0     5206 2023-05-03 21:04:54.108267 skylab-0.1.2/skylab/skylab.py
--rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 skylab-0.1.2/setup.py
--rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 skylab-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-23 21:28:56.735383 skylab-0.2.1/LICENSE
+-rw-r--r--   0        0        0      831 2023-05-09 20:11:40.082775 skylab-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      992 2023-05-09 20:11:40.080758 skylab-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 22:27:55.460381 skylab-0.2.1/skylab/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-09 19:36:42.274492 skylab-0.2.1/skylab/__main__.py
+-rw-r--r--   0        0        0     2289 2023-05-09 20:11:40.082775 skylab-0.2.1/skylab/api.py
+-rw-r--r--   0        0        0     1054 2023-05-09 20:11:40.083772 skylab-0.2.1/skylab/css/styles.css
+-rw-r--r--   0        0        0        0 2023-05-09 20:11:40.083772 skylab-0.2.1/skylab/models/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-09 20:11:40.084775 skylab-0.2.1/skylab/models/event_models.py
+-rw-r--r--   0        0        0     1928 2023-05-09 20:11:40.084775 skylab-0.2.1/skylab/models/launch_models.py
+-rw-r--r--   0        0        0      224 2023-05-09 20:11:40.084775 skylab-0.2.1/skylab/settings.py
+-rw-r--r--   0        0        0     2243 2023-05-09 20:11:40.085772 skylab-0.2.1/skylab/skylab.py
+-rw-r--r--   0        0        0        0 2023-05-09 20:11:40.085772 skylab-0.2.1/skylab/widgets/__init__.py
+-rw-r--r--   0        0        0     2154 2023-05-09 20:11:40.085772 skylab-0.2.1/skylab/widgets/event_widget.py
+-rw-r--r--   0        0        0     2696 2023-05-09 20:11:40.086774 skylab-0.2.1/skylab/widgets/launch_widget.py
+-rw-r--r--   0        0        0     1579 2023-05-09 20:11:40.086774 skylab-0.2.1/skylab/widgets/time_widget.py
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 skylab-0.2.1/setup.py
+-rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 skylab-0.2.1/PKG-INFO
```

### Comparing `skylab-0.1.2/LICENSE` & `skylab-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skylab-0.1.2/pyproject.toml` & `skylab-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "skylab"
-version = "0.1.2"
+version = "0.2.1"
 description = "A TUI for showing latest upcoming rocket launches."
 authors = ["SerhiiStets <stets.serhii@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository="https://github.com/SerhiiStets/skylab"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytest = "^7.3.1"
-textual = {extras = ["dev"], version = "^0.19.1"}
+textual = {version = "^0.19.1", extras = ["dev"]}
 pydantic = "^1.10.7"
 tzlocal = "^4.3"
 requests = "^2.28.2"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `skylab-0.1.2/README.md` & `skylab-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Skylab
 
 Skylab is a text user interface (TUI) tool that displays upcoming space launches in a user-friendly way.
 
+![skylab](https://i.imgur.com/Hopa3mN.png)
+
+Skylab is built using the [Textual](https://github.com/Textualize/textual) framework.
+
 ## Instalation
 
 To install Skylab using pip, run the following command:
 
 ```
 $ pip install skylab
 ```
```

### Comparing `skylab-0.1.2/skylab/models.py` & `skylab-0.2.1/skylab/models/launch_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,42 @@
 
 from typing import Union
 
 from pydantic import BaseModel, Field, validator
 
 
 class LaunchProvier(BaseModel):
+    """Provider information for the launch (i.e. SpaceX)."""
+
     name: str
 
 
 class Mission(BaseModel):
+    """Mission information for the launch."""
+
     name: str
     description: str
 
 
 class Rocket(BaseModel):
+    """Rocket configuration for the launch."""
+
     full_name: str
 
 
 class LaunchPad(BaseModel):
+    """Launch pad information for the launch."""
+
     name: str
     address: str
 
 
 class Launch(BaseModel):
+    """Launch model from SpaceDev API."""
+
     name: str
     net: str
     pad: LaunchPad = Field(LaunchPad(name="Unknown", address="Unknown"))
     rocket: Rocket = Field(Rocket(full_name="Rocket name not yet provided."))
     mission: Mission = Field(
         Mission(name="No name", description="No mission description yet.")
     )
```

### Comparing `skylab-0.1.2/setup.py` & `skylab-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['skylab']
+['skylab', 'skylab.models', 'skylab.widgets']
 
 package_data = \
 {'': ['*'], 'skylab': ['css/*']}
 
 install_requires = \
 ['pydantic>=1.10.7,<2.0.0',
  'pytest-cov>=4.0.0,<5.0.0',
@@ -16,17 +16,17 @@
  'tzlocal>=4.3,<5.0']
 
 entry_points = \
 {'console_scripts': ['skylab = skylab.__main__:main']}
 
 setup_kwargs = {
     'name': 'skylab',
-    'version': '0.1.2',
+    'version': '0.2.1',
     'description': 'A TUI for showing latest upcoming rocket launches.',
-    'long_description': '# Skylab\n\nSkylab is a text user interface (TUI) tool that displays upcoming space launches in a user-friendly way.\n\n## Instalation\n\nTo install Skylab using pip, run the following command:\n\n```\n$ pip install skylab\n```\n\n## Usage\n\nTo use Skylab, simply enter the following command in your terminal:\n\n```\n$ skylab\n```\n\n## Contributing\n\nHelp in testing, development, documentation and other tasks is\nhighly appreciated and useful to the project.\n\nTo get started with developing skylab, see [CONTRIBUTING.md](CONTRIBUTING.md).\n\n## Acknowledgments\n\nThis project makes use of the [The Space Devs API](https://thespacedevs.com/) to retrieve data about upcoming space launches. We would like to thank the creators of this API for providing this valuable service.\n\n## License\n\nSkylab is released under the [MIT License](LICENSE.md).\n',
+    'long_description': '# Skylab\n\nSkylab is a text user interface (TUI) tool that displays upcoming space launches in a user-friendly way.\n\n![skylab](https://i.imgur.com/Hopa3mN.png)\n\nSkylab is built using the [Textual](https://github.com/Textualize/textual) framework.\n\n## Instalation\n\nTo install Skylab using pip, run the following command:\n\n```\n$ pip install skylab\n```\n\n## Usage\n\nTo use Skylab, simply enter the following command in your terminal:\n\n```\n$ skylab\n```\n\n## Contributing\n\nHelp in testing, development, documentation and other tasks is\nhighly appreciated and useful to the project.\n\nTo get started with developing skylab, see [CONTRIBUTING.md](CONTRIBUTING.md).\n\n## Acknowledgments\n\nThis project makes use of the [The Space Devs API](https://thespacedevs.com/) to retrieve data about upcoming space launches. We would like to thank the creators of this API for providing this valuable service.\n\n## License\n\nSkylab is released under the [MIT License](LICENSE.md).\n',
     'author': 'SerhiiStets',
     'author_email': 'stets.serhii@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SerhiiStets/skylab',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `skylab-0.1.2/PKG-INFO` & `skylab-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skylab
-Version: 0.1.2
+Version: 0.2.1
 Summary: A TUI for showing latest upcoming rocket launches.
 Home-page: https://github.com/SerhiiStets/skylab
 License: MIT
 Author: SerhiiStets
 Author-email: stets.serhii@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,18 @@
 Project-URL: Repository, https://github.com/SerhiiStets/skylab
 Description-Content-Type: text/markdown
 
 # Skylab
 
 Skylab is a text user interface (TUI) tool that displays upcoming space launches in a user-friendly way.
 
+![skylab](https://i.imgur.com/Hopa3mN.png)
+
+Skylab is built using the [Textual](https://github.com/Textualize/textual) framework.
+
 ## Instalation
 
 To install Skylab using pip, run the following command:
 
 ```
 $ pip install skylab
 ```
```

