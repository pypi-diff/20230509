# Comparing `tmp/chyp-0.2.2.tar.gz` & `tmp/chyp-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.2.2.tar", last modified: Sat May  6 18:11:53 2023, max compression
+gzip compressed data, was "chyp-0.3.tar", last modified: Tue May  9 19:17:03 2023, max compression
```

## Comparing `chyp-0.2.2.tar` & `chyp-0.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 18:11:53.012225 chyp-0.2.2/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.2.2/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9717 2023-05-06 18:11:53.012225 chyp-0.2.2/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9176 2023-05-06 18:09:40.000000 chyp-0.2.2/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 18:11:53.012225 chyp-0.2.2/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.2.2/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.2.2/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15145 2023-05-05 09:54:14.000000 chyp-0.2.2/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 18:11:53.012225 chyp-0.2.2/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.2.2/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1159 2023-05-05 10:07:08.000000 chyp-0.2.2/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.2.2/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5868 2023-05-06 15:16:34.000000 chyp-0.2.2/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    13379 2023-05-06 13:26:34.000000 chyp-0.2.2/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.2.2/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.2.2/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2202 2023-05-06 10:20:10.000000 chyp-0.2.2/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.2.2/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9883 2023-05-05 09:52:49.000000 chyp-0.2.2/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9744 2023-04-28 09:32:11.000000 chyp-0.2.2/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5845 2023-05-05 10:04:52.000000 chyp-0.2.2/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2966 2023-03-29 10:44:17.000000 chyp-0.2.2/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1390 2023-04-26 10:03:49.000000 chyp-0.2.2/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.2.2/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3710 2023-05-05 22:35:47.000000 chyp-0.2.2/chyp/state.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4064 2023-04-23 21:13:55.000000 chyp-0.2.2/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 18:11:53.012225 chyp-0.2.2/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9717 2023-05-06 18:11:53.000000 chyp-0.2.2/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      566 2023-05-06 18:11:53.000000 chyp-0.2.2/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-06 18:11:53.000000 chyp-0.2.2/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-06 18:11:53.000000 chyp-0.2.2/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-06 18:11:53.000000 chyp-0.2.2/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-06 18:11:53.000000 chyp-0.2.2/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.2.2/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-06 18:11:53.012225 chyp-0.2.2/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1065 2023-05-06 18:10:30.000000 chyp-0.2.2/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-09 19:17:03.482142 chyp-0.3/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.3/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9798 2023-05-09 19:17:03.482142 chyp-0.3/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9259 2023-05-07 21:30:27.000000 chyp-0.3/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-09 19:17:03.482142 chyp-0.3/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.3/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.3/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16930 2023-05-08 13:24:18.000000 chyp-0.3/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-09 19:17:03.482142 chyp-0.3/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.3/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3739 2023-05-09 07:10:05.000000 chyp-0.3/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.3/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     5868 2023-05-06 15:16:34.000000 chyp-0.3/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    15080 2023-05-08 20:46:38.000000 chyp-0.3/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2283 2023-05-08 16:45:36.000000 chyp-0.3/chyp/gui/errorlist.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.3/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.3/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2357 2023-05-08 12:36:17.000000 chyp-0.3/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.3/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9883 2023-05-05 09:52:49.000000 chyp-0.3/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10418 2023-05-09 07:19:39.000000 chyp-0.3/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     8707 2023-05-08 16:34:40.000000 chyp-0.3/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3774 2023-05-07 18:11:57.000000 chyp-0.3/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1775 2023-05-08 10:53:38.000000 chyp-0.3/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.3/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4554 2023-05-08 12:31:13.000000 chyp-0.3/chyp/state.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4064 2023-04-23 21:13:55.000000 chyp-0.3/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-09 19:17:03.482142 chyp-0.3/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9798 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      588 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.3/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-09 19:17:03.482142 chyp-0.3/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1063 2023-05-09 19:16:13.000000 chyp-0.3/setup.py
```

### Comparing `chyp-0.2.2/LICENSE` & `chyp-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/PKG-INFO` & `chyp-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.2.2
+Version: 0.3
 Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
@@ -143,22 +143,26 @@
 
 start : statement*
 statement : gen | let | rule | rewrite
 gen : "gen" var ":" num "->" num
 let : "let" var "=" term
 rule : "rule" var ":" term "=" term
 rewrite : "rewrite" var ":" term rewrite_part*
-rewrite_part : "=" term_hole "by" rule_ref num?
+rewrite_part : "=" term_hole "by" inverse? rule_ref
+inverse : "-"
 term  : par_term | seq
 par_term : "(" term ")" | par | perm | id | term_ref
 par : par_term "*" par_term
 seq : term ";" term
-perm : "sw" [ "[" num ("," num)* "]" ]
+perm : "sw" ( "[" num ("," num)* "]" )?
 id : "id"
 term_hole : term | "?"
 
 num : INT
 var : IDENTIFIER
 term_ref : IDENTIFIER
 rule_ref : IDENTIFIER
 
 ```
+
+The parser ignores whitespace and comments starting with `#`.
+
```

### Comparing `chyp-0.2.2/README.md` & `chyp-0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,22 +127,26 @@
 
 start : statement*
 statement : gen | let | rule | rewrite
 gen : "gen" var ":" num "->" num
 let : "let" var "=" term
 rule : "rule" var ":" term "=" term
 rewrite : "rewrite" var ":" term rewrite_part*
-rewrite_part : "=" term_hole "by" rule_ref num?
+rewrite_part : "=" term_hole "by" inverse? rule_ref
+inverse : "-"
 term  : par_term | seq
 par_term : "(" term ")" | par | perm | id | term_ref
 par : par_term "*" par_term
 seq : term ";" term
