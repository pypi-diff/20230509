# Comparing `tmp/ni_measurementlink_generator-1.0.1.tar.gz` & `tmp/ni_measurementlink_generator-1.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_generator-1.0.1.tar", max compression
+gzip compressed data, was "ni_measurementlink_generator-1.1.0.dev0.tar", max compression
```

## Comparing `ni_measurementlink_generator-1.0.1.tar` & `ni_measurementlink_generator-1.1.0.dev0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      593 2023-03-24 16:33:23.227670 ni_measurementlink_generator-1.0.1/README.md
--rw-r--r--   0        0        0      148 2023-03-24 16:33:23.227670 ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/__main__.py
--rw-r--r--   0        0        0     4614 2023-03-24 16:33:23.227670 ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/template.py
--rw-r--r--   0        0        0     1690 2023-03-24 16:33:23.227670 ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/templates/measurement.measproj.mako
--rw-r--r--   0        0        0     5143 2023-03-24 16:33:23.231670 ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/templates/measurement.measui.mako
--rw-r--r--   0        0        0     1491 2023-03-24 16:33:23.231670 ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/templates/measurement.py.mako
--rw-r--r--   0        0        0      341 2023-03-24 16:33:23.231670 ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
--rw-r--r--   0        0        0      241 2023-03-24 16:33:23.231670 ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/templates/start.bat.mako
--rw-r--r--   0        0        0     1123 2023-03-24 16:34:55.772174 ni_measurementlink_generator-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.0.1/setup.py
--rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      593 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/README.md
+-rw-r--r--   0        0        0      148 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/py.typed
+-rw-r--r--   0        0        0     5599 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/template.py
+-rw-r--r--   0        0        0     1690 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.measproj.mako
+-rw-r--r--   0        0        0     5143 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.measui.mako
+-rw-r--r--   0        0        0     1472 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.py.mako
+-rw-r--r--   0        0        0      341 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
+-rw-r--r--   0        0        0      241 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/start.bat.mako
+-rw-r--r--   0        0        0     1602 2023-05-08 22:27:14.811198 ni_measurementlink_generator-1.1.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev0/setup.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev0/PKG-INFO
```

### Comparing `ni_measurementlink_generator-1.0.1/README.md` & `ni_measurementlink_generator-1.1.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/template.py` & `ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/template.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,159 +1,184 @@
 """Utilizes command line args to create a measurement using template files."""
+import logging
 import pathlib
 import re
+from typing import Optional
 
 import click
 from mako import exceptions
 from mako.template import Template
 
+_logger = logging.getLogger(__name__)
 
-def _render_template(template_name: str, **template_args) -> str:
+
+def _render_template(template_name: str, **template_args) -> bytes:
     file_path = str(pathlib.Path(__file__).parent / "templates" / template_name)
 
-    with open(file_path, "r") as file:
-        file_contents = file.read()
-    template = Template(file_contents)
+    template = Template(filename=file_path, input_encoding="utf-8", output_encoding="utf-8")
     try:
         return template.render(**template_args)
-    except:  # noqa: E722
-        print(exceptions.text_error_template().render())
-
-    return ""
+    except Exception as e:
+        _logger.error(exceptions.text_error_template().render())
+        raise click.ClickException(
+            f'An error occurred while rendering template "{template_name}".'
+        ) from e
 
 
-def _create_file(template_name: str, file_name: str, directory_out, **template_args) -> str:
-    output_file = pathlib.Path(directory_out) / file_name
+def _create_file(template_name: str, file_name: str, directory_out: pathlib.Path, **template_args):
+    output_file = directory_out / file_name
 
     output = _render_template(template_name, **template_args)
 
-    with output_file.open("w") as fout:
+    with output_file.open("wb") as fout:
         fout.write(output)
 
-    return ""
-
 
-def _check_version(ctx, param, version):
+def _check_version(ctx: click.Context, param: click.Parameter, version: str) -> str:
     pattern = r"^[0-9]+\.[0-9]+\.[0-9]+\.[0-9]+$"
     if re.match(pattern, version):
         return version
-    raise ValueError("version not entered correctly")
+    raise click.BadParameter(f"Invalid version '{version}'.")
+
+
+def _check_ui_file(
+    ctx: click.Context, param: click.Parameter, ui_file: Optional[str]
+) -> Optional[str]:
+    if ui_file is not None:
+        _ = _get_ui_type(ui_file)
+    return ui_file
 
 
-def _get_ui_type(ui_file):
+def _get_ui_type(ui_file: str) -> str:
     ext = pathlib.Path(ui_file).suffix
     if ext == ".measui":
         return "MeasurementUI"
     elif ext == ".vi":
         return "LabVIEW"
     else:
-        raise ValueError(
-            "UI file extension does not match possible UI file types. Should be .measui or .vi."
+        raise click.BadParameter(
+            f"Unsupported extension '{ext}'. Supported extensions: '.measui', '.vi'"
         )
 
 
-def _resolve_ui_file(ui_file, display_name_for_filenames):
+def _resolve_ui_file(ui_file: Optional[str], display_name_for_filenames: str) -> str:
     if ui_file is None:
         return f"{display_name_for_filenames}.measui"
     else:
         return ui_file
 
 
-def _resolve_service_class(service_class, display_name):
+def _resolve_service_class(service_class: str, display_name: str) -> str:
     if service_class is None:
         return f"{display_name}_Python"
     else:
         return service_class
 
 
 @click.command()
 @click.argument("display_name")
 @click.option(
     "--measurement-version",
     callback=_check_version,
-    help="Version number in the form x.y.z.q",
+    help="Version number in the form 'x.y.z.q'. Default: '1.0.0.0'",
     default="1.0.0.0",
 )
 @click.option(
     "-u",
     "--ui-file",
-    help="Name of the UI File, Default is <display_name>.measui.",
+    callback=_check_ui_file,
+    help="Name of the UI File. Default: '<display_name>.measui'",
 )
 @click.option(
     "-s",
     "--service-class",
-    help="Service Class that the measurement belongs to. Default is <display_name>_Python.",
+    help="Service Class that the measurement belongs to. Default: '<display_name>_Python'",
 )
 @click.option(
     "-d",
     "--description-url",
     default="",
     help="Description URL that links to a web page containing information about the measurement.",
 )
 @click.option(
     "-o",
     "--directory-out",
-    help="Output directory for measurement files. Default is the current directory/<display_name>",
+    help="Output directory for measurement files. Default: '<current_directory>/<display_name>'",
+)
+@click.option(
+    "-v",
+    "--verbose",
+    count=True,
+    help="Enable verbose logging. Repeat to increase verbosity.",
 )
 def create_measurement(
-    display_name,
-    measurement_version,
-    ui_file,
-    service_class,
-    description_url,
-    directory_out,
-):
+    display_name: str,
+    measurement_version: str,
+    ui_file: Optional[str],
+    service_class: str,
+    description_url: str,
+    directory_out: Optional[str],
+    verbose: bool,
+) -> None:
     """Generate a Python measurement service from a template.
 
     You can use this to get started writing your own MeasurementLink services.
 
     DISPLAY_NAME: The measurement display name for client to display to user.
     The created .serviceconfig file will take this as its file name.
     """
+    if verbose > 1:
+        level = logging.DEBUG
+    elif verbose == 1:
+        level = logging.INFO
+    else:
+        level = logging.WARNING
+    logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=level)
+
     service_class = _resolve_service_class(service_class, display_name)
     display_name_for_filenames = re.sub(r"\s+", "", display_name)
     ui_file = _resolve_ui_file(ui_file, display_name_for_filenames)
     ui_file_type = _get_ui_type(ui_file)
     serviceconfig_file = f"{display_name_for_filenames}.serviceconfig"
     if directory_out is None:
-        directory_out = pathlib.Path.cwd() / display_name_for_filenames
+        directory_out_path = pathlib.Path.cwd() / display_name_for_filenames
     else:
-        directory_out = pathlib.Path(directory_out)
+        directory_out_path = pathlib.Path(directory_out)
 
-    directory_out.mkdir(exist_ok=True, parents=True)
+    directory_out_path.mkdir(exist_ok=True, parents=True)
 
     _create_file(
         "measurement.py.mako",
         "measurement.py",
-        directory_out,
+        directory_out_path,
         display_name=display_name,
         version=measurement_version,
         ui_file=ui_file,
         ui_file_type=ui_file_type,
         service_class=service_class,
         description_url=description_url,
         serviceconfig_file=serviceconfig_file,
     )
     _create_file(
         "measurement.serviceconfig.mako",
         serviceconfig_file,
-        directory_out,
+        directory_out_path,
         display_name=display_name,
         service_class=service_class,
         description_url=description_url,
         ui_file_type=ui_file_type,
     )
     if ui_file_type == "MeasurementUI":
         _create_file(
             "measurement.measui.mako",
             ui_file,
-            directory_out,
+            directory_out_path,
             display_name=display_name,
             service_class=service_class,
         )
         _create_file(
             "measurement.measproj.mako",
             f"{display_name_for_filenames}.measproj",
-            directory_out,
+            directory_out_path,
             ui_file=ui_file,
         )
