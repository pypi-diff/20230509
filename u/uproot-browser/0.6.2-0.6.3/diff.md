# Comparing `tmp/uproot_browser-0.6.2.tar.gz` & `tmp/uproot_browser-0.6.3.tar.gz`

## Comparing `uproot_browser-0.6.2.tar` & `uproot_browser-0.6.3.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/noxfile.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.github/dependabot.yml
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/docs/make_logo.py
--rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/docs/_images/iterm.png
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/docs/_images/uproot-browser-logo.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_version.pyi
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/dirs.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/exceptions.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/plot.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/plot_mpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/py.typed
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_compat/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_compat/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_compat/importlib/resources.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/browser.css
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/browser.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/header.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/help.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/left_panel.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/right_panel.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/tests/test_dirs.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/tests/test_printouts.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/LICENSE
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/README.md
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/noxfile.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/docs/make_logo.py
+-rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/docs/_images/iterm.png
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/docs/_images/uproot-browser-logo.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_version.pyi
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/dirs.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/exceptions.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/plot.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/plot_mpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/py.typed
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_compat/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_compat/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/browser.css
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/browser.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/header.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/help.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/left_panel.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/right_panel.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/tests/constraints.txt
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/tests/test_dirs.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/tests/test_printouts.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/tests/test_tui.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/LICENSE
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/README.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/PKG-INFO
```

### Comparing `uproot_browser-0.6.2/.pre-commit-config.yaml` & `uproot_browser-0.6.3/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -15,25 +15,25 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: "v0.0.263"
+  rev: "v0.0.265"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: v1.2.0
   hooks:
   - id: mypy
     files: src
-    additional_dependencies: [rich>=12, click>=8.1.1, hist, numpy, textual>0.18]
+    additional_dependencies: [rich>=12, click>=8.1.1, hist, numpy, textual>=0.24]
 
 - repo: https://github.com/codespell-project/codespell
   rev: v2.2.4
   hooks:
   - id: codespell
     args: [-L, "hist,iterm"]
```

### Comparing `uproot_browser-0.6.2/noxfile.py` & `uproot_browser-0.6.3/noxfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import nox
 
 nox.options.sessions = ["lint", "pylint", "tests"]
 
 
-@nox.session
+@nox.session(reuse_venv=True)
 def lint(session: nox.Session) -> None:
     """
     Run the linter.
     """
     session.install("pre-commit")
     session.run("pre-commit", "run", "--all-files", *session.posargs)
 
@@ -19,26 +19,35 @@
     """
     Run the unit and regular tests.
     """
     session.install(".[test]")
     session.run("pytest", *session.posargs)
 
 
+@nox.session(reuse_venv=True)
+def minimums(session: nox.Session) -> None:
+    """
+    Run the unit and regular tests.
+    """
+    session.install(".[test]", "-ctests/constraints.txt")
+    session.run("pytest", *session.posargs)
+
+
 @nox.session
 def pylint(session: nox.Session) -> None:
     """
     Run pylint.
     """
 
     session.install("pylint", "matplotlib")
     session.install("-e", ".")
     session.run("pylint", "src", *session.posargs)
 
 