-perm : "sw" [ "[" num ("," num)* "]" ]
+perm : "sw" ( "[" num ("," num)* "]" )?
 id : "id"
 term_hole : term | "?"
 
 num : INT
 var : IDENTIFIER
 term_ref : IDENTIFIER
 rule_ref : IDENTIFIER
 
 ```
+
+The parser ignores whitespace and comments starting with `#`.
+
```

### Comparing `chyp-0.2.2/chyp/__init__.py` & `chyp-0.3/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/__main__.py` & `chyp-0.3/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/graph.py` & `chyp-0.3/chyp/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
-from typing import Set, List, Dict, Iterator, Any, Optional
+from typing import Iterable, Set, List, Dict, Iterator, Any, Optional, Tuple
 import json
 import copy
 
 class GraphError(Exception):
     pass
 
 class VData:
@@ -214,14 +214,27 @@
 
     def is_output(self, v: int) -> bool:
         return len(self.vdata[v].out_indices) > 0
 
     def is_boundary(self, v: int) -> bool:
         return self.is_input(v) or self.is_output(v)
 
+    def successors(self, vs: Iterable[int]) -> Set[int]:
+        succ: Set[int] = set()
+        current = list(vs)
+        while len(current) > 0:
+            v = current.pop()
+            for e in self.out_edges(v):
+                for v1 in self.target(e):
+                    if v1 not in succ:
+                        succ.add(v1)
+                        current.append(v1)
+
+        return succ
+
     def merge_vertices(self, v: int, w: int) -> None:
         """Identify the two vertices given
 
         Form the quotient of the graph by identifying v with w. Afterwards, the
         quotiented vertex will be named v.
         """
 
@@ -238,14 +251,53 @@
             ed.s = [v if x == w else x for x in ed.s]
             vd.out_edges.add(e)
 
         self.set_inputs([v if x == w else x for x in self.inputs()])
         self.set_outputs([v if x == w else x for x in self.outputs()])
         self.remove_vertex(w)
 
