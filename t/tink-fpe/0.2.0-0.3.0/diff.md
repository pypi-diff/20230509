# Comparing `tmp/tink_fpe-0.2.0.tar.gz` & `tmp/tink_fpe-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tink_fpe-0.2.0.tar", max compression
+gzip compressed data, was "tink_fpe-0.3.0.tar", max compression
```

## Comparing `tink_fpe-0.2.0.tar` & `tink_fpe-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/LICENSE
--rw-r--r--   0        0        0     7969 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/README.md
--rw-r--r--   0        0        0     2131 2023-02-11 16:47:15.895492 tink_fpe-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      351 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/__init__.py
--rw-r--r--   0        0        0     3106 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/_fpe.py
--rw-r--r--   0        0        0     5698 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/_fpe_ff3.py
--rw-r--r--   0        0        0     2055 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/_fpe_ffx_key_manager.py
--rw-r--r--   0        0        0     1906 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/_fpe_key_templates.py
--rw-r--r--   0        0        0     2276 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/_fpe_wrapper.py
--rw-r--r--   0        0        0     2998 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/_util.py
--rw-r--r--   0        0        0       32 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/proto/__init__.py
--rw-r--r--   0        0        0     3159 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/proto/fpe_ffx_pb2.py
--rw-r--r--   0        0        0     3881 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/proto/fpe_ffx_pb2.pyi
--rw-r--r--   0        0        0        0 2023-02-11 16:46:59.907508 tink_fpe-0.2.0/src/tink_fpe/py.typed
--rw-r--r--   0        0        0     9117 1970-01-01 00:00:00.000000 tink_fpe-0.2.0/setup.py
--rw-r--r--   0        0        0     9055 1970-01-01 00:00:00.000000 tink_fpe-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-09 21:31:02.040064 tink_fpe-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11091 2023-05-09 21:31:02.040064 tink_fpe-0.3.0/README.md
+-rw-r--r--   0        0        0     2168 2023-05-09 21:31:22.932448 tink_fpe-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      351 2023-05-09 21:31:02.040064 tink_fpe-0.3.0/src/tink_fpe/__init__.py
+-rw-r--r--   0        0        0     3169 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/_fpe.py
+-rw-r--r--   0        0        0     5726 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/_fpe_ff3.py
+-rw-r--r--   0        0        0     2055 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/_fpe_ffx_key_manager.py
+-rw-r--r--   0        0        0     1904 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/_fpe_key_templates.py
+-rw-r--r--   0        0        0     2276 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/_fpe_wrapper.py
+-rw-r--r--   0        0        0     2998 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/_util.py
+-rw-r--r--   0        0        0       32 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/proto/__init__.py
+-rw-r--r--   0        0        0     3158 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/proto/fpe_ffx_pb2.py
+-rw-r--r--   0        0        0     3881 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/proto/fpe_ffx_pb2.pyi
+-rw-r--r--   0        0        0        0 2023-05-09 21:31:02.044064 tink_fpe-0.3.0/src/tink_fpe/py.typed
+-rw-r--r--   0        0        0    12166 1970-01-01 00:00:00.000000 tink_fpe-0.3.0/PKG-INFO
```

### Comparing `tink_fpe-0.2.0/LICENSE` & `tink_fpe-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tink_fpe-0.2.0/pyproject.toml` & `tink_fpe-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tink-fpe"
-version = "0.2.0"
+version = "0.3.0"
 description = "Format-Preserving Encryption support for Google Tink"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/tink-fpe-project"
 repository = "https://github.com/statisticsnorway/tink-fpe-python"
 documentation = "https://statisticsnorway.github.io/tink-fpe-project"
@@ -14,16 +14,16 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/tink-fpe-python/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ff3 = "^1.0.1"
-tink-custom = "^1.7.0"
-types-protobuf = "^4.21.0.4"
+types-protobuf = "^3.20.1"
+tink = "^1.7.0"
 
 
 [tool.poetry.scripts]
 tink-fpe = "tink_fpe.__main__:main" #TODO: Remove
 
 [tool.poetry.group.dev.dependencies]
 black = ">=21.10b0"
