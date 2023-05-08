# Comparing `tmp/harlequin-0.0.4.tar.gz` & `tmp/harlequin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin-0.0.4.tar", max compression
+gzip compressed data, was "harlequin-0.0.5.tar", max compression
```

## Comparing `harlequin-0.0.4.tar` & `harlequin-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-05-05 22:15:17.773850 harlequin-0.0.4/LICENSE
--rw-r--r--   0        0        0      827 2023-05-05 22:15:17.773850 harlequin-0.0.4/README.md
--rw-r--r--   0        0        0     1312 2023-05-05 22:15:17.773850 harlequin-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       53 2023-05-05 22:15:17.773850 harlequin-0.0.4/src/harlequin/__init__.py
--rw-r--r--   0        0        0      336 2023-05-05 22:15:17.773850 harlequin-0.0.4/src/harlequin/cli.py
--rw-r--r--   0        0        0        0 2023-05-05 22:15:17.773850 harlequin-0.0.4/src/harlequin/tui/__init__.py
--rw-r--r--   0        0        0     2647 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/app.css
--rw-r--r--   0        0        0     8429 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/app.py
--rw-r--r--   0        0        0      812 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/__init__.py
--rw-r--r--   0        0        0      881 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/code_editor.py
--rw-r--r--   0        0        0     1081 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/error_modal.py
--rw-r--r--   0        0        0      672 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/filename_modal.py
--rw-r--r--   0        0        0     2430 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/results_viewer.py
--rw-r--r--   0        0        0     3677 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/schema_viewer.py
--rw-r--r--   0        0        0    12090 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/textarea.py
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 harlequin-0.0.4/setup.py
--rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 harlequin-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 22:12:37.510522 harlequin-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1473 2023-05-08 22:12:37.510522 harlequin-0.0.5/README.md
+-rw-r--r--   0        0        0     1428 2023-05-08 22:12:37.518522 harlequin-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/__init__.py
+-rw-r--r--   0        0        0      336 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/cli.py
+-rw-r--r--   0        0        0       53 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/__init__.py
+-rw-r--r--   0        0        0     2647 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/app.css
+-rw-r--r--   0        0        0     8744 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/app.py
+-rw-r--r--   0        0        0      812 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/components/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/components/code_editor.py
+-rw-r--r--   0        0        0     1125 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/components/error_modal.py
+-rw-r--r--   0        0        0      672 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/components/filename_modal.py
+-rw-r--r--   0        0        0     2480 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/components/results_viewer.py
+-rw-r--r--   0        0        0     3001 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/components/schema_viewer.py
+-rw-r--r--   0        0        0    14241 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/components/textarea.py
+-rw-r--r--   0        0        0      661 2023-05-08 22:12:37.518522 harlequin-0.0.5/src/harlequin/tui/utils.py
+-rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 harlequin-0.0.5/setup.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 harlequin-0.0.5/PKG-INFO
```

### Comparing `harlequin-0.0.4/LICENSE` & `harlequin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.4/pyproject.toml` & `harlequin-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 [tool.poetry]
 name = "harlequin"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Text User Interface for DuckDB"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "harlequin", from = "src" },
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = "^0.22.3"
+textual = ">=0.22.3,<0.24.0"
 click = "^8.1.3"
 duckdb = "^0.7.1"
 shandy-sqlfmt = "^0.18.0"
 
 [tool.poetry.group.dev.dependencies]
+pre-commit = "^3.3.1"
 textual = {version="*", extras=["dev"]}