+    def explode_vertex(self, v: int) -> Tuple[List[int], List[int]]:
+        """Split a vertex into one copy for each input, in-tentacle, output, and out-tentacle
+
+        This is used for computing pushout complements of rules that aren't left-linear. Returns
+        a pair of lists containing the new input-like and output-like vertices, respectively.
+        """
+
+        new_vs: Tuple[List[int], List[int]] = ([], [])
+        vd = self.vertex_data(v)
+        def fresh(j: int) -> int:
+            v1 = self.add_vertex(vd.x, vd.y, vd.value)
+            new_vs[j].append(v1)
+            return v1
+
+        self.set_inputs([v1 if v1 != v else fresh(0) for v1 in self.inputs()])
+
+        for e in vd.in_edges:
+            ed = self.edge_data(e)
+            for i in range(len(ed.t)):
+                if ed.t[i] == v:
+                    ed.t[i] = fresh(0)
+                    self.vertex_data(ed.t[i]).in_edges.add(e)
+
+        self.set_outputs([v1 if v1 != v else fresh(1) for v1 in self.outputs()])
+
+        for e in vd.out_edges:
+            ed = self.edge_data(e)
+            for i in range(len(ed.s)):
+                if ed.s[i] == v:
+                    ed.s[i] = fresh(1)
+                    self.vertex_data(ed.s[i]).out_edges.add(e)
+
+
+        vd.in_edges = set()
+        vd.out_edges = set()
+        self.remove_vertex(v, strict=True)
+
+        return new_vs
+
     def insert_id_after(self, v: int, reverse: bool = False) -> int:
         """Insert a new identity hyperedge after the given vertex
 
         Insert a dummy identity box with source at the given vertex and redirect
         any out-edges or outputs to the target of the new hyperedge. If `reverse`
         is True, then flip the source and target of the identity wire. This can be
         used to break directed cycles, essentially by introducing a cap and cup.
```

### Comparing `chyp-0.2.2/chyp/gui/__init__.py` & `chyp-0.3/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/gui/app.py` & `chyp-0.3/chyp/gui/graphview.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,33 +10,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
-import sys
 
-from PySide6.QtWidgets import QApplication
+from PySide6.QtGui import QPainter
+from PySide6.QtWidgets import QGraphicsView
 
-from . import editor
-
-
-class Chyp(QApplication):
-    """The main chyp application
-
-    ...
-    """
+from ..graph import Graph
+from .graphscene import GraphScene
 
+class GraphView(QGraphicsView):
     def __init__(self) -> None:
-        super().__init__(sys.argv)
-        self.setApplicationName('chyp')
-        self.setDesktopFileName("chyp")
-        self.main_window = editor.Editor()
-        self.lastWindowClosed.connect(self.quit)
-
-
-def main() -> None:
-    """Main entry point for chyp"""
-
-    chyp = Chyp()
-    chyp.exec_()
+        self.graph_scene = GraphScene()
+        super().__init__(self.graph_scene)
+        self.setMouseTracking(True)
+        self.setRenderHint(QPainter.RenderHint.Antialiasing)
+        self.setResizeAnchor(QGraphicsView.ViewportAnchor.AnchorViewCenter)
+
+    def set_graph(self, g: Graph) -> None:
+        self.graph_scene.set_graph(g)
+        self.centerOn(0,0)
```

### Comparing `chyp-0.2.2/chyp/gui/codeview.py` & `chyp-0.3/chyp/gui/codeview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/gui/document.py` & `chyp-0.3/chyp/gui/document.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/gui/editor.py` & `chyp-0.3/chyp/gui/editor.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 from typing import Callable, Dict, Optional, Tuple
 from PySide6.QtCore import QByteArray, QFileInfo, QObject, QThread, Qt, QSettings
 from PySide6.QtGui import QCloseEvent, QKeySequence, QTextCursor
-from PySide6.QtWidgets import QApplication, QHBoxLayout, QMainWindow, QMenuBar, QSplitter, QVBoxLayout, QWidget
-
-from chyp.term import graph_to_term
+from PySide6.QtWidgets import QApplication, QHBoxLayout, QMainWindow, QMenuBar, QSplitter, QTreeView, QVBoxLayout, QWidget
 
 from ..layout import convex_layout
 from ..graph import Graph
 from ..state import RewriteState, State
+from ..term import graph_to_term
 from ..matcher import match_rule
 from ..rewrite import rewrite
 
+from .errorlist import ErrorListModel
 from .graphview import GraphView
 from .codeview import CodeView
 from .document import ChypDocument
 from .highlighter import STATUS_GOOD, STATUS_BAD
 
 class Editor(QMainWindow):
     def __init__(self) -> None:
@@ -73,14 +73,18 @@
         self.doc.modificationChanged.connect(self.update_file_name)
         self.doc.recentFilesChanged.connect(self.update_recent_files)
         self.update_file_name()
 
         self.splitter.addWidget(self.code_view)
         self.code_view.setFocus()
 
+        self.error_view = QTreeView()
+        self.error_view.setModel(ErrorListModel())
+        self.splitter.addWidget(self.error_view)
+
         self.build_menu()
 
         splitter_state = conf.value("editor_splitter_state")
         if splitter_state and isinstance(splitter_state, QByteArray): self.splitter.restoreState(splitter_state)
 
         self.code_view.cursorPositionChanged.connect(self.show_at_cursor)
         self.code_view.textChanged.connect(self.invalidate_text)
@@ -128,17 +132,21 @@
         edit_undo.setShortcut(QKeySequence(QKeySequence.StandardKey.Undo))
         edit_undo.triggered.connect(self.code_view.undo)
 
         edit_redo = edit_menu.addAction("&Redo")
         edit_redo.setShortcut(QKeySequence(QKeySequence.StandardKey.Redo))
         edit_redo.triggered.connect(self.code_view.redo)
 
-        code_run = code_menu.addAction("&Run")
-        code_run.setShortcut(QKeySequence("Ctrl+R"))
-        code_run.triggered.connect(self.update)
+        # code_run = code_menu.addAction("&Run")
+        # code_run.setShortcut(QKeySequence("Ctrl+R"))
+        # code_run.triggered.connect(self.update_state)
+
+        code_show_errors = code_menu.addAction("Show &Errors")
+        code_show_errors.setShortcut(QKeySequence("F4"))
+        code_show_errors.triggered.connect(self.show_errors)
 
         code_add_rewrite_step = code_menu.addAction("&Add Rewrite Step")
         code_add_rewrite_step.setShortcut(QKeySequence("Ctrl+Return"))
         code_add_rewrite_step.triggered.connect(lambda: self.code_view.add_line_below("  = ? by "))
 
         code_add_rewrite_step = code_menu.addAction("&Repeat Rewrite Step")
         code_add_rewrite_step.setShortcut(QKeySequence("Ctrl+Shift+Return"))
@@ -200,14 +208,35 @@
 
         if i >= 0 and i < len(self.state.parts):
             p1 = self.state.parts[i]
             cursor.setPosition(p1[1])
             self.code_view.setTextCursor(cursor)
             
 
+    def show_errors(self):
+        conf = QSettings('chyp', 'chyp')
+        error_panel_size = conf.value('error_panel_size', 100)
+        if isinstance(error_panel_size, str):
+            error_panel_size = int(error_panel_size)
+        if not isinstance(error_panel_size, int) or error_panel_size == 0:
+            error_panel_size = 100
+        
+        sizes = self.splitter.sizes()
+        if sizes[2] == 0:
+            sizes[2] = error_panel_size
+            if sizes[1] >= error_panel_size + 50:
+                sizes[1] -= error_panel_size
+            else:
+                sizes[0] -= error_panel_size
+        else:
+            conf.setValue('error_panel_size', sizes[2])
+            sizes[1] += sizes[2]
+            sizes[2] = 0
+        self.splitter.setSizes(sizes)
+
     def show_at_cursor(self) -> None:
         if not self.parsed: return
 
         pos = self.code_view.textCursor().position()
         p = self.state.part_with_index_at(pos)
         if p:
             i, part = p
@@ -247,16 +276,16 @@
                                     self.show_at_cursor()
                                 return f
 
                             check_thread = CheckThread(rw, self)
                             check_thread.finished.connect(check_finished(i))
                             check_thread.start()
 
-                    lhs = rw.lhs.copy()
-                    rhs = rw.rhs.copy()
+                    lhs = rw.lhs.copy() if rw.lhs else Graph()
+                    rhs = rw.rhs.copy() if rw.rhs else Graph()
                     convex_layout(lhs)
                     convex_layout(rhs)
                     self.graph_cache[i] = (lhs, rhs)
                 else:
                     lhs, rhs0 = self.graph_cache[i]
                     if not rhs0: raise ValueError("Rewrite step in graph_cache should have RHS")
                     rhs = rhs0
@@ -275,52 +304,61 @@
         self.update_state()
         if not self.parsed: return
 
         pos = self.code_view.textCursor().position()
         part = self.state.part_at(pos)
         if part and part[2] == 'rewrite' and part[3] in self.state.rewrites:
             rw = self.state.rewrites[part[3]]
-            start, end = rw.term_pos
-            text = self.code_view.toPlainText()
-            term = text[start:end]
-
-            found_prev = (term == '?')
-            rw_term = None
-            for m in match_rule(rw.rule, rw.lhs):
-                t = graph_to_term(rewrite(rw.rule, m))
-                if found_prev and term != t:
-                    rw_term = t
-                    break
-                elif not rw_term:
-                    rw_term = t
-
-                found_prev = (term == t)
-
-            if rw_term:
-                cursor = self.code_view.textCursor()
-                cursor.clearSelection()
-                cursor.setPosition(start)
-                cursor.setPosition(end, mode=QTextCursor.MoveMode.KeepAnchor)
-                cursor.insertText(rw_term)
-                self.code_view.setTextCursor(cursor)
-                self.update_state()
+            if rw.rule and rw.lhs:
+                start, end = rw.term_pos
+                text = self.code_view.toPlainText()
+                term = text[start:end]
+                seen = set([term])
+
+                found_prev = (term == '?')
+                rw_term = None
+                for m in match_rule(rw.rule, rw.lhs):
+                    t = graph_to_term(rewrite(rw.rule, m))
+                    if found_prev and not t in seen:
+                        rw_term = t
+                        break
+                    elif not rw_term:
+                        rw_term = t
+
+                    seen.add(t)
+                    found_prev = (term == t)
+
+                if rw_term:
+                    cursor = self.code_view.textCursor()
+                    cursor.clearSelection()
+                    cursor.setPosition(start)
+                    cursor.setPosition(end, mode=QTextCursor.MoveMode.KeepAnchor)
+                    cursor.insertText(rw_term)
+                    self.code_view.setTextCursor(cursor)
+                    self.update_state()
 
     def repeat_step_at_cursor(self) -> None:
         self.update_state()
         pos = self.code_view.textCursor().position()
         part = self.state.part_at(pos)
         if part and part[2] == 'rewrite' and part[3] in self.state.rewrites:
             rule = self.state.rewrites[part[3]].rule
-            self.code_view.add_line_below('  = ? by ' + rule.name)
-            self.update_state()
-            self.next_rewrite_at_cursor()
+
+            if rule:
+                self.code_view.add_line_below('  = ? by ' + rule.name)
+                self.update_state()
+                self.next_rewrite_at_cursor()
 
     def update_state(self, quiet: bool=False) -> None:
         self.code_view.set_current_region(None)
         self.state.update(self.code_view.toPlainText())
+        
+        model = self.error_view.model()
+        if isinstance(model, ErrorListModel):
+            model.set_errors(self.state.errors)
 
         if len(self.state.errors) == 0:
             self.lhs_view.set_graph(Graph())
             self.rhs_view.setVisible(False)
             self.parsed = True
             self.show_at_cursor()
         elif not quiet:
@@ -329,14 +367,17 @@
                 print("%d: %s" % err)
 
     def closeEvent(self, e: QCloseEvent) -> None:
         if self.doc.confirm_close():
             conf = QSettings('chyp', 'chyp')
             conf.setValue("editor_window_geometry", self.saveGeometry())
             conf.setValue("editor_splitter_state", self.splitter.saveState())
+            sizes = self.splitter.sizes()
+            if sizes[2] != 0:
+                conf.setValue('error_panel_size', sizes[2])
             e.accept()
         else:
             e.ignore()
 
 class CheckThread(QThread):
     def __init__(self, rw: RewriteState, parent: Optional[QObject] = None) -> None:
         super().__init__(parent)
```

### Comparing `chyp-0.2.2/chyp/gui/graphscene.py` & `chyp-0.3/chyp/gui/graphscene.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/gui/highlighter.py` & `chyp-0.3/chyp/gui/highlighter.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 FG =      '#cad3f5'
 BG =      '#24273a'
 SEL =     '#363a4f'
 KEYWORD = '#8aadf4'
 IDENT =   '#91d7e3'
 NUM =     '#ed8796'
 OP =      '#eed49f'
+COMMENT = '#8087a2'
 BG_GOOD = '#36504f'
 BG_BAD  = '#863a4f'
 
 class ChypHighlighter(QSyntaxHighlighter):
     def __init__(self, doc: QTextDocument) -> None:
         super().__init__(doc)
         self.region: Optional[Tuple[int,int]] = None
@@ -26,27 +27,31 @@
     def set_current_region(self, region: Optional[Tuple[int,int]], status: int) -> None:
         self.region = region
         self.region_status = status
         self.rehighlight()
 
     def highlightBlock(self, text: str) -> None:
         ident = '[a-zA-Z_][a-zA-Z0-9_]*'
-        for m in re.finditer('(^|\\W)(let|gen|rule|by|rewrite)\\s+(%s)?' % ident, text):
+        for m in re.finditer('(^|\\W)(let|gen|rule|by|rewrite)\\s+\\-?\\s*(%s)?' % ident, text):
             x,y = m.span(2)
             self.setFormat(x, y-x, QColor(KEYWORD))
             x,y = m.span(3)
             self.setFormat(x, y-x, QColor(IDENT))
 
-        for m in re.finditer('[?.>:;*=\\-\\[\\]]', text):
+        for m in re.finditer('[?~.><:;*=\\-\\[\\]]', text):
             self.setFormat(m.start(), 1, QColor(OP))
 
         for m in re.finditer('(\\W|^)([0-9]+)(\\W|$)', text):
             x,y = m.span(2)
             self.setFormat(x, y-x, QColor(NUM))
 
+        for m in re.finditer('#.*$', text):
+            x,y = m.span(0)
+            self.setFormat(x, y-x, QColor(COMMENT))
+
         # highlight the region that is currently in focus
         if self.region:
             x, y = self.region
             start = self.currentBlock().position()
             length = self.currentBlock().length()
             end = start + length
             if y >= start and x < end:
```

### Comparing `chyp-0.2.2/chyp/gui/mainwindow.py` & `chyp-0.3/chyp/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/layout.py` & `chyp-0.3/chyp/layout.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/matcher.py` & `chyp-0.3/chyp/matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,14 +202,21 @@
 
     def is_surjective(self) -> bool:
         return len(self.vimg) == self.cod.num_vertices() and len(self.eimg) == self.cod.num_edges()
 
     def is_injective(self) -> bool:
         return len(self.vmap) == len(self.vimg)
 
+    def is_convex(self) -> bool:
+        future = self.cod.successors([self.vmap[v] for v in self.dom.outputs() if v in self.vmap])
+        for v in self.dom.inputs():
+            if v in self.vmap and self.vmap[v] in future:
+                return False
+        return True
+
     # def is_cospan_iso(self) -> bool:
     #     d_in = self.dom.inputs()
     #     d_out = self.dom.outputs()
     #     c_in = self.cod.inputs()
     #     c_out = self.cod.outputs()
     #
     #     return (len(d_in) == len(c_in) and
@@ -217,47 +224,55 @@
     #             all(self.vmap[d_in[i]] == c_in[i] for i in range(len(d_in))) and
     #             all(self.vmap[d_out[i]] == c_out[i] for i in range(len(d_out))) and
     #             self.is_injective() and self.is_surjective())
 
 
 
 class Matches(Iterable):
-    def __init__(self, dom: Graph, cod: Graph, initial_match: Optional[Match] = None) -> None:
+    def __init__(self, dom: Graph, cod: Graph, initial_match: Optional[Match] = None, convex=True) -> None:
         if initial_match is None: initial_match = Match(dom=dom, cod=cod) 
+        self.convex = convex
         self.match_stack = [initial_match]
 
     def __iter__(self) -> Iterator:
         return self
 
     def __next__(self) -> Match:
         while len(self.match_stack) > 0:
             m = self.match_stack.pop()
             if m.is_total():
                 match_log("got successful match:\n" + str(m))
-                return m
+                if self.convex:
+                    if m.is_convex():
+                        match_log("match is convex, returning")
+                        return m
+                    else:
+                        match_log("match is not convex, dropping")
+                else:
+                    return m
             else:
                 self.match_stack += m.more()
         raise StopIteration
 
-def match_graph(dom: Graph, cod: Graph) -> Iterable[Match]:
-    return Matches(dom, cod)
+def match_graph(dom: Graph, cod: Graph, convex=True) -> Iterable[Match]:
+    return Matches(dom, cod, convex=convex)
 
-def match_rule(r: Rule, g: Graph) -> Iterable[Match]:
-    return Matches(r.lhs, g)
+def match_rule(r: Rule, g: Graph, convex=True) -> Iterable[Match]:
+    return Matches(r.lhs, g, convex=convex)
 
 def find_iso(g: Graph, h: Graph) -> Optional[Match]:
     g_in = g.inputs()
     g_out = g.outputs()
     h_in = h.inputs()
     h_out = h.outputs()
     if len(g_in) != len(h_in) or len(g_out) != len(h_out): return None
 
     m0 = Match(dom=g, cod=h)
     for i in range(len(g_in)):
         if not m0.try_add_vertex(g_in[i], h_in[i]): return None
     for i in range(len(g_out)):
         if not m0.try_add_vertex(g_out[i], h_out[i]): return None
 
-    for m in Matches(dom=g, cod=h, initial_match=m0):
+    for m in Matches(dom=g, cod=h, initial_match=m0, convex=False):
         if m.is_surjective(): return m
 
     return None
```

### Comparing `chyp-0.2.2/chyp/parser.py` & `chyp-0.3/chyp/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 from typing import Any, Dict, List, Optional, Tuple
-from lark import Lark, Transformer, UnexpectedCharacters, UnexpectedEOF, UnexpectedToken, v_args
+from lark import Lark, Transformer, UnexpectedInput, v_args
 from lark.tree import Meta
 
 from .graph import Graph, GraphError, gen, perm, identity
 from .rule import Rule, RuleError
 
 GRAMMAR = Lark("""
     start : statement*
     ?statement : gen | let | rule | rewrite
     gen : "gen" var ":" num "->" num
     let : "let" var "=" term
