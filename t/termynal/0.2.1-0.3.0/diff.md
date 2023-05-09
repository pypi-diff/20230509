# Comparing `tmp/termynal-0.2.1.tar.gz` & `tmp/termynal-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.2.1.tar", max compression
+gzip compressed data, was "termynal-0.3.0.tar", max compression
```

## Comparing `termynal-0.2.1.tar` & `termynal-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1092 2023-01-13 17:07:24.903626 termynal-0.2.1/LICENSE
--rw-r--r--   0        0        0      725 2023-01-13 17:07:24.903626 termynal-0.2.1/README.md
--rw-r--r--   0        0        0     2152 2023-01-13 17:07:24.903626 termynal-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-13 17:07:24.903626 termynal-0.2.1/termynal/__init__.py
--rw-r--r--   0        0        0     2050 2023-01-13 17:07:24.903626 termynal-0.2.1/termynal/assets/termynal.css
--rw-r--r--   0        0        0     7384 2023-01-13 17:07:24.903626 termynal-0.2.1/termynal/assets/termynal.js
--rw-r--r--   0        0        0     3246 2023-01-13 17:07:24.903626 termynal-0.2.1/termynal/markdown.py
--rw-r--r--   0        0        0     1069 2023-01-13 17:07:24.903626 termynal-0.2.1/termynal/plugin.py
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 termynal-0.2.1/setup.py
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 termynal-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-09 07:28:18.968331 termynal-0.3.0/LICENSE
+-rw-r--r--   0        0        0      725 2023-05-09 07:28:18.968331 termynal-0.3.0/README.md
+-rw-r--r--   0        0        0     2390 2023-05-09 07:28:18.968331 termynal-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/__init__.py
+-rw-r--r--   0        0        0     2281 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     3251 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/markdown.py
+-rw-r--r--   0        0        0     1121 2023-05-09 07:28:18.968331 termynal-0.3.0/termynal/plugin.py
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 termynal-0.3.0/setup.py
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 termynal-0.3.0/PKG-INFO
```

### Comparing `termynal-0.2.1/LICENSE` & `termynal-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.2.1/README.md` & `termynal-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `termynal-0.2.1/termynal/assets/termynal.css` & `termynal-0.3.0/termynal/assets/termynal.css`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 }
 
 [data-termynal] {
     width: 750px;
     max-width: 100%;
     background: var(--color-bg);
     color: var(--color-text);
-    font-size: 18px;
-    font-family: 'Fira Mono', Consolas, Menlo, Monaco, 'Courier New', Courier, monospace;
+    /* font-size: 18px; */
+    font-size: 15px;
+    /* font-family: 'Fira Mono', Consolas, Menlo, Monaco, 'Courier New', Courier, monospace; */
+    font-family: 'Roboto Mono', 'Fira Mono', Consolas, Menlo, Monaco, 'Courier New', Courier, monospace;
     border-radius: 4px;
     padding: 75px 45px 35px;
     position: relative;
     -webkit-box-sizing: border-box;
             box-sizing: border-box;
 }
 
@@ -47,14 +49,20 @@
     color: var(--color-text-subtle);
     top: 5px;
     left: 0;
     width: 100%;
     text-align: center;
 }
 