-@nox.session
+@nox.session(reuse_venv=True)
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
     """
 
     session.install("build")
     session.run("python", "-m", "build")
```

### Comparing `uproot_browser-0.6.2/.github/CONTRIBUTING.md` & `uproot_browser-0.6.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/.github/workflows/ci.yml` & `uproot_browser-0.6.3/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -42,18 +42,24 @@
     - uses: actions/checkout@v3
 
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install package
-      run: python -m pip install .[test]
+      run: python -m pip install ".[test]"
 
     - name: Test package
-      run: python -m pytest -ra
+      run: python -m pytest
+
+    - name: Install minimum versions
+      run: python -m pip install ".[test]" -c tests/constraints.txt
+
+    - name: Test minimum versions
+      run: python -m pytest
 
   pass:
     if: always()
     needs: [checks]
     runs-on: ubuntu-latest
     steps:
       - name: Decide whether the needed jobs succeeded or failed
```

### Comparing `uproot_browser-0.6.2/docs/make_logo.py` & `uproot_browser-0.6.3/docs/make_logo.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/docs/_images/iterm.png` & `uproot_browser-0.6.3/docs/_images/iterm.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/docs/_images/uproot-browser-logo.png` & `uproot_browser-0.6.3/docs/_images/uproot-browser-logo.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/__main__.py` & `uproot_browser-0.6.3/src/uproot_browser/__main__.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/dirs.py` & `uproot_browser-0.6.3/src/uproot_browser/dirs.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/plot.py` & `uproot_browser-0.6.3/src/uproot_browser/plot.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/plot_mpl.py` & `uproot_browser-0.6.3/src/uproot_browser/plot_mpl.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/tree.py` & `uproot_browser-0.6.3/src/uproot_browser/tree.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/tui/README.md` & `uproot_browser-0.6.3/src/uproot_browser/tui/README.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/tui/browser.css` & `uproot_browser-0.6.3/src/uproot_browser/tui/browser.css`

 * *Files 11% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 #error{
     overflow: auto;
     min-width: 100%;
 }
 
 #empty {
-    text-align: center;
+    content-align: center middle;
 }
 
 
 Footer > .footer--highlight {
     background: $secondary-darken-2;
 }
```

### Comparing `uproot_browser-0.6.2/src/uproot_browser/tui/browser.py` & `uproot_browser-0.6.3/src/uproot_browser/tui/browser.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/tui/header.py` & `uproot_browser-0.6.3/src/uproot_browser/tui/header.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/src/uproot_browser/tui/help.py` & `uproot_browser-0.6.3/src/uproot_browser/tui/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         markdown = files("uproot_browser.tui").joinpath("README.md").read_text()
         with textual.containers.Container(id="help-dialog", classes="dialog"):
             yield textual.widgets.MarkdownViewer(markdown, id="help-text")
             with textual.containers.Container(id="help-buttons"):
                 yield textual.widgets.Button("Done", variant="primary", id="help-done")
 
     def on_mount(self) -> None:
-        self.query_one(textual.widgets.Markdown).focus()
+        self.query_one("#help-text", textual.widgets.MarkdownViewer).focus()
 
     def on_button_pressed(self, _event: textual.widgets.Button.Pressed) -> None:
         self.app.pop_screen()
 
     def action_done(self) -> None:
         self.app.pop_screen()
```

### Comparing `uproot_browser-0.6.2/src/uproot_browser/tui/left_panel.py` & `uproot_browser-0.6.3/src/uproot_browser/tui/left_panel.py`

 * *Files 24% similar despite different names*

```diff
@@ -81,31 +81,49 @@
     ) -> None:
         event.stop()
         item = event.node.data
         assert item
         if item.is_dir:
             self.load_directory(event.node)
 
+    def _node_expanded(
+        self, node: textual.widgets.tree.TreeNode[UprootEntry]
+    ) -> textual.widgets.Tree.NodeExpanded[UprootEntry]:
+        try:
+            return self.NodeExpanded(self, node)
+        except TypeError:  # textual < 0.24
+            # pylint: disable-next=(no-value-for-parameter)
+            return self.NodeExpanded(node)  # type:ignore[call-arg,arg-type]
+
+    def _node_collapsed(
+        self, node: textual.widgets.tree.TreeNode[UprootEntry]
+    ) -> textual.widgets.Tree.NodeCollapsed[UprootEntry]:
+        try:
+            return self.NodeCollapsed(self, node)
+        except TypeError:  # textual < 0.24
+            # pylint: disable-next=(no-value-for-parameter)
+            return self.NodeCollapsed(node)  # type:ignore[call-arg,arg-type]
+
     def action_cursor_in(self) -> None:
         node = self.cursor_node
         if node is None:
             return
         if node.allow_expand and not node.is_expanded:
             node.expand()
-            self.post_message(self.NodeExpanded(node))
+            self.post_message(self._node_expanded(node))
 
     def action_cursor_out(self) -> None:
         node = self.cursor_node
         if node is None:
             return
         if node.allow_expand and node.is_expanded:
             node.collapse()
-            self.post_message(self.NodeCollapsed(node))
+            self.post_message(self._node_collapsed(node))
         elif (
             node.parent is not None
             and node.parent.allow_expand
             and node.parent.is_expanded
         ):
             node.parent.collapse()
-            self.post_message(self.NodeCollapsed(node.parent))
+            self.post_message(self._node_collapsed(node))
             self.cursor_line = node.parent.line
             self.scroll_to_line(self.cursor_line)
```

### Comparing `uproot_browser-0.6.2/src/uproot_browser/tui/right_panel.py` & `uproot_browser-0.6.3/src/uproot_browser/tui/right_panel.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/tests/test_printouts.py` & `uproot_browser-0.6.3/tests/test_printouts.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/.gitignore` & `uproot_browser-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/LICENSE` & `uproot_browser-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/README.md` & `uproot_browser-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.2/pyproject.toml` & `uproot_browser-0.6.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -39,24 +39,25 @@
 dependencies = [
   'awkward >=1',
   'click >=8',
   'hist >=2.4',
   'importlib_resources; python_version<"3.9"',
   'lz4',
   'numpy >=1.13.3',
-  'plotext >=5.2.2',
-  'rich >=12.0.0',
+  'plotext >=5.2.7',
+  'rich >=13.3.3',
   'textual >=0.18.0',
   'typing_extensions; python_version<"3.8"',
   'uproot >=4.2.1',
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
+  "pytest-asyncio",
   "scikit-hep-testdata",
 ]
 iterm = [
   "matplotlib",
   "itermplot==0.5",
   "mplhep",
 ]
@@ -80,17 +81,20 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = [
   "error",
   "ignore:can't resolve package from __spec__ or __package__, falling back on __name__ and __path__:ImportWarning",  # PyPy NumPy
+  "ignore:module 'sre_.*' is deprecated:DeprecationWarning:awkward",  # Awkward 1
+  "ignore: pkg_resources is deprecated as an API:DeprecationWarning:uproot",  # Uproot 4
 ]
 log_cli_level = "info"
 testpaths = ["tests"]
+asyncio_mode = "auto"
 
 
 [tool.mypy]
 files = "src"
 python_version = "3.8"
 warn_unused_configs = true
 strict = true
```

### Comparing `uproot_browser-0.6.2/PKG-INFO` & `uproot_browser-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uproot_browser
-Version: 0.6.2
+Version: 0.6.3
 Summary: Tools to inspect ROOT files with uproot
 Project-URL: homepage, https://github.com/scikit-hep/uproot-browser
 Project-URL: repository, https://github.com/scikit-hep/uproot-browser
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 Maintainer-email: The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -53,28 +53,29 @@
 Requires-Python: >=3.7
 Requires-Dist: awkward>=1
 Requires-Dist: click>=8
 Requires-Dist: hist>=2.4
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: lz4
 Requires-Dist: numpy>=1.13.3
-Requires-Dist: plotext>=5.2.2
-Requires-Dist: rich>=12.0.0
+Requires-Dist: plotext>=5.2.7
+Requires-Dist: rich>=13.3.3
 Requires-Dist: textual>=0.18.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: uproot>=4.2.1
 Provides-Extra: dev
 Requires-Dist: ipython>=6; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: scikit-hep-testdata; extra == 'dev'
 Provides-Extra: iterm
 Requires-Dist: itermplot==0.5; extra == 'iterm'
 Requires-Dist: matplotlib; extra == 'iterm'
 Requires-Dist: mplhep; extra == 'iterm'
 Provides-Extra: test
+Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Requires-Dist: scikit-hep-testdata; extra == 'test'
 Description-Content-Type: text/markdown
 
 <img alt="uproot-browser" width="100%" src="https://raw.githubusercontent.com/scikit-hep/uproot-browser/main/docs/_images/uproot-browser-logo.png"/>
 
 # uproot-browser
```

