# Comparing `tmp/perpetuo-0.3.2.tar.gz` & `tmp/perpetuo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perpetuo-0.3.2.tar", last modified: Fri Apr 28 07:40:17 2023, max compression
+gzip compressed data, was "perpetuo-0.4.0.tar", last modified: Mon May  8 23:55:57 2023, max compression
```

## Comparing `perpetuo-0.3.2.tar` & `perpetuo-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:40:17.211537 perpetuo-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    49899 2023-04-28 07:40:07.000000 perpetuo-0.3.2/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 07:40:07.000000 perpetuo-0.3.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 07:40:07.000000 perpetuo-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-28 07:40:07.000000 perpetuo-0.3.2/LICENSE.APACHE2
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 07:40:07.000000 perpetuo-0.3.2/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-28 07:40:07.000000 perpetuo-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-28 07:40:17.211537 perpetuo-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-28 07:40:07.000000 perpetuo-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 07:40:07.000000 perpetuo-0.3.2/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-28 07:40:07.000000 perpetuo-0.3.2/prep-manylinux-container.sh
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-28 07:40:07.000000 perpetuo-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:40:17.207538 perpetuo-0.3.2/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:40:17.211537 perpetuo-0.3.2/python/perpetuo/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-28 07:40:07.000000 perpetuo-0.3.2/python/perpetuo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 07:40:07.000000 perpetuo-0.3.2/python/perpetuo/_perpetuo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-28 07:40:07.000000 perpetuo-0.3.2/python/perpetuo/_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:40:17.211537 perpetuo-0.3.2/python/perpetuo/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:40:07.000000 perpetuo-0.3.2/python/perpetuo/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-28 07:40:07.000000 perpetuo-0.3.2/python/perpetuo/_tests/test_perpetuo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:40:07.000000 perpetuo-0.3.2/python/perpetuo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:40:17.211537 perpetuo-0.3.2/python/perpetuo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-28 07:40:17.000000 perpetuo-0.3.2/python/perpetuo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-28 07:40:17.000000 perpetuo-0.3.2/python/perpetuo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:40:17.000000 perpetuo-0.3.2/python/perpetuo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:40:16.000000 perpetuo-0.3.2/python/perpetuo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 07:40:17.000000 perpetuo-0.3.2/python/perpetuo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:40:17.211537 perpetuo-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-28 07:40:07.000000 perpetuo-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:40:17.211537 perpetuo-0.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-28 07:40:07.000000 perpetuo-0.3.2/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-28 07:40:07.000000 perpetuo-0.3.2/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-28 07:40:07.000000 perpetuo-0.3.2/src/shmem.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:55:57.846820 perpetuo-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    49899 2023-05-08 23:55:49.000000 perpetuo-0.4.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 23:55:49.000000 perpetuo-0.4.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 23:55:49.000000 perpetuo-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 23:55:49.000000 perpetuo-0.4.0/LICENSE.APACHE2
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-08 23:55:49.000000 perpetuo-0.4.0/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 23:55:49.000000 perpetuo-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-08 23:55:57.846820 perpetuo-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-08 23:55:49.000000 perpetuo-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 23:55:49.000000 perpetuo-0.4.0/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-08 23:55:49.000000 perpetuo-0.4.0/prep-manylinux-container.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-08 23:55:49.000000 perpetuo-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:55:57.842820 perpetuo-0.4.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:55:57.842820 perpetuo-0.4.0/python/perpetuo/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-08 23:55:49.000000 perpetuo-0.4.0/python/perpetuo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 23:55:49.000000 perpetuo-0.4.0/python/perpetuo/_perpetuo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-08 23:55:49.000000 perpetuo-0.4.0/python/perpetuo/_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:55:57.842820 perpetuo-0.4.0/python/perpetuo/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:55:49.000000 perpetuo-0.4.0/python/perpetuo/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-08 23:55:49.000000 perpetuo-0.4.0/python/perpetuo/_tests/test_perpetuo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:55:49.000000 perpetuo-0.4.0/python/perpetuo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:55:57.842820 perpetuo-0.4.0/python/perpetuo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-08 23:55:57.000000 perpetuo-0.4.0/python/perpetuo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-08 23:55:57.000000 perpetuo-0.4.0/python/perpetuo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:55:57.000000 perpetuo-0.4.0/python/perpetuo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:55:57.000000 perpetuo-0.4.0/python/perpetuo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 23:55:57.000000 perpetuo-0.4.0/python/perpetuo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 23:55:57.846820 perpetuo-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 23:55:49.000000 perpetuo-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:55:57.846820 perpetuo-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-08 23:55:49.000000 perpetuo-0.4.0/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-08 23:55:49.000000 perpetuo-0.4.0/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-08 23:55:49.000000 perpetuo-0.4.0/src/shmem.rs
```

### Comparing `perpetuo-0.3.2/Cargo.lock` & `perpetuo-0.4.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -119,17 +119,17 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
@@ -306,28 +306,28 @@
  "termcolor",
  "terminal_size",
  "textwrap 0.16.0",
 ]
 
 [[package]]
 name = "clap"
