# Comparing `tmp/unblob_native-0.1.0.tar.gz` & `tmp/unblob_native-0.1.1.tar.gz`

## Comparing `unblob_native-0.1.0.tar` & `unblob_native-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 unblob_native-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     4351 2023-05-04 22:35:22.000000 unblob_native-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      798 2023-05-04 22:35:22.000000 unblob_native-0.1.0/.github/workflows/Update.yml
--rw-r--r--   0     1001      123     1181 2023-05-04 22:35:22.000000 unblob_native-0.1.0/.github/workflows/check-mergeable.yml
--rw-r--r--   0     1001      123       45 2023-05-04 22:35:22.000000 unblob_native-0.1.0/.gitignore
--rw-r--r--   0     1001      123      808 2023-05-04 22:35:22.000000 unblob_native-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     2486 2023-05-04 22:35:22.000000 unblob_native-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123     2255 2023-05-04 22:35:22.000000 unblob_native-0.1.0/LICENSE
--rw-r--r--   0     1001      123     1170 2023-05-04 22:35:22.000000 unblob_native-0.1.0/README.md
--rw-r--r--   0     1001      123     3968 2023-05-04 22:35:22.000000 unblob_native-0.1.0/SECURITY.md
--rwxr-xr-x   0     1001      123      908 2023-05-04 22:35:22.000000 unblob_native-0.1.0/benches/benches_main.rs
--rw-r--r--   0     1001      123       10 2023-05-04 22:36:37.000000 unblob_native-0.1.0/dist/unblob_native-0.1.0.tar.gz
--rw-r--r--   0     1001      123     5077 2023-05-04 22:35:22.000000 unblob_native-0.1.0/flake.lock
--rw-r--r--   0     1001      123     6715 2023-05-04 22:35:22.000000 unblob_native-0.1.0/flake.nix
--rw-r--r--   0     1001      123    36941 2023-05-04 22:35:22.000000 unblob_native-0.1.0/pdm.lock
--rw-r--r--   0     1001      123       23 2023-05-04 22:35:22.000000 unblob_native-0.1.0/pdm.toml
--rw-r--r--   0     1001      123     3458 2023-05-04 22:35:22.000000 unblob_native-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123       51 2023-05-04 22:35:22.000000 unblob_native-0.1.0/rust-toolchain.toml
--rw-r--r--   0     1001      123      510 2023-05-04 22:35:22.000000 unblob_native-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123      626 2023-05-04 22:35:22.000000 unblob_native-0.1.0/src/math.rs
--rw-r--r--   0     1001      123      528 2023-05-04 22:35:22.000000 unblob_native-0.1.0/tests/test_math.py
--rw-r--r--   0     1001      123      160 2023-05-04 22:35:22.000000 unblob_native-0.1.0/unblob_native/__init__.py
--rw-r--r--   0     1001      123       65 2023-05-04 22:35:22.000000 unblob_native-0.1.0/unblob_native/_native/__init__.pyi
--rw-r--r--   0     1001      123       47 2023-05-04 22:35:22.000000 unblob_native-0.1.0/unblob_native/_native/math_tools.pyi
--rw-r--r--   0     1001      123        0 2023-05-04 22:35:22.000000 unblob_native-0.1.0/unblob_native/py.typed
--rw-r--r--   0     1001      123    21787 2023-05-04 22:35:22.000000 unblob_native-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 unblob_native-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 unblob_native-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     5683 2023-05-09 08:40:37.000000 unblob_native-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      799 2023-05-09 08:40:37.000000 unblob_native-0.1.1/.github/workflows/Update.yml
+-rw-r--r--   0     1001      123     1181 2023-05-09 08:40:37.000000 unblob_native-0.1.1/.github/workflows/check-mergeable.yml
+-rw-r--r--   0     1001      123       45 2023-05-09 08:40:37.000000 unblob_native-0.1.1/.gitignore
+-rw-r--r--   0     1001      123      808 2023-05-09 08:40:37.000000 unblob_native-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     2486 2023-05-09 08:40:37.000000 unblob_native-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123     2255 2023-05-09 08:40:37.000000 unblob_native-0.1.1/LICENSE
+-rw-r--r--   0     1001      123     1170 2023-05-09 08:40:37.000000 unblob_native-0.1.1/README.md
+-rw-r--r--   0     1001      123     3968 2023-05-09 08:40:37.000000 unblob_native-0.1.1/SECURITY.md
+-rwxr-xr-x   0     1001      123      914 2023-05-09 08:40:37.000000 unblob_native-0.1.1/benches/benches_main.rs
+-rw-r--r--   0     1001      123       10 2023-05-09 08:42:09.000000 unblob_native-0.1.1/dist/unblob_native-0.1.1.tar.gz
+-rw-r--r--   0     1001      123     6485 2023-05-09 08:40:37.000000 unblob_native-0.1.1/flake.lock
+-rw-r--r--   0     1001      123     6256 2023-05-09 08:40:37.000000 unblob_native-0.1.1/flake.nix
+-rw-r--r--   0     1001      123    36941 2023-05-09 08:40:37.000000 unblob_native-0.1.1/pdm.lock
+-rw-r--r--   0     1001      123       23 2023-05-09 08:40:37.000000 unblob_native-0.1.1/pdm.toml
+-rw-r--r--   0     1001      123     3522 2023-05-09 08:40:37.000000 unblob_native-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123       51 2023-05-09 08:40:37.000000 unblob_native-0.1.1/rust-toolchain.toml
+-rw-r--r--   0     1001      123      536 2023-05-09 08:40:37.000000 unblob_native-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123      626 2023-05-09 08:40:37.000000 unblob_native-0.1.1/src/math.rs
+-rw-r--r--   0     1001      123      528 2023-05-09 08:40:37.000000 unblob_native-0.1.1/tests/test_math.py
+-rw-r--r--   0     1001      123      160 2023-05-09 08:40:37.000000 unblob_native-0.1.1/unblob_native/__init__.py
+-rw-r--r--   0     1001      123       65 2023-05-09 08:40:37.000000 unblob_native-0.1.1/unblob_native/_native/__init__.pyi
+-rw-r--r--   0     1001      123       47 2023-05-09 08:40:37.000000 unblob_native-0.1.1/unblob_native/_native/math_tools.pyi
+-rw-r--r--   0     1001      123        0 2023-05-09 08:40:37.000000 unblob_native-0.1.1/unblob_native/py.typed
+-rw-r--r--   0     1001      123    21787 2023-05-09 08:40:37.000000 unblob_native-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 unblob_native-0.1.1/PKG-INFO
```

### Comparing `unblob_native-0.1.0/.github/workflows/CI.yml` & `unblob_native-0.1.1/.github/workflows/CI.yml`

 * *Files 14% similar despite different names*

```diff
@@ -19,23 +19,51 @@
     steps:
       - uses: actions/checkout@v3
       - uses: cachix/install-nix-action@v20
       - uses: cachix/cachix-action@v12
         with:
           name: unblob
           authToken: "${{ secrets.CACHIX_AUTH_TOKEN }}"