+a[data-terminal-control] {
+    text-align: right;
+    display: block;
+    color: #aebbff;
+}
+
 [data-ty] {
     display: block;
     line-height: 2;
 }
 
 [data-ty]:before {
     /* Set up defaults and ensure empty lines are displayed. */
```

### Comparing `termynal-0.2.1/termynal/markdown.py` & `termynal-0.3.0/termynal/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 from typing import List
 
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 
 class Termynal:
-    progress_literal_start = '---&gt; 100%'
-    prompt_literal_start = '$ '
-    custom_literal_start = '# '
+    progress_literal_start = "---&gt; 100%"
+    prompt_literal_start = "$ "
+    custom_literal_start = "# "
 
     def __init__(self, code: str):
         self.code = code
 
     def convert(self) -> List[str]:
         code_lines = []
         code_lines.append('<div class="termy" data-termynal>')
-        for line in self.code.split('\n'):
+        for line in self.code.split("\n"):
             if line.startswith(self.prompt_literal_start):
                 code_lines.append(f'<span data-ty="input">{line[2:]}</span>')
             elif line.startswith(self.custom_literal_start):
                 code_lines.append(
-                    f'<span class="termynal-comment" data-ty>{line}</span>'
+                    f'<span class="termynal-comment" data-ty>{line}</span>',
                 )
             elif line.startswith(self.progress_literal_start):
                 code_lines.append('<span data-ty="progress"></span>')
             else:
-                code_lines.append(f'<span data-ty>{line}</span>')
-        code_lines.append('</div>')
+                code_lines.append(f"<span data-ty>{line}</span>")
+        code_lines.append("</div>")
         return code_lines
 
 
 class TermynalPreprocessor(Preprocessor):
-    rexep = re.compile('(<code.*>)((.|\n)*?)(</code>)')
-    comment = '<!-- termynal -->'
+    rexep = re.compile("(<code.*>)((.|\n)*?)(</code>)")
+    comment = "<!-- termynal -->"
     language_class = 'class="language-console"'
 
-    def run(self, lines):  # noqa:C901
+    def run(self, lines):
         content_by_placeholder = {}
         for i in range(self.md.htmlStash.html_counter):
             placeholder = self.md.htmlStash.get_placeholder(i)
             content = self.md.htmlStash.rawHtmlBlocks[i]
             content_by_placeholder[placeholder] = (content, i)
 
         lines_by_placeholder = self._get_lines(lines, content_by_placeholder)
@@ -50,15 +50,17 @@
             new_lines.append(line)
             if line in lines_by_placeholder:
                 new_lines.extend(lines_by_placeholder[line])
 
         return new_lines
 
     def _get_lines(
-        self, lines, content_by_placeholder
+        self,
+        lines,
+        content_by_placeholder,
     ):  # pylint:disable=too-many-nested-blocks
         lines_by_placeholder = {}
         is_termynal_code = False
         for line in lines:
             if line in content_by_placeholder:
                 (content, i) = content_by_placeholder[line]
                 if content.startswith(self.comment):
@@ -72,24 +74,24 @@
                 if self.language_class in matches.group(1):
                     is_termynal_code = True
 
                 if not is_termynal_code:
                     continue
 
                 is_termynal_code = False
-                self.md.htmlStash.rawHtmlBlocks[i] = ''
+                self.md.htmlStash.rawHtmlBlocks[i] = ""
                 content = matches.group(2)
                 code_lines = Termynal(content).convert()
                 if code_lines:
                     lines_by_placeholder[line] = code_lines
 
         return lines_by_placeholder
 
 
 class TermynalExtension(Extension):
     def extendMarkdown(self, md):  # noqa:N802
         md.registerExtension(self)
-        md.preprocessors.register(TermynalPreprocessor(md), 'termynal', 20)
+        md.preprocessors.register(TermynalPreprocessor(md), "termynal", 20)
 
 
 def makeExtension(**kwargs):  # noqa:N802  # pylint:disable=invalid-name
     return TermynalExtension(**kwargs)
```

### Comparing `termynal-0.2.1/setup.py` & `termynal-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 entry_points = \
 {'markdown.extensions': ['termynal = termynal.markdown:TermynalExtension'],
  'mkdocs.plugins': ['termynal = termynal.plugin:TermynalPlugin']}
 
 setup_kwargs = {
     'name': 'termynal',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': '',
     'long_description': '# Termynal\n\nA lightweight and modern animated terminal window.\nBuilt for [mkdocs](https://www.mkdocs.org/).\n\n## Installation\n\n<!-- termynal -->\n\n```\n$ pip install termynal\n---> 100%\nInstalled\n```\n\n[Example](https://daxartio.github.io/termynal/)\n\n## Usage\n\nUse `<!-- termynal -->` before code block\n\n````\n<!-- termynal -->\n\n```\n// code\n```\n````\n\nor `console` in code block\n\n````\n```console\n// code\n```\n````\n\nprogress, prompt `---> 100%`\n\n````\n```console\n$ show progress\n---> 100%\nDone!\n```\n````\n\ncommand, start with `$`\n\n````\n```console\n$ command\n```\n````\n\ncomment, start with `#`\n\n````\n```console\n# comment\n```\n````\n\n`mkdocs` plugin\n\n```yaml\n...\nplugins:\n  - termynal\n...\n```\n\nThanks [ines](https://github.com/ines/termynal)\n',
     'author': 'Danil Akhtarov',
     'author_email': 'daxartio@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/termynal',
```

### Comparing `termynal-0.2.1/PKG-INFO` & `termynal-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Home-page: https://pypi.org/project/termynal
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