-    rule : "rule" var ":" term "=" term
-    rewrite : "rewrite" var ":" term rewrite_part*
-    rewrite_part : "=" term_hole "by" rule_ref num?
+    rule : "rule" var ":" term (eq | le) term
+    rewrite : "rewrite" [converse] var ":" term rewrite_part*
+    rewrite_part : (eq | le) term_hole [ "by" [converse] rule_ref ]
+    converse : "-"
     ?term  : par_term | seq
     ?par_term : "(" term ")" | par | perm | id | term_ref
     par : par_term "*" par_term
     seq : term ";" term
     perm : "sw" [ "[" num ("," num)* "]" ]
     id : "id"
 
+    eq : "=" | "=="
+    le : "<=" | "~>"
     num : INT
     var : CNAME
     term_ref : CNAME
     rule_ref : CNAME
     term_hole : term | "?"
 
     %import common.CNAME
     %import common.INT
-    %ignore " "
-    %ignore "\\n"
+    %import common.WS
+    %import common.SH_COMMENT
+    %ignore WS
+    %ignore SH_COMMENT
     """,
     parser='lalr',
-    propagate_positions=True)
+    propagate_positions=True,
+    maybe_placeholders=True)
 
 class ChypParseData(Transformer):
 
     def __init__(self) -> None:
         self.graphs: Dict[str, Graph] = dict()
-        self.rules: Dict[str, Rule] = dict()
-        self.rewrites: Dict[str, Tuple[int, int, Optional[Rule], Optional[Graph], Optional[Graph]]] = dict()
+        self.rules: Dict[str, Rule] = {'refl': Rule(Graph(), Graph(), name="refl")}
+        self.rewrites: Dict[str, Tuple[int, int, bool, Optional[Rule],
+                                       Optional[Graph], Optional[Graph],
+                                       Optional[Graph], Optional[Graph]]] = dict()
         self.errors: List[Tuple[int, str]] = list()
         self.parts: List[Tuple[int, int, str, str]] = list()
         self.parsed = False
     
     # def start(self, items: List[List[Tuple[int,int,str,str]]]):
     #     pass
         
@@ -52,14 +60,20 @@
     
     def num(self, items: List[Any]) -> int:
         return int(items[0])
 
     def id(self, _: List[Any]) -> Graph:
         return identity()
 
+    def eq(self, _: List[Any]) -> bool:
+        return True
+
+    def le(self, _: List[Any]) -> bool:
+        return False
+
     @v_args(meta=True)
     def perm(self, meta: Meta, items: List[Any]) -> Optional[Graph]:
         try:
             if items[0] is None:
                 return perm([1,0])
             else:
                 return perm([int(i) for i in items])
@@ -78,15 +92,15 @@
 
     @v_args(meta=True)
     def rule_ref(self, meta: Meta, items: List[Any]) -> Optional[Rule]:
         s = str(items[0])
         if s in self.rules:
             return self.rules[str(items[0])]
         else:
-            self.errors.append((meta.line, 'Undefined term: ' + s))
+            self.errors.append((meta.line, 'Undefined rule: ' + s))
             return None
     
     def par(self, items: List[Any]) -> Optional[Graph]:
         if items[0] and items[1]:
             return items[0] * items[1]
         else:
             return None
@@ -102,76 +116,128 @@
             return g
         else:
             return None
 
     @v_args(meta=True)
     def gen(self, meta: Meta, items: List[Any]) -> None:
         name, arity, coarity = items
-        self.graphs[name] = gen(name, arity, coarity)
+        if not name in self.graphs:
+            self.graphs[name] = gen(name, arity, coarity)
+        else:
+            self.errors.append((meta.line, "Term '{}' already defined.".format(name)))
         self.parts.append((meta.start_pos, meta.end_pos, 'gen', name))
         
     @v_args(meta=True)
     def let(self, meta: Meta, items: List[Any]) -> None:
         name, graph = items
-        if graph:
-            self.graphs[name] = graph
+        if not name in self.graphs:
+            if graph:
+                self.graphs[name] = graph
+        else:
+            self.errors.append((meta.line, "Term '{}' already defined.".format(name)))
         self.parts.append((meta.start_pos, meta.end_pos, 'let', name))
 
     @v_args(meta=True)
     def rule(self, meta: Meta, items: List[Any]) -> None:
-        name, lhs, rhs = items
-        if lhs and rhs:
-            try:
-                self.rules[name] = Rule(lhs, rhs, name=name)
-            except RuleError as e:
-                self.errors.append((meta.line, str(e)))
+        name, lhs, invertible, rhs = items
+        if not name in self.rules:
+            if lhs and rhs:
+                try:
+                    self.rules[name] = Rule(lhs, rhs, name, invertible)
+                except RuleError as e:
+                    self.errors.append((meta.line, str(e)))
+        else:
+            self.errors.append((meta.line, "Rule '{}' already defined.".format(name)))
         self.parts.append((meta.start_pos, meta.end_pos, 'rule', name))
 
     @v_args(meta=True)
     def rewrite(self, meta: Meta, items: List[Any]) -> None:
-        name = items[0]
-        term = items[1]
-        rw_parts = items[2:]
+        converse = True if items[0] else False
+        base_name = items[1]
+        name = '-' + base_name if converse else base_name
+
+        term = items[2]
+        rw_parts = items[3:]
 
         if len(rw_parts) == 0:
             self.parts.append((meta.start_pos, meta.end_pos, "rewrite", name))
-            self.rewrites[name] = (0,0,None,term,None)
+            self.rewrites[name] = (0,0,False,None,term,None,None,None)
         else:
             start = meta.start_pos
             lhs = term
             rhs = None
+            all_equiv = True
+
+            if converse and base_name in self.rules:
+                lhs_match = self.rules[base_name].rhs
+                rhs_match = self.rules[base_name].lhs
+            else:
+                lhs_match = None
+                rhs_match = None
+
+            last_i = len(rw_parts)-1
             for i, rw_part in enumerate(rw_parts):
-                end, t_start, t_end, rule, rhs = rw_part
-                self.rewrites[name + ":" + str(i)] = (t_start, t_end, rule, lhs, rhs)
+                end, t_start, t_end, equiv, rule, rhs = rw_part
+                all_equiv = all_equiv and equiv
+                self.rewrites[name + ":" + str(i)] = (t_start, t_end, equiv, rule, lhs, rhs,
+                                                      lhs_match if i == 0 else None,
+                                                      rhs_match if i == last_i else None)
                 lhs = rhs.copy() if rhs else None
                 self.parts.append((start, end, "rewrite", name + ":" + str(i)))
                 start = end
-            if rhs:
-                self.rules[name] = Rule(term, rhs, name)
+            if term and rhs:
+                try:
+                    if converse:
+                        if base_name in self.rules:
+                            self.rules[base_name].equiv = True
+                        else:
+                            self.errors.append((meta.line, "Trying to prove converse for unknown rule: " + base_name))
+                    else:
+                        if not name in self.rules:
+                            self.rules[name] = Rule(term, rhs, name=name, equiv=all_equiv)
+                        else:
+                            self.errors.append((meta.line, "Rule '{}' already defined.".format(name)))
+                except RuleError as e:
+                    self.errors.append((meta.line, str(e)))
+
+    @v_args(meta=True)
+    def rewrite_part(self, meta: Meta, items: List[Any]) -> Tuple[int, int, int, bool, Optional[Rule], Optional[Graph]]:
+        equiv = items[0]
+        t_start,t_end,rhs = items[1]
+        converse = True if items[2] else False
+
+        rule = items[3] if items[3] else self.rules['refl']
+        if rule and converse:
+            rule = items[3].converse()
 
-    @v_args(meta=True)
-    def rewrite_part(self, meta: Meta, items: List[Any]) -> Tuple[int, int, int, Rule, Graph]:
-        t_start,t_end,rhs = items[0]
-        rule = items[1]
-        return (meta.end_pos, t_start, t_end, rule, rhs)
+        if equiv and rule and not rule.equiv:
+            rule = None
+
+        return (meta.end_pos, t_start, t_end, equiv, rule, rhs)
 
 
     @v_args(meta=True)
     def term_hole(self, meta: Meta, items: List[Any]) -> Tuple[int, int, Optional[Graph]]:
         t = items[0] if len(items) != 0 else None
         return (meta.start_pos, meta.end_pos, t)
 
 def parse(code: str) -> ChypParseData:
     parse_data = ChypParseData()
     try:
         tree = GRAMMAR.parse(code)
         parse_data.transform(tree)
         parse_data.parsed = True
-    except UnexpectedEOF as e:
-        parse_data.errors += [(-1, str(e))]
-    except UnexpectedToken as e:
-        parse_data.errors += [(e.token.line, str(e))]
-    except UnexpectedCharacters as e:
-        parse_data.errors += [(e.line, str(e))]
+    except UnexpectedInput as e:
+        msg = 'Parse error: '
+        e_lines = e.get_context(code).splitlines()
+        if len(e_lines) >= 2:
+            parse_data.errors += [(e.line, msg + e_lines[0] + '\n' + len(msg)*' ' + e_lines[1])]
+        else:
+            parse_data.errors += [(e.line, msg + e_lines[0])]
+
+    # except UnexpectedToken as e:
+    #     parse_data.errors += [(e.line, "Parse error, unexpected token:\n" + e.get_context(code))]
+    # except UnexpectedCharacters as e:
+    #     parse_data.errors += [(e.line, "Parse error, unexpected characters:\n" + e.get_context(code))]
 
     return parse_data
```

### Comparing `chyp-0.2.2/chyp/rewrite.py` & `chyp-0.3/chyp/rewrite.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,40 +22,61 @@
 
 def dpo(r: Rule, m: Match) -> Iterable[Match]:
     """Do double-pushout rewriting
 
     Given a rule r and match of r.lhs into a graph, return a match
     of r.rhs into the rewritten graph.
     """
-    if not r.is_left_linear():
-        raise NotImplementedError("Only left linear rules are supported for now")
+    # if not r.is_left_linear():
+    #     raise NotImplementedError("Only left linear rules are supported for now")
+
+    # store the vertices we have split for id's on the LHS
+    in_map: Dict[int, int] = dict()
+    out_map: Dict[int, int] = dict()
 
     # compute the pushout complement
     ctx = m.cod.copy()
     for e in r.lhs.edges():
         ctx.remove_edge(m.emap[e])
     for v in r.lhs.vertices():
-        if not r.lhs.is_boundary(v):
-            ctx.remove_vertex(m.vmap[v])
+        v1 = m.vmap[v]
+        if r.lhs.is_boundary(v):
+            in_c = len(r.lhs.vertex_data(v).in_indices)
+            out_c = len(r.lhs.vertex_data(v).out_indices)
+            if in_c == 1 and out_c == 1:
+                v1i, v1o = ctx.explode_vertex(v1)
+                if len(v1i) == 1 and len(v1o) == 1:
+                    in_map[v] = v1i[0]
+                    out_map[v] = v1o[0]
+                else:
+                    raise NotImplementedError("Rewriting modulo Frobenius not yet supported.")
+            elif in_c > 1 or out_c > 1:
+                raise NotImplementedError("Rewriting modulo Frobenius not yet supported.")
+        else:
+            ctx.remove_vertex(v1)
 
     # this will be the rewritten graph
     h = ctx
 
-    # TODO: we should make a copy of ctx if we intend to keep it
-    # ctx = ctx.copy()
-    # ctx.set_outputs(ctx.outputs() + [m.vmap[v] for v in r.lhs.inputs()])
-    # ctx.set_inputs(ctx.inputs() + [m.vmap[v] for v in r.lhs.outputs()])
-
     # this will embed r.rhs into h
     m1 = Match(r.rhs, h)
     # vmap1: Dict[int,int] = {}
 
-    # first map the boundary, using the matching of the lhs
-    for vl,vr in zip(r.lhs.inputs(), r.rhs.inputs()): m1.vmap[vr] = m.vmap[vl]
-    for vl,vr in zip(r.lhs.outputs(), r.rhs.outputs()): m1.vmap[vr] = m.vmap[vl]
+    # first map the inputs, using the matching of the lhs
+    for vl,vr in zip(r.lhs.inputs(), r.rhs.inputs()):
+        m1.vmap[vr] = in_map[vl] if vl in in_map else m.vmap[vl]
+
+    # next map the outputs. if the same vertex is an input and an output in r.rhs, then
+    # merge them in h.
+    for vl,vr in zip(r.lhs.outputs(), r.rhs.outputs()):
+        vr1 = out_map[vl] if vl in out_map else m.vmap[vl]
+        if vr in m1.vmap:
+            h.merge_vertices(m1.vmap[vr], vr1)
+        else:
+            m1.vmap[vr] = vr1
 
     # then map the interior to new, fresh vertices
     for v in r.rhs.vertices():
         if not r.rhs.is_boundary(v):
             vd = r.rhs.vertex_data(v)
             v1 = h.add_vertex(vd.x, vd.y, vd.value)
             m1.vmap[v] = v1
@@ -66,15 +87,15 @@
         ed = r.rhs.edge_data(e)
         e1 = h.add_edge([m1.vmap[v] for v in ed.s],
                         [m1.vmap[v] for v in ed.t],
                         ed.value, ed.x, ed.y, ed.hyper)
         m1.emap[e] = e1
         m1.eimg.add(e1)
 
-    return [(m1)]
+    return [m1]
 
 def rewrite(r: Rule, m: Match) -> Graph:
     """Apply the given rewrite r to at match m and return the first result
 
     This is a convience wrapper for `dpo` for when the extra rewrite data
     isn't needed."""
