# Comparing `tmp/issue_db_api-0.7.2.tar.gz` & `tmp/issue_db_api-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.7.2.tar", last modified: Mon May  8 13:34:52 2023, max compression
+gzip compressed data, was "issue_db_api-0.7.3.tar", last modified: Tue May  9 14:48:59 2023, max compression
```

## Comparing `issue_db_api-0.7.2.tar` & `issue_db_api-0.7.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.7.2/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-08 13:34:16.000000 issue_db_api-0.7.2/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.7.2/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8397 2023-05-04 14:07:06.000000 issue_db_api-0.7.2/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    44393 2023-05-08 13:33:40.000000 issue_db_api-0.7.2/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5275 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.7.2/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6638 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    38608 2023-05-04 13:59:32.000000 issue_db_api-0.7.2/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.7.2/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6387 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2514 2023-05-05 12:20:10.000000 issue_db_api-0.7.2/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-08 13:34:52.000000 issue_db_api-0.7.2/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-08 13:34:52.000000 issue_db_api-0.7.2/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-08 13:34:52.000000 issue_db_api-0.7.2/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.7.2/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-08 13:34:52.000000 issue_db_api-0.7.2/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-08 13:34:16.000000 issue_db_api-0.7.2/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.7.3/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.033291 issue_db_api-0.7.3/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-09 14:48:21.000000 issue_db_api-0.7.3/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.7.3/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8397 2023-05-04 14:07:06.000000 issue_db_api-0.7.3/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    44641 2023-05-09 14:47:42.000000 issue_db_api-0.7.3/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5275 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.7.3/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6638 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    38608 2023-05-04 13:59:32.000000 issue_db_api-0.7.3/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.7.3/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6387 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.7.3/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2514 2023-05-05 12:20:10.000000 issue_db_api-0.7.3/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-09 14:48:59.033291 issue_db_api-0.7.3/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-09 14:48:58.000000 issue_db_api-0.7.3/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-09 14:48:58.000000 issue_db_api-0.7.3/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-09 14:48:58.000000 issue_db_api-0.7.3/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.7.3/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-09 14:48:58.000000 issue_db_api-0.7.3/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-09 14:48:21.000000 issue_db_api-0.7.3/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-09 14:48:59.037291 issue_db_api-0.7.3/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.7.3/setup.py
```

### Comparing `issue_db_api-0.7.2/LICENSE` & `issue_db_api-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/PKG-INFO` & `issue_db_api-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.7.2
+Version: 0.7.3
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.7.2/issue_db_api/Cargo.toml` & `issue_db_api-0.7.3/issue_db_api/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.7.2"
+version = "0.7.3"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.7.2/issue_db_api/issue_api.pyi` & `issue_db_api-0.7.3/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/api_core.rs` & `issue_db_api-0.7.3/issue_db_api/src/api_core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 use std::collections::HashMap;
 use std::io::Cursor;
 
 #[cfg(feature = "blocking")]
-use reqwest::blocking::Client;
-use reqwest::blocking::{ClientBuilder, multipart};
+use reqwest::blocking::multipart;
 
 use serde_json::{Map, Value};
 use lazy_init::Lazy;
 
 use crate::comments::UnboundComment;
 use crate::config::IssueAttribute;
 use crate::embedding::UnboundEmbedding;
@@ -29,15 +28,16 @@
 /// This struct provides basics means of session management,
 /// and exposes all available endpoints through Rust functions.
 #[allow(unused)]
 #[derive(Debug, Clone)]
 pub struct IssueAPI {
     url: String,
     token: Option<String>,
-    client: Client,
+    allow_unsafe_ssl: bool,
+    client: reqwest::blocking::Client,
 }
 
 #[allow(unused)]
 #[derive(Debug, Clone)]
 pub struct IssueData {
     ident: String,
     key: Lazy<String>,
@@ -268,18 +268,25 @@
                       allow_self_signed: bool) -> APIResult<Self> {
         let mut read_only_api = Self::new_read_only(url, allow_self_signed)?;
         read_only_api.login(username, password)?;
         Ok(read_only_api)
     }
 
     pub(crate) fn new_read_only(url: String, allow_self_signed: bool) -> APIResult<Self> {
-        let client = ClientBuilder::new()
+        let client = reqwest::blocking::ClientBuilder::new()
             .danger_accept_invalid_certs(allow_self_signed)
             .build()?;
-        Ok(IssueAPI{url, token: None, client})
+        Ok(
+            IssueAPI{
+                url,
+                token: None,
+                client,
+                allow_unsafe_ssl: allow_self_signed
+            }
+        )
     }
 
     fn login(&mut self, username: String, password: String) -> APIResult<()> {
         #[derive(serde::Deserialize)]
         struct TokenResponse {
             access_token: String,
             #[allow(dead_code)] token_type: String
@@ -437,15 +444,17 @@
                                          payload: I,
                                          sink: &mut S) -> APIResult<()>
         where
             I: serde::Serialize,
             S: std::io::Write
     {
         let url = self.get_endpoint(suffix);
-        let client = reqwest::Client::new();
+        let client = reqwest::ClientBuilder::new()
+            .danger_accept_invalid_certs(self.allow_unsafe_ssl)
+            .build()?;
         let rt = tokio::runtime::Builder::new_current_thread().enable_all().build()?;
         let result: APIResult<()> = rt.block_on(async {
             let mut stream = client
                 .get(url)
                 .json(&payload)
                 .send()
                 .await?
```

### Comparing `issue_db_api-0.7.2/issue_db_api/src/comments.rs` & `issue_db_api-0.7.3/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/config.rs` & `issue_db_api-0.7.3/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/embedding.rs` & `issue_db_api-0.7.3/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/errors.rs` & `issue_db_api-0.7.3/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/issues.rs` & `issue_db_api-0.7.3/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/labels.rs` & `issue_db_api-0.7.3/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/lib.rs` & `issue_db_api-0.7.3/issue_db_api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/models.rs` & `issue_db_api-0.7.3/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/query.rs` & `issue_db_api-0.7.3/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/repository.rs` & `issue_db_api-0.7.3/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.7.3/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/tags.rs` & `issue_db_api-0.7.3/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api/src/util.rs` & `issue_db_api-0.7.3/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.7.3/issue_db_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.7.2
+Version: 0.7.3
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.7.2/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.7.3/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.2/pyproject.toml` & `issue_db_api-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

