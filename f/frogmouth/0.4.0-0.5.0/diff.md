# Comparing `tmp/frogmouth-0.4.0.tar.gz` & `tmp/frogmouth-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogmouth-0.4.0.tar", max compression
+gzip compressed data, was "frogmouth-0.5.0.tar", max compression
```

## Comparing `frogmouth-0.4.0.tar` & `frogmouth-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.4.0/LICENSE
--rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.4.0/README.md
--rw-r--r--   0        0        0      283 2023-05-03 09:31:33.035349 frogmouth-0.4.0/frogmouth/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.4.0/frogmouth/__main__.py
--rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.4.0/frogmouth/app/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.4.0/frogmouth/app/app.py
--rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.4.0/frogmouth/data/__init__.py
--rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.4.0/frogmouth/data/bookmarks.py
--rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.4.0/frogmouth/data/config.py
--rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.4.0/frogmouth/data/data_directory.py
--rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.4.0/frogmouth/data/history.py
--rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.4.0/frogmouth/dialogs/__init__.py
--rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.4.0/frogmouth/dialogs/error.py
--rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.4.0/frogmouth/dialogs/help_dialog.py
--rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.4.0/frogmouth/dialogs/information.py
--rw-r--r--   0        0        0     2717 2023-05-03 09:31:33.036023 frogmouth-0.4.0/frogmouth/dialogs/input_dialog.py
--rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.4.0/frogmouth/dialogs/text_dialog.py
--rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.4.0/frogmouth/dialogs/yes_no_dialog.py
--rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.4.0/frogmouth/screens/__init__.py
--rw-r--r--   0        0        0    18746 2023-05-03 09:31:33.036343 frogmouth-0.4.0/frogmouth/screens/main.py
--rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.4.0/frogmouth/utility/__init__.py
--rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.4.0/frogmouth/utility/advertising.py
--rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.4.0/frogmouth/utility/forge.py
--rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.4.0/frogmouth/utility/type_tests.py
--rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.4.0/frogmouth/widgets/__init__.py
--rw-r--r--   0        0        0     4398 2023-05-03 09:31:33.037070 frogmouth-0.4.0/frogmouth/widgets/navigation.py
--rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/__init__.py
--rw-r--r--   0        0        0     5633 2023-05-03 09:31:33.037203 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/bookmarks.py
--rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/history.py
--rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/local_files.py
--rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/navigation_pane.py
--rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/table_of_contents.py
--rw-r--r--   0        0        0    11675 2023-05-03 09:31:33.038042 frogmouth-0.4.0/frogmouth/widgets/omnibox.py
--rw-r--r--   0        0        0    10129 2023-05-01 07:06:00.079325 frogmouth-0.4.0/frogmouth/widgets/viewer.py
--rw-r--r--   0        0        0     1468 2023-05-03 09:31:33.038167 frogmouth-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 frogmouth-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.5.0/README.md
+-rw-r--r--   0        0        0      283 2023-05-09 08:04:58.867459 frogmouth-0.5.0/frogmouth/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.5.0/frogmouth/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.5.0/frogmouth/app/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.5.0/frogmouth/app/app.py
+-rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.5.0/frogmouth/data/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.5.0/frogmouth/data/bookmarks.py
+-rw-r--r--   0        0        0     2270 2023-05-09 08:04:58.867587 frogmouth-0.5.0/frogmouth/data/config.py
+-rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.5.0/frogmouth/data/data_directory.py
+-rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.5.0/frogmouth/data/history.py
+-rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.5.0/frogmouth/dialogs/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.5.0/frogmouth/dialogs/error.py
+-rw-r--r--   0        0        0     4539 2023-05-09 08:04:58.868315 frogmouth-0.5.0/frogmouth/dialogs/help_dialog.py
+-rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.5.0/frogmouth/dialogs/information.py
+-rw-r--r--   0        0        0     2544 2023-05-09 08:04:58.868437 frogmouth-0.5.0/frogmouth/dialogs/input_dialog.py
+-rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.5.0/frogmouth/dialogs/text_dialog.py
+-rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.5.0/frogmouth/dialogs/yes_no_dialog.py
+-rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.5.0/frogmouth/screens/__init__.py
+-rw-r--r--   0        0        0    18617 2023-05-09 08:04:58.868627 frogmouth-0.5.0/frogmouth/screens/main.py
+-rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.5.0/frogmouth/utility/__init__.py
+-rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.5.0/frogmouth/utility/advertising.py
+-rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.5.0/frogmouth/utility/forge.py
+-rw-r--r--   0        0        0     1206 2023-05-09 08:04:58.868785 frogmouth-0.5.0/frogmouth/utility/type_tests.py
+-rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.5.0/frogmouth/widgets/__init__.py
+-rw-r--r--   0        0        0     6015 2023-05-09 08:04:58.868929 frogmouth-0.5.0/frogmouth/widgets/navigation.py
+-rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/__init__.py
+-rw-r--r--   0        0        0     5633 2023-05-03 09:31:33.037203 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/bookmarks.py
+-rw-r--r--   0        0        0     5685 2023-05-09 08:04:58.869061 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/history.py
+-rw-r--r--   0        0        0     3071 2023-05-09 08:04:58.869180 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/local_files.py
+-rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/navigation_pane.py
+-rw-r--r--   0        0        0     2341 2023-05-09 08:04:58.869286 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/table_of_contents.py
+-rw-r--r--   0        0        0    11931 2023-05-09 08:04:58.869453 frogmouth-0.5.0/frogmouth/widgets/omnibox.py
+-rw-r--r--   0        0        0    10750 2023-05-09 08:04:58.872361 frogmouth-0.5.0/frogmouth/widgets/viewer.py
+-rw-r--r--   0        0        0     1468 2023-05-09 08:04:58.873191 frogmouth-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 frogmouth-0.5.0/PKG-INFO
```

### Comparing `frogmouth-0.4.0/LICENSE` & `frogmouth-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/README.md` & `frogmouth-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/app/app.py` & `frogmouth-0.5.0/frogmouth/app/app.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/data/bookmarks.py` & `frogmouth-0.5.0/frogmouth/data/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/data/config.py` & `frogmouth-0.5.0/frogmouth/data/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
     light_mode: bool = False
     """Should we run in light mode?"""
 
     markdown_extensions: list[str] = field(default_factory=lambda: [".md", ".markdown"])
     """What Markdown extensions will we look for?"""
 
