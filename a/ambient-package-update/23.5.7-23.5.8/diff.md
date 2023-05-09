# Comparing `tmp/ambient-package-update-23.5.7.tar.gz` & `tmp/ambient-package-update-23.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-package-update-23.5.7.tar", last modified: Tue May  9 08:20:41 2023, max compression
+gzip compressed data, was "ambient-package-update-23.5.8.tar", last modified: Tue May  9 16:05:53 2023, max compression
```

## Comparing `ambient-package-update-23.5.7.tar` & `ambient-package-update-23.5.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/.gitignore
--rw-r--r--   0        0        0      904 2023-05-04 13:34:24.555311 ambient-package-update-23.5.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      483 2023-05-09 08:20:12.406369 ambient-package-update-23.5.7/CHANGES.md
--rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/LICENSE.md
--rw-r--r--   0        0        0     2537 2023-05-09 08:20:12.421995 ambient-package-update-23.5.7/README.md
--rw-r--r--   0        0        0       93 2023-05-09 08:20:12.406369 ambient-package-update-23.5.7/ambient_package_update/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      396 2023-05-09 08:20:12.406369 ambient-package-update-23.5.7/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0     3541 2023-05-09 08:09:25.681131 ambient-package-update-23.5.7/main.py
--rw-r--r--   0        0        0     2550 2023-05-04 13:59:19.861070 ambient-package-update-23.5.7/pyproject.toml
--rw-r--r--   0        0        0     1744 2023-05-09 08:09:25.681131 ambient-package-update-23.5.7/requirements.txt
--rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/scripts/setup_venv.ps1
--rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient-package-update-23.5.7/scripts/setup_venv_unix.sh
--rw-r--r--   0        0        0       82 2023-05-04 09:31:48.690822 ambient-package-update-23.5.7/templates/.coveragerc.tpl
--rw-r--r--   0        0        0      288 2023-05-04 09:25:12.333150 ambient-package-update-23.5.7/templates/.editorconfig.tpl
--rw-r--r--   0        0        0     1784 2023-05-04 13:49:38.761775 ambient-package-update-23.5.7/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      904 2023-05-04 13:34:24.540644 ambient-package-update-23.5.7/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0     1121 2023-05-04 09:29:00.483983 ambient-package-update-23.5.7/templates/LICENSE.md.tpl
--rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     5131 2023-05-09 08:12:34.842033 ambient-package-update-23.5.7/templates/Readme.md.tpl
--rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     3742 2023-05-04 13:33:46.734472 ambient-package-update-23.5.7/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       56 2023-05-04 09:29:24.289641 ambient-package-update-23.5.7/templates/pytest.init.tpl
--rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.7/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 ambient-package-update-23.5.7/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-04 13:34:24.555311 ambient-package-update-23.5.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      695 2023-05-09 16:05:32.005724 ambient-package-update-23.5.8/CHANGES.md
+-rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/LICENSE.md
+-rw-r--r--   0        0        0     3992 2023-05-09 16:03:59.316283 ambient-package-update-23.5.8/README.md
+-rw-r--r--   0        0        0       93 2023-05-09 16:05:02.684916 ambient-package-update-23.5.8/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      396 2023-05-09 08:20:12.406369 ambient-package-update-23.5.8/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0     3823 2023-05-09 16:01:10.150288 ambient-package-update-23.5.8/main.py
+-rw-r--r--   0        0        0     2550 2023-05-04 13:59:19.861070 ambient-package-update-23.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1744 2023-05-09 08:09:25.681131 ambient-package-update-23.5.8/requirements.txt
+-rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/scripts/setup_venv.ps1
+-rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient-package-update-23.5.8/scripts/setup_venv_unix.sh
+-rw-r--r--   0        0        0       82 2023-05-04 09:31:48.690822 ambient-package-update-23.5.8/templates/.coveragerc.tpl
+-rw-r--r--   0        0        0      288 2023-05-04 09:25:12.333150 ambient-package-update-23.5.8/templates/.editorconfig.tpl
+-rw-r--r--   0        0        0     1784 2023-05-04 13:49:38.761775 ambient-package-update-23.5.8/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      904 2023-05-04 13:34:24.540644 ambient-package-update-23.5.8/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/templates/.readthedocs.yml.tpl
+-rw-r--r--   0        0        0     1121 2023-05-04 09:29:00.483983 ambient-package-update-23.5.8/templates/LICENSE.md.tpl
+-rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     5131 2023-05-09 08:12:34.842033 ambient-package-update-23.5.8/templates/Readme.md.tpl
+-rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     3742 2023-05-04 13:33:46.734472 ambient-package-update-23.5.8/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0       56 2023-05-04 09:29:24.289641 ambient-package-update-23.5.8/templates/pytest.init.tpl
+-rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.8/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 ambient-package-update-23.5.8/PKG-INFO
```

### Comparing `ambient-package-update-23.5.7/.gitignore` & `ambient-package-update-23.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/.pre-commit-config.yaml` & `ambient-package-update-23.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/LICENSE.md` & `ambient-package-update-23.5.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/ambient_package_update/metadata/package.py` & `ambient-package-update-23.5.8/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/main.py` & `ambient-package-update-23.5.8/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,15 +54,18 @@
 
 """
 
 
 @app.command()
 def get_metadata(package_name: str) -> PackageMetadata:
     sys.path.append(f"../{package_name}/.ambient-package-update")
-    m = import_module('metadata')
+    try:
+        m = import_module('metadata')
+    except ModuleNotFoundError as e:
+        raise RuntimeError('Please create a directory ".ambient-package-update" and add a "metadata.py".') from e
     sys.path.pop()
 
     return m.METADATA
 
 
 @app.command()
 def render_templates(package_name: str):
@@ -80,15 +83,19 @@
         j2_template.globals['current_year'] = datetime.now(tz=timezone.utc).date().year
 
         rendered_string = j2_template.render(get_metadata(package_name).__dict__)
 
         relative_template_path = str(template).replace('templates', '')
 
         print(relative_template_path)
+
         rendered_file_path = f'../{package_name}/{relative_template_path[:-4]}'
+        # Create missing directories
+        os.makedirs(os.path.dirname(rendered_file_path), exist_ok=True)
+
         with open(rendered_file_path, 'w') as f:
             f.write(rendered_string)
 
         abs_path = Path(rendered_file_path).resolve()
         print(f'> Successfully rendered template "{abs_path}".')
     print('Rendering finished.')
```

### Comparing `ambient-package-update-23.5.7/pyproject.toml` & `ambient-package-update-23.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/requirements.txt` & `ambient-package-update-23.5.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/scripts/setup_venv_unix.sh` & `ambient-package-update-23.5.8/scripts/setup_venv_unix.sh`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/.github/workflows/ci.yml.tpl` & `ambient-package-update-23.5.8/templates/.github/workflows/ci.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/.pre-commit-config.yaml.tpl` & `ambient-package-update-23.5.8/templates/.pre-commit-config.yaml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/.readthedocs.yml.tpl` & `ambient-package-update-23.5.8/templates/.readthedocs.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/LICENSE.md.tpl` & `ambient-package-update-23.5.8/templates/LICENSE.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/Readme.md.tpl` & `ambient-package-update-23.5.8/templates/Readme.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/docs/Makefile.tpl` & `ambient-package-update-23.5.8/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/docs/conf.py.tpl` & `ambient-package-update-23.5.8/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/docs/make.bat.tpl` & `ambient-package-update-23.5.8/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.7/templates/pyproject.toml.tpl` & `ambient-package-update-23.5.8/templates/pyproject.toml.tpl`

 * *Files identical despite different names*

