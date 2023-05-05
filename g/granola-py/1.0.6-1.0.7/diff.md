# Comparing `tmp/granola_py-1.0.6.tar.gz` & `tmp/granola_py-1.0.7.tar.gz`

## Comparing `granola_py-1.0.6.tar` & `granola_py-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 granola_py-1.0.6/Cargo.toml
--rw-r--r--   0      501       20     6148 2023-04-07 17:31:37.000000 granola_py-1.0.6/.DS_Store
--rw-r--r--   0      501       20       24 2023-04-07 17:31:37.000000 granola_py-1.0.6/.gitignore
--rw-r--r--   0      501       20  1029970 2023-04-07 17:31:37.000000 granola_py-1.0.6/Granola_Logo.png
--rw-r--r--   0      501       20     1063 2023-04-07 17:31:37.000000 granola_py-1.0.6/LICENSE.md
--rw-r--r--   0      501       20     1061 2023-04-07 17:31:37.000000 granola_py-1.0.6/README.md
--rw-r--r--   0      501       20   132240 2023-04-07 17:31:37.000000 granola_py-1.0.6/code_snippet.png
--rw-r--r--   0      501       20      114 2023-04-07 17:31:37.000000 granola_py-1.0.6/examples/hello_world.py
--rw-r--r--   0      501       20      235 2023-04-07 17:31:37.000000 granola_py-1.0.6/main.py
--rw-r--r--   0      501       20      320 2023-04-07 17:31:37.000000 granola_py-1.0.6/pyproject.toml
--rw-r--r--   0      501       20     2122 2023-04-09 00:35:32.000000 granola_py-1.0.6/src/http.rs
--rw-r--r--   0      501       20     4917 2023-04-11 16:50:59.000000 granola_py-1.0.6/src/lib.rs
--rw-r--r--   0      501       20      942 2023-04-07 17:31:37.000000 granola_py-1.0.6/src/net/mod.rs
--rw-r--r--   0      501       20       26 2023-04-07 17:31:37.000000 granola_py-1.0.6/tests/__main__.py
--rw-r--r--   0      501       20      885 2023-04-07 17:31:37.000000 granola_py-1.0.6/user-guide.md
--rw-r--r--   0      501       20     8755 2023-04-11 16:51:37.000000 granola_py-1.0.6/Cargo.lock
--rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 granola_py-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 granola_py-1.0.7/Cargo.toml
+-rw-r--r--   0      501       20     6148 2023-05-05 02:16:39.000000 granola_py-1.0.7/.DS_Store
+-rw-r--r--   0      501       20       24 2023-04-07 17:31:37.000000 granola_py-1.0.7/.gitignore
+-rw-r--r--   0      501       20  1029970 2023-04-07 17:31:37.000000 granola_py-1.0.7/Granola_Logo.png
+-rw-r--r--   0      501       20     1063 2023-04-07 17:31:37.000000 granola_py-1.0.7/LICENSE.md
+-rw-r--r--   0      501       20     1061 2023-04-07 17:31:37.000000 granola_py-1.0.7/README.md
+-rw-r--r--   0      501       20   132240 2023-04-07 17:31:37.000000 granola_py-1.0.7/code_snippet.png
+-rw-r--r--   0      501       20      114 2023-04-07 17:31:37.000000 granola_py-1.0.7/examples/hello_world.py
+-rw-r--r--   0      501       20      235 2023-04-07 17:31:37.000000 granola_py-1.0.7/main.py
+-rw-r--r--   0      501       20      320 2023-04-07 17:31:37.000000 granola_py-1.0.7/pyproject.toml
+-rw-r--r--   0      501       20     2118 2023-05-05 04:10:42.000000 granola_py-1.0.7/src/http.rs
+-rw-r--r--   0      501       20     5179 2023-05-05 04:11:12.000000 granola_py-1.0.7/src/lib.rs
+-rw-r--r--   0      501       20      942 2023-04-07 17:31:37.000000 granola_py-1.0.7/src/net/mod.rs
+-rw-r--r--   0      501       20      108 2023-05-05 01:29:55.000000 granola_py-1.0.7/tests/__main__.py
+-rw-r--r--   0      501       20     1262 2023-05-05 00:54:07.000000 granola_py-1.0.7/tests/class_gen.py
+-rw-r--r--   0      501       20      885 2023-04-07 17:31:37.000000 granola_py-1.0.7/user-guide.md
+-rw-r--r--   0      501       20     8755 2023-05-05 04:12:12.000000 granola_py-1.0.7/Cargo.lock
+-rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 granola_py-1.0.7/PKG-INFO
```

### Comparing `granola_py-1.0.6/Granola_Logo.png` & `granola_py-1.0.7/Granola_Logo.png`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.6/LICENSE.md` & `granola_py-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.6/README.md` & `granola_py-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.6/code_snippet.png` & `granola_py-1.0.7/code_snippet.png`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.6/src/http.rs` & `granola_py-1.0.7/src/http.rs`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     net::TcpStream,
 };
 
 #[derive(Debug, Clone)]
 pub struct Request {
     pub method: String,
     pub host: String,
-        pub route: String,
+    pub route: String,
     pub version: f32,
 }
 
 impl Request {
     pub fn new(mut stream: &TcpStream) -> Self {
         let buf_reader = BufReader::new(&mut stream);
         let http_request_data: Vec<_> = buf_reader
```

### Comparing `granola_py-1.0.6/src/lib.rs` & `granola_py-1.0.7/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 }
 
 enum RouteResult<T> {
     SubRoute(T),
     Failed
 }
 
+fn error(e: PyErr) -> String {
+    let err: Error = e.into();
+    println!("{:?}", err);
+    panic!();
+}
+
 fn extract_path_from_url(url: &str) -> &str {
     match url.find('?') {
         Some(index) => &url[..index],
         None => url,
     }
 }
 
@@ -97,19 +103,25 @@
     let mut response: RouteResult<&PyAny> = RouteResult::SubRoute(app);
     println!("{}", request.to_string());
     for call in request.clone().route.split('/').skip_while(|route| route.is_empty()).take_while(|route| !route.is_empty() ) {
         (response, request) = process_request(extract_path_from_url(call).to_string(), request, response);
     };
 
     let result = if let RouteResult::SubRoute(resp) = response {
-        if resp.hasattr("__granola__").unwrap() {
-            resp.call_method0("__granola__").unwrap().str().unwrap().to_string()
-        } else {
-            resp.str().unwrap().to_string()
-        }
+        match resp.hasattr("__granola__") {
+            Ok(true) => {
+                match resp.call_method0("__granola__") {
+                    Ok(e) => e.str().unwrap().to_string(),
+                    Err(e) => error(e)
+                }
+            }
+            Ok(false) => resp.str().unwrap().to_string(),
+            Err(e) => error(e)
+
+        } 
     } else {
         "INTERNAL SERVER ERROR".to_string()
     };
 
     let content_type = match is_valid_json(&response) {
         true => "application/json".to_string(),
         false => "text/html".to_string()
```

### Comparing `granola_py-1.0.6/src/net/mod.rs` & `granola_py-1.0.7/src/net/mod.rs`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.6/user-guide.md` & `granola_py-1.0.7/user-guide.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.6/Cargo.lock` & `granola_py-1.0.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 dependencies = [
  "nix",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "granola"
-version = "1.0.6"
+version = "1.0.7"
 dependencies = [
  "ctrlc",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
```

### Comparing `granola_py-1.0.6/PKG-INFO` & `granola_py-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granola-py
-Version: 1.0.6
+Version: 1.0.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

