# Comparing `tmp/yaml_config_builder-8.0.0.tar.gz` & `tmp/yaml_config_builder-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_config_builder-8.0.0.tar", max compression
+gzip compressed data, was "yaml_config_builder-8.0.1.tar", max compression
```

## Comparing `yaml_config_builder-8.0.0.tar` & `yaml_config_builder-8.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    12061 2023-02-06 18:47:48.683449 yaml_config_builder-8.0.0/LICENSE
--rw-r--r--   0        0        0      950 2023-02-06 18:47:48.683449 yaml_config_builder-8.0.0/README.md
--rw-r--r--   0        0        0     2832 2023-02-09 14:38:03.194712 yaml_config_builder-8.0.0/pyproject.toml
--rw-r--r--   0        0        0      338 2023-02-06 18:47:48.687449 yaml_config_builder-8.0.0/src/config_builder/__init__.py
--rw-r--r--   0        0        0    17637 2023-02-08 11:32:44.235780 yaml_config_builder-8.0.0/src/config_builder/base_config_class.py
--rw-r--r--   0        0        0    13327 2023-02-09 14:36:15.551210 yaml_config_builder-8.0.0/src/config_builder/config_builder.py
--rw-r--r--   0        0        0      153 2023-02-06 18:47:48.687449 yaml_config_builder-8.0.0/src/config_builder/py.typed
--rw-r--r--   0        0        0     3871 2023-02-09 14:36:15.551210 yaml_config_builder-8.0.0/src/config_builder/replacement_map.py
--rw-r--r--   0        0        0     2639 2023-02-06 18:47:48.687449 yaml_config_builder-8.0.0/src/config_builder/utils.py
--rw-r--r--   0        0        0    10468 2023-02-06 18:47:48.687449 yaml_config_builder-8.0.0/src/config_builder/yaml_constructors.py
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.0/setup.py
--rw-r--r--   0        0        0     2321 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0    12061 2023-05-09 06:24:29.607523 yaml_config_builder-8.0.1/LICENSE
+-rw-r--r--   0        0        0      950 2023-05-09 06:24:29.607523 yaml_config_builder-8.0.1/README.md
+-rw-r--r--   0        0        0     2832 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/pyproject.toml
+-rw-r--r--   0        0        0      338 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/__init__.py
+-rw-r--r--   0        0        0    17637 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/base_config_class.py
+-rw-r--r--   0        0        0    13559 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/config_builder.py
+-rw-r--r--   0        0        0      153 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/py.typed
+-rw-r--r--   0        0        0     3871 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/replacement_map.py
+-rw-r--r--   0        0        0     2642 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/utils.py
+-rw-r--r--   0        0        0    10526 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/yaml_constructors.py
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.1/setup.py
+-rw-r--r--   0        0        0     2321 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.1/PKG-INFO
```

### Comparing `yaml_config_builder-8.0.0/LICENSE` & `yaml_config_builder-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.0/README.md` & `yaml_config_builder-8.0.1/README.md`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.0/pyproject.toml` & `yaml_config_builder-8.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yaml-config-builder"
-version = "8.0.0"
+version = "8.0.1"
 license = "Open Logistics License Version 1.0"
 description = "Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder/-/blob/main/documentation/index.adoc"
 classifiers = [
```

### Comparing `yaml_config_builder-8.0.0/src/config_builder/base_config_class.py` & `yaml_config_builder-8.0.1/src/config_builder/base_config_class.py`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.0/src/config_builder/config_builder.py` & `yaml_config_builder-8.0.1/src/config_builder/config_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # Licensed under the Open Logistics License 1.0.
 # For details on the licensing terms, see the LICENSE file.
 
 import argparse
 import logging
 import os
 from collections import OrderedDict
