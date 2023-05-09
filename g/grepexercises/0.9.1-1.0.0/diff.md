# Comparing `tmp/grepexercises-0.9.1.tar.gz` & `tmp/grepexercises-1.0.0.tar.gz`

## Comparing `grepexercises-0.9.1.tar` & `grepexercises-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/__init__.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/app_guide.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/grep_exercises.css
--rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/grep_exercises.py
--rw-r--r--   0        0        0    33047 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/questions.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/user_progress.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/.hidden
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/code.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/colors_1
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/colors_2.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/lines.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/nul_separated
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/patterns.txt
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/pcre.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/regex_terms.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/sample.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/substitute.sh
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/terms.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/backups/color list.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/backups/dot_files/.bash_aliases
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/backups/dot_files/.inputrc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/projects/python/hello.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/projects/shell/hello.sh
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 grepexercises-0.9.1/LICENSE
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 grepexercises-0.9.1/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 grepexercises-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 grepexercises-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/__init__.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/app_guide.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/grep_exercises.css
+-rw-r--r--   0        0        0    10002 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/grep_exercises.py
+-rw-r--r--   0        0        0    33176 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/questions.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/user_progress.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/.hidden
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/code.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/colors_1
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/colors_2.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/lines.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/nul_separated
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/patterns.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/pcre.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/regex_terms.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/sample.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/substitute.sh
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/terms.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/backups/color list.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/backups/dot_files/.bash_aliases
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/backups/dot_files/.inputrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/projects/python/hello.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-1.0.0/src/grepexercises/sample_input/projects/shell/hello.sh
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 grepexercises-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 grepexercises-1.0.0/README.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 grepexercises-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 grepexercises-1.0.0/PKG-INFO
```

### Comparing `grepexercises-0.9.1/src/grepexercises/app_guide.md` & `grepexercises-1.0.0/src/grepexercises/app_guide.md`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.1/src/grepexercises/grep_exercises.css` & `grepexercises-1.0.0/src/grepexercises/grep_exercises.css`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.1/src/grepexercises/grep_exercises.py` & `grepexercises-1.0.0/src/grepexercises/grep_exercises.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,15 @@
             idx = 2
         self.b_tabs[idx].variant = 'warning'
 
     def on_directory_tree_file_selected(self, event):
         path = event.path
         with open(path, encoding='ascii') as f:
             self.l_viewfile.update(self.trim(f.read()))
-            self.l_viewfile.border_title = path
+            self.l_viewfile.border_title = str(path)
 
     def l_ref_solution_clear(self):
         self.l_ref_solution.update('')
         self.l_ref_solution.styles.border = ('none', 'green')
 
     def action_show_solution(self):
         self.l_ref_solution.update('\n'.join(self.ref_solution))