+
+[tool.poetry.group.static.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.264"
 mypy = "^1.2.0"
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
-pre-commit = "^3.3.1"
+pytest-asyncio = "^0.21.0"
 
 [tool.poetry.scripts]
 harlequin = "harlequin.cli:harlequin"
 
 [tool.ruff]
 select = ["E", "F", "I"]
```

### Comparing `harlequin-0.0.4/src/harlequin/tui/app.css` & `harlequin-0.0.5/src/harlequin/tui/app.css`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.4/src/harlequin/tui/app.py` & `harlequin-0.0.5/src/harlequin/tui/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Iterator, Type
+from typing import Iterator, List, Tuple, Type, Union
 
 import duckdb
 from textual import log, work
 from textual.app import App, ComposeResult, CSSPathType
 from textual.containers import Container
 from textual.driver import Driver
 from textual.reactive import reactive
@@ -16,33 +16,34 @@
     CodeEditor,
     ErrorModal,
     ResultsTable,
     ResultsViewer,
     SchemaViewer,
     TextInput,
 )
+from harlequin.tui.utils import short_type
 
 
 class Harlequin(App):
     """
     A Textual App for a SQL client for DuckDB.
     """
 
     CSS_PATH = "app.css"
     MAX_RESULTS = 50_000
 
     query_text: reactive[str] = reactive(str)
-    relation: reactive[duckdb.DuckDBPyRelation | None] = reactive(None)
-    data: reactive[list[tuple]] = reactive(list)
+    relation: reactive[Union[duckdb.DuckDBPyRelation, None]] = reactive(None)
+    data: reactive[List[Tuple]] = reactive(list)
 
     def __init__(
         self,
         db_path: Path,
-        driver_class: Type[Driver] | None = None,
-        css_path: CSSPathType | None = None,
+        driver_class: Union[Type[Driver], None] = None,
+        css_path: Union[CSSPathType, None] = None,
         watch_css: bool = False,
     ):
         self.db_name = db_path.stem
         self.connection = duckdb.connect(database=str(db_path))
         super().__init__(driver_class, css_path, watch_css)
 
     def compose(self) -> ComposeResult:
@@ -97,15 +98,15 @@
                         error=e,
                     )
                 )
             else:
                 editor.move_cursor(0, 0)
                 editor.lines = [f"{line} " for line in query.splitlines()]
 
-    def set_data(self, data: list[tuple]) -> None:
+    def set_data(self, data: List[Tuple]) -> None:
         log(f"set_data {len(data)}")
         self.data = data
 
     async def watch_query_text(self, query_text: str) -> None:
         pane = self.query_one(ResultsViewer)
         pane.show_loading()
         pane.set_not_responsive()
@@ -136,63 +137,69 @@
                 self.data = []
                 self.update_schema_data()
             else:  # blank query
                 pane.set_responsive(did_run=False)
                 pane.show_table()
                 self.data = []
 
-    def watch_relation(self, relation: duckdb.DuckDBPyRelation | None) -> None:
+    def watch_relation(self, relation: Union[duckdb.DuckDBPyRelation, None]) -> None:
         """
         Only runs for select statements, except when first mounted.
         """
         # invalidate results so watch_data runs even if the results are the same
         self.data = []
         if relation is not None:
             table = self.query_one(ResultsViewer).get_table()
-            table.add_columns(*relation.columns)
+            short_types = [short_type(t) for t in relation.dtypes]
+            table.add_columns(
+                *[
+                    f"{name} [#888888]{type}[/]"
+                    for name, type in zip(relation.columns, short_types)
+                ]
+            )
             self.fetch_relation_data(relation)
 
-    async def watch_data(self, data: list[tuple]) -> None:
+    async def watch_data(self, data: List[Tuple]) -> None:
         if data:
             pane = self.query_one(ResultsViewer)
             pane.set_not_responsive(max_rows=self.MAX_RESULTS, total_rows=len(data))
             table = pane.get_table()
             for i, chunk in self.chunk(data[: self.MAX_RESULTS]):
                 worker = self.add_data_to_table(table, chunk)
                 await worker.wait()
                 pane.increment_progress_bar()
                 if i == 0:
                     pane.show_table()
             pane.set_responsive(max_rows=self.MAX_RESULTS, total_rows=len(data))
 
     @staticmethod
     def chunk(
-        data: list[tuple], chunksize: int = 2000
-    ) -> Iterator[tuple[int, list[tuple]]]:
+        data: List[Tuple], chunksize: int = 2000
+    ) -> Iterator[Tuple[int, List[Tuple]]]:
         log(f"chunk {len(data)}")
         for i in range(len(data) // chunksize + 1):
             log(f"yielding chunk {i}")
             yield i, data[i * chunksize : (i + 1) * chunksize]
 
     @work(exclusive=True, exit_on_error=False)  # type: ignore
-    def build_relation(self, query_text: str) -> duckdb.DuckDBPyRelation | None:
+    def build_relation(self, query_text: str) -> Union[duckdb.DuckDBPyRelation, None]:
         relation = self.connection.sql(query_text)
         return relation
 
     @work(exclusive=True)
     def fetch_relation_data(self, relation: duckdb.DuckDBPyRelation) -> None:
         log(f"fetch_relation_data {hash(relation)}")
         data = relation.fetchall()
         log(f"fetch_relation_data FINISHED {hash(relation)}")
         worker = get_current_worker()
         if not worker.is_cancelled:
             self.call_from_thread(self.set_data, data)
 
     @work(exclusive=False)
-    def add_data_to_table(self, table: ResultsTable, data: list[tuple]) -> Worker:
+    def add_data_to_table(self, table: ResultsTable, data: List[Tuple]) -> Worker:
         log(f"add_data_to_table {len(data)}")
         worker = get_current_worker()
         if not worker.is_cancelled:
             self.call_from_thread(table.add_rows, data)
         return worker
 
     @work(exclusive=True)
```

### Comparing `harlequin-0.0.4/src/harlequin/tui/components/__init__.py` & `harlequin-0.0.5/src/harlequin/tui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.4/src/harlequin/tui/components/code_editor.py` & `harlequin-0.0.5/src/harlequin/tui/components/code_editor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List, Tuple
+
 from textual.binding import Binding
 from textual.message import Message
 
 from harlequin.tui.components.textarea import TextArea, TextInput
 
 
 class CodeEditor(TextArea):
@@ -14,15 +16,15 @@
         """Posted when user runs the query.
 
         Attributes:
             lines: The lines of code being submitted.
             cursor: The position of the cursor
         """
 
-        def __init__(self, lines: list[str], cursor: tuple[int, int]) -> None:
+        def __init__(self, lines: List[str], cursor: Tuple[int, int]) -> None:
             super().__init__()
-            self.lines: list[str] = lines
-            self.cursor: tuple[int, int] = cursor
+            self.lines: List[str] = lines
+            self.cursor: Tuple[int, int] = cursor
 
     async def action_submit(self) -> None:
         input = self.query_one(TextInput)
         self.post_message(self.Submitted(input.lines, input.cursor))
```

### Comparing `harlequin-0.0.4/src/harlequin/tui/components/error_modal.py` & `harlequin-0.0.5/src/harlequin/tui/components/error_modal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import Union
+
 from textual.app import ComposeResult
 from textual.containers import Vertical, VerticalScroll
 from textual.screen import ModalScreen
 from textual.widgets import Static
 
 
 class ErrorModal(ModalScreen):
     def __init__(
         self,
         title: str,
         header: str,
         error: BaseException,
-        name: str | None = None,
-        id: str | None = None,
-        classes: str | None = None,
+        name: Union[str, None] = None,
+        id: Union[str, None] = None,
+        classes: Union[str, None] = None,
     ) -> None:
         self.title = title
         self.header = header
         self.error = error
         super().__init__(name, id, classes)
 
     def compose(self) -> ComposeResult:
```

### Comparing `harlequin-0.0.4/src/harlequin/tui/components/filename_modal.py` & `harlequin-0.0.5/src/harlequin/tui/components/filename_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.4/src/harlequin/tui/components/results_viewer.py` & `harlequin-0.0.5/src/harlequin/tui/components/results_viewer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 from textual.app import ComposeResult
 from textual.widgets import ContentSwitcher, DataTable, LoadingIndicator
 
 
 class ResultsTable(DataTable):
     DEFAULT_CSS = """
         ResultsTable {
@@ -20,15 +22,15 @@
         yield LoadingIndicator(id=self.LOADING_ID)
 
     def on_mount(self) -> None:
         self.border_title = "Query Results"
         self.current = self.TABLE_ID
 
     def set_not_responsive(
-        self, max_rows: int | None = None, total_rows: int | None = None
+        self, max_rows: Union[int, None] = None, total_rows: Union[int, None] = None
     ) -> None:
         if (total_rows and not max_rows) or (
             total_rows and max_rows and total_rows <= max_rows
         ):
             self.border_title = f"LOADING {total_rows:,} Records."
         elif total_rows and max_rows:
             self.border_title = f"LOADING {max_rows:,} of {total_rows:,} Records."
@@ -37,16 +39,16 @@
         self.add_class("non-responsive")
 
     def increment_progress_bar(self) -> None:
         self.border_title = f"{self.border_title}."
 
     def set_responsive(
         self,
-        max_rows: int | None = None,
-        total_rows: int | None = None,
+        max_rows: Union[int, None] = None,
+        total_rows: Union[int, None] = None,
         did_run: bool = True,
     ) -> None:
         if (total_rows and not max_rows) or (
             total_rows and max_rows and total_rows <= max_rows
         ):
             self.border_title = f"Query Results ({total_rows:,} Records)"
         elif total_rows and max_rows:
```

### Comparing `harlequin-0.0.4/src/harlequin/tui/components/schema_viewer.py` & `harlequin-0.0.5/src/harlequin/tui/components/schema_viewer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,50 @@
+from typing import List, Set, Tuple, Union
+
 from duckdb import DuckDBPyConnection
 from rich.text import TextType
 from textual.widgets import Tree
 from textual.widgets.tree import TreeNode
 
-COLS = list[tuple[str, str]]
-TABLES = list[tuple[str, str, COLS]]
-SCHEMAS = list[tuple[str, TABLES]]
+from harlequin.tui.utils import short_type
+
+COLS = List[Tuple[str, str]]
+TABLES = List[Tuple[str, str, COLS]]
+SCHEMAS = List[Tuple[str, TABLES]]
 
 
-class SchemaViewer(Tree[str | None]):
+class SchemaViewer(Tree[Union[str, None]]):
     table_type_mapping = {
         "BASE TABLE": "t",
         "LOCAL TEMPORARY": "tmp",
         "VIEW": "v",
     }
-    column_type_mapping = {
-        "BIGINT": "##",
-        "BIT": "010",
-        "BOOLEAN": "t/f",
-        "BLOB": "0b",
-        "DATE": "d",
-        "DOUBLE": "#.#",
-        "DECIMAL": "#.#",
-        "HUGEINT": "###",
-        "INTEGER": "#",
-        "INTERVAL": "|-|",
-        "REAL": "#.#",
-        "SMALLINT": "#",
-        "TIME": "t",
-        "TIMESTAMP": "ts",
-        "TIMESTAMP WITH TIME ZONE": "ttz",
-        "TINYINT": "#",
-        "UBIGINT": "u##",
-        "UINTEGER": "u#",
-        "USMALLINT": "u#",
-        "UTINYINT": "u#",
-        "UUID": "uid",
-        "VARCHAR": "s",
-        "LIST": "[]",
-        "STRUCT": "{}",
-        "MAP": "{}",
-    }
 
     def __init__(
         self,
         label: TextType,
         connection: DuckDBPyConnection,
-        data: str | None = None,
-        name: str | None = None,
-        id: str | None = None,
-        classes: str | None = None,
+        data: Union[str, None] = None,
+        name: Union[str, None] = None,
+        id: Union[str, None] = None,
+        classes: Union[str, None] = None,
         disabled: bool = False,
     ) -> None:
         self.connection = connection
         super().__init__(
             label, data, name=name, id=id, classes=classes, disabled=disabled
         )
 
     def on_mount(self) -> None:
         self.border_title = "Schema"
         self.root.expand()
 
     def update_tree(self, data: SCHEMAS) -> None:
         tree_state = self.get_node_states(self.root)
-        expanded_nodes: set[str] = set(tree_state[0])
+        expanded_nodes: Set[str] = set(tree_state[0])
         # todo: tree's select_node() not working
         # unless the tree is modified, the selection will stay
         # in the same place
         # selected_node = tree_state[1]
         self.clear()
         if data:
             for schema in data:
@@ -80,26 +57,23 @@
                     table_node = schema_node.add(
                         f"{table[0]} [#888888]{short_table_type}[/]",
                         data=table_identifier,
                         expand=(table_identifier in expanded_nodes),
                     )
                     for col in table[2]:
                         col_identifier = f"{table_identifier}.{col[0]}"
-                        short_col_type = self.column_type_mapping.get(
-                            col[1].split("(")[0], "?"
-                        )
                         table_node.add_leaf(
-                            f"{col[0]} [#888888]{short_col_type}[/]",
+                            f"{col[0]} [#888888]{short_type(col[1])}[/]",
                             data=col_identifier,
                         )
 
     @classmethod
     def get_node_states(
-        cls, node: TreeNode[str | None]
-    ) -> tuple[list[str], str | None]:
+        cls, node: TreeNode[Union[str, None]]
+    ) -> Tuple[List[str], Union[str, None]]:
         expanded_nodes = []
         selected_node = None
         if node.is_expanded and node.data is not None:
             expanded_nodes.append(node.data)
         if node._selected and node.data is not None:
             selected_node = node.data
         for child in node.children:
```

### Comparing `harlequin-0.0.4/src/harlequin/tui/components/textarea.py` & `harlequin-0.0.5/src/harlequin/tui/components/textarea.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import NamedTuple
+import re
+from typing import List, NamedTuple, Union
 
 from rich.console import RenderableType
 from rich.syntax import Syntax
 from sqlfmt.api import Mode, format_string
 from sqlfmt.exception import SqlfmtError
 from textual import events
 from textual.app import ComposeResult
@@ -12,14 +13,16 @@
 from textual.reactive import reactive
 from textual.widget import Widget
 from textual.widgets import Static
 
 from harlequin.tui.components.error_modal import ErrorModal
 from harlequin.tui.components.filename_modal import FilenameModal
 
+WWB = re.compile(r"\W*\w+\b")
+
 
 class Cursor(NamedTuple):
     lno: int
     pos: int
 
 
 class TextInput(Static, can_focus=True):
@@ -34,15 +37,15 @@
     TextInput{
         height: auto;
         width: auto;
         padding: 0 1;
     }
     """
 
-    lines: reactive[list[str]] = reactive(lambda: list(" "))
+    lines: reactive[List[str]] = reactive(lambda: list(" "))
     cursor: reactive[Cursor] = reactive(Cursor(0, 0))
     cursor_visible: reactive[bool] = reactive(True)
 
     class CursorMoved(Message, bubble=True):
         """Posted when the cursor moves
 
         Attributes:
@@ -116,17 +119,64 @@
                 self.cursor = Cursor(0, 0)
             else:
                 max_x = len(self.lines[self.cursor.lno - 1]) - 1
                 self.cursor = Cursor(
                     lno=self.cursor.lno - 1, pos=min(max_x, self.cursor.pos)
                 )
         elif event.key == "home":
+            event.stop()
             self.cursor = Cursor(self.cursor.lno, 0)
         elif event.key == "end":
+            event.stop()
             self.cursor = Cursor(self.cursor.lno, len(self.lines[self.cursor.lno]) - 1)
+        elif event.key == "pageup":
+            event.stop()
+            self.move_cursor(
+                x=self.cursor.pos, y=(self.cursor.lno - self._visible_height() + 1)
+            )
+        elif event.key == "pagedown":
+            event.stop()
+            self.move_cursor(
+                x=self.cursor.pos, y=(self.cursor.lno + self._visible_height() - 1)
+            )
+        elif event.key == "ctrl+right":
+            event.stop()
+            max_x = len(self.lines[self.cursor.lno]) - 1
+            max_y = len(self.lines) - 1
+            if self.cursor.pos == max_x and self.cursor.lno == max_y:
+                return
+            elif self.cursor.pos == max_x:
+                lno = self.cursor.lno + 1
+                pos = 0
+            else:
+                lno = self.cursor.lno
+                pos = self.cursor.pos
+
+            tail = self.lines[lno][pos:]
+            if match := WWB.match(tail):
+                self.cursor = Cursor(lno=lno, pos=pos + match.span()[1])
+            else:  # no more words, move to end of line
+                self.cursor = Cursor(lno=lno, pos=len(self.lines[lno]) - 1)
+        elif event.key == "ctrl+left":
+            event.stop()
+            if self.cursor.pos == 0 and self.cursor.lno == 0:
+                return
+            elif self.cursor.pos == 0:
+                lno = self.cursor.lno - 1
+                pos = len(self.lines[lno]) - 1
+            else:
+                lno = self.cursor.lno
+                pos = self.cursor.pos
+
+            tail = self.lines[lno][pos::-1]
+            self.log(f"lno: {lno}, pos: {pos}, tail: {tail}")
+            if match := WWB.match(tail):
+                self.cursor = Cursor(lno=lno, pos=pos - match.span()[1] + 1)
+            else:  # no more words, move to start of line
+                self.cursor = Cursor(lno=lno, pos=0)
         elif event.key == "ctrl+home":
             self.cursor = Cursor(0, 0)
         elif event.key == "ctrl+end":
             self.cursor = Cursor(lno=len(self.lines) - 1, pos=len(self.lines[-1]) - 1)
         elif event.key == "enter":
             event.stop()
             old_line = self.lines[self.cursor.lno]
@@ -197,14 +247,19 @@
                 (self.cursor.lno + 1, self.cursor.pos + 1),
             )
         return syntax
 
     def _scroll_to_cursor(self) -> None:
         self.post_message(self.CursorMoved(self.cursor.pos, self.cursor.lno))
 
+    def _visible_height(self) -> int:
+        parent = self.parent
+        assert isinstance(parent, TextContainer)
+        return parent.window_region.height
+
     def _toggle_cursor(self) -> None:
         self.cursor_visible = not self.cursor_visible
         self.update(self._content)
 
     def _insert_character_at_cursor(self, character: str) -> None:
         line = self.lines[self.cursor.lno]
         new_line = f"{line[:self.cursor.pos]}{character}{line[self.cursor.pos:]}"
@@ -231,15 +286,15 @@
             ):
                 self._insert_character_at_cursor(closers[character])
                 self.cursor = Cursor(self.cursor.lno, self.cursor.pos - 1)
 
     def _get_character_at_cursor(self) -> str:
         return self.lines[self.cursor.lno][self.cursor.pos]
 
-    def _get_character_before_cursor(self) -> str | None:
+    def _get_character_before_cursor(self) -> Union[str, None]:
         if self.cursor.pos == 0:
             return None
         else:
             return self.lines[self.cursor.lno][self.cursor.pos - 1]
 
     def action_format(self) -> None:
         code = "\n".join(self.lines)
@@ -264,15 +319,16 @@
     def action_load(self) -> None:
         self.app.push_screen(FilenameModal(id="load_modal"))
 
     def move_cursor(self, x: int, y: int) -> None:
         max_y = len(self.lines) - 1
         safe_y = min(max_y, y)
         max_x = len(self.lines[safe_y]) - 1
-        self.cursor = Cursor(safe_y, min(max_x, x))
+        safe_x = min(max_x, x)
+        self.cursor = Cursor(lno=max(0, safe_y), pos=max(0, safe_x))
         self.update(self._content)
 
 
 class TextContainer(
     ScrollableContainer,
     inherit_bindings=False,
     can_focus=False,
```

### Comparing `harlequin-0.0.4/setup.py` & `harlequin-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'duckdb>=0.7.1,<0.8.0',
  'shandy-sqlfmt>=0.18.0,<0.19.0',
- 'textual>=0.22.3,<0.23.0']
+ 'textual>=0.22.3,<0.24.0']
 
 entry_points = \
 {'console_scripts': ['harlequin = harlequin.cli:harlequin']}
 
 setup_kwargs = {
     'name': 'harlequin',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'A Text User Interface for DuckDB',
-    'long_description': '# harlequin\nA Text User Interface for DuckDB.\n\n(A Harlequin is a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)\n\n![harlequin](harlequin.jpg)\n\n## Installing Harlequin\n\nUse `pip` or `pipx`:\n\n```bash\npipx install harlequin\n```\n\n## Using Harlequin\n\nTo open a DuckDB database file:\n\n```bash\nharlequin "path/to/duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\nWhen Harlequin is open, you can view the schema of your DuckDB database in the left sidebar.\n\nTo run a query, enter your code in the main text input, then press Ctrl+Enter. You should see the data appear in the pane below.\n\nYou can press Tab or use your mouse to change the focus between the panes.\n\nWhen the focus is on the data pane, you can use your arrow keys or mouse to select different cells.',
+    'long_description': '# harlequin\nA Terminal-based SQL IDE for DuckDB.\n\n![harlequin TUI](harlequinv004.gif)\n\n(A Harlequin is also a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)\n\n![harlequin duck](harlequin.jpg)\n\n## Installing Harlequin\n\nUse `pip` or `pipx`:\n\n```bash\npipx install harlequin\n```\n\n> **Tip:**\n>\n> You can run invoke directly with [`pipx run`](https://pypa.github.io/pipx/examples/#pipx-run-examples) anywhere that `pipx` is installed. For example:\n> - `pipx run harlequin --help`\n> - `pipx run harlequin ./my.duckdb`\n\n## Using Harlequin\n\nTo open a DuckDB database file:\n\n```bash\nharlequin "path/to/duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\nWhen Harlequin is open, you can view the schema of your DuckDB database in the left sidebar.\n\nTo run a query, enter your code in the main textarea, then press Ctrl+Enter. You should see the data appear in the pane below.\n\nYou can press Tab or use your mouse to change the focus between the panes.\n\nWhen the focus is on the data pane, you can use your arrow keys or mouse to select different cells.\n\nPress Ctrl+c to quit and return to your shell.\n\n### Running Harlequin in a Container\n\nWithout a database file:\n\n```bash\ndocker run ghcr.io/tconbeer/harlequin:latest\n```\n\nMounting a database file `./foo.db` into the container\'s working directory, `/data`:\n\n```bash\ndocker run -v $(pwd)/foo.db:/data/bar.db ghcr.io/tconbeer/harlequin:latest harlequin bar.db\n```\n',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `harlequin-0.0.4/PKG-INFO` & `harlequin-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 Metadata-Version: 2.1
 Name: harlequin
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Text User Interface for DuckDB
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: duckdb (>=0.7.1,<0.8.0)
 Requires-Dist: shandy-sqlfmt (>=0.18.0,<0.19.0)
-Requires-Dist: textual (>=0.22.3,<0.23.0)
+Requires-Dist: textual (>=0.22.3,<0.24.0)
 Description-Content-Type: text/markdown
 
 # harlequin
-A Text User Interface for DuckDB.
+A Terminal-based SQL IDE for DuckDB.
 
-(A Harlequin is a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)
+![harlequin TUI](harlequinv004.gif)
 
-![harlequin](harlequin.jpg)
+(A Harlequin is also a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)
+
+![harlequin duck](harlequin.jpg)
 
 ## Installing Harlequin
 
 Use `pip` or `pipx`:
 
 ```bash
 pipx install harlequin
 ```
 
+> **Tip:**
+>
+> You can run invoke directly with [`pipx run`](https://pypa.github.io/pipx/examples/#pipx-run-examples) anywhere that `pipx` is installed. For example:
+> - `pipx run harlequin --help`
+> - `pipx run harlequin ./my.duckdb`
+
 ## Using Harlequin
 
 To open a DuckDB database file:
 
 ```bash
 harlequin "path/to/duck.db"
 ```
@@ -45,12 +53,29 @@
 
 ```bash
 harlequin
 ```
 
 When Harlequin is open, you can view the schema of your DuckDB database in the left sidebar.
 
-To run a query, enter your code in the main text input, then press Ctrl+Enter. You should see the data appear in the pane below.
+To run a query, enter your code in the main textarea, then press Ctrl+Enter. You should see the data appear in the pane below.
 
 You can press Tab or use your mouse to change the focus between the panes.
 
 When the focus is on the data pane, you can use your arrow keys or mouse to select different cells.
+
+Press Ctrl+c to quit and return to your shell.
+
+### Running Harlequin in a Container
+
+Without a database file:
+
+```bash
+docker run ghcr.io/tconbeer/harlequin:latest
+```
+
+Mounting a database file `./foo.db` into the container's working directory, `/data`:
+
+```bash
+docker run -v $(pwd)/foo.db:/data/bar.db ghcr.io/tconbeer/harlequin:latest harlequin bar.db
+```
+
```