-      - name: Nix Flake checks
-        run: nix flake check --keep-going --print-build-logs
       - name: Check Nix formatting
         run: nix fmt -- --check .
       - name: Check Python formatting
         run: nix develop -c -- black --check --diff --color .
       - name: Ruff
         run: nix develop -c -- ruff .
 
+  build-nix:
+    strategy:
+      matrix:
+        include:
+          - os: ubuntu-latest
+            arch: x86_64-linux
+          - os: ubuntu-latest
+            arch: aarch64-linux
+          - os: macos-latest
+            arch: x86_64-darwin
+    name: Build Nix - ${{ matrix.arch }}.${{ matrix.os }}
+    runs-on: ${{ matrix.os }}
+    steps:
+      - uses: actions/checkout@v3
+      - uses: cachix/install-nix-action@v20
+      - uses: cachix/cachix-action@v12
+        with:
+          name: unblob
+          authToken: ${{ secrets.CACHIX_AUTH_TOKEN }}
+      - name: Setup emulation
+        if: ${{ matrix.arch == 'aarch64-linux' }}
+        run: |
+          sudo apt update
+          sudo apt install -q -y qemu-system-aarch64 qemu-efi binfmt-support qemu-user-static
+          mkdir -p ~/.config/nix
+          echo "system-features = aarch64-linux arm-linux" | sudo tee -a /etc/nix/nix.conf
+      - name: Nix Flake checks
+        run: |
+          nix flake check --keep-going --print-build-logs --option system ${{ matrix.arch }} --extra-platforms ${{ matrix.arch }}
+
   pytest:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
         os: [ubuntu-latest, macOS-latest]
     steps:
@@ -88,24 +116,33 @@
   #    maturin generate-ci --platform linux macos -- github
   #
   wheel-linux:
     runs-on: ubuntu-latest
     needs: [checks, pytest, pyright]
     strategy:
       matrix:
-        target: [x86_64, aarch64]
+        include:
+          - target: x86_64
+          - target: aarch64
+            cross: true
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
+      - name: setup emulation
+        if: ${{ matrix.cross }}
+        run: |
+          sudo apt update
+          sudo apt install -q -y qemu-system-${{ matrix.target }} qemu-efi binfmt-support qemu-user-static
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
+          container: quay.io/pypa/manylinux2014_${{ matrix.target }}:latest
           args: --release --out dist
           sccache: "true"
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
@@ -150,15 +187,15 @@
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [wheel-linux, wheel-macos, sdist]
+    needs: [build-nix, wheel-linux, wheel-macos, sdist]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
```

### Comparing `unblob_native-0.1.0/.github/workflows/Update.yml` & `unblob_native-0.1.1/.github/workflows/Update.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,13 +14,13 @@
           extra_nix_config: |
             access-tokens = github.com=${{ secrets.GITHUB_TOKEN }}
       - uses: cachix/cachix-action@v12
         with:
           name: unblob
           authToken: "${{ secrets.CACHIX_AUTH_TOKEN }}"
       - name: Update flake.lock
-        uses: DeterminateSystems/update-flake-lock@vX
+        uses: DeterminateSystems/update-flake-lock@v19
         with:
           pr-title: "Update flake.lock" # Title of PR to be created
           pr-labels: | # Labels to be set on the PR
             dependencies
             automated
```

### Comparing `unblob_native-0.1.0/.github/workflows/check-mergeable.yml` & `unblob_native-0.1.1/.github/workflows/check-mergeable.yml`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/.pre-commit-config.yaml` & `unblob_native-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/CODE_OF_CONDUCT.md` & `unblob_native-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/LICENSE` & `unblob_native-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/README.md` & `unblob_native-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/SECURITY.md` & `unblob_native-0.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/benches/benches_main.rs` & `unblob_native-0.1.1/benches/benches_main.rs`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     for sample_size in [256, 1 * kB, 64 * kB, 256 * kB, 1 * MB] {
         group.throughput(Throughput::Bytes(sample_size as u64));
         group.bench_with_input(
             BenchmarkId::from_parameter(sample_size),
             &sample_size,
             |b, &size| {
-                b.iter(|| unblob_native::shannon_entropy(&sample[0..size]));
+                b.iter(|| unblob_native::math::shannon_entropy(&sample[0..size]));
             },
         );
     }
     group.finish();
 }
 
 criterion_group!(benches, shannon_entropy);
```

### Comparing `unblob_native-0.1.0/flake.nix` & `unblob_native-0.1.1/flake.nix`

 * *Files 4% similar despite different names*

```diff
@@ -7,45 +7,41 @@
     nix-filter.url = "github:numtide/nix-filter";
 
     crane = {
       url = "github:ipetkov/crane";
       inputs.nixpkgs.follows = "nixpkgs";
     };
 
-    fenix = {
-      url = "github:nix-community/fenix";
+    rust-overlay = {
+      url = "github:oxalica/rust-overlay";
       inputs.nixpkgs.follows = "nixpkgs";
-      inputs.rust-analyzer-src.follows = "";
     };
 
     flake-utils.url = "github:numtide/flake-utils";
 
     advisory-db = {
       url = "github:rustsec/advisory-db";
       flake = false;
     };
   };
 
