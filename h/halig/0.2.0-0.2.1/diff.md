# Comparing `tmp/halig-0.2.0.tar.gz` & `tmp/halig-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halig-0.2.0.tar", last modified: Mon Apr 24 11:57:28 2023, max compression
+gzip compressed data, was "halig-0.2.1.tar", last modified: Tue May  9 07:11:08 2023, max compression
```

## Comparing `halig-0.2.0.tar` & `halig-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34670 2023-04-12 19:46:50.194310 halig-0.2.0/LICENSE
--rw-r--r--   0        0        0     1248 2023-04-24 10:55:32.886664 halig-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.2.0/halig/__init__.py
--rw-r--r--   0        0        0       22 2023-04-24 11:57:00.923504 halig-0.2.0/halig/__version__.py
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.2.0/halig/commands/__init__.py
--rw-r--r--   0        0        0      292 2023-04-12 19:47:22.382591 halig-0.2.0/halig/commands/base.py
--rw-r--r--   0        0        0     2767 2023-04-12 19:47:22.382591 halig-0.2.0/halig/commands/edit.py
--rw-r--r--   0        0        0     1076 2023-04-12 19:47:22.382591 halig-0.2.0/halig/commands/notebooks.py
--rw-r--r--   0        0        0     1199 2023-04-12 19:47:22.382591 halig-0.2.0/halig/commands/show.py
--rw-r--r--   0        0        0     1391 2023-04-12 19:47:22.382591 halig-0.2.0/halig/encryption.py
--rw-r--r--   0        0        0     1354 2023-04-12 19:47:22.382591 halig-0.2.0/halig/literals.py
--rw-r--r--   0        0        0     2868 2023-04-24 11:57:00.923504 halig-0.2.0/halig/main.py
--rw-r--r--   0        0        0     1855 2023-04-12 19:47:22.382591 halig-0.2.0/halig/settings.py
--rw-r--r--   0        0        0      733 2023-04-12 19:47:22.382591 halig-0.2.0/halig/utils.py
--rw-r--r--   0        0        0     2623 2023-04-24 11:57:28.359440 halig-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.202310 halig-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 19:47:22.382591 halig-0.2.0/tests/commands/__init__.py
--rw-r--r--   0        0        0     1645 2023-04-24 10:55:32.886664 halig-0.2.0/tests/commands/conftest.py
--rw-r--r--   0        0        0     1168 2023-04-24 10:55:32.886664 halig-0.2.0/tests/commands/test_edit.py
--rw-r--r--   0        0        0     1563 2023-04-24 10:55:32.886664 halig-0.2.0/tests/commands/test_notebooks.py
--rw-r--r--   0        0        0     1141 2023-04-24 10:55:32.886664 halig-0.2.0/tests/commands/test_show.py
--rw-r--r--   0        0        0     2820 2023-04-12 19:47:22.382591 halig-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1784 2023-04-12 19:47:22.382591 halig-0.2.0/tests/test_encryption.py
--rw-r--r--   0        0        0     1541 2023-04-12 19:47:22.386591 halig-0.2.0/tests/test_settings.py
--rw-r--r--   0        0        0     1482 2023-04-24 10:55:32.886664 halig-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 halig-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34670 2023-04-12 19:46:50.194310 halig-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1632 2023-05-09 07:04:54.570369 halig-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.2.1/halig/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-08 20:59:11.079650 halig-0.2.1/halig/__version__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.2.1/halig/commands/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-12 19:47:22.382591 halig-0.2.1/halig/commands/base.py
+-rw-r--r--   0        0        0     2781 2023-05-09 06:48:39.717700 halig-0.2.1/halig/commands/edit.py
+-rw-r--r--   0        0        0     1076 2023-04-12 19:47:22.382591 halig-0.2.1/halig/commands/notebooks.py
+-rw-r--r--   0        0        0     1199 2023-04-12 19:47:22.382591 halig-0.2.1/halig/commands/show.py
+-rw-r--r--   0        0        0     1418 2023-05-09 06:54:08.876599 halig-0.2.1/halig/encryption.py
+-rw-r--r--   0        0        0     1354 2023-05-08 19:32:21.621775 halig-0.2.1/halig/literals.py
+-rw-r--r--   0        0        0     2868 2023-05-08 20:59:47.779605 halig-0.2.1/halig/main.py
+-rw-r--r--   0        0        0     3142 2023-05-09 06:41:03.315211 halig-0.2.1/halig/settings.py
+-rw-r--r--   0        0        0      733 2023-05-08 21:12:42.122646 halig-0.2.1/halig/utils.py
+-rw-r--r--   0        0        0     2656 2023-05-09 07:11:08.785077 halig-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.202310 halig-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:47:22.382591 halig-0.2.1/tests/commands/__init__.py
+-rw-r--r--   0        0        0     1645 2023-04-24 10:55:32.886664 halig-0.2.1/tests/commands/conftest.py
+-rw-r--r--   0        0        0     1168 2023-04-24 10:55:32.886664 halig-0.2.1/tests/commands/test_edit.py
+-rw-r--r--   0        0        0     1563 2023-04-24 10:55:32.886664 halig-0.2.1/tests/commands/test_notebooks.py
+-rw-r--r--   0        0        0     1141 2023-04-24 10:55:32.886664 halig-0.2.1/tests/commands/test_show.py
+-rw-r--r--   0        0        0     2820 2023-04-12 19:47:22.382591 halig-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     2276 2023-05-09 06:28:25.521779 halig-0.2.1/tests/test_encryption.py
+-rw-r--r--   0        0        0     1541 2023-04-12 19:47:22.386591 halig-0.2.1/tests/test_settings.py
+-rw-r--r--   0        0        0     1482 2023-04-24 10:55:32.886664 halig-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 halig-0.2.1/PKG-INFO
```

### Comparing `halig-0.2.0/LICENSE` & `halig-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/README.md` & `halig-0.2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -7,35 +7,48 @@
 
 [(R)age](https://github.com/woodruffw/pyrage) encrypted note-taking CLI app.
 
 `halig` opens, using your favorite `$EDITOR`, an in-memory copy of a file and upon save-and-exit,
 it encrypts the new contents into an [age](https://github.com/FiloSottile/age) file that
 you can store, _relatively_ safe, anywhere.
 
+
+## Features
+
+- Simple notebooks management with paths autocompletion
+- Passphrase-less, fully-encrypted notes, compatible with existing SSH keys 
+- No external `age` binary needed
+- Almost all `age` advantages, like having multiple keys for encryption and decryption
+- Remote (HTTP) public keys import: e.g: github.com/<username>.keys
+
 ## Install
 
 ```shell
 pipx install halig # or pip
 ```
 
-
 ## Setup TLDR
 
 ```shell
 set -e
 ssh-keygen -t ed25519
 mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/halig"
 cat << EOF > "${XDG_CONFIG_HOME:-$HOME/.config}/halig/halig.yml"
 ---
-notebooks_root_path: /home/$(id -un)/Documents/Notebooks
-identity_path: /home/$(id -un)/.ssh/id_ed25519
-recipient_path: /home/$(id -un)/.ssh/id_ed25519.pub
+notebooks_root_path: ~/Documents/Notebooks
+identity_paths: 
+  - ~/.ssh/id_ed25519
+recipient_path:
+  - ~/.ssh/id_ed25519.pub
+  - https://github.com/<username>.keys
+  - https://gitlab.com/<username>.keys
 EOF
 ```
 
 ## Usage TLDR
 
 ```shell
 halig edit some_notebook     # edit today's note relative to <notebooks_root_path>/some_notebook
 halig edit some_notebook/foo # edit  <notebooks_root_path>/some_notebook/foo.age
 halig notebooks              # list current notebooks
-```
+```
+
```

### Comparing `halig-0.2.0/halig/commands/edit.py` & `halig-0.2.1/halig/commands/edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         """
 
         with tempfile.NamedTemporaryFile(delete=False, suffix=".md") as tf:
             tf.write(original_contents)
             temp_path = Path(tf.name)
 
         editor = os.environ.get("EDITOR", "vim")
-        subprocess.call([editor, temp_path])
+        subprocess.call([editor, temp_path])  # noqa: S603
 
         with temp_path.open("rb") as f:
             new_contents = f.read()
         encrypted_contents = self.encryptor.encrypt(new_contents)
 
         temp_path.unlink()
         return encrypted_contents
```

### Comparing `halig-0.2.0/halig/commands/notebooks.py` & `halig-0.2.1/halig/commands/notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/halig/commands/show.py` & `halig-0.2.1/halig/commands/show.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/halig/literals.py` & `halig-0.2.1/halig/literals.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/halig/main.py` & `halig-0.2.1/halig/main.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/halig/utils.py` & `halig-0.2.1/halig/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,11 @@
         except OSError as exc:
             print(f"[red]{exc.strerror} on {exc.filename or exc.filename2}")
             sys.exit(exc.errno)
         except ValueError as exc:
             print(f"[red]{exc}")
             sys.exit(1)
         except Exception as exc:  # noqa: BLE001
-            print(f"[bold red] Unexpected error: {exc}")
+            print(f"[beld red] Unexpected error: {exc}")
             sys.exit(2)
 
     return wrapper
```

### Comparing `halig-0.2.0/pyproject.toml` & `halig-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 dependencies = [
     "typer<1.0.0,>=0.6.1",
     "rich>=13.3.3",
     "pydantic>=1.10.7",
     "pyyaml>=6.0",
     "pyrage>=1.0.3",
     "pendulum>=2.1.2",
+    "httpx>=0.24.0",
 ]
 name = "halig"
 dynamic = []
 description = "age-encrypted, file-based, note-taking CLI app"
 readme = "README.md"
 keywords = [
     "cli",
@@ -31,15 +32,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Terminals",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-version = "0.2.0"
+version = "0.2.1"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "https://git.roboces.dev/catalin/halig"
 Repository = "https://git.roboces.dev/catalin/halig"
@@ -131,14 +132,15 @@
 warn_unused_configs = true
 
 [[tool.mypy.overrides]]
 module = [
     "pyrage",
     "pyrage.ssh",
     "pyrage.x25519",
+    "attr",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `halig-0.2.0/tests/commands/conftest.py` & `halig-0.2.1/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/tests/commands/test_edit.py` & `halig-0.2.1/tests/commands/test_edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/tests/commands/test_notebooks.py` & `halig-0.2.1/tests/commands/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/tests/commands/test_show.py` & `halig-0.2.1/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/tests/conftest.py` & `halig-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/tests/test_encryption.py` & `halig-0.2.1/tests/test_encryption.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 from pyrage import decrypt, encrypt, x25519
 
 from halig.encryption import Encryptor
 from halig.settings import Settings
 
 
 def test_instance_encryptor_from_age_keys(halig_path, notebooks_path):
-    identity = x25519.Identity.generate()
-    identity_path = halig_path / "identity.key"
-    identity_path.touch()
-    recipient_path = halig_path / "recipient.key"
-    recipient_path.touch()
-    with identity_path.open("w") as f:
-        f.write(str(identity))
+    identity_paths = []
+    recipient_paths = []
+    identities = []
+    for i in range(5):
+        identity = x25519.Identity.generate()
+        identities.append(identity)
+        identity_path = halig_path / f"identity_{i}.key"
+        identity_path.touch()
+        with identity_path.open("w") as f:
+            f.write(str(identity))
+        identity_paths.append(identity_path)
 
-    with recipient_path.open("w") as f:
-        f.write(str(identity.to_public()))
+        recipient_path = halig_path / f"recipient_{i}.key"
+        recipient_path.touch()
+
+        with recipient_path.open("w") as f:
+            f.write(str(identity.to_public()))
+
+        recipient_paths.append(recipient_path)
 
     settings = Settings(
         notebooks_root_path=notebooks_path,
-        identity_path=identity_path,
-        recipient_path=recipient_path,
+        identity_paths=identity_paths,
+        recipient_paths=recipient_paths,
     )
-    assert Encryptor(settings)
+    encryptor = Encryptor(settings)
+    for identity in identities:
+        assert str(identity) in [str(identity) for identity in encryptor.identities]
+        assert str(identity.to_public()) in [str(recipient) for recipient in encryptor.recipients]
 
 
 def test_encrypt(encryptor: Encryptor, ssh_identity):
     unencrypted_data = "foo"
     encrypted_data = encryptor.encrypt(unencrypted_data)
-
     assert isinstance(encrypted_data, bytes)
     assert unencrypted_data == decrypt(encrypted_data, [ssh_identity]).decode()
 
 
 def test_encrypt_bytes(encryptor: Encryptor, ssh_identity):
     unencrypted_data = b"foo"
     encrypted_data = encryptor.encrypt(unencrypted_data)
```

### Comparing `halig-0.2.0/tests/test_settings.py` & `halig-0.2.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/tests/test_utils.py` & `halig-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.2.0/PKG-INFO` & `halig-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halig
-Version: 0.2.0
+Version: 0.2.1
 Summary: age-encrypted, file-based, note-taking CLI app
 Keywords: cli notes age rage encryption notebook
 Author-Email: cătălin <185504a9@duck.com>
 License: GPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -22,14 +22,15 @@
 Requires-Python: >=3.10
 Requires-Dist: typer<1.0.0,>=0.6.1
 Requires-Dist: rich>=13.3.3
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: pyrage>=1.0.3
 Requires-Dist: pendulum>=2.1.2
+Requires-Dist: httpx>=0.24.0
 Requires-Dist: pytest>=7.2.2; extra == "testing"
 Requires-Dist: pytest-cov>=4.0.0; extra == "testing"
 Requires-Dist: pyfakefs>=5.1.0; extra == "testing"
 Requires-Dist: pytest-clarity>=1.0.1; extra == "testing"
 Requires-Dist: pytest-reportlog>=0.2.1; extra == "testing"
 Requires-Dist: pytest-duration-insights>=0.1.1; extra == "testing"
 Requires-Dist: pytest-pretty>=1.1.1; extra == "testing"
@@ -56,35 +57,48 @@
 
 [(R)age](https://github.com/woodruffw/pyrage) encrypted note-taking CLI app.
 
 `halig` opens, using your favorite `$EDITOR`, an in-memory copy of a file and upon save-and-exit,
 it encrypts the new contents into an [age](https://github.com/FiloSottile/age) file that
 you can store, _relatively_ safe, anywhere.
 
+
+## Features
+
+- Simple notebooks management with paths autocompletion
+- Passphrase-less, fully-encrypted notes, compatible with existing SSH keys 
+- No external `age` binary needed
+- Almost all `age` advantages, like having multiple keys for encryption and decryption
+- Remote (HTTP) public keys import: e.g: github.com/<username>.keys
+
 ## Install
 
 ```shell
 pipx install halig # or pip
 ```
 
-
 ## Setup TLDR
 
 ```shell
 set -e
 ssh-keygen -t ed25519
 mkdir -p "${XDG_CONFIG_HOME:-$HOME/.config}/halig"
 cat << EOF > "${XDG_CONFIG_HOME:-$HOME/.config}/halig/halig.yml"
 ---
-notebooks_root_path: /home/$(id -un)/Documents/Notebooks
-identity_path: /home/$(id -un)/.ssh/id_ed25519
-recipient_path: /home/$(id -un)/.ssh/id_ed25519.pub
+notebooks_root_path: ~/Documents/Notebooks
+identity_paths: 
+  - ~/.ssh/id_ed25519
+recipient_path:
+  - ~/.ssh/id_ed25519.pub
+  - https://github.com/<username>.keys
+  - https://gitlab.com/<username>.keys
 EOF
 ```
 
 ## Usage TLDR
 
 ```shell
 halig edit some_notebook     # edit today's note relative to <notebooks_root_path>/some_notebook
 halig edit some_notebook/foo # edit  <notebooks_root_path>/some_notebook/foo.age
 halig notebooks              # list current notebooks
-```
+```
+
```

