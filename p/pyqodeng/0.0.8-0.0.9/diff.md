# Comparing `tmp/pyqodeng-0.0.8.tar.gz` & `tmp/pyqodeng-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqodeng-0.0.8.tar", last modified: Mon May  1 00:22:29 2023, max compression
+gzip compressed data, was "pyqodeng-0.0.9.tar", last modified: Mon May  8 22:10:54 2023, max compression
```

## Comparing `pyqodeng-0.0.8.tar` & `pyqodeng-0.0.9.tar`

### file list

```diff
@@ -1,356 +1,356 @@
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.385162 pyqodeng-0.0.8/
--rw-rw-r--   0 fish      (1000) fish      (1000)     1260 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/.coveragerc
--rw-rw-r--   0 fish      (1000) fish      (1000)      144 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/AUTHORS.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)    25317 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/CHANGELOG.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      950 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/CONTRIBUTING.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     1119 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/LICENSE
--rw-rw-r--   0 fish      (1000) fish      (1000)      397 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/MANIFEST.in
--rw-rw-r--   0 fish      (1000) fish      (1000)     4023 2023-05-01 00:22:29.385162 pyqodeng-0.0.8/PKG-INFO
--rw-rw-r--   0 fish      (1000) fish      (1000)     3076 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/README.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     2405 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/conftest.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.313168 pyqodeng-0.0.8/doc/
--rw-rw-r--   0 fish      (1000) fish      (1000)     5593 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/Makefile
--rw-rw-r--   0 fish      (1000) fish      (1000)     5125 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/make.bat
--rwxrwxr-x   0 fish      (1000) fish      (1000)      175 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/make_html.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      348 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/readme.rst
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.317168 pyqodeng-0.0.8/doc/source/
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.317168 pyqodeng-0.0.8/doc/source/_static/
--rw-rw-r--   0 fish      (1000) fish      (1000)    22868 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/_static/editor_widget.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     8397 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/doc/source/conf.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4412 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/examples.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     1747 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/index.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     1946 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.api.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     1142 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.backend.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      622 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.dialogs.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      882 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.managers.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     2855 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.modes.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     1261 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.panels.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      573 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      160 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.styles.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      264 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.tools.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     2605 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/doc/source/pyqode.core.widgets.rst
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.309169 pyqodeng-0.0.8/examples/
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.321168 pyqodeng-0.0.8/examples/encodings/
--rw-rw-r--   0 fish      (1000) fish      (1000)      879 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/encodings/common.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1085 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/encodings/detect.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      606 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/encodings/dialog.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      309 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/encodings/error.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      639 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/encodings/menu.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      409 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/encodings/panel.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      857 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/encodings/readme.rst
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.325167 pyqodeng-0.0.8/examples/modes/
--rw-rw-r--   0 fish      (1000) fish      (1000)      691 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/autocomplete.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      685 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/autoindent.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      912 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/caret_line_highlighter_with_syntax_highlighter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      832 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/caret_line_highlighter_without_syntax_highlighter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      773 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/case_converter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1798 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/checker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      712 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/code_completion_backend.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      896 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/code_completion_frontend.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      632 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/extended_selections.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1086 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/filewatcher.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      644 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/indenter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      691 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/occurences.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      665 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/pygments_syntax_highlighter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)       81 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/modes/readme.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      641 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/right_margin.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      316 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/server.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      783 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/smart_backspace.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      644 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/symbol_matcher.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      737 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/modes/zoom.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.325167 pyqodeng-0.0.8/examples/notepad/
--rw-rw-r--   0 fish      (1000) fish      (1000)     1119 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/LICENSE
--rw-rw-r--   0 fish      (1000) fish      (1000)      237 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/MANIFEST.in
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.329167 pyqodeng-0.0.8/examples/notepad/forms/
--rw-rw-r--   0 fish      (1000) fish      (1000)    17612 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/about.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     3216 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/close.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     2574 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/document-new.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1681 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/document-open.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     2747 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/document-save-as.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1117 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/document-save.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     6663 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/main_window.ui
--rw-rw-r--   0 fish      (1000) fish      (1000)    16578 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/pyqode.png
--rw-rw-r--   0 fish      (1000) fish      (1000)      281 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/forms/resources.qrc
--rw-rw-r--   0 fish      (1000) fish      (1000)     1876 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/notepad/freeze_setup.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.329167 pyqodeng-0.0.8/examples/notepad/notepad/
--rw-rw-r--   0 fish      (1000) fish      (1000)      567 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/notepad/notepad/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      636 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/notepad/notepad/editor.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.329167 pyqodeng-0.0.8/examples/notepad/notepad/forms/
--rw-rw-r--   0 fish      (1000) fish      (1000)      297 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/notepad/forms/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     8275 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/notepad/notepad/forms/main_window_ui.py
--rw-rw-r--   0 fish      (1000) fish      (1000)   184960 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/notepad/notepad/forms/resources_rc.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     9473 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/notepad/notepad/main_window.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      382 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/notepad/notepad/server.py
--rwxrwxr-x   0 fish      (1000) fish      (1000)      165 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/notepad.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      293 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/pyuic.cfg
--rw-rw-r--   0 fish      (1000) fish      (1000)      915 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/readme.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)     2086 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/setup.iss
--rw-rw-r--   0 fish      (1000) fish      (1000)     2197 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/notepad/setup.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.333167 pyqodeng-0.0.8/examples/notepad/share/
--rw-rw-r--   0 fish      (1000) fish      (1000)      186 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/share/notepad.desktop
--rw-rw-r--   0 fish      (1000) fish      (1000)   152126 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/share/notepad.ico
--rw-rw-r--   0 fish      (1000) fish      (1000)    16578 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/notepad/share/notepad.png
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.333167 pyqodeng-0.0.8/examples/panels/
--rw-rw-r--   0 fish      (1000) fish      (1000)     1872 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/panels/checker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1106 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/panels/folding.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2059 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/panels/global_checker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      609 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/panels/line_numbers.py
--rw-rw-r--   0 fish      (1000) fish      (1000)       82 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/panels/readme.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      735 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/panels/search_and_replace.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      316 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/panels/server.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.333167 pyqodeng-0.0.8/examples/simple/
--rw-rw-r--   0 fish      (1000) fish      (1000)     1310 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/simple/basic.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1152 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/simple/custom_actions.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      162 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/simple/readme.rst
--rw-rw-r--   0 fish      (1000) fish      (1000)      316 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/simple/server.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1149 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/simple/style_and_settings.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.337166 pyqodeng-0.0.8/examples/widgets/
--rw-rw-r--   0 fish      (1000) fish      (1000)      496 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/widgets/errors_table.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      716 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/widgets/filesystem_treeview.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      857 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/widgets/generic_code_edit.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      539 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/widgets/interactive_process.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      361 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/widgets/output_window.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      899 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/widgets/splittable_codeedit_tab_widget.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1220 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/widgets/splittable_tab_widget.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      275 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/examples/widgets/terminal.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.337166 pyqodeng-0.0.8/examples/widgets/test_dir/
--rw-rw-r--   0 fish      (1000) fish      (1000)        7 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/widgets/test_dir/module.hpp
--rw-rw-r--   0 fish      (1000) fish      (1000)        0 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/widgets/test_dir/module.pyx
--rw-rw-r--   0 fish      (1000) fish      (1000)      145 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/widgets/test_dir/readme.txt
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.337166 pyqodeng-0.0.8/examples/widgets/test_dir/subdir/
--rw-rw-r--   0 fish      (1000) fish      (1000)       75 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/widgets/test_dir/subdir/module.exe
--rw-rw-r--   0 fish      (1000) fish      (1000)        0 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/widgets/test_dir/subdir/module.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      145 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/examples/widgets/test_dir/subdir/readme.txt
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.337166 pyqodeng-0.0.8/forms/
--rw-rw-r--   0 fish      (1000) fish      (1000)     3492 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/dlg_encodings.ui
--rw-rw-r--   0 fish      (1000) fish      (1000)     2696 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/dlg_goto_line.ui
--rw-rw-r--   0 fish      (1000) fish      (1000)     5938 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/dlg_preferred_encodings_editor.ui
--rw-rw-r--   0 fish      (1000) fish      (1000)     1815 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/dlg_unsaved_files.ui
--rw-rw-r--   0 fish      (1000) fish      (1000)     3094 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/pnl_encoding.ui
--rw-rw-r--   0 fish      (1000) fish      (1000)     1091 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/pnl_read_only.ui
--rw-rw-r--   0 fish      (1000) fish      (1000)     2875 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/popup_open_files.ui
--rw-rw-r--   0 fish      (1000) fish      (1000)     1216 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/pyqode_core.qrc
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.349165 pyqodeng-0.0.8/forms/rc/
--rw-rw-r--   0 fish      (1000) fish      (1000)   120504 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/SourceCodePro-Bold.ttf
--rw-rw-r--   0 fish      (1000) fish      (1000)   120548 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/SourceCodePro-Regular.ttf
--rw-rw-r--   0 fish      (1000) fish      (1000)      372 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/arrow_down_off.png
--rw-rw-r--   0 fish      (1000) fish      (1000)      290 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/arrow_down_on.png
--rw-rw-r--   0 fish      (1000) fish      (1000)      357 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/arrow_right_off.png
--rw-rw-r--   0 fish      (1000) fish      (1000)      269 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/arrow_right_on.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     2288 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/clear-left.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     2168 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/close.png
--rw-rw-r--   0 fish      (1000) fish      (1000)      814 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/dialog-error.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1063 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/dialog-info.png
--rw-rw-r--   0 fish      (1000) fish      (1000)      621 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/dialog-warning.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     2230 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/document-save-as.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1333 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/document-save.png
--rw-rw-r--   0 fish      (1000) fish      (1000)      913 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-copy.png
--rw-rw-r--   0 fish      (1000) fish      (1000)      911 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-cut.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1587 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-delete.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     2318 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-find-replace.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1841 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-find.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1697 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-paste.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     2046 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-redo.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1400 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-select-all.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1925 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-trash.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     2065 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/edit-undo.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1081 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/format-indent-less.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1064 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/format-indent-more.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1555 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/go-down.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1575 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/go-next.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1600 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/go-previous.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1620 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/go-up.png
--rw-rw-r--   0 fish      (1000) fish      (1000)     1003 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/rc/goto-line.png
--rw-rw-r--   0 fish      (1000) fish      (1000)    12723 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/forms/search_panel.ui
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.349165 pyqodeng-0.0.8/pyqodeng/
--rw-rw-r--   0 fish      (1000) fish      (1000)      204 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/__init__.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.353165 pyqodeng-0.0.8/pyqodeng/core/
--rw-rw-r--   0 fish      (1000) fish      (1000)      701 2023-05-01 00:20:51.000000 pyqodeng-0.0.8/pyqodeng/core/__init__.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.353165 pyqodeng-0.0.8/pyqodeng/core/_designer_plugins/
--rw-rw-r--   0 fish      (1000) fish      (1000)     1403 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_designer_plugins/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      365 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_designer_plugins/code_edit_plugin.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      381 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_designer_plugins/errors_table_plugin.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      409 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_designer_plugins/interactive_console_plugin.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      373 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_designer_plugins/tab_widget_plugin.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.357164 pyqodeng-0.0.8/pyqodeng/core/_forms/
--rw-rw-r--   0 fish      (1000) fish      (1000)      227 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2965 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/dlg_encodings_ui.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2749 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/dlg_goto_line_ui.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6077 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/dlg_preferred_encodings_editor_ui.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1645 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/dlg_unsaved_files_ui.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3470 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/pnl_encoding_ui.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1448 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/pnl_read_only_ui.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2775 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/popup_open_files_ui.py
--rw-rw-r--   0 fish      (1000) fish      (1000)  1159362 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/pyqode_core_rc.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    11393 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/_forms/search_panel_ui.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.361164 pyqodeng-0.0.8/pyqodeng/core/api/
--rw-rw-r--   0 fish      (1000) fish      (1000)     1174 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/api/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    14433 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/api/client.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    51429 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/api/code_edit.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6861 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/api/decoration.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     5246 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/api/encodings.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    13327 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/api/folding.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1198 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/api/manager.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3654 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/api/mode.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3788 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/api/panel.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    13415 2023-05-01 00:20:22.000000 pyqodeng-0.0.8/pyqodeng/core/api/syntax_highlighter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    39800 2022-10-31 22:04:49.000000 pyqodeng-0.0.8/pyqodeng/core/api/utils.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.361164 pyqodeng-0.0.8/pyqodeng/core/backend/
--rw-rw-r--   0 fish      (1000) fish      (1000)     3868 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/backend/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     7531 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/backend/server.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     8127 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/backend/workers.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4991 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/cache.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.361164 pyqodeng-0.0.8/pyqodeng/core/dialogs/
--rw-rw-r--   0 fish      (1000) fish      (1000)      347 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/dialogs/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     7407 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/dialogs/encodings.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1496 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/dialogs/goto.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2035 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/dialogs/unsaved_files.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1924 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/icons.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.361164 pyqodeng-0.0.8/pyqodeng/core/managers/
--rw-rw-r--   0 fish      (1000) fish      (1000)      827 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/managers/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     8565 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/managers/backend.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1768 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/managers/decorations.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    15501 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/managers/file.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2251 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/managers/modes.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    10676 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/managers/panels.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.365164 pyqodeng-0.0.8/pyqodeng/core/modes/
--rw-rw-r--   0 fish      (1000) fish      (1000)     1663 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4414 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/modes/autocomplete.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2267 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/modes/autoindent.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1916 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/modes/backspace.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2730 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/caret_line_highlight.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2001 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/case_converter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    12394 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/checker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    24630 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/code_completion.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2862 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/cursor_history.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6255 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/extended_selection.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     7527 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/filewatcher.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6483 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/modes/indenter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2625 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/line_highlighter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     9859 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/modes/matcher.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6454 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/occurences.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2859 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/outline.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    14801 2022-10-31 22:04:49.000000 pyqodeng-0.0.8/pyqodeng/core/modes/pygments_sh.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2704 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/right_margin.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4847 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/wordclick.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3047 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/modes/zoom.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.365164 pyqodeng-0.0.8/pyqodeng/core/panels/
--rw-rw-r--   0 fish      (1000) fish      (1000)      621 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/panels/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4450 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/panels/checker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     8132 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/panels/encodings.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    31988 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/panels/folding.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3440 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/panels/global_checker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4207 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/panels/line_number.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     8022 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/panels/marker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2580 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/panels/read_only.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    25200 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/panels/search_and_replace.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2488 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/share.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.365164 pyqodeng-0.0.8/pyqodeng/core/styles/
--rw-rw-r--   0 fish      (1000) fish      (1000)      290 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/styles/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2109 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/styles/darcula.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2067 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/styles/qt.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.365164 pyqodeng-0.0.8/pyqodeng/core/tools/
--rw-rw-r--   0 fish      (1000) fish      (1000)      254 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/tools/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1134 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/tools/console.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.369164 pyqodeng-0.0.8/pyqodeng/core/widgets/
--rw-rw-r--   0 fish      (1000) fish      (1000)     2553 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     5160 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/_pty.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6797 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/code_edits.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     7222 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/encodings.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     5821 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/errors_table.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2006 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/file_icons_provider.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    30761 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/filesystem_treeview.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    15542 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/interactive.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6957 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/menu_recents.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     9679 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/outline.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    57289 2022-10-24 23:25:59.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/output_window.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1931 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/preview.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4287 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/prompt_line_edit.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      476 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/pty_wrapper.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    63620 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/splittable_tab_widget.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      958 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/tab_bar.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    16204 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/tabs.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2333 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/pyqodeng/core/widgets/terminal.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.349165 pyqodeng-0.0.8/pyqodeng.egg-info/
--rw-rw-r--   0 fish      (1000) fish      (1000)     4023 2023-05-01 00:22:29.000000 pyqodeng-0.0.8/pyqodeng.egg-info/PKG-INFO
--rw-rw-r--   0 fish      (1000) fish      (1000)    10130 2023-05-01 00:22:29.000000 pyqodeng-0.0.8/pyqodeng.egg-info/SOURCES.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)        1 2023-05-01 00:22:29.000000 pyqodeng-0.0.8/pyqodeng.egg-info/dependency_links.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)      238 2023-05-01 00:22:29.000000 pyqodeng-0.0.8/pyqodeng.egg-info/entry_points.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)        9 2023-05-01 00:22:29.000000 pyqodeng-0.0.8/pyqodeng.egg-info/namespace_packages.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)        1 2022-10-17 22:19:07.000000 pyqodeng-0.0.8/pyqodeng.egg-info/not-zip-safe
--rw-rw-r--   0 fish      (1000) fish      (1000)       47 2023-05-01 00:22:29.000000 pyqodeng-0.0.8/pyqodeng.egg-info/requires.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)        9 2023-05-01 00:22:29.000000 pyqodeng-0.0.8/pyqodeng.egg-info/top_level.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)      233 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/pytest.ini
--rw-rw-r--   0 fish      (1000) fish      (1000)      120 2023-05-01 00:22:29.385162 pyqodeng-0.0.8/setup.cfg
--rw-rw-r--   0 fish      (1000) fish      (1000)     3396 2022-10-24 23:23:21.000000 pyqodeng-0.0.8/setup.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.369164 pyqodeng-0.0.8/test/
--rw-rw-r--   0 fish      (1000) fish      (1000)       48 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/__init__.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.373163 pyqodeng-0.0.8/test/files/
--rw-rw-r--   0 fish      (1000) fish      (1000)        4 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/files/big5hkscs.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)      287 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/files/foo.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6850 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/helpers.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      634 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/server.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.373163 pyqodeng-0.0.8/test/test_api/
--rw-rw-r--   0 fish      (1000) fish      (1000)        1 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/__init__.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.377163 pyqodeng-0.0.8/test/test_api/folding_cases/
--rw-rw-r--   0 fish      (1000) fish      (1000)      155 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/folding_cases/01.ctx
--rw-rw-r--   0 fish      (1000) fish      (1000)      264 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/folding_cases/01.results
--rw-rw-r--   0 fish      (1000) fish      (1000)      142 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/folding_cases/02.ctx
--rw-rw-r--   0 fish      (1000) fish      (1000)      271 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/folding_cases/02.results
--rw-rw-r--   0 fish      (1000) fish      (1000)      144 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/folding_cases/03.ctx
--rw-rw-r--   0 fish      (1000) fish      (1000)      264 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/folding_cases/03.results
--rw-rw-r--   0 fish      (1000) fish      (1000)      143 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/folding_cases/04.ctx
--rw-rw-r--   0 fish      (1000) fish      (1000)      481 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_api/folding_cases/foo.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      264 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/folding_cases/foo.static_results
--rw-rw-r--   0 fish      (1000) fish      (1000)       59 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_api/test_client.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    11739 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_api/test_code_edit.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2561 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_api/test_decoration.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      136 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_api/test_encodings.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1782 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_api/test_extension.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     7015 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_api/test_folding.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     9903 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_api/test_text.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3163 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_api/test_utils.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.377163 pyqodeng-0.0.8/test/test_backend/
--rw-rw-r--   0 fish      (1000) fish      (1000)        0 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_backend/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      403 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_backend/server.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3307 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_backend/test_workers.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      959 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_cache.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.377163 pyqodeng-0.0.8/test/test_managers/
--rw-rw-r--   0 fish      (1000) fish      (1000)        1 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_managers/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2289 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_managers/test_backend.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2677 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_managers/test_file_manager.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.381163 pyqodeng-0.0.8/test/test_modes/
--rw-rw-r--   0 fish      (1000) fish      (1000)        1 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_modes/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1533 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_autocomplete.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      536 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_autoindent.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      618 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_backspace.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      825 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_caret_line_highlight.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      332 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_case_converter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2721 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_checker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     6585 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_code_completion.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3150 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_extended_selection.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2181 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_filewatcher.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      997 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_indenter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     3452 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_matcher.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1549 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_occurrences.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      700 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_pygments_highlighter.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      620 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_right_margin.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1404 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_word_click.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1546 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_modes/test_zoom.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.385162 pyqodeng-0.0.8/test/test_panels/
--rw-rw-r--   0 fish      (1000) fish      (1000)        0 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_panels/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      681 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_panels/test_checker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2063 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_panels/test_encoding.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4713 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_panels/test_folding.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1624 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_panels/test_line_nbr.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2543 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_panels/test_marker.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     4232 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_panels/test_search_and_replace.py
-drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-01 00:22:29.385162 pyqodeng-0.0.8/test/test_widgets/
--rw-rw-r--   0 fish      (1000) fish      (1000)      151 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_widgets/__init__.py
--rw-rw-r--   0 fish      (1000) fish      (1000)    11648 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_widgets/parsed_output.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)    17616 2020-04-03 07:00:13.000000 pyqodeng-0.0.8/test/test_widgets/raw_output.txt
--rw-rw-r--   0 fish      (1000) fish      (1000)      278 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_widgets/test_fstreeview.py
--rw-rw-r--   0 fish      (1000) fish      (1000)      294 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_widgets/test_interactive_console.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     2306 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_widgets/test_output_window.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1741 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_widgets/test_recent_files.py
--rw-rw-r--   0 fish      (1000) fish      (1000)     1231 2022-10-17 22:17:51.000000 pyqodeng-0.0.8/test/test_widgets/test_splittable_tab_widget.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.858096 pyqodeng-0.0.9/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1260 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/.coveragerc
+-rw-rw-r--   0 fish      (1000) fish      (1000)      144 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/AUTHORS.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)    25317 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/CHANGELOG.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      950 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/CONTRIBUTING.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1119 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/LICENSE
+-rw-rw-r--   0 fish      (1000) fish      (1000)      397 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/MANIFEST.in
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4023 2023-05-08 22:10:54.858096 pyqodeng-0.0.9/PKG-INFO
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3076 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/README.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2405 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/conftest.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.766095 pyqodeng-0.0.9/doc/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     5593 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/Makefile
+-rw-rw-r--   0 fish      (1000) fish      (1000)     5125 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/make.bat
+-rwxrwxr-x   0 fish      (1000) fish      (1000)      175 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/make_html.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      348 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/readme.rst
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.770095 pyqodeng-0.0.9/doc/source/
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.770095 pyqodeng-0.0.9/doc/source/_static/
+-rw-rw-r--   0 fish      (1000) fish      (1000)    22868 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/_static/editor_widget.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     8397 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/doc/source/conf.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4412 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/examples.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1747 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/index.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1946 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.api.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1142 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.backend.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      622 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.dialogs.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      882 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.managers.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2855 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.modes.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1261 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.panels.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      573 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      160 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.styles.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      264 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.tools.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2605 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/doc/source/pyqode.core.widgets.rst
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.762095 pyqodeng-0.0.9/examples/
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.770095 pyqodeng-0.0.9/examples/encodings/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      879 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/encodings/common.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1085 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/encodings/detect.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      606 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/encodings/dialog.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      309 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/encodings/error.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      639 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/encodings/menu.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      409 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/encodings/panel.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      857 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/encodings/readme.rst
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.778095 pyqodeng-0.0.9/examples/modes/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      691 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/autocomplete.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      685 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/autoindent.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      912 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/caret_line_highlighter_with_syntax_highlighter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      832 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/caret_line_highlighter_without_syntax_highlighter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      773 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/case_converter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1798 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/checker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      712 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/code_completion_backend.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      896 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/code_completion_frontend.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      632 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/extended_selections.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1086 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/filewatcher.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      644 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/indenter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      691 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/occurences.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      665 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/pygments_syntax_highlighter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)       81 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/modes/readme.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      641 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/right_margin.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      316 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/server.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      783 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/smart_backspace.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      644 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/symbol_matcher.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      737 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/modes/zoom.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.778095 pyqodeng-0.0.9/examples/notepad/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1119 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/LICENSE
+-rw-rw-r--   0 fish      (1000) fish      (1000)      237 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/MANIFEST.in
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.782095 pyqodeng-0.0.9/examples/notepad/forms/
+-rw-rw-r--   0 fish      (1000) fish      (1000)    17612 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/about.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3216 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/close.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2574 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/document-new.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1681 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/document-open.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2747 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/document-save-as.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1117 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/document-save.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6663 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/main_window.ui
+-rw-rw-r--   0 fish      (1000) fish      (1000)    16578 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/pyqode.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)      281 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/forms/resources.qrc
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1876 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/notepad/freeze_setup.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.782095 pyqodeng-0.0.9/examples/notepad/notepad/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      567 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/notepad/notepad/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      636 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/notepad/notepad/editor.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.782095 pyqodeng-0.0.9/examples/notepad/notepad/forms/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      297 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/notepad/forms/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     8275 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/notepad/notepad/forms/main_window_ui.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)   184960 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/notepad/notepad/forms/resources_rc.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     9473 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/notepad/notepad/main_window.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      382 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/notepad/notepad/server.py
+-rwxrwxr-x   0 fish      (1000) fish      (1000)      165 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/notepad.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      293 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/pyuic.cfg
+-rw-rw-r--   0 fish      (1000) fish      (1000)      915 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/readme.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2086 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/setup.iss
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2197 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/notepad/setup.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.786095 pyqodeng-0.0.9/examples/notepad/share/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      186 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/share/notepad.desktop
+-rw-rw-r--   0 fish      (1000) fish      (1000)   152126 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/share/notepad.ico
+-rw-rw-r--   0 fish      (1000) fish      (1000)    16578 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/notepad/share/notepad.png
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.790095 pyqodeng-0.0.9/examples/panels/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1872 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/panels/checker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1106 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/panels/folding.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2059 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/panels/global_checker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      609 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/panels/line_numbers.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)       82 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/panels/readme.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      735 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/panels/search_and_replace.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      316 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/panels/server.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.790095 pyqodeng-0.0.9/examples/simple/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1310 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/simple/basic.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1152 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/simple/custom_actions.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      162 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/simple/readme.rst
+-rw-rw-r--   0 fish      (1000) fish      (1000)      316 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/simple/server.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1149 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/simple/style_and_settings.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.790095 pyqodeng-0.0.9/examples/widgets/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      496 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/widgets/errors_table.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      716 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/widgets/filesystem_treeview.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      857 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/widgets/generic_code_edit.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      539 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/widgets/interactive_process.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      361 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/widgets/output_window.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      899 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/widgets/splittable_codeedit_tab_widget.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1220 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/widgets/splittable_tab_widget.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      275 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/examples/widgets/terminal.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.794095 pyqodeng-0.0.9/examples/widgets/test_dir/
+-rw-rw-r--   0 fish      (1000) fish      (1000)        7 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/widgets/test_dir/module.hpp
+-rw-rw-r--   0 fish      (1000) fish      (1000)        0 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/widgets/test_dir/module.pyx
+-rw-rw-r--   0 fish      (1000) fish      (1000)      145 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/widgets/test_dir/readme.txt
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.794095 pyqodeng-0.0.9/examples/widgets/test_dir/subdir/
+-rw-rw-r--   0 fish      (1000) fish      (1000)       75 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/widgets/test_dir/subdir/module.exe
+-rw-rw-r--   0 fish      (1000) fish      (1000)        0 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/widgets/test_dir/subdir/module.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      145 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/examples/widgets/test_dir/subdir/readme.txt
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.794095 pyqodeng-0.0.9/forms/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3492 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/dlg_encodings.ui
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2696 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/dlg_goto_line.ui
+-rw-rw-r--   0 fish      (1000) fish      (1000)     5938 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/dlg_preferred_encodings_editor.ui
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1815 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/dlg_unsaved_files.ui
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3094 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/pnl_encoding.ui
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1091 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/pnl_read_only.ui
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2875 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/popup_open_files.ui
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1216 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/pyqode_core.qrc
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.802096 pyqodeng-0.0.9/forms/rc/
+-rw-rw-r--   0 fish      (1000) fish      (1000)   120504 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/SourceCodePro-Bold.ttf
+-rw-rw-r--   0 fish      (1000) fish      (1000)   120548 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/SourceCodePro-Regular.ttf
+-rw-rw-r--   0 fish      (1000) fish      (1000)      372 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/arrow_down_off.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)      290 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/arrow_down_on.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)      357 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/arrow_right_off.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)      269 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/arrow_right_on.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2288 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/clear-left.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2168 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/close.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)      814 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/dialog-error.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1063 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/dialog-info.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)      621 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/dialog-warning.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2230 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/document-save-as.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1333 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/document-save.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)      913 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-copy.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)      911 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-cut.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1587 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-delete.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2318 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-find-replace.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1841 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-find.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1697 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-paste.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2046 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-redo.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1400 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-select-all.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1925 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-trash.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2065 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/edit-undo.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1081 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/format-indent-less.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1064 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/format-indent-more.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1555 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/go-down.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1575 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/go-next.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1600 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/go-previous.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1620 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/go-up.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1003 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/rc/goto-line.png
+-rw-rw-r--   0 fish      (1000) fish      (1000)    12723 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/forms/search_panel.ui
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.802096 pyqodeng-0.0.9/pyqodeng/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      204 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/__init__.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.802096 pyqodeng-0.0.9/pyqodeng/core/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      701 2023-05-08 22:06:23.000000 pyqodeng-0.0.9/pyqodeng/core/__init__.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.806095 pyqodeng-0.0.9/pyqodeng/core/_designer_plugins/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1403 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_designer_plugins/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      365 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_designer_plugins/code_edit_plugin.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      381 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_designer_plugins/errors_table_plugin.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      409 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_designer_plugins/interactive_console_plugin.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      373 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_designer_plugins/tab_widget_plugin.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.814096 pyqodeng-0.0.9/pyqodeng/core/_forms/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      227 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2965 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/dlg_encodings_ui.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2749 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/dlg_goto_line_ui.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6077 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/dlg_preferred_encodings_editor_ui.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1645 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/dlg_unsaved_files_ui.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3470 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/pnl_encoding_ui.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1448 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/pnl_read_only_ui.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2775 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/popup_open_files_ui.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)  1159362 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/pyqode_core_rc.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    11393 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/_forms/search_panel_ui.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.818096 pyqodeng-0.0.9/pyqodeng/core/api/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1174 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/api/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    14433 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/api/client.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    51871 2023-05-08 09:21:15.000000 pyqodeng-0.0.9/pyqodeng/core/api/code_edit.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6861 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/api/decoration.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     5246 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/api/encodings.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    13327 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/api/folding.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1198 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/api/manager.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3654 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/api/mode.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3788 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/api/panel.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    13415 2023-05-01 00:20:22.000000 pyqodeng-0.0.9/pyqodeng/core/api/syntax_highlighter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    39800 2022-10-31 22:04:49.000000 pyqodeng-0.0.9/pyqodeng/core/api/utils.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.822096 pyqodeng-0.0.9/pyqodeng/core/backend/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3868 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/backend/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     7531 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/backend/server.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     8127 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/backend/workers.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4991 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/cache.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.822096 pyqodeng-0.0.9/pyqodeng/core/dialogs/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      347 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/dialogs/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     7407 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/dialogs/encodings.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1496 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/dialogs/goto.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2035 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/dialogs/unsaved_files.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1924 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/icons.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.822096 pyqodeng-0.0.9/pyqodeng/core/managers/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      827 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/managers/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     8565 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/managers/backend.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1768 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/managers/decorations.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    15501 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/managers/file.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2251 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/managers/modes.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    10676 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/managers/panels.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.830096 pyqodeng-0.0.9/pyqodeng/core/modes/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1663 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4414 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/modes/autocomplete.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2267 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/modes/autoindent.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1916 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/modes/backspace.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2730 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/caret_line_highlight.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2001 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/case_converter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    12394 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/checker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    24630 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/code_completion.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2862 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/cursor_history.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6255 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/extended_selection.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     7527 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/filewatcher.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6483 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/modes/indenter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2625 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/line_highlighter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     9859 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/modes/matcher.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6454 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/occurences.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2859 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/outline.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    14801 2022-10-31 22:04:49.000000 pyqodeng-0.0.9/pyqodeng/core/modes/pygments_sh.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2704 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/right_margin.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4847 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/wordclick.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3047 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/modes/zoom.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.834096 pyqodeng-0.0.9/pyqodeng/core/panels/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      621 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/panels/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4450 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/panels/checker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     8132 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/panels/encodings.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    31988 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/panels/folding.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3440 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/panels/global_checker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4207 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/panels/line_number.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     8022 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/panels/marker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2580 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/panels/read_only.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    25200 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/panels/search_and_replace.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2488 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/share.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.834096 pyqodeng-0.0.9/pyqodeng/core/styles/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      290 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/styles/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2109 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/styles/darcula.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2067 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/styles/qt.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.834096 pyqodeng-0.0.9/pyqodeng/core/tools/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      254 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/tools/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1134 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/tools/console.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.842096 pyqodeng-0.0.9/pyqodeng/core/widgets/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2553 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     5160 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/_pty.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6797 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/code_edits.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     7222 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/encodings.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     5821 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/errors_table.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2006 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/file_icons_provider.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    30761 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/filesystem_treeview.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    15542 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/interactive.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6957 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/menu_recents.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     9679 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/outline.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    57289 2022-10-24 23:25:59.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/output_window.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1931 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/preview.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4287 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/prompt_line_edit.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      476 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/pty_wrapper.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    63620 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/splittable_tab_widget.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      958 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/tab_bar.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    16204 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/tabs.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2333 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/pyqodeng/core/widgets/terminal.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.802096 pyqodeng-0.0.9/pyqodeng.egg-info/
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4023 2023-05-08 22:10:54.000000 pyqodeng-0.0.9/pyqodeng.egg-info/PKG-INFO
+-rw-rw-r--   0 fish      (1000) fish      (1000)    10130 2023-05-08 22:10:54.000000 pyqodeng-0.0.9/pyqodeng.egg-info/SOURCES.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)        1 2023-05-08 22:10:54.000000 pyqodeng-0.0.9/pyqodeng.egg-info/dependency_links.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)      238 2023-05-08 22:10:54.000000 pyqodeng-0.0.9/pyqodeng.egg-info/entry_points.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)        9 2023-05-08 22:10:54.000000 pyqodeng-0.0.9/pyqodeng.egg-info/namespace_packages.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)        1 2022-10-17 22:19:07.000000 pyqodeng-0.0.9/pyqodeng.egg-info/not-zip-safe
+-rw-rw-r--   0 fish      (1000) fish      (1000)       47 2023-05-08 22:10:54.000000 pyqodeng-0.0.9/pyqodeng.egg-info/requires.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)        9 2023-05-08 22:10:54.000000 pyqodeng-0.0.9/pyqodeng.egg-info/top_level.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)      233 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/pytest.ini
+-rw-rw-r--   0 fish      (1000) fish      (1000)      120 2023-05-08 22:10:54.858096 pyqodeng-0.0.9/setup.cfg
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3396 2022-10-24 23:23:21.000000 pyqodeng-0.0.9/setup.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.842096 pyqodeng-0.0.9/test/
+-rw-rw-r--   0 fish      (1000) fish      (1000)       48 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/__init__.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.842096 pyqodeng-0.0.9/test/files/
+-rw-rw-r--   0 fish      (1000) fish      (1000)        4 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/files/big5hkscs.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)      287 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/files/foo.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6850 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/helpers.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      634 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/server.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.846096 pyqodeng-0.0.9/test/test_api/
+-rw-rw-r--   0 fish      (1000) fish      (1000)        1 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/__init__.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.846096 pyqodeng-0.0.9/test/test_api/folding_cases/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      155 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/folding_cases/01.ctx
+-rw-rw-r--   0 fish      (1000) fish      (1000)      264 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/folding_cases/01.results
+-rw-rw-r--   0 fish      (1000) fish      (1000)      142 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/folding_cases/02.ctx
+-rw-rw-r--   0 fish      (1000) fish      (1000)      271 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/folding_cases/02.results
+-rw-rw-r--   0 fish      (1000) fish      (1000)      144 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/folding_cases/03.ctx
+-rw-rw-r--   0 fish      (1000) fish      (1000)      264 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/folding_cases/03.results
+-rw-rw-r--   0 fish      (1000) fish      (1000)      143 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/folding_cases/04.ctx
+-rw-rw-r--   0 fish      (1000) fish      (1000)      481 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_api/folding_cases/foo.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      264 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/folding_cases/foo.static_results
+-rw-rw-r--   0 fish      (1000) fish      (1000)       59 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_api/test_client.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    11739 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_api/test_code_edit.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2561 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_api/test_decoration.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      136 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_api/test_encodings.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1782 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_api/test_extension.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     7015 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_api/test_folding.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     9903 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_api/test_text.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3163 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_api/test_utils.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.846096 pyqodeng-0.0.9/test/test_backend/
+-rw-rw-r--   0 fish      (1000) fish      (1000)        0 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_backend/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      403 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_backend/server.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3307 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_backend/test_workers.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      959 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_cache.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.850096 pyqodeng-0.0.9/test/test_managers/
+-rw-rw-r--   0 fish      (1000) fish      (1000)        1 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_managers/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2289 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_managers/test_backend.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2677 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_managers/test_file_manager.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.854096 pyqodeng-0.0.9/test/test_modes/
+-rw-rw-r--   0 fish      (1000) fish      (1000)        1 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_modes/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1533 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_autocomplete.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      536 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_autoindent.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      618 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_backspace.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      825 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_caret_line_highlight.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      332 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_case_converter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2721 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_checker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     6585 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_code_completion.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3150 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_extended_selection.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2181 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_filewatcher.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      997 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_indenter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     3452 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_matcher.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1549 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_occurrences.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      700 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_pygments_highlighter.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      620 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_right_margin.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1404 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_word_click.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1546 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_modes/test_zoom.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.858096 pyqodeng-0.0.9/test/test_panels/
+-rw-rw-r--   0 fish      (1000) fish      (1000)        0 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_panels/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      681 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_panels/test_checker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2063 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_panels/test_encoding.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4713 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_panels/test_folding.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1624 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_panels/test_line_nbr.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2543 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_panels/test_marker.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     4232 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_panels/test_search_and_replace.py
+drwxrwxr-x   0 fish      (1000) fish      (1000)        0 2023-05-08 22:10:54.858096 pyqodeng-0.0.9/test/test_widgets/
+-rw-rw-r--   0 fish      (1000) fish      (1000)      151 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_widgets/__init__.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)    11648 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_widgets/parsed_output.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)    17616 2020-04-03 07:00:13.000000 pyqodeng-0.0.9/test/test_widgets/raw_output.txt
+-rw-rw-r--   0 fish      (1000) fish      (1000)      278 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_widgets/test_fstreeview.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)      294 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_widgets/test_interactive_console.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     2306 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_widgets/test_output_window.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1741 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_widgets/test_recent_files.py
+-rw-rw-r--   0 fish      (1000) fish      (1000)     1231 2022-10-17 22:17:51.000000 pyqodeng-0.0.9/test/test_widgets/test_splittable_tab_widget.py
```

### Comparing `pyqodeng-0.0.8/.coveragerc` & `pyqodeng-0.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/CHANGELOG.rst` & `pyqodeng-0.0.9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/CONTRIBUTING.rst` & `pyqodeng-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/LICENSE` & `pyqodeng-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/PKG-INFO` & `pyqodeng-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqodeng
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyQt/PySide Source Code Editor Widget
 Home-page: https://github.com/angr/pyqodeng
 Author: Colin Duquesnoy and others
 Author-email: colin.duquesnoy@gmail.com
 License: MIT
 Keywords: CodeEdit PyQt source code editor widget qt
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyqodeng-0.0.8/README.rst` & `pyqodeng-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/conftest.py` & `pyqodeng-0.0.9/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/Makefile` & `pyqodeng-0.0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/make.bat` & `pyqodeng-0.0.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/_static/editor_widget.png` & `pyqodeng-0.0.9/doc/source/_static/editor_widget.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/conf.py` & `pyqodeng-0.0.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/examples.rst` & `pyqodeng-0.0.9/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/index.rst` & `pyqodeng-0.0.9/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/pyqode.core.api.rst` & `pyqodeng-0.0.9/doc/source/pyqode.core.api.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/pyqode.core.backend.rst` & `pyqodeng-0.0.9/doc/source/pyqode.core.backend.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/pyqode.core.dialogs.rst` & `pyqodeng-0.0.9/doc/source/pyqode.core.dialogs.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/pyqode.core.managers.rst` & `pyqodeng-0.0.9/doc/source/pyqode.core.managers.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/pyqode.core.modes.rst` & `pyqodeng-0.0.9/doc/source/pyqode.core.modes.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/pyqode.core.panels.rst` & `pyqodeng-0.0.9/doc/source/pyqode.core.panels.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/pyqode.core.rst` & `pyqodeng-0.0.9/doc/source/pyqode.core.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/doc/source/pyqode.core.widgets.rst` & `pyqodeng-0.0.9/doc/source/pyqode.core.widgets.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/encodings/common.py` & `pyqodeng-0.0.9/examples/encodings/common.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/encodings/detect.py` & `pyqodeng-0.0.9/examples/encodings/detect.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/encodings/dialog.py` & `pyqodeng-0.0.9/examples/encodings/dialog.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/encodings/menu.py` & `pyqodeng-0.0.9/examples/encodings/menu.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/encodings/readme.rst` & `pyqodeng-0.0.9/examples/encodings/readme.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/autocomplete.py` & `pyqodeng-0.0.9/examples/modes/autocomplete.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/autoindent.py` & `pyqodeng-0.0.9/examples/modes/autoindent.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/caret_line_highlighter_with_syntax_highlighter.py` & `pyqodeng-0.0.9/examples/modes/caret_line_highlighter_with_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/caret_line_highlighter_without_syntax_highlighter.py` & `pyqodeng-0.0.9/examples/modes/caret_line_highlighter_without_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/case_converter.py` & `pyqodeng-0.0.9/examples/modes/case_converter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/checker.py` & `pyqodeng-0.0.9/examples/modes/checker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/code_completion_backend.py` & `pyqodeng-0.0.9/examples/modes/code_completion_backend.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/code_completion_frontend.py` & `pyqodeng-0.0.9/examples/modes/code_completion_frontend.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/extended_selections.py` & `pyqodeng-0.0.9/examples/modes/extended_selections.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/filewatcher.py` & `pyqodeng-0.0.9/examples/modes/filewatcher.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/indenter.py` & `pyqodeng-0.0.9/examples/modes/indenter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/occurences.py` & `pyqodeng-0.0.9/examples/modes/occurences.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/pygments_syntax_highlighter.py` & `pyqodeng-0.0.9/examples/modes/pygments_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/right_margin.py` & `pyqodeng-0.0.9/examples/modes/right_margin.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/smart_backspace.py` & `pyqodeng-0.0.9/examples/modes/smart_backspace.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/symbol_matcher.py` & `pyqodeng-0.0.9/examples/modes/symbol_matcher.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/modes/zoom.py` & `pyqodeng-0.0.9/examples/modes/zoom.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/LICENSE` & `pyqodeng-0.0.9/examples/notepad/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/forms/about.png` & `pyqodeng-0.0.9/examples/notepad/forms/about.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/forms/close.png` & `pyqodeng-0.0.9/examples/notepad/forms/close.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/forms/document-new.png` & `pyqodeng-0.0.9/examples/notepad/forms/document-new.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/forms/document-open.png` & `pyqodeng-0.0.9/examples/notepad/forms/document-open.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/forms/document-save-as.png` & `pyqodeng-0.0.9/examples/notepad/forms/document-save-as.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/forms/document-save.png` & `pyqodeng-0.0.9/examples/notepad/forms/document-save.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/forms/main_window.ui` & `pyqodeng-0.0.9/examples/notepad/forms/main_window.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/forms/pyqode.png` & `pyqodeng-0.0.9/examples/notepad/forms/pyqode.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/freeze_setup.py` & `pyqodeng-0.0.9/examples/notepad/freeze_setup.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/notepad/__init__.py` & `pyqodeng-0.0.9/examples/notepad/notepad/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/notepad/editor.py` & `pyqodeng-0.0.9/examples/notepad/notepad/editor.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/notepad/forms/main_window_ui.py` & `pyqodeng-0.0.9/examples/notepad/notepad/forms/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/notepad/forms/resources_rc.py` & `pyqodeng-0.0.9/examples/notepad/notepad/forms/resources_rc.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/notepad/main_window.py` & `pyqodeng-0.0.9/examples/notepad/notepad/main_window.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/readme.rst` & `pyqodeng-0.0.9/examples/notepad/readme.rst`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/setup.iss` & `pyqodeng-0.0.9/examples/notepad/setup.iss`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/setup.py` & `pyqodeng-0.0.9/examples/notepad/setup.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/share/notepad.ico` & `pyqodeng-0.0.9/examples/notepad/share/notepad.ico`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/notepad/share/notepad.png` & `pyqodeng-0.0.9/examples/notepad/share/notepad.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/panels/checker.py` & `pyqodeng-0.0.9/examples/panels/checker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/panels/folding.py` & `pyqodeng-0.0.9/examples/panels/folding.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/panels/global_checker.py` & `pyqodeng-0.0.9/examples/panels/global_checker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/panels/line_numbers.py` & `pyqodeng-0.0.9/examples/panels/line_numbers.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/panels/search_and_replace.py` & `pyqodeng-0.0.9/examples/panels/search_and_replace.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/simple/basic.py` & `pyqodeng-0.0.9/examples/simple/basic.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/simple/custom_actions.py` & `pyqodeng-0.0.9/examples/simple/custom_actions.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/simple/style_and_settings.py` & `pyqodeng-0.0.9/examples/simple/style_and_settings.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/widgets/filesystem_treeview.py` & `pyqodeng-0.0.9/examples/widgets/filesystem_treeview.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/widgets/generic_code_edit.py` & `pyqodeng-0.0.9/examples/widgets/generic_code_edit.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/widgets/interactive_process.py` & `pyqodeng-0.0.9/examples/widgets/interactive_process.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/widgets/splittable_codeedit_tab_widget.py` & `pyqodeng-0.0.9/examples/widgets/splittable_codeedit_tab_widget.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/examples/widgets/splittable_tab_widget.py` & `pyqodeng-0.0.9/examples/widgets/splittable_tab_widget.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/dlg_encodings.ui` & `pyqodeng-0.0.9/forms/dlg_encodings.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/dlg_goto_line.ui` & `pyqodeng-0.0.9/forms/dlg_goto_line.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/dlg_preferred_encodings_editor.ui` & `pyqodeng-0.0.9/forms/dlg_preferred_encodings_editor.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/dlg_unsaved_files.ui` & `pyqodeng-0.0.9/forms/dlg_unsaved_files.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/pnl_encoding.ui` & `pyqodeng-0.0.9/forms/pnl_encoding.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/pnl_read_only.ui` & `pyqodeng-0.0.9/forms/pnl_read_only.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/popup_open_files.ui` & `pyqodeng-0.0.9/forms/popup_open_files.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/pyqode_core.qrc` & `pyqodeng-0.0.9/forms/pyqode_core.qrc`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/SourceCodePro-Bold.ttf` & `pyqodeng-0.0.9/forms/rc/SourceCodePro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/SourceCodePro-Regular.ttf` & `pyqodeng-0.0.9/forms/rc/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/clear-left.png` & `pyqodeng-0.0.9/forms/rc/clear-left.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/close.png` & `pyqodeng-0.0.9/forms/rc/close.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/dialog-error.png` & `pyqodeng-0.0.9/forms/rc/dialog-error.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/dialog-info.png` & `pyqodeng-0.0.9/forms/rc/dialog-info.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/dialog-warning.png` & `pyqodeng-0.0.9/forms/rc/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/document-save-as.png` & `pyqodeng-0.0.9/forms/rc/document-save-as.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/document-save.png` & `pyqodeng-0.0.9/forms/rc/document-save.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-copy.png` & `pyqodeng-0.0.9/forms/rc/edit-copy.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-cut.png` & `pyqodeng-0.0.9/forms/rc/edit-cut.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-delete.png` & `pyqodeng-0.0.9/forms/rc/edit-delete.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-find-replace.png` & `pyqodeng-0.0.9/forms/rc/edit-find-replace.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-find.png` & `pyqodeng-0.0.9/forms/rc/edit-find.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-paste.png` & `pyqodeng-0.0.9/forms/rc/edit-paste.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-redo.png` & `pyqodeng-0.0.9/forms/rc/edit-redo.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-select-all.png` & `pyqodeng-0.0.9/forms/rc/edit-select-all.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-trash.png` & `pyqodeng-0.0.9/forms/rc/edit-trash.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/edit-undo.png` & `pyqodeng-0.0.9/forms/rc/edit-undo.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/format-indent-less.png` & `pyqodeng-0.0.9/forms/rc/format-indent-less.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/format-indent-more.png` & `pyqodeng-0.0.9/forms/rc/format-indent-more.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/go-down.png` & `pyqodeng-0.0.9/forms/rc/go-down.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/go-next.png` & `pyqodeng-0.0.9/forms/rc/go-next.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/go-previous.png` & `pyqodeng-0.0.9/forms/rc/go-previous.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/go-up.png` & `pyqodeng-0.0.9/forms/rc/go-up.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/rc/goto-line.png` & `pyqodeng-0.0.9/forms/rc/goto-line.png`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/forms/search_panel.ui` & `pyqodeng-0.0.9/forms/search_panel.ui`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/__init__.py` & `pyqodeng-0.0.9/pyqodeng/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 It contains the base classes for both the backend and the frontend and provides
 a series of modes and panels that might be useful for any kind of code editor
 widget, i.e. pyqode.core is a generic code editor widget.
 """
 import logging
 
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 
 logging.addLevelName(1, "PYQODEDEBUGCOMM")
 logging.addLevelName(5, "PYQODEDEBUG")
 
 
 try:
```

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_designer_plugins/__init__.py` & `pyqodeng-0.0.9/pyqodeng/core/_designer_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/dlg_encodings_ui.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/dlg_encodings_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/dlg_goto_line_ui.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/dlg_goto_line_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/dlg_preferred_encodings_editor_ui.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/dlg_preferred_encodings_editor_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/dlg_unsaved_files_ui.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/dlg_unsaved_files_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/pnl_encoding_ui.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/pnl_encoding_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/pnl_read_only_ui.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/pnl_read_only_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/popup_open_files_ui.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/popup_open_files_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/pyqode_core_rc.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/pyqode_core_rc.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/_forms/search_panel_ui.py` & `pyqodeng-0.0.9/pyqodeng/core/_forms/search_panel_ui.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/__init__.py` & `pyqodeng-0.0.9/pyqodeng/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/client.py` & `pyqodeng-0.0.9/pyqodeng/core/api/client.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/code_edit.py` & `pyqodeng-0.0.9/pyqodeng/core/api/code_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -884,20 +884,25 @@
         signal, the :class:`pyqode.core.modes.IndenterMode` will
         perform the actual un-indentation.
         """
         self.unindent_requested.emit()
 
     def eventFilter(self, obj, event):
         if obj == self and event.type() == QtCore.QEvent.KeyPress:
-            if event.key() == QtCore.Qt.Key_X and \
-                    int(event.modifiers()) == QtCore.Qt.ControlModifier:
+            modifiers = event.modifiers()
+            if event.key() == QtCore.Qt.Key_X and (
+                    modifiers == QtCore.Qt.ControlModifier if isinstance(modifiers, int)
+                    else modifiers & QtCore.Qt.ControlModifier
+            ):
                 self.cut()
                 return True
-            if event.key() == QtCore.Qt.Key_C and \
-                    int(event.modifiers()) == QtCore.Qt.ControlModifier:
+            if event.key() == QtCore.Qt.Key_C and (
+                    modifiers == QtCore.Qt.ControlModifier if isinstance(modifiers, int)
+                    else modifiers & QtCore.Qt.ControlModifier
+            ):
                 self.copy()
                 return True
         return False
 
     def cut(self):
         """
         Cuts the selected text or the whole line if no text was selected. When
@@ -1017,26 +1022,30 @@
         :param event: QKeyEvent
         """
         initial_state = event.isAccepted()
         event.ignore()
         self.key_pressed.emit(event)
         state = event.isAccepted()
         if not event.isAccepted():
-            if event.key() == QtCore.Qt.Key_Tab and event.modifiers() == \
-                    QtCore.Qt.NoModifier:
+            modifiers = event.modifiers()
+            if event.key() == QtCore.Qt.Key_Tab and modifiers == QtCore.Qt.NoModifier:
                 self.indent()
                 event.accept()
