# Comparing `tmp/issue_db_api-0.6.6.tar.gz` & `tmp/issue_db_api-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.6.6.tar", last modified: Tue May  2 11:43:38 2023, max compression
+gzip compressed data, was "issue_db_api-0.7.0.tar", last modified: Thu May  4 14:07:40 2023, max compression
```

## Comparing `issue_db_api-0.6.6.tar` & `issue_db_api-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.6/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.932177 issue_db_api-0.6.6/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-02 11:43:06.000000 issue_db_api-0.6.6/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.6/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.6/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    44849 2023-05-02 11:19:21.000000 issue_db_api-0.6.6/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.6/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    37039 2023-05-02 11:42:57.000000 issue_db_api-0.6.6/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-24 16:50:02.000000 issue_db_api-0.6.6/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.6.6/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6385 2023-04-29 11:56:43.000000 issue_db_api-0.6.6/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.6/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.932177 issue_db_api-0.6.6/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-02 11:43:38.000000 issue_db_api-0.6.6/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-02 11:43:38.000000 issue_db_api-0.6.6/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-02 11:43:38.000000 issue_db_api-0.6.6/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.6/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-02 11:43:38.000000 issue_db_api-0.6.6/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-02 11:43:06.000000 issue_db_api-0.6.6/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-04 14:07:40.655643 issue_db_api-0.7.0/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.7.0/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.7.0/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.7.0/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-04 14:07:40.655643 issue_db_api-0.7.0/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.7.0/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-04 14:07:40.655643 issue_db_api-0.7.0/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-04 13:52:47.000000 issue_db_api-0.7.0/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.7.0/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8397 2023-05-04 14:07:06.000000 issue_db_api-0.7.0/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-04 14:07:40.655643 issue_db_api-0.7.0/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    44361 2023-05-04 14:03:45.000000 issue_db_api-0.7.0/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.7.0/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5275 2023-05-04 13:53:55.000000 issue_db_api-0.7.0/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.7.0/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.7.0/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6638 2023-05-04 13:53:55.000000 issue_db_api-0.7.0/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.7.0/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    38608 2023-05-04 13:59:32.000000 issue_db_api-0.7.0/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.7.0/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.7.0/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6387 2023-05-04 13:53:55.000000 issue_db_api-0.7.0/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-04 14:07:40.655643 issue_db_api-0.7.0/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.7.0/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.7.0/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.7.0/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2401 2023-05-04 13:56:26.000000 issue_db_api-0.7.0/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-04 14:07:40.655643 issue_db_api-0.7.0/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-04 14:07:40.000000 issue_db_api-0.7.0/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-04 14:07:40.000000 issue_db_api-0.7.0/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-04 14:07:40.000000 issue_db_api-0.7.0/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.7.0/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-04 14:07:40.000000 issue_db_api-0.7.0/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-04 13:52:47.000000 issue_db_api-0.7.0/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-04 14:07:40.655643 issue_db_api-0.7.0/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.7.0/setup.py
```

### Comparing `issue_db_api-0.6.6/LICENSE` & `issue_db_api-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.6/PKG-INFO` & `issue_db_api-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.6.6
+Version: 0.7.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.6/issue_db_api/Cargo.toml` & `issue_db_api-0.7.0/issue_db_api/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.6.6"
+version = "0.7.0"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.6.6/issue_db_api/issue_api.pyi` & `issue_db_api-0.7.0/issue_db_api/issue_api.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 import typing
 
 
+class IssueAPIError(Exception):
+    ...
+
+class InvalidCredentialsException(IssueAPIError):
+    ...
+
+class NotAuthorizedException(IssueAPIError):
+    ...
+
+class InvalidTokenException(IssueAPIError):
+    ...
+
+class HTTPException(IssueAPIError):
+    ...
+
+class LibraryException(IssueAPIError):
+    ...
+
+
 class IssueRepository:
     def __init__(self,
                  url: str, *,
                  credentials: tuple[str, str] | None = None,
                  label_caching_policy: str = 'no_caching',
                  config_handling_policy: str = 'read_fetch_write_fetch',
                  allow_self_signed_certificates: bool = False):
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/api_core.rs` & `issue_db_api-0.7.0/issue_db_api/src/api_core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 use crate::config::IssueAttribute;
 use crate::embedding::UnboundEmbedding;
 use crate::schemas::raw_issue_response::RawIssueData;
 use crate::query::Query;
 use crate::labels::Label;
 use crate::tags::UnboundTag;
 use crate::util::initialize_lazy_field;