+    navigation_left: bool = True
+    """Should navigation be docked to the left side of the screen?"""
+
 
 def config_file() -> Path:
     """Get the path to the configuration file.
 
     Returns:
         The path to the configuration file.
```

### Comparing `frogmouth-0.4.0/frogmouth/data/data_directory.py` & `frogmouth-0.5.0/frogmouth/data/data_directory.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/data/history.py` & `frogmouth-0.5.0/frogmouth/data/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/dialogs/error.py` & `frogmouth-0.5.0/frogmouth/dialogs/error.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/dialogs/help_dialog.py` & `frogmouth-0.5.0/frogmouth/dialogs/help_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 Press `/` or click the address bar, then enter any of the following commands:
 
 | Command | Aliases | Arguments | Command |
 | -- | -- | -- | -- |
 | `about` | `a` | | Show details about the application |
 | `bookmarks` | `b`, `bm` | | Show the bookmarks list |
 | `bitbucket` | `bb` | `<repo-info>` | View a file on BitBucket (see below) |
+| `changelog` | `cl` | | View the Frogmouth ChangeLog |
 | `chdir` | `cd` | `<dir>` | Switch the local file browser to a new directory |
 | `contents` | `c`, `toc` | | Show the table of contents for the document |
 | `discord` | | | Visit the Textualize Discord server |
 | `github` | `gh` | `<repo-info>` | View a file on GitHub (see below) |
 | `gitlab` | `gl` | `<repo-info>` | View a file on GitLab (see below) |
 | `help` | `?` | | Show this document |
 | `history` | `h` | | Show the history |
```

### Comparing `frogmouth-0.4.0/frogmouth/dialogs/input_dialog.py` & `frogmouth-0.5.0/frogmouth/dialogs/input_dialog.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Provides a modal dialog for getting a value from the user."""
 
 from __future__ import annotations
 
+from textual import on
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Horizontal, Vertical
 from textual.screen import ModalScreen
 from textual.widgets import Button, Input, Label
 
 
