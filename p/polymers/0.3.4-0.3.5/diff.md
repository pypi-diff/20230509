# Comparing `tmp/polymers-0.3.4-cp39-none-win_amd64.whl.zip` & `tmp/polymers-0.3.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1446874 bytes, number of entries: 6
--rw-r--r--  4.6 unx     4213 b- defN 23-May-01 22:10 polymers-0.3.4.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-May-01 22:10 polymers-0.3.4.dist-info/WHEEL
--rw-r--r--  4.6 unx     1569 b- defN 23-May-01 22:10 polymers-0.3.4.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      115 b- defN 23-May-01 22:10 polymers/__init__.py
--rwxr-xr-x  4.6 unx  6094336 b- defN 23-May-01 22:10 polymers/polymers.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      484 b- defN 23-May-01 22:10 polymers-0.3.4.dist-info/RECORD
-6 files, 6100813 bytes uncompressed, 1446004 bytes compressed:  76.3%
+Zip file size: 1479291 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     3523 b- defN 23-May-08 23:32 polymers-0.3.5.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-May-08 23:32 polymers-0.3.5.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1569 b- defN 23-May-08 23:32 polymers-0.3.5.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      115 b- defN 23-May-08 23:32 polymers/__init__.py
+-rwxr-xr-x  4.6 unx  6302208 b- defN 23-May-08 23:32 polymers/polymers.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      484 b- defN 23-May-08 23:32 polymers-0.3.5.dist-info/RECORD
+6 files, 6307994 bytes uncompressed, 1478421 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: polymers-0.3.4.dist-info/METADATA
+Filename: polymers-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: polymers-0.3.4.dist-info/WHEEL
+Filename: polymers-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: polymers-0.3.4.dist-info/license_files/LICENSE
+Filename: polymers-0.3.5.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: polymers/__init__.py
 Comment: 
 
 Filename: polymers/polymers.cp39-win_amd64.pyd
 Comment: 
 
-Filename: polymers-0.3.4.dist-info/RECORD
+Filename: polymers-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `polymers-0.3.4.dist-info/METADATA` & `polymers-0.3.5.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymers
-Version: 0.3.4
+Version: 0.3.5
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: cffi
@@ -37,61 +37,37 @@
 
 The library can be installed as a Python package:
 
 ```shell
 pip install polymers
 ```
 
-If Rust is installed, the latest edition of the library can be installed from the GitHub repository:
-
-```shell
-git clone git@github.com:sandialabs/Polymers.git
-cd Polymers/
-pip install maturin
-maturin build --features python
-pip install target/wheels/*.whl
-```
-
 ## Julia
 
 [![docs (stable)](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/julia-docs-stable.svg)](https://sandialabs.github.io/Polymers/julia/docs/stable)
 [![docs (latest)](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/julia-docs-latest.svg)](https://sandialabs.github.io/Polymers/julia/docs/latest)
 [![Pkg](https://img.shields.io/github/v/release/sandialabs/Polymers?color=cb3c33&label=Pkg&logo=Julia&logoColor=cb3c33)](#)
 
 The library can be installed as a Julia package:
 
 ```julia
 using Pkg
 Pkg.add("Polymers")
 ```
 
-If Rust is installed, the latest edition of the library can be installed from the GitHub repository:
-
-```julia
-using Pkg
-Pkg.add(url="https://github.com/sandialabs/Polymers")
-```
-
 ## Rust
 
 [![docs (stable)](https://img.shields.io/badge/Docs-stable-e57300?logo=rust&logoColor=000000)](https://docs.rs/crate/polymers)
 [![docs (latest)](https://img.shields.io/badge/Docs-latest-e57300?logo=rust&logoColor=000000)](https://sandialabs.github.io/Polymers/rust/docs/latest)
 [![crates](https://img.shields.io/crates/v/polymers?logo=rust&logoColor=000000&label=Crates&color=32592f)](https://crates.io/crates/polymers)
 
-The library can be used in an existing Rust project by adding the `polymers` crate to Cargo.toml:
+The library can be added to an existing Rust project:
 
-```toml
-[dependencies]
-polymers = "*"
-```
-To use the latest edition of the library, add the GitHub repository to Cargo.toml:
-
-```toml
-[dependencies]
-regex = { git = "https://github.com/sandialabs/polymers" }
+```shell
+cargo add polymers
 ```
 
 ## Citation
 
 [![doi](https://img.shields.io/badge/Zenodo-10.5281%2Fzenodo.7041983-blue)](https://doi.org/10.5281/zenodo.7041983)
 
 Michael R. Buche. Polymers Modeling Library. [Zenodo (2023)](https://doi.org/10.5281/zenodo.7041983).
```

## Comparing `polymers-0.3.4.dist-info/license_files/LICENSE` & `polymers-0.3.5.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