-use crate::util::APIResult;
+use crate::errors::APIResult;
 use crate::errors::*;
 use crate::models::{ModelInfo, UnboundModelConfig, UnboundModelVersion, UnboundTestRun};
 
 //////////////////////////////////////////////////////////////////////////////////////////////////
 //////////////////////////////////////////////////////////////////////////////////////////////////
 // Core Structs
 //////////////////////////////////////////////////////////////////////////////////////////////////
@@ -30,15 +30,14 @@
 /// and exposes all available endpoints through Rust functions.
 #[allow(unused)]
 #[derive(Debug, Clone)]
 pub struct IssueAPI {
     url: String,
     token: Option<String>,
     client: Client,
-    debug: bool
 }
 
 #[allow(unused)]
 #[derive(Debug, Clone)]
 pub struct IssueData {
     ident: String,
     key: Lazy<String>,
@@ -272,26 +271,15 @@
         Ok(read_only_api)
     }
 
     pub(crate) fn new_read_only(url: String, allow_self_signed: bool) -> APIResult<Self> {
         let client = ClientBuilder::new()
             .danger_accept_invalid_certs(allow_self_signed)
             .build()?;
-        println!("Debug state: {}", Self::get_debug_state()?);
-        Ok(IssueAPI{url, token: None, client, debug: Self::get_debug_state()?})
-    }
-
-    fn get_debug_state() -> APIResult<bool> {
-        match std::env::var("ISSUE_API_CLIENT_DEBUG") {
-            Ok(value) => {
-                let converted = value.to_lowercase();
-                Ok(converted == "true" || converted == "1")
-            }
-            Err(_) => Ok(false)
-        }
+        Ok(IssueAPI{url, token: None, client})
     }
 
     fn login(&mut self, username: String, password: String) -> APIResult<()> {
         #[derive(serde::Deserialize)]
         struct TokenResponse {
             access_token: String,
             #[allow(dead_code)] token_type: String
@@ -317,15 +305,15 @@
 
     fn get_endpoint(&self, suffix: &str) -> String {
         self.url.clone() + "/" + suffix
     }
 
     fn get_auth(&self) -> APIResult<String> {
         if self.token.is_none() {
-            Err(Box::try_from(AuthenticationError {}).unwrap())
+            Err(APIError::NotAuthorized)
         } else {
             Ok(self.token.clone().unwrap())
         }
     }
 
     fn build_request_base(&self, suffix: &str, verb: Verb) -> APIResult<reqwest::blocking::RequestBuilder> {
         let url = self.get_endpoint(suffix);
@@ -358,44 +346,46 @@
                                 suffix: &str,
                                 verb: Verb,
                                 payload: I) -> APIResult<O>
     where
         I: serde::Serialize + std::fmt::Debug,
         O: for <'de> serde::Deserialize<'de>,
     {
-        if self.debug {
-            println!("Performing {:?} request to endpoint {}", verb, suffix);
-            println!("Request payload: {:?}", payload);
-        }
-        let response = self.build_request_base(suffix, verb)?.json(&payload).send()?;
+        let response = self.build_request_base(suffix, verb)?
+            .json(&payload)
+            .send()?;
         let result = self.unpack_response(response)?;
         Ok(result)
     }
 
     fn call_endpoint_form<I, O>(&self,
                                 suffix: &str,
                                 verb: Verb,
                                 payload: &I) -> APIResult<O>
         where
             I: serde::Serialize + ?Sized,
             O: for <'de> serde::Deserialize<'de>,
     {
-        let response = self.build_request_base(suffix, verb)?.form(payload).send()?;
+        let response = self.build_request_base(suffix, verb)?
+            .form(payload)
+            .send()?;
         let result = self.unpack_response(response)?;
         Ok(result)
     }
 
     fn call_endpoint_multipart<O>(&self,
                                   suffix: &str,
                                   verb: Verb,
                                   payload: multipart::Form) -> APIResult<O>
         where
             O: for <'de> serde::Deserialize<'de>,
     {
-        let response = self.build_request_base(suffix, verb)?.multipart(payload).send()?;
+        let response = self.build_request_base(suffix, verb)?
+            .multipart(payload)
+            .send()?;
         let result = self.unpack_response(response)?;
         Ok(result)
     }
 
     fn call_endpoint_multipart_object<I, O>(&self,
                                             suffix: &str,
                                             verb: Verb,
@@ -453,15 +443,16 @@
         let url = self.get_endpoint(suffix);
         let client = reqwest::Client::new();
         let rt = tokio::runtime::Builder::new_current_thread().enable_all().build()?;
         let result: APIResult<()> = rt.block_on(async {
             let mut stream = client
                 .get(url)
                 .send()
-                .await?;
+                .await?
+                .error_for_status()?;
             while let Some(chunk) = stream.chunk().await? {
                 sink.write_all(chunk.as_ref())?;
             }
             Ok(())
         });
         result
     }
@@ -518,15 +509,15 @@
             Value::Object(map)
         )?;
         let mut ids: Vec<String> = Vec::with_capacity(keys.len());
         for key in keys {
             match result.issue_ids.get(&key) {
                 None => {
                     let msg = format!("No ID found for key \"{}\"", key);
-                    return Err(Box::new(APIError::new(msg)));
+                    return Err(APIError::GenericError(msg));
                 },
                 Some(id) => ids.push(id.clone())
             }
         }
         Ok(ids)
     }
 
