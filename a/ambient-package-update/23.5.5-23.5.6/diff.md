# Comparing `tmp/ambient-package-update-23.5.5.tar.gz` & `tmp/ambient-package-update-23.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-package-update-23.5.5.tar", last modified: Thu May  4 14:01:38 2023, max compression
+gzip compressed data, was "ambient-package-update-23.5.6.tar", last modified: Tue May  9 08:15:40 2023, max compression
```

## Comparing `ambient-package-update-23.5.5.tar` & `ambient-package-update-23.5.6.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/.gitignore
--rw-r--r--   0        0        0      904 2023-05-04 13:34:24.555311 ambient-package-update-23.5.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      305 2023-05-04 14:01:17.467891 ambient-package-update-23.5.5/CHANGES.md
--rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/LICENSE.md
--rw-r--r--   0        0        0     1861 2023-05-04 13:44:21.438513 ambient-package-update-23.5.5/README.md
--rw-r--r--   0        0        0       93 2023-05-04 14:00:38.526432 ambient-package-update-23.5.5/ambient_package_update/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      396 2023-05-04 14:00:38.526432 ambient-package-update-23.5.5/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0     3526 2023-05-03 13:01:45.765213 ambient-package-update-23.5.5/main.py
--rw-r--r--   0        0        0     2550 2023-05-04 13:59:19.861070 ambient-package-update-23.5.5/pyproject.toml
--rw-r--r--   0        0        0     1820 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/requirements.txt
--rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/scripts/setup_venv.ps1
--rw-r--r--   0        0        0       82 2023-05-04 09:31:48.690822 ambient-package-update-23.5.5/templates/.coveragerc.tpl
--rw-r--r--   0        0        0      288 2023-05-04 09:25:12.333150 ambient-package-update-23.5.5/templates/.editorconfig.tpl
--rw-r--r--   0        0        0     1784 2023-05-04 13:49:38.761775 ambient-package-update-23.5.5/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      904 2023-05-04 13:34:24.540644 ambient-package-update-23.5.5/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0     1121 2023-05-04 09:29:00.483983 ambient-package-update-23.5.5/templates/LICENSE.md.tpl
--rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     4625 2023-05-04 09:47:17.310181 ambient-package-update-23.5.5/templates/Readme.md.tpl
--rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     3742 2023-05-04 13:33:46.734472 ambient-package-update-23.5.5/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       56 2023-05-04 09:29:24.289641 ambient-package-update-23.5.5/templates/pytest.init.tpl
--rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 ambient-package-update-23.5.5/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-04 13:34:24.555311 ambient-package-update-23.5.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      417 2023-05-09 08:11:31.104801 ambient-package-update-23.5.6/CHANGES.md
+-rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/LICENSE.md
+-rw-r--r--   0        0        0     2432 2023-05-09 08:09:25.681131 ambient-package-update-23.5.6/README.md
+-rw-r--r--   0        0        0       93 2023-05-09 08:10:19.929713 ambient-package-update-23.5.6/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      396 2023-05-04 14:00:38.526432 ambient-package-update-23.5.6/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0     3541 2023-05-09 08:09:25.681131 ambient-package-update-23.5.6/main.py
+-rw-r--r--   0        0        0     2550 2023-05-04 13:59:19.861070 ambient-package-update-23.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1744 2023-05-09 08:09:25.681131 ambient-package-update-23.5.6/requirements.txt
+-rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/scripts/setup_venv.ps1
+-rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient-package-update-23.5.6/scripts/setup_venv_unix.sh
+-rw-r--r--   0        0        0       82 2023-05-04 09:31:48.690822 ambient-package-update-23.5.6/templates/.coveragerc.tpl
+-rw-r--r--   0        0        0      288 2023-05-04 09:25:12.333150 ambient-package-update-23.5.6/templates/.editorconfig.tpl
+-rw-r--r--   0        0        0     1784 2023-05-04 13:49:38.761775 ambient-package-update-23.5.6/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      904 2023-05-04 13:34:24.540644 ambient-package-update-23.5.6/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/templates/.readthedocs.yml.tpl
+-rw-r--r--   0        0        0     1121 2023-05-04 09:29:00.483983 ambient-package-update-23.5.6/templates/LICENSE.md.tpl
+-rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     5131 2023-05-09 08:12:34.842033 ambient-package-update-23.5.6/templates/Readme.md.tpl
+-rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     3742 2023-05-04 13:33:46.734472 ambient-package-update-23.5.6/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0       56 2023-05-04 09:29:24.289641 ambient-package-update-23.5.6/templates/pytest.init.tpl
+-rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.6/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 ambient-package-update-23.5.6/PKG-INFO
```

### Comparing `ambient-package-update-23.5.5/.gitignore` & `ambient-package-update-23.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/.pre-commit-config.yaml` & `ambient-package-update-23.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/LICENSE.md` & `ambient-package-update-23.5.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/README.md` & `ambient-package-update-23.5.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,30 +2,43 @@
 [![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 
 # Ambient Package Update
 
 This repository will help keep all Python packages maintained by 
 [Ambient Digital](https://ambient.digital) tidy and up-to-date.
 
-## Installation
+This package will render all required configuration and installation files for your target package.
 
-1. Ensure you have installed Python >=3.10 and the binary is in your system path
-2. Navigate into the project directory
-3. Execute scripts/setup_venv.ps1 (on Windows) or rename the file to "setup_venv.sh" and execute it for macOS and UNIX
+Typical use-cases:
+* A new Python or Django version was release
+* A Python or Django version was deprecated
+* You want to update the Sphinx documentation builder
+* You want to update the linter versions
+* You want to add the third-party dependencies
 
 ## Versioning
 
 This project follows the CalVer versioning pattern: `YY.MM.[RELEASE]`
 
+# Installation
+
+1. Ensure you have installed Python >=3.11 and the binary is in your system path
+2. Clone this package from GitHub
+3. Navigate into the project directory
+4. Execute scripts/setup_venv.ps1 on Windows or scripts/setup_venv_unix.sh on Unix/macOS
+
 ## Usage
 
-* python .\main.py render-templates [PACKAGE_NAME]
+* Navigate to the main directory of this package
+* Activate your virtualenv
+* Run `python .\main.py render-templates [PACKAGE_NAME]`
+* Open your target package in the IDE, validate the changes and increment the version accordingly
+* Release a new version of your target package
 
 todo:
-- write usage paragraph
 - docs how to create a new package
 - create template dirs if not existing (without .github/workflows it's failing)
 - package-readme hat dopplungen zu docs und enthält zeug, das nicht da drinstehen muss
 - ambient-toolbox branch löschen und nur rest von core da ablegen
 
 ## Contribution
```

### Comparing `ambient-package-update-23.5.5/ambient_package_update/metadata/package.py` & `ambient-package-update-23.5.6/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/main.py` & `ambient-package-update-23.5.6/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import datetime
 import os
 import subprocess
 import sys
+from datetime import datetime, timezone
 from importlib import import_module
 from pathlib import Path
 
 import typer
 from jinja2 import Template
 
 from ambient_package_update.metadata.package import PackageMetadata
@@ -73,15 +73,15 @@
         print(path, subdirs, files)
         for file in files:
             template_list.append(Path(f"{path}/{file}"))
 
     print(f'Start rending distribution templates for package "{package_name}".')
     for template in template_list:
         j2_template = Template(template.read_text(), keep_trailing_newline=True)
-        j2_template.globals['current_year'] = datetime.datetime.now(tz=datetime.UTC).date().year
+        j2_template.globals['current_year'] = datetime.now(tz=timezone.utc).date().year
 
         rendered_string = j2_template.render(get_metadata(package_name).__dict__)
 
         relative_template_path = str(template).replace('templates', '')
 
         print(relative_template_path)
         rendered_file_path = f'../{package_name}/{relative_template_path[:-4]}'
```

### Comparing `ambient-package-update-23.5.5/pyproject.toml` & `ambient-package-update-23.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/requirements.txt` & `ambient-package-update-23.5.6/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   typer
-colorama==0.4.6
-    # via click
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via flit
 filelock==3.12.0
     # via virtualenv
 flit==3.8.0
@@ -54,16 +52,14 @@
     # via black
 platformdirs==3.5.0
     # via
     #   black
     #   virtualenv
 pre-commit==3.3.1
     # via ambient-package-update (pyproject.toml)
-pywin32-ctypes==0.2.0
-    # via keyring
 pyyaml==6.0
     # via pre-commit
 requests==2.29.0
     # via flit
 tomli-w==1.0.0
     # via flit
 typer==0.9.0
```

### Comparing `ambient-package-update-23.5.5/templates/.github/workflows/ci.yml.tpl` & `ambient-package-update-23.5.6/templates/.github/workflows/ci.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/templates/.pre-commit-config.yaml.tpl` & `ambient-package-update-23.5.6/templates/.pre-commit-config.yaml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/templates/.readthedocs.yml.tpl` & `ambient-package-update-23.5.6/templates/.readthedocs.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/templates/LICENSE.md.tpl` & `ambient-package-update-23.5.6/templates/LICENSE.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/templates/Readme.md.tpl` & `ambient-package-update-23.5.6/templates/Readme.md.tpl`

 * *Files 11% similar despite different names*

```diff
@@ -124,7 +124,16 @@
 
   To publish to TestPyPI use the following ensure that you have set up your .pypirc as
   shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
 
   ```
   flit publish --repository testpypi
   ```
+
+### Maintenance
+
+Please note that this package supports the [ambient-package-update](https://pypi.org/project/ambient-package-update/).
+So you don't have to worry about the maintenance of this package. All important configuration and setup files are
+being rendered by this updater. It works similar to well-known updaters like `pyupgrade` or `django-upgrade`.
+
+To run an update, refer to the [documentation page](https://pypi.org/project/ambient-package-update/)
+of the "ambient-package-update".
```

### Comparing `ambient-package-update-23.5.5/templates/docs/Makefile.tpl` & `ambient-package-update-23.5.6/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/templates/docs/conf.py.tpl` & `ambient-package-update-23.5.6/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/templates/docs/make.bat.tpl` & `ambient-package-update-23.5.6/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/templates/pyproject.toml.tpl` & `ambient-package-update-23.5.6/templates/pyproject.toml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.5/PKG-INFO` & `ambient-package-update-23.5.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 23.5.5
+Version: 23.5.6
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -30,30 +30,43 @@
 [![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 
 # Ambient Package Update
 
 This repository will help keep all Python packages maintained by 
 [Ambient Digital](https://ambient.digital) tidy and up-to-date.
 
-## Installation
+This package will render all required configuration and installation files for your target package.
 
-1. Ensure you have installed Python >=3.10 and the binary is in your system path
-2. Navigate into the project directory
-3. Execute scripts/setup_venv.ps1 (on Windows) or rename the file to "setup_venv.sh" and execute it for macOS and UNIX
+Typical use-cases:
+* A new Python or Django version was release
+* A Python or Django version was deprecated
+* You want to update the Sphinx documentation builder
+* You want to update the linter versions
+* You want to add the third-party dependencies
 
 ## Versioning
 
 This project follows the CalVer versioning pattern: `YY.MM.[RELEASE]`
 
+# Installation
+
+1. Ensure you have installed Python >=3.11 and the binary is in your system path
+2. Clone this package from GitHub
+3. Navigate into the project directory
+4. Execute scripts/setup_venv.ps1 on Windows or scripts/setup_venv_unix.sh on Unix/macOS
+
 ## Usage
 
-* python .\main.py render-templates [PACKAGE_NAME]
+* Navigate to the main directory of this package
+* Activate your virtualenv
+* Run `python .\main.py render-templates [PACKAGE_NAME]`
+* Open your target package in the IDE, validate the changes and increment the version accordingly
+* Release a new version of your target package
 
 todo:
-- write usage paragraph
 - docs how to create a new package
 - create template dirs if not existing (without .github/workflows it's failing)
 - package-readme hat dopplungen zu docs und enthält zeug, das nicht da drinstehen muss
 - ambient-toolbox branch löschen und nur rest von core da ablegen
 
 ## Contribution
```

