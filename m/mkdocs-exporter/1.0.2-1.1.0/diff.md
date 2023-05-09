# Comparing `tmp/mkdocs_exporter-1.0.2.tar.gz` & `tmp/mkdocs_exporter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-1.0.2.tar", max compression
+gzip compressed data, was "mkdocs_exporter-1.1.0.tar", max compression
```

## Comparing `mkdocs_exporter-1.0.2.tar` & `mkdocs_exporter-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.0.2/LICENSE
--rw-r--r--   0        0        0     3008 2023-05-08 20:05:08.751775 mkdocs_exporter-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.0.2/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-08 19:20:51.901769 mkdocs_exporter-1.0.2/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-1.0.2/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.0.2/mkdocs_exporter/page.py
--rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-1.0.2/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      894 2023-05-08 15:35:52.373552 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0      629 2023-05-08 15:31:52.723552 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      633 2023-05-08 14:24:00.883541 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0      969 2023-05-08 14:02:42.383538 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4467 2023-05-09 08:52:26.827115 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2257 2023-05-08 19:33:11.371770 mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     3712 2023-05-08 19:28:57.781770 mkdocs_exporter-1.0.2/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.0.2/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.0.2/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.0.2/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.0.2/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0     1298 2023-05-09 08:52:37.767115 mkdocs_exporter-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 mkdocs_exporter-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3084 2023-05-09 09:12:35.847118 mkdocs_exporter-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.1.0/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1899 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-1.1.0/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.1.0/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-1.1.0/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      977 2023-05-09 09:27:33.387117 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0      812 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      731 2023-05-09 09:13:25.647118 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1088 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4793 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2330 2023-05-09 11:31:09.967140 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     4073 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.1.0/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.1.0/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.1.0/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.1.0/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0     1298 2023-05-09 17:08:04.297189 mkdocs_exporter-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4479 1970-01-01 00:00:00.000000 mkdocs_exporter-1.1.0/PKG-INFO
```

### Comparing `mkdocs_exporter-1.0.2/LICENSE` & `mkdocs_exporter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.2/README.md` & `mkdocs_exporter-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         front: resources/templates/covers/front.html.j2
         back: resources/templates/covers/back.html.j2
       stylesheets:
         - resources/stylesheets/pdf.scss
   - mkdocs/exporter/extras:
       buttons:
         - title: Download as PDF
+          enabled: !!python/name:mkdocs_exporter.plugins.pdf.button.enabled
           icon: !!python/name:mkdocs_exporter.plugins.pdf.button.icon
           href: !!python/name:mkdocs_exporter.plugins.pdf.button.href
           download: !!python/name:mkdocs_exporter.plugins.pdf.button.download
 ```
 
 Check out a [sample PDF generated by this plugin](examples/example.pdf) from the default page of the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) theme.  
 It has been built with some custom CSS and features cover pages.
```

### Comparing `mkdocs_exporter-1.0.2/mkdocs_exporter/browser.py` & `mkdocs_exporter-1.1.0/mkdocs_exporter/browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 
     return self._launched
 
 
   def __init__(self):
     """The constructor."""
 
+    self.browser = None
+    self.context = None
     self._launched = False
+    self.playwright = None
     self.lock = asyncio.Lock()
 
 
   async def launch(self) -> Browser:
     """Launches the browser."""
 
     if self.launched:
@@ -54,14 +57,16 @@
   async def close(self) -> Browser:
     """Closes the browser."""
 
     if self.context:
       await self.context.close()
     if self.browser:
       await self.browser.close()
+    if self.playwright:
+      await self.playwright.stop()
 
     self._launched = False
 
     return self
 
 
   async def print(self, html: str) -> bytes:
```

### Comparing `mkdocs_exporter-1.0.2/mkdocs_exporter/plugin.py` & `mkdocs_exporter-1.1.0/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from mkdocs.config import config_options as c
 from mkdocs.config.base import Config as BaseConfig
 
 
 class ButtonConfig(BaseConfig):
   """The configuration of a button."""
 
+  enabled = c.Type((bool, Callable), default=True)
+  """Is the button enabled?"""
+
   title = c.Type((str, Callable))
   """The button's title."""
 
   icon = c.Type((str, Callable))
   """The button's icon (typically, an SVG element)."""
 
   href = c.Type((str, Callable))
```

### Comparing `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from typing import Optional
 from mkdocs.plugins import BasePlugin
 from mkdocs_exporter.page import Page
+from mkdocs.plugins import event_priority
 from mkdocs_exporter.preprocessor import Preprocessor
 from mkdocs_exporter.plugins.extras.config import Config
 
 
 class Plugin(BasePlugin[Config]):
   """The plugin."""
 
 
+  @event_priority(-85)
   def on_post_page(self, html: str, page: Page, **kwargs) -> Optional[str]:
     """Invoked after a page has been built."""
 