@@ -704,15 +695,15 @@
         // Get object IDS in order to restore comment order
         let mut object_ids: Vec<u128> = Vec::with_capacity(converted.len());
         for c in converted.iter() {
             // let id = c.id
             //     .parse::<u128>()
             //     .map_err(|e| IDParsingError{msg: e.to_string()})?;
             let id = u128::from_str_radix(c.id.as_str(), 16)
-                .map_err(|e| IDParsingError{msg: e.to_string()})?;
+                .map_err(|e| APIError::IDParsingError(e.to_string()))?;
             object_ids.push(id);
         }
         // Sort comments
         let mut pairs = object_ids.into_iter()
             .zip(converted.into_iter()).collect::<Vec<_>>();
         pairs.sort_by_key(|p| p.0);
         // Extract comments without ids
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/comments.rs` & `issue_db_api-0.7.0/issue_db_api/src/comments.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use std::sync::Arc;
 use crate::api_core::IssueAPI;
-use crate::APIResult;
+use crate::errors::APIResult;
 
 #[allow(unused)]
 #[derive(Debug)]
 pub struct UnboundComment {
     pub(crate) id: String,
     pub(crate) author: String,
     pub(crate) text: String
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/config.rs` & `issue_db_api-0.7.0/issue_db_api/src/config.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::collections::HashMap;
 use std::error::Error;
 use std::sync::Arc;
 use crate::api_core::IssueAPI;
-use crate::{APIResult, Query, QueryCMP};
-use crate::errors::APIError;
+use crate::{Query, QueryCMP};
+use crate::errors::{APIError, APIResult};
 use crate::issues::Issue;
 
 #[allow(unused)]
 #[derive(Debug, Copy, Clone, PartialEq, Eq)]
 pub enum ConfigHandlingPolicy {
     ReadLocalWriteNoFetch,
     ReadLocalWriteWithFetch,
@@ -61,15 +61,15 @@
             IssueAttribute::FixVersions => "fixVersions"
         };
         write!(f, "{}", text)
     }
 }
 
 impl TryFrom<String> for IssueAttribute {
-    type Error = Box<dyn Error>;
+    type Error = APIError;
 
     fn try_from(value: String) -> Result<Self, Self::Error> {
         let attr = match value.as_str() {
             "key" => IssueAttribute::Key,
             "summary" => IssueAttribute::Summary,
             "description" => IssueAttribute::Description,
             "comments" => IssueAttribute::Comments,
@@ -87,15 +87,15 @@
             "date_resolved" => IssueAttribute::DateResolved,
             "labels" => IssueAttribute::Labels,
             "components" => IssueAttribute::Components,
             "affected+versions" => IssueAttribute::AffectedVersions,
             "fix_versions" => IssueAttribute::FixVersions,
             _ => {
                 let msg = format!("\"{}\" is an invalid issue attribute", value);
-                return Err(Box::new(APIError::new(msg)));
+                return Err(APIError::GenericError(msg));
             }
         };
         Ok(attr)
     }
 }
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/embedding.rs` & `issue_db_api-0.7.0/issue_db_api/src/embedding.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::collections::HashMap;
 use std::hash::{Hash, Hasher};
 use std::sync::Arc;
 use serde_json::Value;
 use crate::api_core::IssueAPI;