@@ -78,21 +79,18 @@
                 yield Button("OK", id="ok", variant="primary")
                 yield Button("Cancel", id="cancel")
 
     def on_mount(self) -> None:
         """Set up the dialog once the DOM is ready."""
         self.query_one(Input).focus()
 
-    def on_button_pressed(self, event: Button.Pressed) -> None:
-        """Handle one of the dialog's buttons been pressed.
-
-        Args:
-            event: The button press event.
-        """
-        if event.button.id == "cancel":
-            self.app.pop_screen()
-        elif event.button.id == "ok" and self.query_one(Input).value.strip():
-            self.dismiss(self.query_one(Input).value)
-
-    def on_input_submitted(self) -> None:
-        """Do default processing when the user hits enter in the input."""
-        self.query_one("#ok", Button).press()
+    @on(Button.Pressed, "#cancel")
+    def cancel_input(self) -> None:
+        """Cancel the input operation."""
+        self.app.pop_screen()
+
+    @on(Input.Submitted)
+    @on(Button.Pressed, "#ok")
+    def accept_input(self) -> None:
+        """Accept and return the input."""
+        if value := self.query_one(Input).value.strip():
+            self.dismiss(value)
```

### Comparing `frogmouth-0.4.0/frogmouth/dialogs/text_dialog.py` & `frogmouth-0.5.0/frogmouth/dialogs/text_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/dialogs/yes_no_dialog.py` & `frogmouth-0.5.0/frogmouth/dialogs/yes_no_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/screens/main.py` & `frogmouth-0.5.0/frogmouth/screens/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,58 +37,41 @@
 from ..widgets.navigation_panes import Bookmarks, History, LocalFiles
 
 
 class Main(Screen[None]):  # pylint:disable=too-many-public-methods
     """The main screen for the application."""
 
     DEFAULT_CSS = """
-
     .focusable {
-        border-top: blank;
-        border-right: blank;
-        border-bottom: blank;
-        border-left: blank;
+        border: blank;
     }
 
     .focusable:focus {
-        border-top: heavy $accent !important;
-        border-right: heavy $accent !important;
-        border-bottom: heavy $accent !important;
-        border-left: heavy $accent !important;
+        border: heavy $accent !important;
     }
 
 
     Screen Tabs {
         border: blank;
         height: 5;
     }
 
     Screen Tabs:focus {
-        border-top: heavy $accent !important;
-        border-right: heavy $accent !important;
-        border-bottom: heavy $accent !important;
-        border-left: heavy $accent !important;
+        border: heavy $accent !important;
         height: 5;
     }
 
     Screen TabbedContent TabPane {
         padding: 0 1;
-        border-top: blank;
-        border-right: blank;
-        border-bottom: blank;
-        border-left: blank;
+        border: blank;
     }
 
     Screen TabbedContent TabPane:focus-within {
-        border-top: heavy $accent !important;
-        border-right: heavy $accent !important;
-        border-bottom: heavy $accent !important;
-        border-left: heavy $accent !important;
+        border: heavy $accent !important;
     }
-
     """
 
     BINDINGS = [
         Binding("/,:", "omnibox", "Omnibox", show=False),
         Binding("ctrl+b", "bookmarks", "", show=False),
         Binding("ctrl+d", "bookmark_this", "", show=False),
         Binding("ctrl+l", "local_files", "", show=False),
@@ -183,14 +166,18 @@
             self.query_one(Omnibox).value = str(history[-1])
         elif self._initial_location is not None:
             # Seems there is an initial location; so let's start up looking
             # at that.
             (omnibox := self.query_one(Omnibox)).value = self._initial_location
             await omnibox.action_submit()
 
+    def on_navigation_hidden(self) -> None:
+        """React to the navigation sidebar being hidden."""
+        self.query_one(Viewer).focus()
+
     def on_omnibox_local_view_command(self, event: Omnibox.LocalViewCommand) -> None:
         """Handle the omnibox asking us to view a particular file.
 
         Args:
             event: The local view command event.
         """
         self.visit(event.path)
@@ -203,40 +190,38 @@
         """
         self.visit(event.url)
 
     def on_omnibox_contents_command(self) -> None:
         """Handle being asked to show the table of contents."""
         self.action_table_of_contents()
 
-    async def on_omnibox_local_files_command(self) -> None:
+    def on_omnibox_local_files_command(self) -> None:
         """Handle being asked to view the local files picker."""
-        await self.action_local_files()
+        self.action_local_files()
 
     def on_omnibox_bookmarks_command(self) -> None:
         """Handle being asked to view the bookmarks."""
         self.action_bookmarks()
 
-    async def on_omnibox_local_chdir_command(
-        self, event: Omnibox.LocalChdirCommand
-    ) -> None:
+    def on_omnibox_local_chdir_command(self, event: Omnibox.LocalChdirCommand) -> None:
         """Handle being asked to view a new directory in the local files picker.
 
         Args:
             event: The chdir command event to handle.
         """
         if not event.target.exists():
             self.app.push_screen(
                 ErrorDialog("No such directory", f"{event.target} does not exist.")
             )
         elif not event.target.is_dir():
             self.app.push_screen(
                 ErrorDialog("Not a directory", f"{event.target} is not a directory.")
             )
         else:
-            await self.query_one(Navigation).jump_to_local_files(event.target)
+            self.query_one(Navigation).jump_to_local_files(event.target)
 
     def on_omnibox_history_command(self) -> None:
         """Handle being asked to view the history."""
         self.action_history()
 
     async def _from_forge(
         self,
@@ -316,14 +301,26 @@
         Args:
             event: The event to handle.
         """
         self.visit(
             event.location, remember=event.location != self.query_one(Viewer).location
         )
 
+    def on_history_delete(self, event: History.Delete) -> None:
+        """Handle a request to delete an item from history.
+
+        Args:
+            event: The event to handle.
+        """
+        self.query_one(Viewer).delete_history(event.history_id)
+
+    def on_history_clear(self) -> None:
+        """handle a request to clear down all of history."""
+        self.query_one(Viewer).clear_history()
+
     def on_bookmarks_goto(self, event: Bookmarks.Goto) -> None:
         """Handle a request to go to a bookmark.
 
         Args:
             event: The event to handle.
         """
         self.visit(event.bookmark.location)
@@ -432,17 +429,17 @@
         """Jump to the omnibox."""
         self.query_one(Omnibox).focus()
 
     def action_table_of_contents(self) -> None:
         """Display and focus the table of contents pane."""
         self.query_one(Navigation).jump_to_contents()
 
-    async def action_local_files(self) -> None:
+    def action_local_files(self) -> None:
         """Display and focus the local files selection pane."""
-        await self.query_one(Navigation).jump_to_local_files()
+        self.query_one(Navigation).jump_to_local_files()
 
     def action_bookmarks(self) -> None:
         """Display and focus the bookmarks selection pane."""
         self.query_one(Navigation).jump_to_bookmarks()
 
     def action_history(self) -> None:
         """Display and focus the history pane."""
```

### Comparing `frogmouth-0.4.0/frogmouth/utility/advertising.py` & `frogmouth-0.5.0/frogmouth/utility/advertising.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/utility/forge.py` & `frogmouth-0.5.0/frogmouth/utility/forge.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/utility/type_tests.py` & `frogmouth-0.5.0/frogmouth/utility/type_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     return maybe_markdown(resource.path)
 
 
 def is_likely_url(candidate: str) -> bool:
     """Does the given value look something like a URL?
 
     Args:
-        candiate: The candidate to check.
+        candidate: The candidate to check.
 
     Returns:
         `True` if the string is likely a URL, `False` if not.
     """
     # Quick and dirty for now.
     url = URL(candidate)
     return url.is_absolute_url and url.scheme in ("http", "https")
```

### Comparing `frogmouth-0.4.0/frogmouth/widgets/navigation.py` & `frogmouth-0.5.0/frogmouth/widgets/navigation.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Vertical
+from textual.message import Message
 from textual.reactive import var
 from textual.widgets import TabbedContent, Tabs
 from typing_extensions import Self
 
+from ..data import load_config, save_config
 from .navigation_panes.bookmarks import Bookmarks
 from .navigation_panes.history import History
 from .navigation_panes.local_files import LocalFiles
 from .navigation_panes.navigation_pane import NavigationPane
 from .navigation_panes.table_of_contents import TableOfContents
 
 
@@ -41,20 +43,24 @@
         height: 1fr !important;
     }
     """
 
     BINDINGS = [
         Binding("comma,a,ctrl+left,shift+left,h", "previous_tab", "", show=False),
         Binding("full_stop,d,ctrl+right,shift+right,l", "next_tab", "", show=False),
+        Binding("\\", "toggle_dock", "Dock left/right"),
     ]
     """Bindings local to the navigation pane."""
 
     popped_out: var[bool] = var(False)
     """Is the navigation popped out?"""
 
+    docked_left: var[bool] = var(True)
+    """Should navigation be docked to the left side of the screen?"""
+
     def compose(self) -> ComposeResult:
         """Compose the content of the navigation pane."""
         self.popped_out = False
         # pylint:disable=attribute-defined-outside-init
         self._contents = TableOfContents()
         self._local_files = LocalFiles()
         self._bookmarks = Bookmarks()
@@ -62,22 +68,35 @@
         with TabbedContent() as tabs:
             self._tabs = tabs
             yield self._contents
             yield self._local_files
             yield self._bookmarks
             yield self._history
 
+    def on_mount(self) -> None:
+        """Configure navigation once the DOM is set up."""
+        self.docked_left = load_config().navigation_left
+
+    class Hidden(Message):
+        """Message sent when the navigation is hidden."""
+
     def watch_popped_out(self) -> None:
         """Watch for changes to the popped out state."""
         self.set_class(not self.popped_out, "hidden")
+        if not self.popped_out:
+            self.post_message(self.Hidden())
 
     def toggle(self) -> None:
         """Toggle the popped/unpopped state."""
         self.popped_out = not self.popped_out
 
+    def watch_docked_left(self) -> None:
+        """Watch for changes to the left-docking status."""
+        self.styles.dock = "left" if self.docked_left else "right"
+
     @property
     def table_of_contents(self) -> TableOfContents:
         """The table of contents widget."""
         return self._contents
 
     @property
     def local_files(self) -> LocalFiles:
@@ -90,65 +109,88 @@
         return self._bookmarks
 
     @property
     def history(self) -> History:
         """The history widget."""
         return self._history
 
-    async def jump_to_local_files(self, target: Path | None = None) -> Self:
+    def jump_to_local_files(self, target: Path | None = None) -> Self:
         """Switch to and focus the local files pane.
 
         Returns:
             Self.
         """
-        self.popped_out = True
-        if target is not None:
-            await self._local_files.chdir(target)
-        self._local_files.activate().set_focus_within()
+        if (
+            self.popped_out
+            and target is None
+            and self.query_one(Tabs).active == self._local_files.id
+        ):
+            self.popped_out = False
+        else:
+            self.popped_out = True
+            if target is not None:
+                self._local_files.chdir(target)
+            self._local_files.activate().set_focus_within()
         return self
 
     def jump_to_bookmarks(self) -> Self:
         """Switch to and focus the bookmarks pane.
 
         Returns:
             Self.
         """
-        self.popped_out = True
-        self._bookmarks.activate().set_focus_within()
+        if self.popped_out and self.query_one(Tabs).active == self._bookmarks.id:
+            self.popped_out = False
+        else:
+            self.popped_out = True
+            self._bookmarks.activate().set_focus_within()
         return self
 
     def jump_to_history(self) -> Self:
         """Switch to and focus the history pane.
 
         Returns:
             Self.
         """
-        self.popped_out = True
-        self._history.activate().set_focus_within()
+        if self.popped_out and self.query_one(Tabs).active == self._history.id:
+            self.popped_out = False
+        else:
+            self.popped_out = True
+            self._history.activate().set_focus_within()
         return self
 
     def jump_to_contents(self) -> Self:
         """Switch to and focus the table of contents pane.
 
         Returns:
             Self.
         """
-        self.popped_out = True
-        self._contents.activate().set_focus_within()
+        if self.popped_out and self.query_one(Tabs).active == self._contents.id:
+            self.popped_out = False
+        else:
+            self.popped_out = True
+            self._contents.activate().set_focus_within()
         return self
 
     def action_previous_tab(self) -> None:
         """Switch to the previous tab in the navigation pane."""
         self.query_one(Tabs).action_previous_tab()
         self.focus_tab()
 
     def action_next_tab(self) -> None:
         """Switch to the next tab in the navigation pane."""
         self.query_one(Tabs).action_next_tab()
         self.focus_tab()
 
+    def action_toggle_dock(self) -> None:
+        """Toggle the dock side for the navigation."""
+        config = load_config()
+        config.navigation_left = not config.navigation_left
+        save_config(config)
+        self.docked_left = config.navigation_left
+
     def focus_tab(self) -> None:
         """Focus the currently active tab."""
         if active := self.query_one(Tabs).active:
             self.query_one(
                 f"NavigationPane#{active}", NavigationPane
             ).set_focus_within()
```

### Comparing `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/bookmarks.py` & `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/local_files.py` & `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/local_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,24 +65,21 @@
         """Initialise the local files navigation pane."""
         super().__init__("Local")
 
     def compose(self) -> ComposeResult:
         """Compose the child widgets."""
         yield FilteredDirectoryTree(Path("~").expanduser())
 
-    async def chdir(self, path: Path) -> None:
-        """Change the filesystem view to the given directory."""
-        # At the moment Textual's DirectoryTree doesn't support changing
-        # directory to a new root, so here we're going to remove it and
-        # mount a fresh one with a new root.
-        #
-        # Once https://github.com/Textualize/textual/issues/2056 is taken
-        # care of update this to use whatever new approach is taken.
-        await self.query_one(FilteredDirectoryTree).remove()
-        await self.mount(FilteredDirectoryTree(path))
+    def chdir(self, path: Path) -> None:
+        """Change the filesystem view to the given directory.
+
+        Args:
+            path: The path to change to.
+        """
+        self.query_one(FilteredDirectoryTree).path = path
 
     def set_focus_within(self) -> None:
         """Focus the directory tree.."""
         self.query_one(DirectoryTree).focus(scroll_visible=False)
 
     class Goto(Message):
         """Message that requests the viewer goes to a given location."""
```

### Comparing `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/navigation_pane.py` & `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/navigation_pane.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/table_of_contents.py` & `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/table_of_contents.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,15 +40,25 @@
         """Ensure the tree in the table of contents is focused."""
         self.query_one("MarkdownTableOfContents > Tree", Tree).focus(
             scroll_visible=False
         )
 
     def compose(self) -> ComposeResult:
         """Compose the child widgets."""
-        yield MarkdownTableOfContents()
+        # Note the use of a throwaway Markdown object. Textual 0.24
+        # introduced a requirement for MarkdownTableOfContents to take a
+        # reference to a Markdown document; this is a problem if you're
+        # composing the ToC in a location somewhere unrelated to the
+        # document itself, such that you can't guarantee the order in which
+        # they're compose. I'm not using the ToC in a way that's
+        # tightly-coupled to the document, neither am I using multiple ToCs
+        # and documents. So... we make one and ignore it.
+        #
+        # https://github.com/Textualize/textual/issues/2516
+        yield MarkdownTableOfContents(Markdown())
 
     def on_table_of_contents_updated(
         self, event: Markdown.TableOfContentsUpdated
     ) -> None:
         """Handle a table of contents update event.
 
         Args:
```

### Comparing `frogmouth-0.4.0/frogmouth/widgets/omnibox.py` & `frogmouth-0.5.0/frogmouth/widgets/omnibox.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from httpx import URL
 from textual.message import Message
 from textual.reactive import var
 from textual.widgets import Input
 
 from ..utility import is_likely_url
-from ..utility.advertising import DISCORD
+from ..utility.advertising import DISCORD, ORGANISATION_NAME, PACKAGE_NAME
 
 
 class Omnibox(Input):
     """The command and location input widget for the viewer."""
 
     DEFAULT_CSS = """
     Omnibox {
@@ -44,14 +44,15 @@
     _ALIASES: dict[str, str] = {
         "a": "about",
         "b": "bookmarks",
         "bm": "bookmarks",
         "bb": "bitbucket",
         "c": "contents",
         "cd": "chdir",
+        "cl": "changelog",
         "gh": "github",
         "gl": "gitlab",
         "h": "history",
         "l": "local",
         "obs": "obsidian",
         "toc": "contents",
         "q": "quit",
@@ -331,14 +332,18 @@
         """
         self._forge_quick_look(self.BitBucketCommand, tail)
 
     def command_discord(self, _: str) -> None:
         """The command to visit the Textualize discord server."""
         open_url(DISCORD)
 
