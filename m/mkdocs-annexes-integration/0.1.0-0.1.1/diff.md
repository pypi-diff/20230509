# Comparing `tmp/mkdocs-annexes-integration-0.1.0.tar.gz` & `tmp/mkdocs-annexes-integration-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-annexes-integration-0.1.0.tar", last modified: Tue May  9 06:25:19 2023, max compression
+gzip compressed data, was "mkdocs-annexes-integration-0.1.1.tar", last modified: Tue May  9 06:34:13 2023, max compression
```

## Comparing `mkdocs-annexes-integration-0.1.0.tar` & `mkdocs-annexes-integration-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:25:19.308522 mkdocs-annexes-integration-0.1.0/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      678 2023-05-09 06:25:19.305522 mkdocs-annexes-integration-0.1.0/PKG-INFO
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:25:19.202520 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6448 2023-05-08 13:39:14.000000 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:25:19.289523 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      678 2023-05-09 06:25:18.000000 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      386 2023-05-09 06:25:18.000000 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2023-05-09 06:25:18.000000 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       93 2023-05-09 06:25:18.000000 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       32 2023-05-09 06:25:18.000000 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       27 2023-05-09 06:25:18.000000 mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2023-05-09 06:25:19.309523 mkdocs-annexes-integration-0.1.0/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1064 2023-05-02 08:45:07.000000 mkdocs-annexes-integration-0.1.0/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:34:13.591688 mkdocs-annexes-integration-0.1.1/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3871 2023-05-09 06:34:13.589691 mkdocs-annexes-integration-0.1.1/PKG-INFO
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:34:13.490625 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6454 2023-05-09 06:32:03.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:34:13.574636 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3871 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      386 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       93 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       32 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       27 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2023-05-09 06:34:13.592692 mkdocs-annexes-integration-0.1.1/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1169 2023-05-09 06:33:50.000000 mkdocs-annexes-integration-0.1.1/setup.py
```

### Comparing `mkdocs-annexes-integration-0.1.0/mkdocs_annexes_integration/plugin.py` & `mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 self._logger.info(f'Integrating annex "{title}"')
                 src, dest = self.get_src_and_dest(path)
                 extension = os.path.splitext(src)[1][1:]
                 original = os.path.join(config.docs_dir, src)
                 root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
                 embedded = f'{root}.md'
                 if os.path.exists(original):
-                    if extension in ['cs', 'css', 'dart', 'html', 'js', 'json', 'php']:
+                    if extension in ['cs', 'css', 'dart', 'html', 'js', 'json', 'php', 'py']:
                         self._logger.info(f'    With content as code block')
                         with open(original, 'r') as file:
                             content = file.read()
                         # Create a markdown file that take care of showing source code annex
                         if not os.path.exists(os.path.dirname(embedded)):
                             os.makedirs(os.path.dirname(embedded))
                         with open(embedded, 'w') as f:
```

### Comparing `mkdocs-annexes-integration-0.1.0/setup.py` & `mkdocs-annexes-integration-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from setuptools import setup, find_packages
+import io
 
+from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-annexes-integration',
-    version='0.1.0',
+    version='0.1.1',
     description='A MkDocs plugin transforming annexes files into images to be integrated in markdown pages',
-    long_description='',
+    long_description=io.open('readme.md', encoding='utf8').read(),
+    long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
     license='MIT',
     python_requires='>=3.8',
     install_requires=[
```

