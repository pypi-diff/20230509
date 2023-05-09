# Comparing `tmp/halig-0.2.2.tar.gz` & `tmp/halig-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halig-0.2.2.tar", last modified: Tue May  9 07:57:38 2023, max compression
+gzip compressed data, was "halig-0.3.0.tar", last modified: Tue May  9 18:30:22 2023, max compression
```

## Comparing `halig-0.2.2.tar` & `halig-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34670 2023-04-12 19:46:50.194310 halig-0.2.2/LICENSE
--rw-r--r--   0        0        0     1632 2023-05-09 07:04:54.570369 halig-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.2.2/halig/__init__.py
--rw-r--r--   0        0        0       22 2023-05-09 07:53:56.492340 halig-0.2.2/halig/__version__.py
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.2.2/halig/commands/__init__.py
--rw-r--r--   0        0        0      292 2023-04-12 19:47:22.382591 halig-0.2.2/halig/commands/base.py
--rw-r--r--   0        0        0     2781 2023-05-09 06:48:39.717700 halig-0.2.2/halig/commands/edit.py
--rw-r--r--   0        0        0     1076 2023-04-12 19:47:22.382591 halig-0.2.2/halig/commands/notebooks.py
--rw-r--r--   0        0        0     1199 2023-04-12 19:47:22.382591 halig-0.2.2/halig/commands/show.py
--rw-r--r--   0        0        0     1418 2023-05-09 06:54:08.876599 halig-0.2.2/halig/encryption.py
--rw-r--r--   0        0        0     1354 2023-05-08 19:32:21.621775 halig-0.2.2/halig/literals.py
--rw-r--r--   0        0        0     2868 2023-05-08 20:59:47.779605 halig-0.2.2/halig/main.py
--rw-r--r--   0        0        0     3482 2023-05-09 07:56:30.411843 halig-0.2.2/halig/settings.py
--rw-r--r--   0        0        0      733 2023-05-08 21:12:42.122646 halig-0.2.2/halig/utils.py
--rw-r--r--   0        0        0     2656 2023-05-09 07:57:38.483623 halig-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.202310 halig-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 19:47:22.382591 halig-0.2.2/tests/commands/__init__.py
--rw-r--r--   0        0        0     1645 2023-04-24 10:55:32.886664 halig-0.2.2/tests/commands/conftest.py
--rw-r--r--   0        0        0     1168 2023-04-24 10:55:32.886664 halig-0.2.2/tests/commands/test_edit.py
--rw-r--r--   0        0        0     1563 2023-04-24 10:55:32.886664 halig-0.2.2/tests/commands/test_notebooks.py
--rw-r--r--   0        0        0     1141 2023-04-24 10:55:32.886664 halig-0.2.2/tests/commands/test_show.py
--rw-r--r--   0        0        0     2820 2023-04-12 19:47:22.382591 halig-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     2276 2023-05-09 06:28:25.521779 halig-0.2.2/tests/test_encryption.py
--rw-r--r--   0        0        0     1541 2023-04-12 19:47:22.386591 halig-0.2.2/tests/test_settings.py
--rw-r--r--   0        0        0     1482 2023-04-24 10:55:32.886664 halig-0.2.2/tests/test_utils.py
--rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 halig-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34670 2023-04-12 19:46:50.194310 halig-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1633 2023-05-09 17:54:18.830294 halig-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.3.0/halig/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-09 18:28:41.005848 halig-0.3.0/halig/__version__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.3.0/halig/commands/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-12 19:47:22.382591 halig-0.3.0/halig/commands/base.py
+-rw-r--r--   0        0        0     2781 2023-05-09 06:48:39.717700 halig-0.3.0/halig/commands/edit.py
+-rw-r--r--   0        0        0     1076 2023-04-12 19:47:22.382591 halig-0.3.0/halig/commands/notebooks.py
+-rw-r--r--   0        0        0     1199 2023-04-12 19:47:22.382591 halig-0.3.0/halig/commands/show.py
+-rw-r--r--   0        0        0     1418 2023-05-09 18:17:46.623174 halig-0.3.0/halig/encryption.py
+-rw-r--r--   0        0        0     1354 2023-05-08 19:32:21.621775 halig-0.3.0/halig/literals.py
+-rw-r--r--   0        0        0     2868 2023-05-08 20:59:47.779605 halig-0.3.0/halig/main.py
+-rw-r--r--   0        0        0     3454 2023-05-09 18:26:48.286072 halig-0.3.0/halig/settings.py
+-rw-r--r--   0        0        0      733 2023-05-08 21:12:42.122646 halig-0.3.0/halig/utils.py
+-rw-r--r--   0        0        0     2656 2023-05-09 18:30:22.105654 halig-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.202310 halig-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:47:22.382591 halig-0.3.0/tests/commands/__init__.py
+-rw-r--r--   0        0        0     1645 2023-04-24 10:55:32.886664 halig-0.3.0/tests/commands/conftest.py
+-rw-r--r--   0        0        0     1168 2023-05-09 17:58:32.738050 halig-0.3.0/tests/commands/test_edit.py
+-rw-r--r--   0        0        0     1563 2023-04-24 10:55:32.886664 halig-0.3.0/tests/commands/test_notebooks.py
+-rw-r--r--   0        0        0     1141 2023-04-24 10:55:32.886664 halig-0.3.0/tests/commands/test_show.py
+-rw-r--r--   0        0        0     2820 2023-04-12 19:47:22.382591 halig-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     2276 2023-05-09 06:28:25.521779 halig-0.3.0/tests/test_encryption.py
+-rw-r--r--   0        0        0     1541 2023-04-12 19:47:22.386591 halig-0.3.0/tests/test_settings.py
+-rw-r--r--   0        0        0     1482 2023-04-24 10:55:32.886664 halig-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 halig-0.3.0/PKG-INFO
```

### Comparing `halig-0.2.2/LICENSE` & `halig-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/README.md` & `halig-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ssh-keygen -t ed25519
 mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/halig"
 cat << EOF > "${XDG_CONFIG_HOME:-$HOME/.config}/halig/halig.yml"
 ---
 notebooks_root_path: ~/Documents/Notebooks
 identity_paths: 
   - ~/.ssh/id_ed25519