```

### Comparing `chyp-0.2.2/chyp/rule.py` & `chyp-0.3/chyp/rule.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,29 +11,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 import itertools
+from typing import Optional
+
 from .graph import Graph
 
 class RuleError(Exception):
     pass
 
 class Rule:
     lhs: Graph
     rhs: Graph
 
-    def __init__(self, lhs: Graph, rhs: Graph, name: str=''):
+    def __init__(self, lhs: Graph, rhs: Graph, name: str='', equiv: bool=True):
         if len(lhs.inputs()) != len(rhs.inputs()) or len(lhs.outputs()) != len(rhs.outputs()):
             raise RuleError("Inputs and outputs must match on LHS and RHS of rule")
         self.lhs = lhs
         self.rhs = rhs
         self.name = name
+        self.equiv = equiv
+
+    def converse(self) -> Optional[Rule]:
+        if self.equiv:
+            if self.name.startswith('-'):
+                name = self.name[1:]
+            else:
+                name = '-' + self.name
+
+            return Rule(self.rhs.copy(), self.lhs.copy(), name, True)
+        else:
+            return None
 
     def is_left_linear(self) -> bool:
         """Returns True if boundary on lhs embeds injectively"""
         verts = set()
         for v in itertools.chain(self.lhs.inputs(), self.lhs.outputs()):
             if v in verts: return False
             verts.add(v)