-from typing import Callable, Dict, List, Optional, Type, cast
+from pathlib import Path
+from typing import Callable, Dict, Optional, Type, cast
 
 import yaml
 from related import from_yaml, to_model
 
 from config_builder import BaseConfigClass
 from config_builder.replacement_map import (
     clear_replacement_map,
@@ -92,24 +93,30 @@
             self.parser = self.setup_argparse(
                 configure_argparse=configure_argparse,
             )
             self.args = self.parser.parse_args()
 
             logger.info(f"Parsed arguments from command-line: {self.args}")
 
-            self.yaml_config_path = self.args.yaml_config_path
+            self.yaml_config_path = (
+                str(Path(self.args.yaml_config_path))
+                if self.args.yaml_config_path
+                else None
+            )
 
             # Check any placeholder of the replacement-map whether they have
             # an entry in the parsed arguments
             ConfigBuilder.__update_placeholder_from_argparse(args=self.args)
 
             # Parse a replacement-map if the filepath is given as commandline argument
             ConfigBuilder.__update_replacement_map(
                 string_replacement_map=self.__parse_replacement_map(
-                    replacement_config_path=self.args.replacement_config_path
+                    replacement_config_path=str(Path(self.args.replacement_config_path))
+                    if self.args.replacement_config_path
+                    else None
                 )
             )
 
         if self.yaml_config_path is None:
             raise ValueError(f"Can not build a configuration, yaml-config-path is None")
 
         # Update the placeholder value in order to be able to prepare the yaml-config-path,
```

### Comparing `yaml_config_builder-8.0.0/src/config_builder/replacement_map.py` & `yaml_config_builder-8.0.1/src/config_builder/replacement_map.py`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.0/src/config_builder/utils.py` & `yaml_config_builder-8.0.1/src/config_builder/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Definition of utility methods that are used across the config-builder
 """
 
 from __future__ import absolute_import, division, print_function
 
 import logging
 import os
+from pathlib import Path
 from typing import Any, Dict, List
 
 from config_builder.replacement_map import get_current_replacement_map
 
 logger = logging.getLogger(__name__)
 
 
@@ -29,26 +30,23 @@
         replacement_key: String, defining what is about to be replaced
         replacement_value: String, defining what the replacement looks like
 
     Returns: String, the updated file path
 
     """
 
-    path_list = os.path.normpath(file_path).split(os.sep)
+    path_list = file_path.split(os.sep)
 
     path_list = list(
         map(
             lambda x: x if x != replacement_key else replacement_value,
             path_list,
         )
     )
-
-    new_path = os.sep.join(path_list)
-
-    return new_path
+    return str(Path(os.sep.join(path_list)))
 
 
 def prepare_config_path(config_path: str) -> str:
     """
     Take a config-path and an os-string-replacement-map and try to build a
     valid config-path by using the values of the os-string-replacement-map
 
@@ -78,15 +76,15 @@
                 f"with '{value}' "
             )
 
             config_path = replace_directory_in_path(
                 file_path=config_path, replacement_key=key, replacement_value=value
             )
 
-    return config_path
+    return str(Path(config_path))
 
 
 def check_list_type(obj: List[Any], obj_type: Any) -> bool:
     """
     Check if the given list-object only contains objects of type 'obj_type'
 
     Args:
```

### Comparing `yaml_config_builder-8.0.0/src/config_builder/yaml_constructors.py` & `yaml_config_builder-8.0.1/src/config_builder/yaml_constructors.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 
 from __future__ import absolute_import, annotations, division, print_function
 
 import logging
 import os
 from collections import OrderedDict
+from pathlib import Path
 from typing import Any, List, Optional, Tuple, Union
 
 import yaml
 from yaml import FullLoader, Loader, Node, UnsafeLoader
 
 from config_builder.utils import prepare_config_path
 
@@ -99,15 +100,15 @@
 
     logger.debug(f"join path for a configuration item: {seq}")
 
     joined_path = ""
     for path in seq:
         joined_path = os.path.join(joined_path, str(path))
 
-    return joined_path
+    return str(Path(joined_path))
 
 
 def join_object(loader: Union[Loader, FullLoader, UnsafeLoader], node: Node) -> Any:
     """
     Define a custom tag handler that can be added as constructor to
     the python yaml package.
 
@@ -139,15 +140,15 @@
     class_type = str(seq[0])
 
     transformed_data: Union[List[Any], OrderedDict[Any, Any]]
 
     transformed_data_list: List[Union[List[Any], OrderedDict[Any, Any]]] = []
 
     for index in range(1, len(seq)):
-        config_path = str(seq[index])
+        config_path = str(Path(str(seq[index])))
         data, config_path = __get_config_data(config_path=config_path)
 
         if data is not None and class_type != "":
             logger.debug(
                 f"Parsed configuration via !join_object "
                 f"for class-type '{class_type}' from '{config_path}'"
             )
@@ -229,15 +230,15 @@
     transformed_data: Optional[OrderedDict[Any, Any]] = None
 
     for _, config_dir in enumerate(config_dirs):
         if transformed_data is not None:
             break
 
         data, config_path = __get_config_data(
-            config_path=os.path.join(str(config_dir), config_file_name)
+            config_path=str(Path(os.path.join(str(config_dir), config_file_name)))
         )
 
         if data is not None and class_type != "":
             logger.debug(
                 f"Parsed configuration via !join_object_from_config_dir "
                 f"for class-type '{class_type}' from '{config_path}'"
             )
```

### Comparing `yaml_config_builder-8.0.0/setup.py` & `yaml_config_builder-8.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'attrs>=20',
  'future>=0.18,<0.19',
  'python-dateutil>=2.8,<3.0',
  'related-mltoolbox>=1.0.1,<2']
 
 setup_kwargs = {
     'name': 'yaml-config-builder',
-    'version': '8.0.0',
+    'version': '8.0.1',
     'description': 'Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files',
     'long_description': '# Config Builder\n\nThe ConfigBuilder provides an SDK for building configuration classes on the basis of \ngiven content from YAML configuration files. Details about the ConfigBuilder can be\nfound in the [documentation](documentation/index.adoc).\n\n## Install\n\nThe installation and setup of the ConfigBuilder is described in [chapter 11](documentation/12_tutorial.adoc) \nof the documentation.\n\n# Technology stack\n\n- Python \n\n## License\nSee the license file in the top directory.\n\n## Contact information\n\n\nMaintainer: \n- Maximilian Otten <a href="mailto:maximilian.otten@iml.fraunhofer.de?">maximilian.otten@iml.fraunhofer.de</a>\n\nDevelopment Team: \n- Christian Hoppe <a href="mailto:christian.hoppe@iml.fraunhofer.de?">christian.hoppe@iml.fraunhofer.de</a>\n- Oliver Bredtmann <a href="mailto:oliver.bredtmann@dbschenker.com?">oliver.bredtmann@dbschenker.com</a>\n- Thilo Bauer <a href="mailto:thilo.bauer@dbschenker.com?">thilo.bauer@dbschenker.com</a>\n\n\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['config_builder'] package_data = \ {'': ['*']}
 install_requires = \ ['PyYAML>=5.4,<6.0', 'attrs>=20', 'future>=0.18,<0.19',
 'python-dateutil>=2.8,<3.0', 'related-mltoolbox>=1.0.1,<2'] setup_kwargs =
-{ 'name': 'yaml-config-builder', 'version': '8.0.0', 'description': 'Yaml-
+{ 'name': 'yaml-config-builder', 'version': '8.0.1', 'description': 'Yaml-
 Config-Builder: SDK for building configuration classes on the basis of given
 content from YAML configuration files', 'long_description': '# Config
 Builder\n\nThe ConfigBuilder provides an SDK for building configuration classes
 on the basis of \ngiven content from YAML configuration files. Details about
 the ConfigBuilder can be\nfound in the [documentation](documentation/
 index.adoc).\n\n## Install\n\nThe installation and setup of the ConfigBuilder
 is described in [chapter 11](documentation/12_tutorial.adoc) \nof the
```

### Comparing `yaml_config_builder-8.0.0/PKG-INFO` & `yaml_config_builder-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-config-builder
-Version: 8.0.0
+Version: 8.0.1
 Summary: Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
 License: Open Logistics License Version 1.0
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaml-config-builder Version: 8.0.0 Summary: Yaml-
+Metadata-Version: 2.1 Name: yaml-config-builder Version: 8.0.1 Summary: Yaml-
 Config-Builder: SDK for building configuration classes on the basis of given
 content from YAML configuration files Home-page: https://
 git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
 License: Open Logistics License Version 1.0 Author: Maximilian Otten Author-
 email: maximilian.otten@iml.fraunhofer.de Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: Other/Proprietary License
```