-version = "4.2.5"
+version = "4.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a1f23fa97e1d1641371b51f35535cb26959b8e27ab50d167a8b996b5bada819"
+checksum = "34d21f9bf1b425d2968943631ec91202fe5e837264063503708b83013f8fc938"
 dependencies = [
  "clap_builder",
  "clap_derive 4.2.0",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.5"
+version = "4.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fdc5d93c358224b4d6867ef1356d740de2303e9892edc06c5340daeccd96bab"
+checksum = "914c8c79fb560f238ef6429439a30023c862f7a28e688c58f7203f12b29970bd"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex 0.4.1",
  "strsim 0.10.0",
  "terminal_size",
@@ -609,17 +609,17 @@
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "getrandom"
@@ -767,15 +767,15 @@
 [[package]]
 name = "inferno"
 version = "0.11.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fb7c1b80a1dfa604bb4a649a5c5aeef3d913f7c520cb42b40e534e8a61bcdfc"
 dependencies = [
  "ahash 0.8.3",
- "clap 4.2.5",
+ "clap 4.2.7",
  "crossbeam-channel",
  "crossbeam-utils",
  "dashmap",
  "env_logger 0.10.0",
  "indexmap",
  "is-terminal",
  "itoa",
@@ -844,17 +844,17 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
@@ -896,17 +896,17 @@
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.5"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e8776872cdc2f073ccaab02e336fa321328c1e02646ebcb9d2108d0baab480d"
+checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -985,17 +985,17 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "nix"
 version = "0.26.2"
@@ -1103,19 +1103,19 @@
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
 [[package]]
 name = "perpetuo"
-version = "0.3.2"
+version = "0.4.0"
 dependencies = [
  "anyhow",
  "bytemuck",
- "clap 4.2.5",
+ "clap 4.2.7",
  "indoc 2.0.1",
  "libc",
  "memmap",
  "once_cell",
  "proc-maps 0.3.1",
  "py-spy",
  "pyo3",
@@ -1299,17 +1299,17 @@
 checksum = "7f50b1c63b38611e7d4d7f68b82d3ad0cc71a2ad2e7f61fc10f1328d917c93cd"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1438,17 +1438,17 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.15"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0661814f891c57c930a610266415528da53c4933e6dea5fb350cbfe048a9ece"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
  "errno 0.3.1",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -1490,23 +1490,23 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.160"
+version = "1.0.162"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
 
 [[package]]
 name = "serde_derive"
-version = "1.0.160"
+version = "1.0.162"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
```

### Comparing `perpetuo-0.3.2/Cargo.toml` & `perpetuo-0.4.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "perpetuo"
-version = "0.3.2"
+version = "0.4.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "perpetuo"
```

### Comparing `perpetuo-0.3.2/LICENSE.APACHE2` & `perpetuo-0.4.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.2/LICENSE.MIT` & `perpetuo-0.4.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.2/PKG-INFO` & `perpetuo-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perpetuo
-Version: 0.3.2
+Version: 0.4.0
 Summary: A stall tracker for Python's GIL and Trio tasks
 Author-email: "Nathaniel J. Smith" <njs@pobox.com>
 License: MIT OR Apache-2.0
 Project-URL: repository, https://github.com/njsmith/perpetuo
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
```

### Comparing `perpetuo-0.3.2/README.md` & `perpetuo-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.2/prep-manylinux-container.sh` & `perpetuo-0.4.0/prep-manylinux-container.sh`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.2/pyproject.toml` & `perpetuo-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel", "setuptools-rust"]
 
 [project]
 name = "perpetuo"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   {name = "Nathaniel J. Smith", email = "njs@pobox.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT OR Apache-2.0"}
 description = "A stall tracker for Python's GIL and Trio tasks"
```

### Comparing `perpetuo-0.3.2/python/perpetuo/_tests/test_perpetuo.py` & `perpetuo-0.4.0/python/perpetuo/_tests/test_perpetuo.py`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.2/python/perpetuo.egg-info/PKG-INFO` & `perpetuo-0.4.0/python/perpetuo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perpetuo
-Version: 0.3.2
+Version: 0.4.0
 Summary: A stall tracker for Python's GIL and Trio tasks
 Author-email: "Nathaniel J. Smith" <njs@pobox.com>
 License: MIT OR Apache-2.0
 Project-URL: repository, https://github.com/njsmith/perpetuo
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
```

### Comparing `perpetuo-0.3.2/python/perpetuo.egg-info/SOURCES.txt` & `perpetuo-0.4.0/python/perpetuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.2/setup.py` & `perpetuo-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.2/src/lib.rs` & `perpetuo-0.4.0/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -50,14 +50,18 @@
             Err(err) => return Err(PyRuntimeError::new_err(err.to_string())),
         };
         Ok(PyStallTracker {
             stall_tracker: Some(stall_tracker),
         })
     }
 
+    fn _leak(this: PyRef<'_, Self>, py: Python) {
+        std::mem::forget(this.into_py(py));
+    }
+
     fn go_active(&self) -> PyResult<()> {
         let stall_tracker = rustify(&self)?;
         if stall_tracker.is_active() {
             return Err(PyRuntimeError::new_err("Already active"));
         }
         stall_tracker.toggle();
         Ok(())
```

### Comparing `perpetuo-0.3.2/src/main.rs` & `perpetuo-0.4.0/src/main.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,86 @@
 use std::time::{Duration, Instant};
 
 use anyhow::{bail, Result};
-use clap::{Parser, Subcommand};
+use clap::{ArgAction, Parser, Subcommand};
 use indoc::indoc;
 use py_spy::StackTrace;
 
 use perpetuo::shmem::PerpetuoProc;
 
 #[derive(Parser, Debug)]
 #[command(about = "A stall tracker for Python", long_about = None)]
 struct Cli {
     #[command(subcommand)]
     command: Commands,
-    #[arg(short, long, value_name = "SECONDS", default_value_t = 0.5)]
-    poll_interval: f64,
+    /// How often we inspect the target process to check for progress.
+    #[arg(long, value_name = "SECONDS", default_value = "0.05", value_parser=parse_duration)]
+    poll_interval: Duration,
+    /// How long a stall is required to trigger a traceback.
+    ///
+    /// We only alert if we issue two polls that both see the same stall and are at
+    /// least alert-interval apart. So you want poll-interval to be smaller than
+    /// alert-interval.
+    #[arg(long, value_name = "SECONDS", default_value = "0.2", value_parser=parse_duration)]
+    alert_interval: Duration,
+
     /// We'll print at most one traceback per this many seconds. This reduces spam, and
     /// also reduces interference with the monitored process, since each traceback
     /// requires briefly pausing the process. And in some specific cases, this might
     /// cause system calls to be restarted, which might cause timeouts to be reset, and
     /// thus extend stalls...
     ///
     /// Hypothetically.
-    #[arg(long, value_name = "SECONDS", default_value_t = 30.0)]
-    traceback_interval: f64,
+    #[arg(long, value_name = "SECONDS", default_value = "30.0", value_parser=parse_duration)]
+    traceback_suppress: Duration,
+
+    // This is super confusing -- the options are intentionally swapped. For reasons
+    // (such as they are) see: https://jwodder.github.io/kbits/posts/clap-bool-negate/
+    /// Don't print local variable values in tracebacks
+    #[clap(long = "no-print-locals", action = ArgAction::SetFalse)]
+    print_locals: bool,
+    /// Print local variable values in tracebacks [default]
+    #[clap(long = "print-locals", overrides_with = "print_locals")]
+    _no_print_locals: bool,
+}
+
+fn parse_duration(s: &str) -> std::result::Result<Duration, String> {
+    let seconds: f64 = s.parse().map_err(|_| format!("{s}: not a valid float"))?;
+    Ok(Duration::from_secs_f64(seconds))
 }
 
 #[derive(Subcommand, Debug)]
 enum Commands {
     /// Watch a given process, which must have set up at least one
     /// perpetuo.StallTracker.
     #[command(arg_required_else_help = true)]
     Watch { pid: u32 },
 }
 
 fn main() -> Result<()> {
     let cli = Cli::parse();
-    let poll_interval = Duration::from_secs_f64(cli.poll_interval);
-    let traceback_interval = Duration::from_secs_f64(cli.traceback_interval);
 
     match cli.command {
-        Commands::Watch { pid } => watch_process(pid, poll_interval, traceback_interval)?,
+        Commands::Watch { pid } => watch_process(pid, &cli)?,
     }
     Ok(())
 }
 
-fn watch_process(pid: u32, poll_interval: Duration, traceback_interval: Duration) -> Result<()> {
+fn watch_process(pid: u32, cli: &Cli) -> Result<()> {
     let mut config = py_spy::Config::default();
     // We only collect a stack trace if we've already determined that the program is
     // misbehaving, so we're happy to pay some extra cost to get more detailed
     // information.
     config.native = true;
     // py-spy fetches up to 128 * this number of bytes of locals
-    config.dump_locals = 10;
+    if cli.print_locals {
+        config.dump_locals = 10;
+    } else {
+        config.dump_locals = 0;
+    }
     config.full_filenames = true;
     eprintln!("Attempting to monitor pid {pid}...");
     // let mut proc = loop {
     //     if let Some(proc) = PerpetuoProc::new(pid, &config)? {
     //         break proc;
     //     }
     //     std::thread::sleep(poll_interval);
@@ -91,16 +116,21 @@
             );
         }
     }
     let mut proc = result?;
     eprintln!("Successfully monitoring pid {pid}");
     let mut next_traceback = Instant::now();
     loop {
-        std::thread::sleep(poll_interval);
-        if let Err(err) = check_once(&mut proc, &mut next_traceback, traceback_interval) {
+        std::thread::sleep(cli.poll_interval);
+        if let Err(err) = check_once(
+            &mut proc,
+            &mut next_traceback,
+            cli.alert_interval,
+            cli.traceback_suppress,
+        ) {
             if proc.spy.process.exe().is_err() {
                 eprintln!("Process {} has exited", pid);
                 return Ok(());
             }
             return Err(err);
         }
     }
@@ -120,17 +150,18 @@
         }
     })
 }
 
 fn check_once(
     proc: &mut PerpetuoProc,
     next_traceback: &mut Instant,
+    alert_interval: Duration,
     traceback_interval: Duration,
 ) -> Result<()> {
-    for stall in proc.check_stalls()? {
+    for stall in proc.check_stalls(alert_interval)? {
         eprintln!(
             "{} stall detected in process {} for at least {:?}",
             stall.name, proc.spy.process.pid, stall.duration
         );
         let now = Instant::now();
         if now < *next_traceback {
             eprintln!("  (no traceback due to rate-limiting)");
```

### Comparing `perpetuo-0.3.2/src/shmem.rs` & `perpetuo-0.4.0/src/shmem.rs`

 * *Files 6% similar despite different names*

```diff
@@ -247,41 +247,46 @@
         }
         if !read_any {
             bail!("Couldn't access any process memory -- maybe you need ptrace permission?");
         }
         bail!("Couldn't find perpetuo instrumentation (did you enable it?)");
     }
 
-    pub fn check_stalls(&mut self) -> Result<Vec<StallReport>> {
+    pub fn check_stalls(&mut self, alert_interval: Duration) -> Result<Vec<StallReport>> {
         let now = Instant::now();
         let current_slots = self
             .spy
             .process
             .copy_vec::<StallTracker>(self.slots_ptr, self.slots_count)?;
 
         let mut stalls = Vec::new();
 
         for (id, current) in current_slots.into_iter().enumerate() {
             let mut snapshot = &mut self.last_updates[id];
             if current.is_active()
                 && current.count.load(Ordering::Relaxed)
                     == snapshot.stall_tracker.count.load(Ordering::Relaxed)
             {
-                // stall detected!
-                let name = self
-                    .spy
-                    .process
-                    .copy(current.metadata.name_ptr, current.metadata.name_len)?;
-                let name = String::from_utf8(name)?;
-                stalls.push(StallReport {
-                    id,
-                    name,
-                    thread_hint: current.metadata.thread_hint,
-                    duration: now.duration_since(snapshot.last_updated),
-                })
+                if now.duration_since(snapshot.last_updated) >= alert_interval {
+                    // stall detected!
+                    let name = self
+                        .spy
+                        .process
+                        .copy(current.metadata.name_ptr, current.metadata.name_len)?;
+                    let name = String::from_utf8(name)?;
+                    stalls.push(StallReport {
+                        id,
+                        name,
+                        thread_hint: current.metadata.thread_hint,
+                        duration: now.duration_since(snapshot.last_updated),
+                    })
+                } else {
+                    // stall in progress, but it hasn't hit our alerting threshold
+                    // yet... leave the snapshot alone so we can continue tracking it.
+                }
             } else {
                 snapshot.stall_tracker = current;
                 snapshot.last_updated = now;
             }
         }
         Ok(stalls)
     }
```