```

### Comparing `chyp-0.2.2/chyp/scraps.py` & `chyp-0.3/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp/state.py` & `chyp-0.3/chyp/state.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,43 +32,58 @@
     UNCHECKED = 0
     CHECKING = 1
     VALID = 2
     INVALID = 3
 
     def __init__(self,
                  term_pos: Tuple[int,int] = (0,0),
+                 equiv: bool=True,
                  rule: Optional[Rule]=None,
                  lhs: Optional[Graph]=None,
                  rhs: Optional[Graph]=None,
+                 lhs_match: Optional[Graph]=None,
+                 rhs_match: Optional[Graph]=None,
                  stub: bool=False) -> None:
         self.status = RewriteState.UNCHECKED
         self.term_pos = term_pos
-        self.rule = rule if rule else Rule(Graph(), Graph())
-        self.lhs = lhs if lhs else Graph()
-        self.rhs = rhs if rhs else Graph()
+        self.equiv = equiv
+        self.rule = rule
+        self.lhs = lhs
+        self.rhs = rhs
+        self.lhs_match = lhs_match
+        self.rhs_match = rhs_match
         self.stub = stub
 
     def check(self) -> None:
-        for m_lhs in match_rule(self.rule, self.lhs):
-            for m_rhs in dpo(self.rule, m_lhs):
-                iso = find_iso(m_rhs.cod, self.rhs)
-                if iso:
-                    self.status = RewriteState.VALID
-
-                    for v in m_lhs.dom.vertices():
-                        self.lhs.vertex_data(m_lhs.vmap[v]).highlight = True
-                    for e in m_lhs.dom.edges():
-                        self.lhs.edge_data(m_lhs.emap[e]).highlight = True
-
-                    for v in m_rhs.dom.vertices():
-                        self.rhs.vertex_data(iso.vmap[m_rhs.vmap[v]]).highlight = True
-                    for e in m_rhs.dom.edges():
-                        self.rhs.edge_data(iso.emap[m_rhs.emap[e]]).highlight = True
+        if self.rule and self.lhs and self.rhs:
+            # check for any constraints on the LHS and RHS first
+            if self.lhs_match and not find_iso(self.lhs, self.lhs_match):
+                self.status = RewriteState.INVALID
+            if self.rhs_match and not find_iso(self.rhs, self.rhs_match):
+                self.status = RewriteState.INVALID
+
+            # if all LHS/RHS constraints are satisfied, try to prove the rule step by rewriting
+            if self.status == RewriteState.CHECKING:
+                for m_lhs in match_rule(self.rule, self.lhs):
+                    for m_rhs in dpo(self.rule, m_lhs):
+                        iso = find_iso(m_rhs.cod, self.rhs)
+                        if iso:
+                            self.status = RewriteState.VALID
+
+                            for v in m_lhs.dom.vertices():
+                                self.lhs.vertex_data(m_lhs.vmap[v]).highlight = True
+                            for e in m_lhs.dom.edges():
+                                self.lhs.edge_data(m_lhs.emap[e]).highlight = True
+
+                            for v in m_rhs.dom.vertices():
+                                self.rhs.vertex_data(iso.vmap[m_rhs.vmap[v]]).highlight = True
+                            for e in m_rhs.dom.edges():
+                                self.rhs.edge_data(iso.emap[m_rhs.emap[e]]).highlight = True
 
