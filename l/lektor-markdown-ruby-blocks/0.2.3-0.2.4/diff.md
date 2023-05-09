# Comparing `tmp/lektor_markdown_ruby_blocks-0.2.3.tar.gz` & `tmp/lektor_markdown_ruby_blocks-0.2.4.tar.gz`

## Comparing `lektor_markdown_ruby_blocks-0.2.3.tar` & `lektor_markdown_ruby_blocks-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.3/lektor_markdown_ruby_blocks.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.3/LICENSE
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.3/README.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.4/lektor_markdown_ruby_blocks.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.4/README.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 lektor_markdown_ruby_blocks-0.2.4/PKG-INFO
```

### Comparing `lektor_markdown_ruby_blocks-0.2.3/lektor_markdown_ruby_blocks.py` & `lektor_markdown_ruby_blocks-0.2.4/lektor_markdown_ruby_blocks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+""" Plugin that introduces a new syntax to Markdown for generating HTML ruby tags. """
+
 import re
 from collections import namedtuple
 
 from lektor.pluginsystem import Plugin
 
 # group 1: color of the text, group 2: the content
 rb_block_pattern = re.compile(r'^\^\^(#[0-9a-fA-F]{6,8})?\n(.*)\^\^$', flags=re.DOTALL)
 # group 1: base text, group 2: ruby text
 ruby_pattern = re.compile(r'\((.+?)\)\[(.+?)]')
 
 
-def convert(base, ruby):
+def _convert(base, ruby):
     return f'<ruby>{base}<rp>(</rp><rt>{ruby}</rt><rp>)</rp></ruby>'
 
 
 Conversion = namedtuple('Conversion', 'span text')
 
 
 class RubyBlockMixin:
+    """ Mixin class for parsing markdown and generate ruby tags """
+
     def paragraph(self, text):
+        """ Parsing Markdown paragraph """
         match = rb_block_pattern.match(text)
         if match is None:
             return super().paragraph(text)
         color = match[1]
         ruby_text = self._rubify(match[2].strip(), color)
 
         return f'<p>{ruby_text}</p>'
@@ -36,36 +41,39 @@
                 rb_line = self._rubify_line(line, color)
             converted_line.append(rb_line)
         return '<br />\n'.join(converted_line)
 
     def _rubify_line(self, line, color, ignore=False):
         if line == "-##-":
             return ''
-        elif ignore:
+        if ignore:
             return f'<span class="non-ruby-line">{line}</span>'
 
-        cvts = self._collect_convertions(line)
-        for (start, end), rt in cvts[::-1]:
+        conversions = self._collect_conversions(line)
+        for (start, end), rt in conversions[::-1]:
             line = line[:start] + rt + line[end:]
 
         if color is not None:
             rb_line = f'<span class="ruby-line" style="color: {color};">{line}</span>'
         else:
             rb_line = f'<span class="ruby-line">{line}</span>'
 
         return rb_line
 
-    def _collect_convertions(self, line):
+    def _collect_conversions(self, line):
         replacement = []
         for match in ruby_pattern.finditer(line):
             base, ruby = match[1].split('|'), match[2].split('|')
-            cvt_text = ''.join(convert(b, r) for b, r in zip(base, ruby))
+            cvt_text = ''.join(_convert(b, r) for b, r in zip(base, ruby))
             replacement.append(Conversion(match.span(), cvt_text))
         return replacement
 
 
 class RubyBlockPlugin(Plugin):
+    """ Introduces a new syntax to Markdown for generating HTML ruby tags """
+
     name = 'Markdown Ruby Block'
-    description = 'Add supports to ruby blocks syntax in Markdown'
+    description = __doc__
 
-    def on_markdown_config(self, config, **extra):
+    def on_markdown_config(self, config, **_extra):
+        """ Add ruby-syntax handler to the renderer """
         config.renderer_mixins.append(RubyBlockMixin)
```

### Comparing `lektor_markdown_ruby_blocks-0.2.3/.github/workflows/python-publish.yml` & `lektor_markdown_ruby_blocks-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lektor_markdown_ruby_blocks-0.2.3/LICENSE` & `lektor_markdown_ruby_blocks-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lektor_markdown_ruby_blocks-0.2.3/README.md` & `lektor_markdown_ruby_blocks-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lektor_markdown_ruby_blocks-0.2.3/pyproject.toml` & `lektor_markdown_ruby_blocks-0.2.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "lektor-markdown-ruby-blocks"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     { name = "25349023", email = "25349023.qq@gmail.com" },
 ]
-description = "Add supports for ruby blocks syntax in Markdown"
+description = "Introduces a new syntax to Markdown for generating HTML ruby tags"
 long_description = { file = "README.md" }
 long_description_content_type = "text/markdown"
 keywords = ["Lektor", "plugin", "Markdown", "HTML", "ruby-tag"]
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `lektor_markdown_ruby_blocks-0.2.3/PKG-INFO` & `lektor_markdown_ruby_blocks-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: lektor-markdown-ruby-blocks
-Version: 0.2.3
-Summary: Add supports for ruby blocks syntax in Markdown
+Version: 0.2.4
+Summary: Introduces a new syntax to Markdown for generating HTML ruby tags
 Project-URL: Homepage, https://github.com/25349023/lektor-markdown-ruby-blocks
 Author-email: 25349023 <25349023.qq@gmail.com>
 License: MIT License
+License-File: LICENSE
 Keywords: HTML,Lektor,Markdown,plugin,ruby-tag
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Lektor
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