-recipient_path:
+recipient_paths:
   - ~/.ssh/id_ed25519.pub
   - https://github.com/<username>.keys
   - https://gitlab.com/<username>.keys
 EOF
 ```
 
 ## Usage TLDR
```

### Comparing `halig-0.2.2/halig/commands/edit.py` & `halig-0.3.0/halig/commands/edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/halig/commands/notebooks.py` & `halig-0.3.0/halig/commands/notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/halig/commands/show.py` & `halig-0.3.0/halig/commands/show.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/halig/encryption.py` & `halig-0.3.0/halig/encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/halig/literals.py` & `halig-0.3.0/halig/literals.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/halig/main.py` & `halig-0.3.0/halig/main.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/halig/settings.py` & `halig-0.3.0/halig/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,24 +28,23 @@
     recipient_paths: list[FilePath | HttpUrl] = [
         Path("~/.ssh/id_ed25519.pub").expanduser(),
     ]
 
     @validator("identity_paths", "recipient_paths", pre=True)
     def validate_paths(cls, v: Any):  # noqa: N805
         if not isinstance(v, list):
-            return v
+            v = [v]
         new_v = []
         for path in v:
-            if isinstance(path, str):
-                if not path.startswith("http"):
-                    new_v.append(Path(path).expanduser())
-            elif isinstance(path, Path):
-                new_v.append(path.expanduser())
-            else:
-                new_v.append(path)
+            new_path = path
+            if isinstance(path, str) and not path.startswith("http"):
+                new_path = Path(path)
+            new_v.append(
+                new_path.expanduser() if isinstance(new_path, Path) else new_path,
+            )
         return new_v
 
     @validator("notebooks_root_path", pre=True)
     def validate_notebooks_path(cls, v: Any):  # noqa: N805
         if isinstance(v, str):
             return Path(v).expanduser()
         if isinstance(v, Path):
```

### Comparing `halig-0.2.2/halig/utils.py` & `halig-0.3.0/halig/utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/pyproject.toml` & `halig-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Terminals",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-version = "0.2.2"
+version = "0.3.0"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "https://git.roboces.dev/catalin/halig"
 Repository = "https://git.roboces.dev/catalin/halig"
```

### Comparing `halig-0.2.2/tests/commands/conftest.py` & `halig-0.3.0/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/tests/commands/test_edit.py` & `halig-0.3.0/tests/commands/test_edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/tests/commands/test_notebooks.py` & `halig-0.3.0/tests/commands/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/tests/commands/test_show.py` & `halig-0.3.0/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/tests/conftest.py` & `halig-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/tests/test_encryption.py` & `halig-0.3.0/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/tests/test_settings.py` & `halig-0.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/tests/test_utils.py` & `halig-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.2/PKG-INFO` & `halig-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halig
-Version: 0.2.2
+Version: 0.3.0
 Summary: age-encrypted, file-based, note-taking CLI app
 Keywords: cli notes age rage encryption notebook
 Author-Email: cătălin <185504a9@duck.com>
 License: GPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -83,15 +83,15 @@
 ssh-keygen -t ed25519
 mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/halig"
 cat << EOF > "${XDG_CONFIG_HOME:-$HOME/.config}/halig/halig.yml"
 ---
 notebooks_root_path: ~/Documents/Notebooks
 identity_paths: 
   - ~/.ssh/id_ed25519
-recipient_path:
+recipient_paths:
   - ~/.ssh/id_ed25519.pub
   - https://github.com/<username>.keys
   - https://gitlab.com/<username>.keys
 EOF
 ```
 
 ## Usage TLDR
```