-                    break
+                            break
 
         if self.status != RewriteState.VALID:
             self.status = RewriteState.INVALID
 
 class State:
     def __init__(self) -> None:
         self.graphs: Dict[str, Graph] = dict()
@@ -80,17 +95,17 @@
     def update(self, code: str) -> None:
         parse_data = parse(code)
         self.graphs = parse_data.graphs
         self.rules = parse_data.rules
         self.parts = parse_data.parts
         self.errors = parse_data.errors
 
-        for name, (t_start, t_end, rule, lhs, rhs) in parse_data.rewrites.items():
-            stub = rule == None
-            self.rewrites[name] = RewriteState((t_start, t_end), rule, lhs, rhs, stub)
+        for name, (t_start, t_end, equiv, rule, lhs, rhs, lhs_match, rhs_match) in parse_data.rewrites.items():
+            stub = not (':' in name)
+            self.rewrites[name] = RewriteState((t_start, t_end), equiv, rule, lhs, rhs, lhs_match, rhs_match, stub)
 
     def part_with_index_at(self, pos: int) -> Optional[Tuple[int, Tuple[int,int,str,str]]]:
         p0 = None
         for (i,p) in enumerate(self.parts):
             if p[0] <= pos:
                 p0 = (i,p)
                 if p[1] >= pos:
```

### Comparing `chyp-0.2.2/chyp/term.py` & `chyp-0.3/chyp/term.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2.2/chyp.egg-info/PKG-INFO` & `chyp-0.3/chyp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.2.2
+Version: 0.3
 Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
@@ -143,22 +143,26 @@
 
 start : statement*
 statement : gen | let | rule | rewrite
 gen : "gen" var ":" num "->" num
 let : "let" var "=" term
 rule : "rule" var ":" term "=" term
 rewrite : "rewrite" var ":" term rewrite_part*
-rewrite_part : "=" term_hole "by" rule_ref num?
+rewrite_part : "=" term_hole "by" inverse? rule_ref
+inverse : "-"
 term  : par_term | seq
 par_term : "(" term ")" | par | perm | id | term_ref
 par : par_term "*" par_term
 seq : term ";" term
-perm : "sw" [ "[" num ("," num)* "]" ]
+perm : "sw" ( "[" num ("," num)* "]" )?
 id : "id"
 term_hole : term | "?"
 
 num : INT
 var : IDENTIFIER
 term_ref : IDENTIFIER
 rule_ref : IDENTIFIER
 
 ```
+
+The parser ignores whitespace and comments starting with `#`.
+
```

### Comparing `chyp-0.2.2/chyp.egg-info/SOURCES.txt` & `chyp-0.3/chyp.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 chyp.egg-info/requires.txt
 chyp.egg-info/top_level.txt
 chyp/gui/__init__.py
 chyp/gui/app.py
 chyp/gui/codeview.py
 chyp/gui/document.py
 chyp/gui/editor.py
+chyp/gui/errorlist.py
 chyp/gui/graphscene.py
 chyp/gui/graphview.py
 chyp/gui/highlighter.py
 chyp/gui/mainwindow.py
```

### Comparing `chyp-0.2.2/setup.py` & `chyp-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.2.2",
+    version="0.3",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
     description="An interactive theorem prover for monoidal categories",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
```