+    def resolve(value):
+      if callable(value):
+        return value(page)
+
+      return value
+
     preprocessor = Preprocessor()
 
     preprocessor.preprocess(html)
 
     for button in self.config.buttons:
-      preprocessor.button(**{k: v(page) if callable(v) else v for k, v in button.items()})
+      if resolve(button['enabled']):
+        preprocessor.button(**{k: resolve(v) for k, v in button.items()})
 
     return preprocessor.done()
```

### Comparing `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,28 +41,29 @@
     self.config.scripts = [resolve(path) for path in self.config.scripts]
     self.config.stylesheets = [resolve(path) for path in self.config.stylesheets]
 
 
   def on_serve(self, server: LiveReloadServer, **kwargs) -> LiveReloadServer:
     """Invoked when the website is being served."""
 
-    if not self.config.enabled:
+    if not self._enabled():
       return
     for path in [*self.config.stylesheets, *self.config.scripts]:
       server.watch(path)
     for cover in self.config.covers:
-      server.watch(self.config.covers[cover])
+      if self.config.covers[cover]:
+        server.watch(self.config.covers[cover])
 
     return server
 
 
-  def on_page_markdown(self, markdown: str, **kwargs) -> str:
+  def on_page_markdown(self, markdown: str, page: Page, **kwargs) -> str:
     """Invoked when the page's markdown has been loaded."""
 
-    if not self.config.enabled:
+    if not self._enabled(page) or 'cover' in page.meta.get('hide', []):
       return
 
     content = markdown
 
     if self.config.covers.front:
       with open(self.config.covers.front, 'r') as file:
         content = self.renderer.cover(file.read()) + content
@@ -72,15 +73,15 @@
 
     return content
 
 
   def on_pre_build(self, **kwargs) -> None:
     """Invoked before the build process starts."""
 
-    if not self.config.enabled:
+    if not self._enabled():
       return
     if self.loop and self.loop.is_running():
       self.loop.close()
 
     self.tasks.clear()
 
     self.renderer = Renderer()
@@ -90,32 +91,33 @@
     for script in self.config.scripts:
       self.renderer.add_script(script)
 
 
   def on_pre_page(self, page: Page, config: dict, **kwargs):
     """Invoked before building the page."""
 
-    if not self.config.enabled:
+    if not self._enabled():
       return
 
     directory = os.path.dirname(page.file.abs_dest_path)
     filename = os.path.splitext(os.path.basename(page.file.abs_src_path))[0] + '.pdf'
     fullpath = os.path.join(directory, filename)
 
-    if page.meta.get('pdf', True):
-      page.formats['pdf'] = os.path.relpath(fullpath, config['site_dir'])
+    page.formats['pdf'] = os.path.relpath(fullpath, config['site_dir'])
 
 
   @event_priority(-75)
   def on_post_page(self, html: str, page: Page, config: dict) -> Optional[str]:
     """Invoked after a page has been built."""
 
     page.html = html
 
-    if not self.config.enabled or 'pdf' not in page.formats:
+    if not self._enabled(page):
+      del page.formats['pdf']
+    if 'pdf' not in page.formats:
       return html
 
     async def render(page: Page) -> None:
       logger.info('Rendering PDF for %s...', page.file.src_path)
 
       pdf = await self.renderer.render(page, polyfills=self.config['polyfills'])
       fullpath = os.path.join(config['site_dir'], page.formats['pdf'])
@@ -129,15 +131,15 @@
 
     return page.html
 
 
   def on_post_build(self, **kwargs) -> None:
     """Invoked after the build process."""
 
-    if not self.config.enabled:
+    if not self._enabled():
       return
 
     self.loop = asyncio.new_event_loop()
 
     def partition(list, n):
       for i in range(0, len(list), n):
         yield [self.loop.create_task(task) for task in list[i:i + n]]
@@ -153,7 +155,18 @@
 
 
   def on_shutdown(self) -> None:
     """Invoked on shutdown..."""
 
     if self.loop and self.loop.is_running():
       self.loop.stop()
+
+
+  def _enabled(self, page: Page = None) -> bool:
+    """Is the plugin enabled for this page?"""
+
+    if not self.config.enabled:
+      return False
+    if page and not page.meta.get('pdf', not self.config.explicit):
+      return False
+
+    return True
```

### Comparing `mkdocs_exporter-1.0.2/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
 import os
 import importlib_resources
 
+from urllib.parse import unquote
 from mkdocs_exporter.page import Page
 from mkdocs_exporter.resources import js
 from mkdocs_exporter.browser import Browser
 from mkdocs_exporter.preprocessor import Preprocessor
 from mkdocs_exporter.renderer import Renderer as BaseRenderer
 
 
 class Renderer(BaseRenderer):
   """The renderer."""
 
   def __init__(self, browser: Browser = None):
     """The constructor."""
 
