# Comparing `tmp/mkdocs_exporter-1.0.1.tar.gz` & `tmp/mkdocs_exporter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-1.0.1.tar", max compression
+gzip compressed data, was "mkdocs_exporter-1.0.2.tar", max compression
```

## Comparing `mkdocs_exporter-1.0.1.tar` & `mkdocs_exporter-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.0.1/LICENSE
--rw-r--r--   0        0        0     2661 2023-05-08 17:27:32.453564 mkdocs_exporter-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.0.1/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-08 19:20:51.901769 mkdocs_exporter-1.0.1/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-1.0.1/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.0.1/mkdocs_exporter/page.py
--rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-1.0.1/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      894 2023-05-08 15:35:52.373552 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0      629 2023-05-08 15:31:52.723552 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      633 2023-05-08 14:24:00.883541 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0      969 2023-05-08 14:02:42.383538 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4376 2023-05-08 19:29:05.711770 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2257 2023-05-08 19:33:11.371770 mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     3712 2023-05-08 19:28:57.781770 mkdocs_exporter-1.0.1/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.0.1/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.0.1/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.0.1/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.0.1/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0     1298 2023-05-08 19:34:30.941769 mkdocs_exporter-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 mkdocs_exporter-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3008 2023-05-08 20:05:08.751775 mkdocs_exporter-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.0.2/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-08 19:20:51.901769 mkdocs_exporter-1.0.2/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-1.0.2/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.0.2/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-1.0.2/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      894 2023-05-08 15:35:52.373552 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0      629 2023-05-08 15:31:52.723552 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      633 2023-05-08 14:24:00.883541 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0      969 2023-05-08 14:02:42.383538 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4467 2023-05-09 08:52:26.827115 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2257 2023-05-08 19:33:11.371770 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     3712 2023-05-08 19:28:57.781770 mkdocs_exporter-1.0.2/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.0.2/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.0.2/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.0.2/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.0.2/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0     1298 2023-05-09 08:52:37.767115 mkdocs_exporter-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 mkdocs_exporter-1.0.2/PKG-INFO
```

### Comparing `mkdocs_exporter-1.0.1/LICENSE` & `mkdocs_exporter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/README.md` & `mkdocs_exporter-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 pip install mkdocs-exporter
 ```
 
 ## Usage
 
 Three plugins are currently available:
 
-- `mkdocs/exporter` (*required*): base plugin that must precedes the others
-- `mkdocs/exporter/pdf` (*optional*): the plugin that exports your pages as individual PDF documents
+- `mkdocs/exporter` (*required*): base plugin which must precede the others
+- `mkdocs/exporter/pdf` (*optional*): plugin that exports your pages as individual PDF documents
 - `mkdocs/exporter/extras` (*optional*): provides extra functionalities (buttons, HTML utilities...)
 
 ### Example
 
 The following configuration excerpt from `mkdocs.yml` should cover the basic functionalities of this plugin:
 
 ```yaml
@@ -53,16 +53,21 @@
       buttons:
         - title: Download as PDF
           icon: !!python/name:mkdocs_exporter.plugins.pdf.button.icon
           href: !!python/name:mkdocs_exporter.plugins.pdf.button.href
           download: !!python/name:mkdocs_exporter.plugins.pdf.button.download
 ```
 
+Check out a [sample PDF generated by this plugin](examples/example.pdf) from the default page of the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) theme.  
+It has been built with some custom CSS and features cover pages.
+
 ## Roadmap
 
 - Documentation (based on `MkDocs` and featuring this plugin)
 - Ensure full compatibility with other themes than `mkdocs-material`
 - Combine all pages as one PDF
 
+Feel free to request additional features by submitting an issue or by contributing through a pull request.
+
 ## License
 
 This project is licensed under the `MIT License (MIT)`, which you can read [here](LICENSE.md).
```

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/browser.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/plugin.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,25 +41,30 @@
     self.config.scripts = [resolve(path) for path in self.config.scripts]
     self.config.stylesheets = [resolve(path) for path in self.config.stylesheets]
 
 
   def on_serve(self, server: LiveReloadServer, **kwargs) -> LiveReloadServer:
     """Invoked when the website is being served."""
 
+    if not self.config.enabled:
+      return
     for path in [*self.config.stylesheets, *self.config.scripts]:
       server.watch(path)
     for cover in self.config.covers:
       server.watch(self.config.covers[cover])
 
     return server
 
 
   def on_page_markdown(self, markdown: str, **kwargs) -> str:
     """Invoked when the page's markdown has been loaded."""
 
+    if not self.config.enabled:
+      return
+
     content = markdown
 
     if self.config.covers.front:
       with open(self.config.covers.front, 'r') as file:
         content = self.renderer.cover(file.read()) + content
     if self.config.covers.back:
       with open(self.config.covers.back, 'r') as file:
```

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-1.0.2/mkdocs_exporter/preprocessor.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-1.0.2/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.1/pyproject.toml` & `mkdocs_exporter-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "1.0.1"
+version = "1.0.2"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-1.0.1/PKG-INFO` & `mkdocs_exporter-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -60,16 +60,16 @@
 pip install mkdocs-exporter
 ```
 
 ## Usage
 
 Three plugins are currently available:
 
-- `mkdocs/exporter` (*required*): base plugin that must precedes the others
-- `mkdocs/exporter/pdf` (*optional*): the plugin that exports your pages as individual PDF documents
+- `mkdocs/exporter` (*required*): base plugin which must precede the others
+- `mkdocs/exporter/pdf` (*optional*): plugin that exports your pages as individual PDF documents
 - `mkdocs/exporter/extras` (*optional*): provides extra functionalities (buttons, HTML utilities...)
 
 ### Example
 
 The following configuration excerpt from `mkdocs.yml` should cover the basic functionalities of this plugin:
 
 ```yaml
@@ -86,17 +86,22 @@
       buttons:
         - title: Download as PDF
           icon: !!python/name:mkdocs_exporter.plugins.pdf.button.icon
           href: !!python/name:mkdocs_exporter.plugins.pdf.button.href
           download: !!python/name:mkdocs_exporter.plugins.pdf.button.download
 ```
 
+Check out a [sample PDF generated by this plugin](examples/example.pdf) from the default page of the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) theme.  
+It has been built with some custom CSS and features cover pages.
+
 ## Roadmap
 
 - Documentation (based on `MkDocs` and featuring this plugin)
 - Ensure full compatibility with other themes than `mkdocs-material`
 - Combine all pages as one PDF
 
+Feel free to request additional features by submitting an issue or by contributing through a pull request.
+
 ## License
 
 This project is licensed under the `MIT License (MIT)`, which you can read [here](LICENSE.md).
```