-  outputs = { self, nixpkgs, nix-filter, crane, fenix, flake-utils, advisory-db, ... }:
+  outputs = { self, nixpkgs, nix-filter, crane, rust-overlay, flake-utils, advisory-db, ... }:
     flake-utils.lib.eachDefaultSystem (system:
       let
         pkgs = import nixpkgs {
           inherit system;
+          overlays = [ (import rust-overlay) ];
         };
 
         filter = nix-filter.lib;
 
         inherit (pkgs) lib makeRustPlatform python3Packages;
 
-        channel = (builtins.fromTOML (builtins.readFile ./rust-toolchain.toml)).toolchain.channel;
-        rust-toolchain = fenix.packages.${system}.toolchainOf {
-          inherit channel;
-          sha256 = "sha256-otgm+7nEl94JG/B+TYhWseZsHV1voGcBsW/lOD2/68g=";
-        };
-        craneLib = crane.lib.${system}.overrideToolchain rust-toolchain.toolchain;
+        rust-toolchain = pkgs.rust-bin.fromRustupToolchainFile ./rust-toolchain.toml;
+        craneLib = crane.lib.${system}.overrideToolchain rust-toolchain;
         src = craneLib.cleanCargoSource (craneLib.path ./.);
 
         # Common arguments can be set here to avoid repeating them later
         commonArgs = {
           inherit src;
 
           buildInputs = [
@@ -57,32 +53,35 @@
           ];
 
           # Additional environment variables can be set directly
           # MY_CUSTOM_VAR = "some value";
         };
 
         craneLibLLvmTools = craneLib.overrideToolchain
-          (fenix.packages.${system}.complete.withComponents [
-            "cargo"
-            "llvm-tools"
-            "rustc"
-          ]);
+          (rust-toolchain.override {
+            extensions = [
+              "cargo"
+              "llvm-tools-preview"
+              "rustc"
+            ];
+          });
 
         # Build *just* the cargo dependencies, so we can reuse
         # all of that work (e.g. via cachix) when running in CI
         cargoArtifacts = craneLib.buildDepsOnly commonArgs;
 
         # Build the actual crate itself, reusing the dependency
         # artifacts from above.
         libunblob-native = craneLib.buildPackage (commonArgs // {
           inherit cargoArtifacts;
         });
 
         rustPlatform = makeRustPlatform {
-          inherit (rust-toolchain) cargo rustc;
+          rustc = rust-toolchain;
+          cargo = rust-toolchain;
         };
 
         unblob-native = python3Packages.buildPythonPackage
           {
             inherit (libunblob-native) pname version;
             format = "pyproject";
 
@@ -96,15 +95,15 @@
                 "benches"
                 "src"
                 "README.md"
                 "LICENSE"
               ];
             };
 
-            buildInputs = [ pkgs.maturin ];
+            buildInputs = commonArgs.buildInputs ++ [ pkgs.maturin ];
 
             strictDeps = true;
             doCheck = false;
             cargoDeps = rustPlatform.importCargoLock {
               lockFile = ./Cargo.lock;
             };
 
@@ -169,22 +168,14 @@
           };
 
           # Audit dependencies
           libunblob-native-audit = craneLib.cargoAudit {
             inherit src advisory-db;
           };
 
-          # Run tests with cargo-nextest
-          # Consider setting `doCheck = false` on `libunblob-native` if you do not want
-          # the tests to run twice
-          libunblob-native-nextest = craneLib.cargoNextest (commonArgs // {
-            inherit cargoArtifacts;
-            partitions = 1;
-            partitionType = "count";
-          });
         } // lib.optionalAttrs (system == "x86_64-linux") {
           # NB: cargo-tarpaulin only supports x86_64 systems
           # Check code coverage (note: this will not upload coverage anywhere)
           libunblob-native-coverage = craneLib.cargoTarpaulin (commonArgs // {
             inherit cargoArtifacts;
           });
         };
```

### Comparing `unblob_native-0.1.0/pdm.lock` & `unblob_native-0.1.1/pdm.lock`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/pyproject.toml` & `unblob_native-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 authors = [
   {name = "ONEKEY", email = "support@onekey.com"},
 ]
 description = "Performance-critical functionality for Unblob"
 license = {file = "LICENSE"}
 readme = "README.md"
 
-requires-python = "~=3.8"
+requires-python = ">=3.8"
+dynamic = ["version"] # Calculated from the rust module version
 
 [project.urls]
 homepage = "https://unblob.org"
 repository = "https://github.com/onekey-sec/unblob-native"
 
 [tool.pdm.scripts]
 venv = "pdm sync -d"
```

### Comparing `unblob_native-0.1.0/src/math.rs` & `unblob_native-0.1.1/src/math.rs`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/tests/test_math.py` & `unblob_native-0.1.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `unblob_native-0.1.0/Cargo.lock` & `unblob_native-0.1.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -632,15 +632,15 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "unblob-native"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "approx",
  "criterion",
  "pyo3",
  "rand",
 ]
```

### Comparing `unblob_native-0.1.0/PKG-INFO` & `unblob_native-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: unblob-native
-Version: 0.1.0
+Version: 0.1.1
 License-File: LICENSE
 Summary: Performance-critical functionality for Unblob
 Author-email: ONEKEY <support@onekey.com>
 License: MIT
-Requires-Python: ~=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://unblob.org
 Project-URL: repository, https://github.com/onekey-sec/unblob-native
+Project-URL: homepage, https://unblob.org
 
 # unblob-native
 
 Looking for Unblob? Check out at https://unblob.org.
 
 This package holds performance-critical components of Unblob,
 an _accurate, fast, and easy-to-use_ **extraction suite**. It parses
```