@@ -33,19 +33,20 @@
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.930"
-mypy-protobuf = "^3.4.0"
+mypy-protobuf = "^3.3.0"
 myst-parser = {version = ">=0.16.1"}
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
+protobuf = ">=3.20.1"
 Pygments = ">=2.10.0"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
@@ -81,14 +82,15 @@
 show_error_codes = true
 show_error_context = true
 
 [[tool.mypy.overrides]]
 module = [
     'ff3',
     'tink',
+    'tink.integration',
     'tink.proto'
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tink_fpe-0.2.0/src/tink_fpe/_fpe.py` & `tink_fpe-0.3.0/src/tink_fpe/_fpe.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     implies that the length of the plaintext and ciphertext may differ. Furthermore, decryption may not result in the
     exact same plaintext being restored."""
 
 
 class CharacterGroup:
     """CharacterGroup holds different types of character groups, suitable for composing FPE alphabets."""
 
-    ALPHANUMERIC = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789"
-    """Default alphanumeric characters: ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789"""
+    ALPHANUMERIC = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
+    """Default alphanumeric characters: 0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"""
 
     """Numeric characters: 0123456789"""
     DIGITS = "0123456789"
 
 
 class FpeParams:
     """FpeParams is used as an argument when invoking encrypt and decrypt functions.
@@ -46,18 +46,20 @@
     """
 
     def __init__(
         self,
         strategy: UnknownCharacterStrategy = UnknownCharacterStrategy.FAIL,
         tweak: bytes = b"",
         redaction_char: str = "",
+        charset: str = "utf-8",
     ):
         self.unknown_character_strategy = strategy
         self.tweak = tweak
         self.redaction_char = redaction_char
+        self.charset = charset
 
 
 _DEFAULT_FPE_PARAMS = FpeParams()
 
 
 class Fpe(metaclass=abc.ABCMeta):
     """Interface for Format-Preserving Encryption.
```

### Comparing `tink_fpe-0.2.0/src/tink_fpe/_fpe_ff3.py` & `tink_fpe-0.3.0/src/tink_fpe/_fpe_ff3.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def encrypt(self, plaintext: bytes, params: FpeParams = _DEFAULT_FPE_PARAMS) -> bytes:
         """Deterministically encrypt plaintext using FF3-1 mode.
 
         :param plaintext: plaintext to encrypt
         :param params: options that adjust how encryption will be performed
         :return: resulting ciphertext
         """
-        pt: str = plaintext.decode("utf-8")
+        pt: str = plaintext.decode(params.charset)
         tweak: str = _hex_tweak_of(params.tweak)
         char_skipper = None
 
         if params.unknown_character_strategy == UnknownCharacterStrategy.FAIL:
             if _util.has_unknown_chars(text=pt, known_chars=self._alphabet):
                 raise ValueError(f"Plaintext can only contain characters from the alphabet {self._alphabet}")
         elif params.unknown_character_strategy == UnknownCharacterStrategy.SKIP:
@@ -90,25 +90,25 @@
             else:
                 ct.append(self._ff3.encrypt_with_tweak(plaintext=chunk, tweak=tweak))
         ciphertext = "".join(ct)
 
         if char_skipper and char_skipper.has_skipped():
             ciphertext = char_skipper.inject_skipped_into(ciphertext)
 
-        return ciphertext.encode("utf-8")
+        return ciphertext.encode(params.charset)
 
     def decrypt(self, ciphertext: bytes, params: FpeParams = _DEFAULT_FPE_PARAMS) -> bytes:
         """Deterministically decrypt ciphertext using FF3-1 mode.
 
         :param ciphertext: ciphertext to decrypt
         :param params: options that adjust how decryption will be performed. This should usually be the same as the
                        params used to encrypt.
         :return: resulting plaintext
         """
-        ct: str = ciphertext.decode("utf-8")
+        ct: str = ciphertext.decode(params.charset)
         tweak: str = _hex_tweak_of(params.tweak)
         char_skipper = None
 
         if params.unknown_character_strategy == UnknownCharacterStrategy.SKIP:
             char_skipper = _util.CharacterSkipper(ct, self._alphabet)
             ct = char_skipper.get_processed_text()
 
@@ -120,8 +120,8 @@
             else:
                 pt.append(self._ff3.decrypt_with_tweak(ciphertext=chunk, tweak=tweak))
         plaintext = "".join(pt)
 
         if char_skipper and char_skipper.has_skipped():
             plaintext = char_skipper.inject_skipped_into(plaintext)
 
-        return plaintext.encode("utf-8")
+        return plaintext.encode(params.charset)
```

### Comparing `tink_fpe-0.2.0/src/tink_fpe/_fpe_ffx_key_manager.py` & `tink_fpe-0.3.0/src/tink_fpe/_fpe_ffx_key_manager.py`

 * *Files identical despite different names*

### Comparing `tink_fpe-0.2.0/src/tink_fpe/_fpe_key_templates.py` & `tink_fpe-0.3.0/src/tink_fpe/_fpe_key_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Pre-generated KeyTemplate for FPE FFX DeterministicAead.
 
 One can use these templates to generate a new tink_pb2.Keyset with
 tink_pb2.KeysetHandle. To generate a new keyset that contains a single
 fpe_ffx_pb2.FpeFfxKey, one can do:
-handle = keyset_handle.KeysetHandle(fpe_key_templates.FPE_FF31_256_F_ALPHANUMERIC).
+handle = keyset_handle.KeysetHandle(fpe_key_templates.FPE_FF31_256_ALPHANUMERIC).
 """
 
 from tink.proto import tink_pb2
 
 from tink_fpe import _fpe_ffx_key_manager
 from tink_fpe._fpe import CharacterGroup
 from tink_fpe.proto.fpe_ffx_pb2 import FfxMode
```

### Comparing `tink_fpe-0.2.0/src/tink_fpe/_fpe_wrapper.py` & `tink_fpe-0.3.0/src/tink_fpe/_fpe_wrapper.py`

 * *Files identical despite different names*

### Comparing `tink_fpe-0.2.0/src/tink_fpe/_util.py` & `tink_fpe-0.3.0/src/tink_fpe/_util.py`

 * *Files identical despite different names*

### Comparing `tink_fpe-0.2.0/src/tink_fpe/proto/fpe_ffx_pb2.py` & `tink_fpe-0.3.0/src/tink_fpe/proto/fpe_ffx_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         "__module__": "proto.fpe_ffx_pb2"
         # @@protoc_insertion_point(class_scope:ssb.crypto.tink.FpeFfxKey)
     },
 )
 _sym_db.RegisterMessage(FpeFfxKey)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"\n\030no.ssb.crypto.tink.protoP\001"
     _FFXMODE._serialized_start = 338
     _FFXMODE._serialized_end = 375
     _FPEFFXKEYPARAMS._serialized_start = 40
     _FPEFFXKEYPARAMS._serialized_end = 133
     _FPEFFXKEYFORMAT._serialized_start = 135
```

### Comparing `tink_fpe-0.2.0/src/tink_fpe/proto/fpe_ffx_pb2.pyi` & `tink_fpe-0.3.0/src/tink_fpe/proto/fpe_ffx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tink_fpe-0.2.0/setup.py` & `tink_fpe-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,265 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# Tink FPE Python
 
-package_dir = \
-{'': 'src'}
+[![PyPI](https://img.shields.io/pypi/v/tink-fpe.svg)][pypi_]
+[![Status](https://img.shields.io/pypi/status/tink-fpe.svg)][status]
+[![Python Version](https://img.shields.io/pypi/pyversions/tink-fpe)][python version]
+[![License](https://img.shields.io/pypi/l/tink-fpe)][license]
 
-packages = \
-['tink_fpe', 'tink_fpe.proto']
+[![Tests](https://github.com/statisticsnorway/tink-fpe-python/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/statisticsnorway/tink-fpe-python/branch/main/graph/badge.svg)][codecov]
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['ff3>=1.0.1,<2.0.0',
- 'tink-custom>=1.7.0,<2.0.0',
- 'types-protobuf>=4.21.0.4,<5.0.0.0']
-
-entry_points = \
-{'console_scripts': ['tink-fpe = tink_fpe.__main__:main']}
-
-setup_kwargs = {
-    'name': 'tink-fpe',
-    'version': '0.2.0',
-    'description': 'Format-Preserving Encryption support for Google Tink',
-    'long_description': '# Tink FPE Python\n\n[![PyPI](https://img.shields.io/pypi/v/tink-fpe.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/tink-fpe.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/tink-fpe)][python version]\n[![License](https://img.shields.io/pypi/l/tink-fpe)][license]\n\n[![Tests](https://github.com/statisticsnorway/tink-fpe-python/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/statisticsnorway/tink-fpe-python/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/tink-fpe/\n[status]: https://pypi.org/project/tink-fpe-python/\n[python version]: https://pypi.org/project/tink-fpe-python\n[tests]: https://github.com/statisticsnorway/tink-fpe-python/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/statisticsnorway/tink-fpe-python\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nFormat-Preserving Encryption (FPE) is a type of encryption that encrypts data in a way that preserves the format of the original plaintext. This means that after encryption, the encrypted data retains the same format as the original plaintext, such as a specific length or character set.\n\n## Features\n\n- _Tink FPE_ implements a [Primitive](https://developers.google.com/tink/glossary) that extends the Google Tink framework with support for Format-Preserving Encryption (FPE).\n- The following [NIST compliant](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-38Gr1-draft.pdf) algorithms are currently supported: `FF3-1`.\n- The implementation of the underlying algorithm is built on top of the excellent [Mysto FPE](https://github.com/mysto/python-fpe) library.\n- Tink FPE is currently available for Python and Java.\n- Regarding sensitivity for alphabet, FPE is designed to work with a specific alphabet, which is typically defined in the encryption algorithm. If the plaintext data contains characters that are not part of the defined alphabet, Tink FPE supports different _strategies_ for dealing with the data or substitute the characters with ones that are part of the alphabet.\n\n## Requirements\n\n- Google Tink for Python - the bleeding edge version (until [this issue](https://github.com/google/tink/issues/623) is resolved)\n\n## Installation\n\nYou can install _Tink FPE_ via [pip] from [PyPI]:\n\n```console\n$ pip install tink-fpe\n```\n\n## Usage\n\n```python\nimport tink\nimport tink_fpe\n\n# Register Tink FPE with the Tink runtime\ntink_fpe.register()\n\n# Specify the key template to use. In this example we want a 256 bits FF3-1 key that can handle\n# alphanumeric characters (ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789)\nkey_template = tink_fpe.fpe_key_templates.FPE_FF31_256_ALPHANUMERIC\n\n# Create a keyset\nkeyset_handle = tink.new_keyset_handle(key_template)\n\n# Get the FPE primitive\nfpe = keyset_handle.primitive(tink_fpe.Fpe)\n\n# Encrypt\nciphertext = fpe.encrypt(b\'Secret123\')\nprint(ciphertext.decode(\'utf-8\')) #-> sN3gt6q0V\n\n# Decrypt\ndecrypted = fpe.decrypt(ciphertext)\nprint(decrypted.decode(\'utf-8\')) #-> Secret123\n```\n\n### Handling non-alphabet characters\n\nA characteristic of Format-Preserving Encryption is that plaintext can only be composed of letters or symbols\nfrom a predefined set of characters called the "alphabet". Tink FPE supports different ways of coping with\ntexts that contain non-alphabet characters. The approach to use can be expressed via the `UnknownCharacterStrategy` enum.\n\nThe following _stragies_ are supported:\n\n- `FAIL` - Raise an error and bail out if encountering a non-alphabet character. **(this is the default)**\n- `SKIP` - Ignore non-alphabet characters, leaving them unencrypted (nested into the ciphertext).\n- `DELETE` - Remove all characters that are not part of the alphabet prior to processing. \\_Warning: Using this strategy implies that the length of the plaintext and ciphertext may differ.\n- `REDACT` - Replace non-alphabet characters with an alphabet-compliant character prior to processing. _Warning: Using this strategy means that decryption may not result in the exact same plaintext being restored._\n\n```python\nfrom tink_fpe import FpeParams, UnknownCharacterStrategy\n\n# The following will raise an Error\nciphertext = fpe.encrypt(b\'Ken sent me...\', FpeParams(strategy=UnknownCharacterStrategy.FAIL))\n\n# Skipping non-supported characters might reveal too much of the plaintext, but it is currently the only\n# approach that will handle any plaintext without either failing or irreversibly transforming the plaintext.\nparams = FpeParams(strategy=UnknownCharacterStrategy.SKIP)\nfpe.encrypt(b\'Ken sent me...\', params) #-> UEj l1Ns sj...\nfpe.decrypt(ciphertext, params) #-> Ken sent me...\n\n# Notice that using the DELETE strategy implies that the length of the plaintext and ciphertext may differ.\n# Furthermore, it might be impossible to go back to the original plaintext.\nparams = FpeParams(strategy=UnknownCharacterStrategy.DELETE)\nciphertext = fpe.encrypt(b\'Ken sent me...\', params) #-> EsQPgkE9Y\ndecrypted = fpe.decrypt(ciphertext, params) #-> Kensentme\n\n# Notice that using the REDACT strategy it might be impossible to go back to the original plaintext.\n# If not specified, the redaction character will be deduced automatically from the alphabet.\n# For alphanumeric alphabets the \'X\' character is used.\nparams = FpeParams(strategy=UnknownCharacterStrategy.REDACT)\nciphertext = fpe.encrypt(b\'Ken sent me...\', params) #-> MMY2HXvLwzIDoY\ndecrypted = fpe.decrypt(ciphertext, params) #-> KenXsentXmeXXX\n\n# It is also possible to specify the redaction character explicitly, like so:\nparams = FpeParams(strategy=UnknownCharacterStrategy.REDACT, redaction_char=\'Q\')\nciphertext = fpe.encrypt(b\'Ken sent me...\', params) #-> 9fVDzAODt2vvdz\ndecrypted = fpe.decrypt(ciphertext, params) #-> KenQsentQmeQQQ\n```\n\n### Loading predefined key material\n\nIt is easy to initialize key material from a predefined JSON. The following uses a cleartext keyset,\nbut it will be similar for a wrapped/encrypted key as well.\n\n```python\nimport json\nfrom tink import JsonKeysetReader\nfrom tink import cleartext_keyset_handle\nimport tink_fpe\n\ntink_fpe.register()\n\nkeyset_json = json.dumps({\n    "primaryKeyId": 1382079328,\n    "key": [\n        {\n            "keyData": {\n                "typeUrl": "type.googleapis.com/ssb.crypto.tink.FpeFfxKey",\n                "value": "EhD4978shQNRpBNaBjbF4KO4GkIQAho+QUJDREVGR0hJSktMTU5PUFFSU1RVVldYWVphYmNkZWZnaGlqa2xtbm9wcXJzdHV2d3h5ejAxMjM0NTY3ODk=",\n                "keyMaterialType": "SYMMETRIC"\n            },\n            "status": "ENABLED",\n            "keyId": 1382079328,\n            "outputPrefixType": "RAW"\n        }\n    ]\n})\n\nkeyset_handle = cleartext_keyset_handle.read(JsonKeysetReader(keyset_json))\nfpe = keyset_handle.primitive(tink_fpe.Fpe)\n```\n\n## Known issues\n\n// TODO: Describe issue about chunking that results in up to last 3 characters not being encrypted.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Tink FPE Python_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/statisticsnorway/tink-fpe/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/statisticsnorway/tink-fpe-python/blob/main/LICENSE\n[contributor guide]: https://github.com/statisticsnorway/tink-fpe-python/blob/main/CONTRIBUTING.md\n',
-    'author': 'Statistics Norway',
-    'author_email': 'stat-dev@ssb.no',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/statisticsnorway/tink-fpe-project',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi_]: https://pypi.org/project/tink-fpe/
+[status]: https://pypi.org/project/tink-fpe-python/
+[python version]: https://pypi.org/project/tink-fpe-python
+[tests]: https://github.com/statisticsnorway/tink-fpe-python/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/statisticsnorway/tink-fpe-python
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+Format-Preserving Encryption (FPE) is a type of encryption that encrypts data in a way that preserves the format of the original plaintext. This means that after encryption, the encrypted data retains the same format as the original plaintext, such as a specific length or character set.
+
+## Features
+
+- _Tink FPE_ implements a [Primitive](https://developers.google.com/tink/glossary) that extends the Google Tink framework with support for Format-Preserving Encryption (FPE).
+- The following [NIST compliant](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-38Gr1-draft.pdf) algorithms are currently supported: `FF3-1`.
+- The implementation of the underlying algorithm is built on top of the excellent [Mysto FPE](https://github.com/mysto/python-fpe) library.
+- Tink FPE is currently available for Python and Java.
+- Regarding sensitivity for alphabet, FPE is designed to work with a specific alphabet, which is typically defined in the encryption algorithm. If the plaintext data contains characters that are not part of the defined alphabet, Tink FPE supports different _strategies_ for dealing with the data or substitute the characters with ones that are part of the alphabet.
+
+## Requirements
+
+- Google Tink for Python - the bleeding edge version (until [this issue](https://github.com/google/tink/issues/623) is resolved)
+
+## Installation
+
+You can install _Tink FPE_ via [pip] from [PyPI]:
+
+```console
+$ pip install tink-fpe
+```
+
+## Usage
+
+```python
+import tink
+import tink_fpe
+
+# Register Tink FPE with the Tink runtime
+tink_fpe.register()
+
+# Specify the key template to use. In this example we want a 256 bits FF3-1 key that can handle
+# alphanumeric characters (ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789)
+key_template = tink_fpe.fpe_key_templates.FPE_FF31_256_ALPHANUMERIC
+
+# Create a keyset
+keyset_handle = tink.new_keyset_handle(key_template)
+
+# Get the FPE primitive
+fpe = keyset_handle.primitive(tink_fpe.Fpe)
+
+# Encrypt
+ciphertext = fpe.encrypt(b'Secret123')
+print(ciphertext.decode('utf-8')) #-> sN3gt6q0V
+
+# Decrypt
+decrypted = fpe.decrypt(ciphertext)
+print(decrypted.decode('utf-8')) #-> Secret123
+```
+
+### Handling non-alphabet characters
+
+A characteristic of Format-Preserving Encryption is that plaintext can only be composed of letters or symbols
+from a predefined set of characters called the "alphabet". Tink FPE supports different ways of coping with
+texts that contain non-alphabet characters. The approach to use can be expressed via the `UnknownCharacterStrategy` enum.
+
+The following _stragies_ are supported:
+
+- `FAIL` - Raise an error and bail out if encountering a non-alphabet character. **(this is the default)**
+- `SKIP` - Ignore non-alphabet characters, leaving them unencrypted (nested into the ciphertext).
+- `DELETE` - Remove all characters that are not part of the alphabet prior to processing. \_Warning: Using this strategy implies that the length of the plaintext and ciphertext may differ.
+- `REDACT` - Replace non-alphabet characters with an alphabet-compliant character prior to processing. _Warning: Using this strategy means that decryption may not result in the exact same plaintext being restored._
+
+```python
+from tink_fpe import FpeParams, UnknownCharacterStrategy
+
+# The following will raise an Error
+ciphertext = fpe.encrypt(b'Ken sent me...', FpeParams(strategy=UnknownCharacterStrategy.FAIL))
+
+# Skipping non-supported characters might reveal too much of the plaintext, but it is currently the only
+# approach that will handle any plaintext without either failing or irreversibly transforming the plaintext.
+params = FpeParams(strategy=UnknownCharacterStrategy.SKIP)
+fpe.encrypt(b'Ken sent me...', params) #-> UEj l1Ns sj...
+fpe.decrypt(ciphertext, params) #-> Ken sent me...
+
+# Notice that using the DELETE strategy implies that the length of the plaintext and ciphertext may differ.
+# Furthermore, it might be impossible to go back to the original plaintext.
+params = FpeParams(strategy=UnknownCharacterStrategy.DELETE)
+ciphertext = fpe.encrypt(b'Ken sent me...', params) #-> EsQPgkE9Y
+decrypted = fpe.decrypt(ciphertext, params) #-> Kensentme
+
+# Notice that using the REDACT strategy it might be impossible to go back to the original plaintext.
+# If not specified, the redaction character will be deduced automatically from the alphabet.
+# For alphanumeric alphabets the 'X' character is used.
+params = FpeParams(strategy=UnknownCharacterStrategy.REDACT)
+ciphertext = fpe.encrypt(b'Ken sent me...', params) #-> MMY2HXvLwzIDoY
+decrypted = fpe.decrypt(ciphertext, params) #-> KenXsentXmeXXX
+
+# It is also possible to specify the redaction character explicitly, like so:
+params = FpeParams(strategy=UnknownCharacterStrategy.REDACT, redaction_char='Q')
+ciphertext = fpe.encrypt(b'Ken sent me...', params) #-> 9fVDzAODt2vvdz
+decrypted = fpe.decrypt(ciphertext, params) #-> KenQsentQmeQQQ
+```
+
+### Loading predefined key material
+
+It is easy to initialize key material from a predefined JSON. The following uses a cleartext keyset,
+but it will be similar for a wrapped/encrypted key as well.
+
+```python
+import json
+from tink import JsonKeysetReader
+from tink import cleartext_keyset_handle
+import tink_fpe
+
+tink_fpe.register()
+
+keyset_json = json.dumps({
+    "primaryKeyId": 1382079328,
+    "key": [
+        {
+            "keyData": {
+                "typeUrl": "type.googleapis.com/ssb.crypto.tink.FpeFfxKey",
+                "value": "EhD4978shQNRpBNaBjbF4KO4GkIQAho+QUJDREVGR0hJSktMTU5PUFFSU1RVVldYWVphYmNkZWZnaGlqa2xtbm9wcXJzdHV2d3h5ejAxMjM0NTY3ODk=",
+                "keyMaterialType": "SYMMETRIC"
+            },
+            "status": "ENABLED",
+            "keyId": 1382079328,
+            "outputPrefixType": "RAW"
+        }
+    ]
+})
+
+keyset_handle = cleartext_keyset_handle.read(JsonKeysetReader(keyset_json))
+fpe = keyset_handle.primitive(tink_fpe.Fpe)
+```
+
+### Using key material protected by Google Cloud KMS
+
+```python
+import json
+
+from tink import JsonKeysetReader
+from tink import read_keyset_handle
+from tink.integration import gcpkms
+
+import tink_fpe
+
+
+# Define uri to key encryption key and path to GCP credentials
+gcp_credentials = "path/to/sa-key.json"
+
+# Register Tink FPE with the Tink runtime
+tink_fpe.register()
+
+# Get hold of a wrapped data encryption key (WDEK)
+keyset_json = {
+    "kekUri": "gcp-kms://projects/<project-id>/locations/<region>/keyRings/my-keyring/cryptoKeys/my-kek",
+    "encryptedKeyset": "CiQAp91NBsClBYjw4AS9sOdB65peMwlzY4AiOzyMe+b+dFjSBuIS2QEAZ30rtRcDkuvtUgeENQCt29Vsalf+FtaNZc8wpOXKb3sD2c8hTXKaf34iq2QRMaQUBXxG+YSJPV4PvJZMGydZpjowM9K2eAJFZs5JaVxb3BMfUt0miNaORZmczqZhKlXXHbMoQ71GLwfSnf4jJnIRJK4s38ThnxS2ebm4b5T0qno6PWg84TtUw9eIIieqlUFhIqBjCcMugGTsE+xfWIOct22RDEUI3cAboCew5ppjOREAxzbaH8LaUBct5eLN8wtakY3Vv8KxBoT3Hq6fnNSSGOKmkqMVrK0p",
+    "keysetInfo":
+        {
+            "primaryKeyId": 593699223,
+            "keyInfo":
+                [
+                    {
+                        "typeUrl": "type.googleapis.com/ssb.crypto.tink.FpeFfxKey",
+                        "status": "ENABLED",
+                        "keyId": 593699223,
+                        "outputPrefixType": "RAW"
+                    }
+                ]
+        }
 }
 
+# Extract the kek uri from the keyset json
+kek_uri = keyset_json.pop('kekUri')
+
+# Unwrap key using Google Cloud KMS
+kms_client = gcpkms.GcpKmsClient(kek_uri, gcp_credentials)
+kms_aead = kms_client.get_aead(kek_uri)
+keyset_handle = read_keyset_handle(keyset_reader=JsonKeysetReader(json.dumps(keyset_json)),
+                                   master_key_aead=kms_aead)
+
+# Get the FPE primitive
+fpe = keyset_handle.primitive(tink_fpe.Fpe)
+```
+
+### Dockerfile
+
+As of this writing (27.03.2023), Tink does not yet provide Python wheels for versions `>1.6.x`.
+Thus, in order to use Tink FPE, we need to build Tink, which involves using bazel and and
+compiling protobuf sources. The following shows a Dockerfile that demonstrates how this can
+be done. Notice that this is for the `x86` architecture. If you are on another
+architecture (e.g. `arm`), you need to substitute the bazel and protobuf references to match
+your system architecture.
+
+```dockerfile
+FROM python:3.10-bullseye
+
+RUN apt-get update && apt-get upgrade -y
+
+# Install curl and git
+RUN apt-get install -y curl git
+
+# Install bazel
+RUN curl -L https://github.com/bazelbuild/bazelisk/releases/download/v1.16.0/bazelisk-linux-amd64 > /usr/local/bin/bazelisk && chmod +x /usr/local/bin/bazelisk
+
+# Install latest protobuf compiler (note: protobuf-compiler from apt is an older non-compliant version)
+WORKDIR /opt/protobuf
+RUN curl -L https://github.com/protocolbuffers/protobuf/releases/download/v21.12/protoc-21.12-linux-x86_64.zip > protoc.zip
+RUN unzip protoc.zip && chmod +x ./bin/protoc
+RUN ln -s /opt/protobuf/bin/protoc /usr/local/bin/protoc
+
+# Update pip
+RUN pip install --upgrade pip
+
+# ...
+WORKDIR /app
+```
+
+## Known issues
+
+// TODO: Describe issue about chunking that results in up to last 3 characters not being encrypted.
+// TODO: Describe issue with minimum length depending on the alphabet radix (e.g. 4 characters for alphanumeric and 6 for digits)
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+_Tink FPE Python_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[pypi]: https://pypi.org/
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[file an issue]: https://github.com/statisticsnorway/tink-fpe/issues
+[pip]: https://pip.pypa.io/
+
+<!-- github-only -->
 
-setup(**setup_kwargs)
+[license]: https://github.com/statisticsnorway/tink-fpe-python/blob/main/LICENSE
+[contributor guide]: https://github.com/statisticsnorway/tink-fpe-python/blob/main/CONTRIBUTING.md
```