-use crate::APIResult;
+use crate::errors::APIResult;
 use crate::config::ConfigHandlingPolicy;
 
 #[allow(unused)]
 #[derive(Debug, serde::Deserialize)]
 pub(crate) struct UnboundEmbedding {
     pub(crate) embedding_id: String,
     pub(crate) name: String,
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/errors.rs` & `issue_db_api-0.7.0/issue_db_api/src/errors.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,64 @@
-//////////////////////////////////////////////////////////////////////////////////////////////////
-//////////////////////////////////////////////////////////////////////////////////////////////////
-// Custom errors
-//////////////////////////////////////////////////////////////////////////////////////////////////
-
-use std::error::Error;
-
 #[allow(unused)]
 #[derive(Debug)]
-pub struct AuthenticationError {}
-
-impl std::fmt::Display for AuthenticationError {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        write!(f, "Attempted to invoke an authenticated endpoint without token")
-    }
+pub enum APIError {
+    InvalidCredentials,
+    InvalidToken,
+    NotAuthorized,
+    HTTPError{message: String, status_code: u16},
+    IDParsingError(String),
+    LibraryError(String),
+    GenericError(String)
 }
 
-impl Error for AuthenticationError {
-    fn source(&self) -> Option<&(dyn Error + 'static)> {
-        None
+impl std::fmt::Display for APIError {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        match self {
+            APIError::InvalidCredentials => write!(f, "Invalid credentials"),
+            APIError::InvalidToken => write!(f, "Invalid token"),
+            APIError::NotAuthorized => write!(f, "Calling authorized endpoint without token"),
+            APIError::HTTPError { message, status_code } => {
+                write!(f, "Error in HTTP (code = {status_code}): {message}")
+            },
+            APIError::IDParsingError(msg) => write!(f, "Error while parsing ObjectID: {msg}"),
+            APIError::LibraryError(msg) => write!(f, "Internal error in library: {msg}"),
+            APIError::GenericError(msg) => write!(f, "Error: {msg}")
+        }
     }
 }
 
+impl std::error::Error for APIError {}
 
-#[allow(unused)]
-#[derive(Debug)]
-pub struct IDParsingError {
-    pub msg: String
-}
-
-impl std::fmt::Display for IDParsingError {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        write!(f, "Failed to parse ObjectID: {}", self.msg)
+impl From<reqwest::Error> for APIError {
+    fn from(value: reqwest::Error) -> Self {
+        if value.is_status() {
+            let code = value.status().expect("Expected status code");
+            if code == reqwest::StatusCode::UNAUTHORIZED {
+                APIError::InvalidCredentials
+            } else {
+                APIError::HTTPError{message: value.to_string(), status_code: code.as_u16()}
+            }
+        } else {
+            APIError::LibraryError(value.to_string())
+        }
     }
 }
 
-impl Error for IDParsingError {
-    fn source(&self) -> Option<&(dyn Error + 'static)> {
-        None
+impl From<std::io::Error> for APIError {
+    fn from(value: std::io::Error) -> Self {
+        APIError::GenericError(value.to_string())
     }
 }
 
-
-#[allow(unused)]
-#[derive(Debug)]
-pub struct APIError {
-    msg: String
-}
-
-impl APIError {
-    pub fn new(msg: String) -> Self {
-        APIError{msg}
+impl From<serde_json::Error> for APIError {
+    fn from(value: serde_json::Error) -> Self {
+        APIError::GenericError(value.to_string())
     }
 }
 
-impl std::fmt::Display for APIError {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        write!(f, "Error in API: {}", self.msg)
+impl From<crate::util::CacheLockError> for APIError {
+    fn from(value: crate::util::CacheLockError) -> Self {
+        APIError::LibraryError(value.to_string())
     }
 }
 
-impl Error for APIError {
-    fn source(&self) -> Option<&(dyn Error + 'static)> {
-        None
-    }
-}
+pub type APIResult<T> = Result<T, APIError>;
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/issues.rs` & `issue_db_api-0.7.0/issue_db_api/src/issues.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 use std::hash::{Hash, Hasher};
-use std::sync::{Arc, RwLock};
+use std::sync::Arc;
 use std::sync::atomic::{AtomicBool, Ordering};
 use crate::api_core::{IssueAPI, IssueData};
 use crate::comments::Comment;
 use crate::config::{CachingPolicy, IssueLoadingSettings};
+use crate::errors::APIResult;
 use crate::labels::Label;
-use crate::util::APIResult;
+use crate::util::CacheContainer;
 
 #[allow(unused)]
 #[derive(Debug)]
 pub struct Issue {
     api: Arc<IssueAPI>,
     ident: String,
     data: IssueData,
     caching_policy: CachingPolicy,
-    label: RwLock<Option<Label>>,
+    label: CacheContainer<Option<Label>>,
     dirty: AtomicBool
 }
 
 impl Hash for Issue {
     fn hash<H: Hasher>(&self, state: &mut H) {
         self.ident.hash(state);
     }
@@ -38,84 +39,37 @@
                       ident: String,
                       data: IssueData,
                       caching: CachingPolicy,
                       label: Option<Label>) -> Self {
          Self{
              api, ident, data,
              caching_policy: caching,
-             label: RwLock::new(label),
+             label: CacheContainer::new(Some(label)),
              dirty: AtomicBool::new(false)
         }
     }
 
     #[inline(always)]
     pub fn ident(&self) -> &String {
         &self.ident
     }
 
     pub fn get_manual_label(&self) -> APIResult<Option<Label>> {
-        match self.caching_policy {
-            CachingPolicy::NoCaching => {
-                self.load_label()
-            }
-            CachingPolicy::UseLocalAfterLoad => {
-                let label = self.label
-                    .read()
-                    .expect("RwLock has been poisoned. Cannot recover");
-                if label.is_some() && !self.dirty.load(Ordering::Acquire) {
-                    Ok(Some(label.unwrap()))
-                } else {
-                    // First, acquire the write lock
-                    std::mem::drop(label);
-                    let mut label = self.label
-                        .write()
-                        .expect("RwLock has been poisoned. Cannot recover");
-                    // With the write lock in hand, check if another thread
-                    // updated the label in the meantime.
-                    if self.dirty.load(Ordering::Relaxed) && label.is_none() {
-                        // The label is definitely dirty; update it
-                        if let Some(inner) = self.load_label()? {
-                            label.insert(inner);
-                            self.dirty.store(false, Ordering::Release);
-                            Ok(Some(inner))
-                        } else {
-                            label.take();
-                            self.dirty.store(false, Ordering::Release);
-                            Ok(None)
-                        }
-                    } else {
-                        // Another thread updated the label; use a recursive
-                        // call to fetch the label.
-                        self.get_manual_label()
-                    }
-                }
-            }
-        }
+        self.label.get(|| self.load_label())
     }
 
     fn load_label(&self) -> APIResult<Option<Label>> {
         let labels = self.api.get_manual_labels(
             vec![self.ident.clone()]
         )?;
         Ok(labels.get(&self.ident).copied())
     }
 
     pub fn set_manual_label(&self, label: Label) -> APIResult<()> {
-        self.api.update_manual_label_for_issue(self.ident.clone(), label)?;
-        if self.caching_policy == CachingPolicy::UseLocalAfterLoad {
-            let mut label = self.label
-                .write()
-                .expect("RwLock has been poisoned. Cannot recover");
-            if let Some(inner) = self.load_label()? {
-                label.insert(inner);
-            } else {
-                label.take();
-            }
-        }
-        Ok(())
+        self.label.set(Some(label))
     }
 
     pub fn invalidate_cached_label(&self) {
         self.dirty.store(true, Ordering::Release);
     }
 
     pub fn get_tags(&self) -> APIResult<Vec<String>> {
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/labels.rs` & `issue_db_api-0.7.0/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.6/issue_db_api/src/lib.rs` & `issue_db_api-0.7.0/issue_db_api/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 mod comments;
 mod issues;
 mod config;
 mod errors;
 mod models;
 
 pub use repository::IssueRepository;
-pub use util::APIResult;
+pub use errors::APIResult;
 pub use query::{Query, QueryCMP};
 
 
 #[cfg(feature = "pyo3")]
 mod python {
     use std::collections::HashMap;
     use std::hash::{Hash, Hasher};
@@ -26,31 +26,48 @@
     use pyo3::create_exception;
     use pyo3::exceptions::{PyException, PyTypeError, PyValueError};
     use pyo3::types::{IntoPyDict, PyBool, PyDict, PyFloat, PyInt, PyList, PyLong, PyString, PyTuple};
     use serde_json::{Map, Number, Value};
     use crate::comments::Comment;
     use crate::config::{CachingPolicy, ConfigHandlingPolicy, IssueAttribute, IssueLoadingSettings};
     use crate::embedding::Embedding;
+    use crate::errors::APIError;
     use crate::issues::Issue;
     use crate::labels::Label;
     use crate::models::{Model, ModelVersion, TestRun};
     use crate::repository::IssueRepo;
     use crate::tags::{Tag, TagType};
-    use crate::util::APIResult;
+    use crate::errors::APIResult;
     use super::*;
 
     create_exception!(issue_api, IssueAPIError, PyException);
+    create_exception!(issue_api, InvalidCredentialsException, IssueAPIError);
+    create_exception!(issue_api, NotAuthorizedException, IssueAPIError);
+    create_exception!(issue_api, InvalidTokenException, IssueAPIError);
+    create_exception!(issue_api, HTTPException, IssueAPIError);
+    create_exception!(issue_api, LibraryException, IssueAPIError);
 
     #[inline(always)]
     fn api2py_error<T>(e: APIResult<T>) -> PyResult<T> {
         match e {
-            Ok(e) => Ok(e),
-            Err(e) => Err(
-                IssueAPIError::new_err(e.to_string())
-            )
+            Ok(obj) => Ok(obj),
+            Err(inner) => Err({
+                match inner {
+                    APIError::InvalidCredentials => InvalidCredentialsException::new_err(inner.to_string()),
+                    APIError::InvalidToken => InvalidTokenException::new_err(inner.to_string()),
+                    APIError::NotAuthorized => NotAuthorizedException::new_err(inner.to_string()),
+                    APIError::HTTPError{message, status_code} => {
+                        let o = (message, status_code);
+                        HTTPException::new_err(o)
+                    },
+                    APIError::IDParsingError(_) => IssueAPIError::new_err(inner.to_string()),
+                    APIError::LibraryError(_) => LibraryException::new_err(inner.to_string()),
+                    APIError::GenericError(_) => IssueAPIError::new_err(inner.to_string())
+                }
+            })
         }
     }
 
     fn json_to_py(py: Python<'_>, j: Value) -> PyObject {
         match j {
             Value::Null => Option::<bool>::None.into_py(py),
             Value::Bool(b) => b.into_py(py),
@@ -1107,14 +1124,19 @@
             api2py_error(self.inner.update_description(description))
         }
     }
 
     #[pymodule]
     fn issue_api(py: Python<'_>, m: &PyModule) -> PyResult<()> {
         m.add("IssueAPIError", py.get_type::<IssueAPIError>())?;
+        m.add("InvalidCredentialsException", py.get_type::<InvalidCredentialsException>())?;
+        m.add("NotAuthorizedException", py.get_type::<NotAuthorizedException>())?;
+        m.add("InvalidTokenException", py.get_type::<InvalidTokenException>())?;
+        m.add("HTTPException", py.get_type::<HTTPException>())?;
+        m.add("LibraryException", py.get_type::<LibraryException>())?;
         m.add_class::<PyIssueRepository>()?;
         m.add_class::<PyIssue>()?;
         m.add_class::<PyQuery>()?;
         m.add_class::<PyLabel>()?;
         m.add_class::<PyRepo>()?;
         m.add_class::<PyTag>()?;
         m.add_class::<PyModel>()?;
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/models.rs` & `issue_db_api-0.7.0/issue_db_api/src/models.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::collections::HashMap;
 use std::hash::{Hash, Hasher};
 use std::sync::Arc;
 use serde_json::Value;
 use crate::api_core::IssueAPI;
-use crate::APIResult;
+use crate::errors::APIResult;
 use crate::config::ConfigHandlingPolicy;
 use crate::errors::APIError;
 use crate::util::CacheContainer;
 
 //////////////////////////////////////////////////////////////////////////////////////////////////
 //////////////////////////////////////////////////////////////////////////////////////////////////
 // Raw Models -- Used for Raw API responses
@@ -211,15 +211,15 @@
     pub fn get_version_by_id(&self, id: String) -> APIResult<ModelVersion> {
         let versions = self.model_versions()?;
         let version = versions.into_iter()
             .find(|v| v.version == id);
         match version {
             None => {
                 let text = format!("Could not find version with ID {id}");
-                Err(Box::new(APIError::new(text)))
+                Err(APIError::GenericError(text))
             },
             Some(v) => Ok(v)
         }
     }
 
     pub fn model_runs(&self) -> APIResult<Vec<TestRun>> {
         let runs = self.api.get_performances_for_model(self.id.clone())?;
@@ -256,15 +256,15 @@
     pub fn get_run_by_id(&self, id: String) -> APIResult<TestRun> {
         let runs = self.model_runs()?;
         let run = runs.into_iter()
             .find(|r| r.run == id);
         match run {
             None => {
                 let text = format!("Could not find test run with ID {id}");
-                Err(Box::new(APIError::new(text)))
+                Err(APIError::GenericError(text))
             },
             Some(v) => Ok(v)
         }
     }
 
     pub fn delete_run(&self, run: TestRun) -> APIResult<()> {
         self.api.delete_performance_data(run.model, run.run)
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/query.rs` & `issue_db_api-0.7.0/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.6/issue_db_api/src/repository.rs` & `issue_db_api-0.7.0/issue_db_api/src/repository.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use crate::api_core::IssueAPI;
 use crate::config::{CachingPolicy, IssueLoadingSettings, ConfigHandlingPolicy};
 use crate::embedding::Embedding;
 use crate::issues::Issue;
 use crate::models::Model;
 use crate::query::Query;
 use crate::tags::Tag;
-use crate::util::APIResult;
+use crate::errors::APIResult;
 
 
 #[allow(unused)]
 #[derive(Debug)]
 pub struct IssueRepository {
     label_caching: CachingPolicy,
     config_handling: ConfigHandlingPolicy,
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.7.0/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.6/issue_db_api/src/tags.rs` & `issue_db_api-0.7.0/issue_db_api/src/tags.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use std::hash::{Hash, Hasher};
 use std::sync::Arc;
 use crate::api_core::IssueAPI;
-use crate::APIResult;
+use crate::errors::APIResult;
 
 #[allow(unused)]
 #[derive(Debug, Clone, Copy, serde::Deserialize)]
 pub enum TagType {
     #[serde(rename="author")] Author,
     #[serde(rename="project")] Project,
     #[serde(rename="manual-tag")] Custom
```

### Comparing `issue_db_api-0.6.6/issue_db_api/src/util.rs` & `issue_db_api-0.7.0/issue_db_api/src/util.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use std::sync::atomic::{AtomicBool, Ordering};
-use std::sync::{RwLock};
-
-pub type APIResult<T> = Result<T, Box<dyn std::error::Error>>;
+use std::sync::RwLock;
+use crate::errors::{APIResult};
 
 
 macro_rules! initialize_lazy_field {
     ($e:expr) => {
         {
             let value: Option<_> = $e;
             let lazy = lazy_init::Lazy::new();
@@ -17,17 +16,18 @@
     }
 }
 
 
 pub(crate) use initialize_lazy_field;
 
 
+
 #[allow(unused)]
 #[derive(Debug)]
-struct CacheLockError {}
+pub struct CacheLockError {}
 
 impl std::fmt::Display for CacheLockError {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f, "Poisoned lock in cache. Cannot recover.")
     }
 }
 
@@ -52,23 +52,23 @@
             dirty: AtomicBool::new(true)
         }
     }
 
     pub fn get<F: FnOnce() -> APIResult<T>>(&self, f: F) -> APIResult<T> {
         let obj = self.value
             .read()
-            .map_err(|_| Box::new(CacheLockError{}))?;
+            .map_err(|_| CacheLockError{})?;
         if obj.is_some() && !self.dirty.load(Ordering::Acquire) {
             Ok(obj.clone().unwrap())
         } else {
             drop(obj);    // unlock
             // First, acquire the write lock
             let mut obj = self.value
                 .write()
-                .map_err(|_| Box::new(CacheLockError{}))?;
+                .map_err(|_| CacheLockError{})?;
             // With the write lock in hand, check if another thread
             // updated the object in the meantime.
             if self.dirty.load(Ordering::Relaxed) && obj.is_none() {
                 let inner = (f)()?;
                 let _ = obj.insert(inner.clone());
                 Ok(inner)
             } else {
@@ -78,15 +78,15 @@
             }
         }
     }
 
     pub fn set(&self, value: T) -> APIResult<()> {
         let mut obj = self.value
             .write()
-            .map_err(|_| Box::new(CacheLockError{}))?;
+            .map_err(|_| CacheLockError{})?;
         let _ = obj.insert(value);
         Ok(())
     }
 
     pub fn invalidate(&self) {
         self.dirty.store(true, Ordering::Release);
     }
```

### Comparing `issue_db_api-0.6.6/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.7.0/issue_db_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.6.6
+Version: 0.7.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.6/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.7.0/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.6/pyproject.toml` & `issue_db_api-0.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.6.6"
+version = "0.7.0"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