-            elif event.key() == QtCore.Qt.Key_Backtab and \
-                    event.modifiers() == QtCore.Qt.NoModifier:
+            elif event.key() == QtCore.Qt.Key_Backtab and modifiers == QtCore.Qt.NoModifier:
                 self.un_indent()
                 event.accept()
-            elif event.key() == QtCore.Qt.Key_Home and \
-                    int(event.modifiers()) & QtCore.Qt.ControlModifier == 0:
+            elif event.key() == QtCore.Qt.Key_Home and (
+                    modifiers & QtCore.Qt.ControlModifier == 0 if isinstance(modifiers, int)
+                    else bool(modifiers & QtCore.Qt.ControlModifier) is False
+            ):
                 self._do_home_key(
-                    event, int(event.modifiers()) & QtCore.Qt.ShiftModifier)
+                    event,
+                    modifiers & QtCore.Qt.ShiftModifier if isinstance(modifiers, int)
+                    else bool(modifiers & QtCore.Qt.ShiftModifier)
+                )
             if not event.isAccepted():
                 event.setAccepted(initial_state)
                 super(CodeEdit, self).keyPressEvent(event)
         new_state = event.isAccepted()
         event.setAccepted(state)
         self.post_key_pressed.emit(event)
         event.setAccepted(new_state)
