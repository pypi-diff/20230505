# Comparing `tmp/nats_nsc-0.1.0.tar.gz` & `tmp/nats_nsc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats_nsc-0.1.0.tar", last modified: Fri May  5 06:55:50 2023, max compression
+gzip compressed data, was "nats_nsc-0.1.1.tar", last modified: Fri May  5 09:15:43 2023, max compression
```

## Comparing `nats_nsc-0.1.0.tar` & `nats_nsc-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-05 06:55:32.622314 nats_nsc-0.1.0/LICENSE
--rw-r--r--   0        0        0      191 2023-05-05 06:55:32.622314 nats_nsc-0.1.0/README.md
--rw-r--r--   0        0        0      516 2023-05-05 06:55:50.426609 nats_nsc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3444 2023-05-05 06:55:32.622314 nats_nsc-0.1.0/src/nats_nsc/__init__.py
--rw-r--r--   0        0        0     4460 2023-05-05 06:55:32.622314 nats_nsc-0.1.0/src/nats_nsc/nsc_utils.py
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 nats_nsc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 09:15:21.904690 nats_nsc-0.1.1/LICENSE
+-rw-r--r--   0        0        0      191 2023-05-05 09:15:21.904690 nats_nsc-0.1.1/README.md
+-rw-r--r--   0        0        0      516 2023-05-05 09:15:43.725042 nats_nsc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3460 2023-05-05 09:15:21.904690 nats_nsc-0.1.1/src/nats_nsc/__init__.py
+-rw-r--r--   0        0        0     4460 2023-05-05 09:15:21.904690 nats_nsc-0.1.1/src/nats_nsc/nsc_utils.py
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 nats_nsc-0.1.1/PKG-INFO
```

### Comparing `nats_nsc-0.1.0/LICENSE` & `nats_nsc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.1.0/pyproject.toml` & `nats_nsc-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 package-dir = "src"
 
 [tool.ruff]
 line-length = 120
 
 [project]
 name = "nats-nsc"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python wrapper for nsc, nats credential manager"
 authors = [
     { name = "Mikołaj Nowak", email = "12396461+m3nowak@users.noreply.github.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
```

### Comparing `nats_nsc-0.1.0/src/nats_nsc/__init__.py` & `nats_nsc-0.1.1/src/nats_nsc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,30 +67,30 @@
         try:
             return json.loads(base64.b64decode(jwt.split('.')[1]))
         except Exception:
             raise ValueError("Invalid JWT")
     
     def add_operator(self, jwt: str) -> Operator:
         payload = self._decode_jwt_payload(jwt)
-        if payload['type'] != 'operator':
+        if payload['nats']['type'] != 'operator':
             raise ValueError("Invalid JWT type")
         nsc_utils.load_operator(self._nsc_path, self.work_dir, jwt)
         op_name = payload['name']
         operator = Operator(
             name=op_name,
             jwt_path=os.path.join(self.work_dir, f"{op_name}/{op_name}.jwt"),
             pub_key=payload['sub'],
             jwt_payload=payload
         )
         self.operators[op_name] = operator
         return operator
 
     def add_account(self, jwt: str, priv_key: str) -> Account:
         payload = self._decode_jwt_payload(jwt)
-        if payload['type'] != 'account':
+        if payload['nats']['type'] != 'account':
             raise ValueError("Invalid JWT type")
         if priv_key is not None:
             nsc_utils.load_key(self._nsc_path, self.work_dir, priv_key)
         acc_name = payload['name']
         nsc_utils.load_account(self.work_dir, jwt, acc_name)
         account = Account(
             name=acc_name,
```

### Comparing `nats_nsc-0.1.0/src/nats_nsc/nsc_utils.py` & `nats_nsc-0.1.1/src/nats_nsc/nsc_utils.py`

 * *Files identical despite different names*