-    self.back_cover = None
-    self.front_cover = None
     self.scripts: list[str] = []
     self.stylesheets: list[str] = []
     self.browser = browser or Browser()
 
 
   def add_stylesheet(self, path: str) -> Renderer:
     """Adds a stylesheet to the renderer."""
@@ -51,32 +50,34 @@
     """Renders a page as a PDF document."""
 
     if not self.browser.launched:
       await self.browser.launch()
 
     preprocessor = Preprocessor()
     base = os.path.dirname(page.file.abs_dest_path)
-    root = base.replace(page.url.rstrip('/'), '', 1).rstrip('/')
+    root = base.replace(unquote(page.url).rstrip('/'), '', 1).rstrip('/')
 
     preprocessor.preprocess(page.html)
-    preprocessor.remove(['.md-sidebar.md-sidebar--primary', '.md-sidebar.md-sidebar--secondary', 'header.md-header', '.md-container > nav'])
+    preprocessor.remove(['.md-sidebar.md-sidebar--primary', '.md-sidebar.md-sidebar--secondary', 'header.md-header', '.md-container > nav', 'nav.md-tags'])
     preprocessor.remove_scripts()
-    preprocessor.update_links(base, root)
-    preprocessor.teleport()
+    preprocessor.set_attribute('details:not([open])', 'open', 'open')
 
     for stylesheet in self.stylesheets:
       with open(stylesheet, 'r') as file:
         preprocessor.stylesheet(file.read())
     for script in self.scripts:
       with open(script, 'r') as file:
         preprocessor.script(file.read())
 
     if kwargs.get('polyfills', True):
       preprocessor.script(importlib_resources.files(js).joinpath('pagedjs.min.js').read_text())
 
+    preprocessor.teleport()
+    preprocessor.update_links(base, root)
+
     html = preprocessor.done()
 
     return await self.browser.print(html)
 
 
   async def dispose(self) -> None:
     """Dispose of the renderer."""
```

### Comparing `mkdocs_exporter-1.0.2/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-1.1.0/mkdocs_exporter/preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,24 @@
 
     return self
 
 
   def button(self, title: str, href: str, icon: str, **kwargs) -> Preprocessor:
     """Adds a button at the top of the page."""
 
+    tags = self.html.find('nav', {'class': 'md-tags'})
     button = self.html.new_tag('a', title=title, href=href, **kwargs, attrs={'class': 'md-content__button md-icon'})
     svg = BeautifulSoup(icon, 'lxml')
 
     button.append(svg)
-    self.html.find('article', {'class': 'md-content__inner'}).insert(0, button)
+
+    if tags:
+      tags.insert_after(button)
+    else:
+      self.html.find('article', {'class': 'md-content__inner'}).insert(0, button)
 
     return self
 
 
   def teleport(self) -> Preprocessor:
     """Teleport elements to their destination."""
 
@@ -105,14 +110,23 @@
     for element in self.html.find_all('script'):
       if predicate(element):
         element.decompose()
 
     return self
 
 
+  def set_attribute(self, selector: str, key: str, value: str) -> Preprocessor:
+    """Set an attribute on elements matching the given selector."""
+
+    for element in self.html.select(selector):
+      element.attrs[key] = value
+
+    return self
+
+
   def update_links(self, base: str, root: str = None) -> Preprocessor:
     """Updates links to their new base location."""
 
     for element in self.html.find_all('link', href=True):
       element['href'] = self._resolve_link(element['href'], base, root)
     for element in self.html.find_all(src=True):
       element['src'] = self._resolve_link(element['src'], base, root)
```

### Comparing `mkdocs_exporter-1.0.2/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-1.1.0/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.0.2/pyproject.toml` & `mkdocs_exporter-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "1.0.2"
+version = "1.1.0"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-1.0.2/PKG-INFO` & `mkdocs_exporter-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 1.0.2
+Version: 1.1.0
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -81,14 +81,15 @@
         front: resources/templates/covers/front.html.j2
         back: resources/templates/covers/back.html.j2
       stylesheets:
         - resources/stylesheets/pdf.scss
   - mkdocs/exporter/extras:
       buttons:
         - title: Download as PDF
+          enabled: !!python/name:mkdocs_exporter.plugins.pdf.button.enabled
           icon: !!python/name:mkdocs_exporter.plugins.pdf.button.icon
           href: !!python/name:mkdocs_exporter.plugins.pdf.button.href
           download: !!python/name:mkdocs_exporter.plugins.pdf.button.download
 ```
 
 Check out a [sample PDF generated by this plugin](examples/example.pdf) from the default page of the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) theme.  
 It has been built with some custom CSS and features cover pages.
```