+    def command_changelog(self, _: str) -> None:
+        """The command to show the application's own ChangeLog"""
+        self.command_github(f"{ORGANISATION_NAME}/{PACKAGE_NAME} ChangeLog.md")
+
     def command_obsidian(self, vault: str) -> None:
         """The command to visit an obsidian vault, if one can be seen.
 
         Args:
             vault: The vault to visit.
 
         If the vault name is empty, an attempt will be made to visit the
```

### Comparing `frogmouth-0.4.0/frogmouth/widgets/viewer.py` & `frogmouth-0.5.0/frogmouth/widgets/viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,18 @@
             `True` if the location changed, `False` if not.
         """
         if self._current < len(self._history) - 1:
             self._current += 1
             return True
         return False
 
+    def __delitem__(self, index: int) -> None:
+        del self._history[index]
+        self._current = max(len(self._history) - 1, self._current)
+
 
 class Viewer(VerticalScroll, can_focus=True, can_focus_children=True):
     """The markdown viewer class."""
 
     DEFAULT_CSS = """
     Viewer {
         width: 1fr;
@@ -292,7 +296,24 @@
         """Load up a history list from the given history.
 
         Args:
             history: The history load up from.
         """
         self.history = History(history)
         self.post_message(self.HistoryUpdated(self))
+
+    def delete_history(self, history_id: int) -> None:
+        """Delete an item from the history.
+
+        Args:
+            history_id: The ID of the history item to delete.
+        """
+        try:
+            del self.history[history_id]
+        except IndexError:
+            pass
+        else:
+            self.post_message(self.HistoryUpdated(self))
+
+    def clear_history(self) -> None:
+        """Clear down the whole of history."""
+        self.load_history([])
```

### Comparing `frogmouth-0.4.0/pyproject.toml` & `frogmouth-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "frogmouth"
 homepage = "https://github.com/Textualize/frogmouth"
-version = "0.4.0"
+version = "0.5.0"
 description = "A Markdown document viewer for the terminal"
 authors = ["Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "frogmouth"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -24,22 +24,22 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Documentation",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = {version = "^0.22.2"}
+textual = {version = "^0.24.0"}
 typing-extensions = "^4.5.0"
 httpx = "^0.23.3"
 xdg = "^6.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
-textual = {extras = ["dev"], version = "^0.22.2"}
+textual = {extras = ["dev"], version = "^0.24.0"}
 mypy = "^1.1.1"
 pylint = "^2.17.1"
 pre-commit = "^3.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `frogmouth-0.4.0/PKG-INFO` & `frogmouth-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogmouth
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Markdown document viewer for the terminal
 Home-page: https://github.com/Textualize/frogmouth
 License: MIT
 Author: Dave Pearson
 Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: textual (>=0.22.2,<0.23.0)
+Requires-Dist: textual (>=0.24.0,<0.25.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-ac35-0d0545bf0d24.png"  width="300" align="center"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frogmouth Version: 0.4.0 Summary: A Markdown
+Metadata-Version: 2.1 Name: frogmouth Version: 0.5.0 Summary: A Markdown
 document viewer for the terminal Home-page: https://github.com/Textualize/
 frogmouth License: MIT Author: Dave Pearson Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
 Development :: Documentation Classifier: Topic :: Text Processing :: Markup ::
 Markdown Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: textual
-(>=0.22.2,<0.23.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-
+(>=0.24.0,<0.25.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-
 Dist: xdg (>=6.0.0,<7.0.0) Description-Content-Type: text/markdown
 [https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-
                             ac35-0d0545bf0d24.png]
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://
 discord.gg/Enf6Z3qhVr) # Frogmouth Frogmouth is a Markdown viewer / browser for
 your terminal, built with [Textual](https://github.com/Textualize/textual).
 Frogmouth can open `*.md` files locally or via a URL. There is a familiar
```