```

### Comparing `grepexercises-0.9.1/src/grepexercises/questions.json` & `grepexercises-1.0.0/src/grepexercises/questions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978535353535356%*

 * *Differences: {"'17'": "{'question': 'For the input file `patterns.txt`, match all lines that start with `den` "*

 * *         "or end with `ly`.'}",*

 * * "'22'": '{\'ref_solution\': {insert: [(0, "grep -xE \'(\\\\w)(.*\\\\1)?\' patterns.txt"), (2, "rg '*

 * *         '-xNP \'(\\\\w)(.*\\\\1)?\' patterns.txt")]}}',*

 * * "'28'": '{\'ref_solution\': {insert: [(0, "grep -o \'\\\\-\\\\w*$\' patterns.txt"), (2, "rg -No '*

 * *         '\'\\\\-\\\\w*$\' patterns.txt")]}}',*

 * * "'47'": "{'ref_solution': {delete: [1]}}",*

 * * "'49'": '{\'ref_solution\': {ins […]*

```diff
@@ -104,15 +104,15 @@
         "sort_op": false
     },
     "17": {
         "ip_file": [
             "patterns.txt"
         ],
         "op_file": "2 lonely\ndent\nlovely\n",
-        "question": "For the input file `patterns.txt`, match all lines that start with `den` or end with `ly`",
+        "question": "For the input file `patterns.txt`, match all lines that start with `den` or end with `ly`.",
         "ref_solution": [
             "grep -E '^den|ly$' patterns.txt",
             "rg -N '^den|ly$' patterns.txt"
         ],
         "sort_op": false
     },
     "18": {
@@ -178,15 +178,17 @@
     "22": {
         "ip_file": [
             "patterns.txt"
         ],
         "op_file": "sets tests\nNot a pip DOWN\ny\n1 dentist 1\n_42_\n",
         "question": "From the input file `patterns.txt`, extract all whole lines having the same first and last word character.",
         "ref_solution": [
+            "grep -xE '(\\w)(.*\\1)?' patterns.txt",
             "grep -xE '\\w|(\\w).*\\1' patterns.txt",
+            "rg -xNP '(\\w)(.*\\1)?' patterns.txt",
             "rg -xNP '\\w|(\\w).*\\1' patterns.txt"
         ],
         "sort_op": false
     },
     "23": {
         "ip_file": [
             "patterns.txt"
@@ -251,15 +253,17 @@
     "28": {
         "ip_file": [
             "patterns.txt"
         ],
         "op_file": "-handy\n-icy\n",
         "question": "From the input file `patterns.txt`, extract from `-` till the end of the line, provided the characters after the hyphen are all word characters only.",
         "ref_solution": [
+            "grep -o '\\-\\w*$' patterns.txt",
             "grep -o -- '-\\w*$' patterns.txt",
+            "rg -No '\\-\\w*$' patterns.txt",
             "rg -No -- '-\\w*$' patterns.txt"
         ],
         "sort_op": false
     },
     "29": {
         "ip_file": [
             "patterns.txt"
@@ -486,15 +490,14 @@
     },
     "47": {
         "ip_file": [],
         "op_file": "projects/shell/hello.sh\n.hidden\ncolors_1\nsample.txt\ncolors_2.txt\nhello.py\n",
         "question": "Search recursively and list the names of files that contain `Hello` or `blue`. Hidden files and symbolic links should be searched as well. Do not search within `python` or `backups` directories.",
         "ref_solution": [
             "grep -RlE --exclude-dir='python' --exclude-dir='backups' 'Hello|blue'",
-            "grep -RlE --exclude-dir={python,backups} 'Hello|blue'",
             "rg --hidden -lL -g '!{python,backups}' 'Hello|blue'"
         ],
         "sort_op": true
     },
     "48": {
         "ip_file": [],
         "op_file": "61\n",
@@ -507,15 +510,15 @@
     },
     "49": {
         "ip_file": [],
         "op_file": "colors_2.txt:red\nhello.py:    print(\"Hello, Python!\")\npatterns.txt:refused reed redo received\npatterns.txt:refused refused and retired\nsample.txt:Hello World\n",
         "question": "Display lines containing `Hello` or `red` only from files in the current hierarchy, i.e. don't search recursively. Hidden files and symbolic links should be searched as well.",
         "ref_solution": [
             "grep -d skip 'Hello\\|red' *",
-            "rg --hidden --no-heading -NL -g '!*/*' 'Hello|red'",
+            "rg --hidden --no-heading -NL -g '!*/' 'Hello|red'",
             "rg --hidden --no-heading -NL --max-depth 1 'Hello|red'"
         ],
         "sort_op": true
     },
     "5": {
         "ip_file": [
             "sample.txt"
```

### Comparing `grepexercises-0.9.1/src/grepexercises/sample_input/patterns.txt` & `grepexercises-1.0.0/src/grepexercises/sample_input/patterns.txt`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.1/LICENSE` & `grepexercises-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.1/README.md` & `grepexercises-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.1/pyproject.toml` & `grepexercises-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "grepexercises"
-version = "0.9.1"
+version = "1.0.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "50+ exercises for GNU grep (or alternatives like ripgrep)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "textual>=0.22.3",
+  "textual>=0.24.1",
 ]
 
 [project.scripts]
 grepexercises = "grepexercises.grep_exercises:main"
 
 [project.urls]
 "Source" = "https://github.com/learnbyexample/TUI-apps/tree/main/GrepExercises"
```

### Comparing `grepexercises-0.9.1/PKG-INFO` & `grepexercises-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: grepexercises
-Version: 0.9.1
+Version: 1.0.0
 Summary: 50+ exercises for GNU grep (or alternatives like ripgrep)
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/GrepExercises
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: textual>=0.22.3
+Requires-Dist: textual>=0.24.1
 Description-Content-Type: text/markdown
 
 # Grep Exercises
 
 This TUI application includes 50+ questions meant to be solved using `GNU grep` (or alternate implementations like `ripgrep`). Some exercises will require you to combine `grep` with other standard commands such as `cat`, `wc` and `find`.
 
 > **Note:** This application is intended to be run in a Linux-like environment. You might still be able to solve the exercises on other platforms, but I do not know if that'll work.
```

