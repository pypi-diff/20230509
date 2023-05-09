# Comparing `tmp/reddit_decider-1.2.8.tar.gz` & `tmp/reddit_decider-1.2.9.tar.gz`

## Comparing `reddit_decider-1.2.8.tar` & `reddit_decider-1.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 reddit_decider-1.2.8/local_dependencies/decider/Cargo.toml
--rw-r--r--   0        0        0       19 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/local_dependencies/decider/.gitignore
--rw-r--r--   0        0        0      710 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/local_dependencies/decider/README.md
--rw-r--r--   0        0        0     6148 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/local_dependencies/decider/benches/decider.rs
--rw-r--r--   0        0        0    46902 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/local_dependencies/decider/src/events.rs
--rw-r--r--   0        0        0    80020 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/local_dependencies/decider/src/lib.rs
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 reddit_decider-1.2.8/Cargo.toml
--rw-r--r--   0        0        0       66 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/.gitignore
--rw-r--r--   0        0        0      910 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/README.md
--rw-r--r--   0        0        0       34 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/__init__.py
--rw-r--r--   0        0        0       76 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/pyproject.toml
--rw-r--r--   0        0        0       40 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/setup.cfg
--rw-r--r--   0        0        0     1284 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/setup.py
--rw-r--r--   0        0        0    20979 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/src/lib.rs
--rw-r--r--   0        0        0       66 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/test/.gitignore
--rw-r--r--   0        0        0    10110 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/test/integration_test.py
--rw-r--r--   0        0        0       93 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/test/requirements.txt
--rw-r--r--   0        0        0     2903 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/test/test_rust.py
--rw-r--r--   0        0        0    33983 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/test/unit_test.py
--rw-r--r--   0        0        0     3088 2022-07-05 21:06:01.000000 reddit_decider-1.2.8/test/utils.py
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 reddit_decider-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 reddit_decider-1.2.9/local_dependencies/decider/Cargo.toml
+-rw-r--r--   0        0        0       19 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/.gitignore
+-rw-r--r--   0        0        0      710 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/README.md
+-rw-r--r--   0        0        0     6148 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/benches/decider.rs
+-rw-r--r--   0        0        0    46902 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/src/events.rs
+-rw-r--r--   0        0        0    80028 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/src/lib.rs
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 reddit_decider-1.2.9/Cargo.toml
+-rw-r--r--   0        0        0       66 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/.gitignore
+-rw-r--r--   0        0        0      910 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/README.md
+-rw-r--r--   0        0        0       34 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/__init__.py
+-rw-r--r--   0        0        0       76 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0       40 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/setup.cfg
+-rw-r--r--   0        0        0     1284 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/setup.py
+-rw-r--r--   0        0        0    20979 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/src/lib.rs
+-rw-r--r--   0        0        0       66 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/.gitignore
+-rw-r--r--   0        0        0    10110 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/integration_test.py
+-rw-r--r--   0        0        0       93 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/requirements.txt
+-rw-r--r--   0        0        0     2903 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/test_rust.py
+-rw-r--r--   0        0        0    33983 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/unit_test.py
+-rw-r--r--   0        0        0     3088 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/utils.py
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 reddit_decider-1.2.9/PKG-INFO
```

### Comparing `reddit_decider-1.2.8/local_dependencies/decider/Cargo.toml` & `reddit_decider-1.2.9/local_dependencies/decider/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "decider"
-version = "1.2.8"
+version = "1.2.9"
 edition = "2021"
 description = "a package for AB-testing and dynamic config"
 homepage = "https://mattknox.com"
 license = "MIT"
 documentation = "https://mattknox.com/decider"
 readme = "README.md"
```

### Comparing `reddit_decider-1.2.8/local_dependencies/decider/README.md` & `reddit_decider-1.2.9/local_dependencies/decider/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/local_dependencies/decider/benches/decider.rs` & `reddit_decider-1.2.9/local_dependencies/decider/benches/decider.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/local_dependencies/decider/src/events.rs` & `reddit_decider-1.2.9/local_dependencies/decider/src/events.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/local_dependencies/decider/src/lib.rs` & `reddit_decider-1.2.9/local_dependencies/decider/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -958,16 +958,16 @@
     }
 }
 
 /// An `Event` holds a hydrated exposure event, serialized as a json string, as well as an explicit
 /// `DecisionKind`. The kind can be used by the client to choose whether to expose this event.
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub struct Event {
-    kind: DecisionKind,
-    json: String,
+    pub kind: DecisionKind,
+    pub json: String,
 }
 
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub struct Decision {
     pub feature_id: u32,
     pub feature_name: String,
     pub feature_version: u32,
```

### Comparing `reddit_decider-1.2.8/Cargo.toml` & `reddit_decider-1.2.9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "reddit-decider"
-version = "1.2.8"
+version = "1.2.9"
 edition = "2021"
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 decider = { path = "local_dependencies/decider" }
 pythonize = "0.16.0"
 serde_json = "^1.0.59"
```

### Comparing `reddit_decider-1.2.8/README.md` & `reddit_decider-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/setup.py` & `reddit_decider-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/src/lib.rs` & `reddit_decider-1.2.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/test/integration_test.py` & `reddit_decider-1.2.9/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/test/test_rust.py` & `reddit_decider-1.2.9/test/test_rust.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/test/unit_test.py` & `reddit_decider-1.2.9/test/unit_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/test/utils.py` & `reddit_decider-1.2.9/test/utils.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.8/PKG-INFO` & `reddit_decider-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-decider
-Version: 1.2.8
+Version: 1.2.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # rust_decider
 
 Rust implementation of bucketing, targeting, overrides, and dynamic config logic.
 
 ## Usage
```