-    _create_file("start.bat.mako", "start.bat", directory_out)
+    _create_file("start.bat.mako", "start.bat", directory_out_path)
```

### Comparing `ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/templates/measurement.measproj.mako` & `ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.measproj.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/templates/measurement.measui.mako` & `ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.measui.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.0.1/ni_measurementlink_generator/templates/measurement.py.mako` & `ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.py.mako`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <%page args="display_name, version, ui_file, ui_file_type, service_class, description_url, serviceconfig_file"/>\
 \
 """A default measurement with an array in and out."""
 import logging
 import pathlib
-import sys
 
 import click
 import ni_measurementlink_service as nims
 
 service_directory = pathlib.Path(__file__).resolve().parent
 measurement_service = nims.MeasurementService(
     service_config_path=service_directory / "${serviceconfig_file}",
@@ -28,15 +27,15 @@
 @click.command
 @click.option(
     "-v",
     "--verbose",
     count=True,
     help="Enable verbose logging. Repeat to increase verbosity.",
 )
-def main(verbose: int):
+def main(verbose: int) -> None:
     """Host the ${display_name} service."""
     if verbose > 1:
         level = logging.DEBUG
     elif verbose == 1:
         level = logging.INFO
     else:
         level = logging.WARNING
@@ -44,8 +43,7 @@
 
     with measurement_service.host_service():
         input("Press enter to close the measurement service.\n")
 
 
 if __name__ == "__main__":
     main()
-    sys.exit(0)
```

### Comparing `ni_measurementlink_generator-1.0.1/pyproject.toml` & `ni_measurementlink_generator-1.1.0.dev0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,47 @@
-[tool.poetry]
-name = "ni_measurementlink_generator"
-version = "1.0.1"
-description = "MeasurementLink Code Generator for Python"
-authors = ["NI <opensource@ni.com>"]
-readme = "README.md"
-repository = "https://github.com/ni/measurementlink-python/"
-license = "MIT"
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Manufacturing",
-    "Intended Audience :: Science/Research",
-    "Operating System :: Microsoft :: Windows",
-    # Poetry automatically adds classifiers for the license and the supported Python versions.
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Topic :: Scientific/Engineering",
-    "Topic :: System :: Hardware",
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-Mako = "^1.2.1"
-click = "^8.1.3"
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-ni-python-styleguide = ">=0.1.9"
-mypy = "^0.961"
-
-[tool.poetry.scripts]
-ni-measurementlink-generator = "ni_measurementlink_generator.template:create_measurement"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+Metadata-Version: 2.1
+Name: ni-measurementlink-generator
+Version: 1.1.0.dev0
+Summary: MeasurementLink Code Generator for Python
+Home-page: https://github.com/ni/measurementlink-python/
+License: MIT
+Author: NI
+Author-email: opensource@ni.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Requires-Dist: Mako (>=1.2.1,<2.0.0)
+Requires-Dist: click (>=8.1.3)
+Project-URL: Repository, https://github.com/ni/measurementlink-python/
+Description-Content-Type: text/markdown
+
+# MeasurementLink™ Code Generator for Python
+
+---
+
+## Introduction
+
+MeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a tool for generating measurement plugins.
+
+For installation and usage, see [MeasurementLink Support for Python (`ni-measurementlink-service`)](https://pypi.org/project/ni-measurementlink-service/).
+
+---
+
+## Dependencies
+
+- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)
+- [mako >= 1.2.1, < 2.x](https://pypi.org/project/Mako/1.2.1/)
+- [click >= 8.1.3, < 9.x](https://pypi.org/project/click/8.1.3/)
+
+---
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ni_measurementlink_generator-1.0.1/setup.py` & `ni_measurementlink_generator-1.1.0.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['ni_measurementlink_generator']
 
 package_data = \
 {'': ['*'], 'ni_measurementlink_generator': ['templates/*']}
 
 install_requires = \
-['Mako>=1.2.1,<2.0.0', 'click>=8.1.3,<9.0.0']
+['Mako>=1.2.1,<2.0.0', 'click>=8.1.3']
 
 entry_points = \
 {'console_scripts': ['ni-measurementlink-generator = '
                      'ni_measurementlink_generator.template:create_measurement']}
 
 setup_kwargs = {
     'name': 'ni-measurementlink-generator',
-    'version': '1.0.1',
+    'version': '1.1.0.dev0',
     'description': 'MeasurementLink Code Generator for Python',
     'long_description': '# MeasurementLink™ Code Generator for Python\n\n---\n\n## Introduction\n\nMeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a tool for generating measurement plugins.\n\nFor installation and usage, see [MeasurementLink Support for Python (`ni-measurementlink-service`)](https://pypi.org/project/ni-measurementlink-service/).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [mako >= 1.2.1, < 2.x](https://pypi.org/project/Mako/1.2.1/)\n- [click >= 8.1.3, < 9.x](https://pypi.org/project/click/8.1.3/)\n\n---',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/measurementlink-python/',
```