```

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/decoration.py` & `pyqodeng-0.0.9/pyqodeng/core/api/decoration.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/encodings.py` & `pyqodeng-0.0.9/pyqodeng/core/api/encodings.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/folding.py` & `pyqodeng-0.0.9/pyqodeng/core/api/folding.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/manager.py` & `pyqodeng-0.0.9/pyqodeng/core/api/manager.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/mode.py` & `pyqodeng-0.0.9/pyqodeng/core/api/mode.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/panel.py` & `pyqodeng-0.0.9/pyqodeng/core/api/panel.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/syntax_highlighter.py` & `pyqodeng-0.0.9/pyqodeng/core/api/syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/api/utils.py` & `pyqodeng-0.0.9/pyqodeng/core/api/utils.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/backend/__init__.py` & `pyqodeng-0.0.9/pyqodeng/core/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/backend/server.py` & `pyqodeng-0.0.9/pyqodeng/core/backend/server.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/backend/workers.py` & `pyqodeng-0.0.9/pyqodeng/core/backend/workers.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/cache.py` & `pyqodeng-0.0.9/pyqodeng/core/cache.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/dialogs/encodings.py` & `pyqodeng-0.0.9/pyqodeng/core/dialogs/encodings.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/dialogs/goto.py` & `pyqodeng-0.0.9/pyqodeng/core/dialogs/goto.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/dialogs/unsaved_files.py` & `pyqodeng-0.0.9/pyqodeng/core/dialogs/unsaved_files.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/icons.py` & `pyqodeng-0.0.9/pyqodeng/core/icons.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/managers/__init__.py` & `pyqodeng-0.0.9/pyqodeng/core/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/managers/backend.py` & `pyqodeng-0.0.9/pyqodeng/core/managers/backend.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/managers/decorations.py` & `pyqodeng-0.0.9/pyqodeng/core/managers/decorations.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/managers/file.py` & `pyqodeng-0.0.9/pyqodeng/core/managers/file.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/managers/modes.py` & `pyqodeng-0.0.9/pyqodeng/core/managers/modes.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/managers/panels.py` & `pyqodeng-0.0.9/pyqodeng/core/managers/panels.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/__init__.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/autocomplete.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/autocomplete.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/autoindent.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/autoindent.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/backspace.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/backspace.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/caret_line_highlight.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/caret_line_highlight.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/case_converter.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/case_converter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/checker.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/checker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/code_completion.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/code_completion.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/cursor_history.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/cursor_history.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/extended_selection.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/extended_selection.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/filewatcher.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/filewatcher.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/indenter.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/indenter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/line_highlighter.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/line_highlighter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/matcher.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/matcher.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/occurences.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/occurences.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/outline.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/outline.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/pygments_sh.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/pygments_sh.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/right_margin.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/right_margin.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/wordclick.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/wordclick.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/modes/zoom.py` & `pyqodeng-0.0.9/pyqodeng/core/modes/zoom.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/__init__.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/checker.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/checker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/encodings.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/encodings.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/folding.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/folding.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/global_checker.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/global_checker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/line_number.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/line_number.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/marker.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/marker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/read_only.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/read_only.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/panels/search_and_replace.py` & `pyqodeng-0.0.9/pyqodeng/core/panels/search_and_replace.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/share.py` & `pyqodeng-0.0.9/pyqodeng/core/share.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/styles/darcula.py` & `pyqodeng-0.0.9/pyqodeng/core/styles/darcula.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/styles/qt.py` & `pyqodeng-0.0.9/pyqodeng/core/styles/qt.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/tools/console.py` & `pyqodeng-0.0.9/pyqodeng/core/tools/console.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/__init__.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/_pty.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/_pty.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/code_edits.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/code_edits.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/encodings.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/encodings.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/errors_table.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/errors_table.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/file_icons_provider.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/file_icons_provider.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/filesystem_treeview.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/filesystem_treeview.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/interactive.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/menu_recents.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/menu_recents.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/outline.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/outline.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/output_window.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/output_window.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/preview.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/preview.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/prompt_line_edit.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/prompt_line_edit.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/splittable_tab_widget.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/splittable_tab_widget.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/tab_bar.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/tabs.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng/core/widgets/terminal.py` & `pyqodeng-0.0.9/pyqodeng/core/widgets/terminal.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/pyqodeng.egg-info/PKG-INFO` & `pyqodeng-0.0.9/pyqodeng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqodeng
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyQt/PySide Source Code Editor Widget
 Home-page: https://github.com/angr/pyqodeng
 Author: Colin Duquesnoy and others
 Author-email: colin.duquesnoy@gmail.com
 License: MIT
 Keywords: CodeEdit PyQt source code editor widget qt
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyqodeng-0.0.8/pyqodeng.egg-info/SOURCES.txt` & `pyqodeng-0.0.9/pyqodeng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/setup.py` & `pyqodeng-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/helpers.py` & `pyqodeng-0.0.9/test/helpers.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/server.py` & `pyqodeng-0.0.9/test/server.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_api/test_code_edit.py` & `pyqodeng-0.0.9/test/test_api/test_code_edit.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_api/test_decoration.py` & `pyqodeng-0.0.9/test/test_api/test_decoration.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_api/test_extension.py` & `pyqodeng-0.0.9/test/test_api/test_extension.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_api/test_folding.py` & `pyqodeng-0.0.9/test/test_api/test_folding.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_api/test_text.py` & `pyqodeng-0.0.9/test/test_api/test_text.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_api/test_utils.py` & `pyqodeng-0.0.9/test/test_api/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_backend/test_workers.py` & `pyqodeng-0.0.9/test/test_backend/test_workers.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_cache.py` & `pyqodeng-0.0.9/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_managers/test_backend.py` & `pyqodeng-0.0.9/test/test_managers/test_backend.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_managers/test_file_manager.py` & `pyqodeng-0.0.9/test/test_managers/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_autocomplete.py` & `pyqodeng-0.0.9/test/test_modes/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_autoindent.py` & `pyqodeng-0.0.9/test/test_modes/test_autoindent.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_backspace.py` & `pyqodeng-0.0.9/test/test_modes/test_backspace.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_caret_line_highlight.py` & `pyqodeng-0.0.9/test/test_modes/test_caret_line_highlight.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_checker.py` & `pyqodeng-0.0.9/test/test_modes/test_checker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_code_completion.py` & `pyqodeng-0.0.9/test/test_modes/test_code_completion.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_extended_selection.py` & `pyqodeng-0.0.9/test/test_modes/test_extended_selection.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_filewatcher.py` & `pyqodeng-0.0.9/test/test_modes/test_filewatcher.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_indenter.py` & `pyqodeng-0.0.9/test/test_modes/test_indenter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_matcher.py` & `pyqodeng-0.0.9/test/test_modes/test_matcher.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_occurrences.py` & `pyqodeng-0.0.9/test/test_modes/test_occurrences.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_pygments_highlighter.py` & `pyqodeng-0.0.9/test/test_modes/test_pygments_highlighter.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_right_margin.py` & `pyqodeng-0.0.9/test/test_modes/test_right_margin.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_word_click.py` & `pyqodeng-0.0.9/test/test_modes/test_word_click.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_modes/test_zoom.py` & `pyqodeng-0.0.9/test/test_modes/test_zoom.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_panels/test_checker.py` & `pyqodeng-0.0.9/test/test_panels/test_checker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_panels/test_encoding.py` & `pyqodeng-0.0.9/test/test_panels/test_encoding.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_panels/test_folding.py` & `pyqodeng-0.0.9/test/test_panels/test_folding.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_panels/test_line_nbr.py` & `pyqodeng-0.0.9/test/test_panels/test_line_nbr.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_panels/test_marker.py` & `pyqodeng-0.0.9/test/test_panels/test_marker.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_panels/test_search_and_replace.py` & `pyqodeng-0.0.9/test/test_panels/test_search_and_replace.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_widgets/parsed_output.txt` & `pyqodeng-0.0.9/test/test_widgets/parsed_output.txt`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_widgets/raw_output.txt` & `pyqodeng-0.0.9/test/test_widgets/raw_output.txt`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_widgets/test_output_window.py` & `pyqodeng-0.0.9/test/test_widgets/test_output_window.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_widgets/test_recent_files.py` & `pyqodeng-0.0.9/test/test_widgets/test_recent_files.py`

 * *Files identical despite different names*

### Comparing `pyqodeng-0.0.8/test/test_widgets/test_splittable_tab_widget.py` & `pyqodeng-0.0.9/test/test_widgets/test_splittable_tab_widget.py`

 * *Files identical despite different names*

