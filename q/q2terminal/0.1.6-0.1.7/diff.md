# Comparing `tmp/q2terminal-0.1.6.tar.gz` & `tmp/q2terminal-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2terminal-0.1.6.tar", max compression
+gzip compressed data, was "q2terminal-0.1.7.tar", max compression
```

## Comparing `q2terminal-0.1.6.tar` & `q2terminal-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      384 2023-05-07 20:23:34.343483 q2terminal-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2424 2023-05-07 20:22:00.315642 q2terminal-0.1.6/q2terminal/q2terminal.py
--rw-r--r--   0        0        0       21 2023-05-07 20:23:36.403703 q2terminal-0.1.6/q2terminal/version.py
--rw-r--r--   0        0        0      523 2023-05-06 22:10:01.827611 q2terminal-0.1.6/README.md
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 q2terminal-0.1.6/setup.py
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 q2terminal-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      384 2023-05-09 10:02:36.679482 q2terminal-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2421 2023-05-08 11:48:24.661192 q2terminal-0.1.7/q2terminal/q2terminal.py
+-rw-r--r--   0        0        0       21 2023-05-09 10:02:40.549764 q2terminal-0.1.7/q2terminal/version.py
+-rw-r--r--   0        0        0      523 2023-05-06 22:10:01.827611 q2terminal-0.1.7/README.md
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 q2terminal-0.1.7/setup.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 q2terminal-0.1.7/PKG-INFO
```

### Comparing `q2terminal-0.1.6/q2terminal/q2terminal.py` & `q2terminal-0.1.7/q2terminal/q2terminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if terminal is None:
             if "win32" in sys.platform:
                 terminal = "powershell"
             elif "darwin" in sys.platform:
                 terminal = "zsh"
             else:
                 terminal = "bash"
-        if "win32" not in sys.platform:
+        if "win32" in sys.platform:
             self.shell = True
         self.proc = Popen(
             [terminal],
             shell=self.shell,
             stdin=PIPE,
             stdout=PIPE,
             stderr=STDOUT,
@@ -61,13 +61,13 @@
             elif line == "":
                 continue
             else:
                 rez.append(line)
                 if echo or self.echo:
                     print(f"{ctime()}:\t{line}")
                 if callable(_callback):
-                    callback(line)
+                    _callback(line)
 
         return rez
 
     def close(self):
         self.proc.terminate()
```

### Comparing `q2terminal-0.1.6/README.md` & `q2terminal-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `q2terminal-0.1.6/setup.py` & `q2terminal-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['q2terminal']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'q2terminal',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '',
     'long_description': '[![Python application](https://github.com/AndreiPuchko/q2terminal/actions/workflows/main.yml/badge.svg)](https://github.com/AndreiPuchko/q2terminal/actions/workflows/main.yml)\n# Interaction with a terminal session\n\n```python\nfrom q2terminal.q2terminal import Q2Terminal\nimport sys\n\nt = Q2Terminal()\nt.run("programm", echo=True)\nassert t.exit_code != 0\n\nassert t.run("$q2 = 123") == []\nassert t.run("echo $q2") == ["123"]\n\n\nif "win32" in sys.platform:\n    t.run("notepad")\n    assert t.exit_code == 0\n```\n',
     'author': 'Andrei Puchko',
     'author_email': 'andrei.puchko@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `q2terminal-0.1.6/PKG-INFO` & `q2terminal-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2terminal
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

