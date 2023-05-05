# Comparing `tmp/sui_brownie-1.0.1-py3-none-any.whl.zip` & `tmp/sui_brownie-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27695 bytes, number of entries: 16
+Zip file size: 27837 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-21 09:58 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    92661 b- defN 23-May-05 08:03 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    94069 b- defN 23-May-05 10:22 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-05 08:05 sui_brownie-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 08:05 sui_brownie-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-05 08:05 sui_brownie-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1296 b- defN 23-May-05 08:05 sui_brownie-1.0.1.dist-info/RECORD
-16 files, 158464 bytes uncompressed, 25561 bytes compressed:  83.9%
+-rw-r--r--  2.0 unx     1002 b- defN 23-May-05 10:31 sui_brownie-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 10:31 sui_brownie-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-05 10:31 sui_brownie-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1297 b- defN 23-May-05 10:31 sui_brownie-1.0.2.dist-info/RECORD
+16 files, 159893 bytes uncompressed, 25703 bytes compressed:  83.9%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-1.0.1.dist-info/METADATA
+Filename: sui_brownie-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-1.0.1.dist-info/WHEEL
+Filename: sui_brownie-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-1.0.1.dist-info/top_level.txt
+Filename: sui_brownie-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-1.0.1.dist-info/RECORD
+Filename: sui_brownie-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -1192,19 +1192,19 @@
                 abi = result[module_name]["exposedFunctions"][func_name]
                 abi["module_name"] = module_name
                 abi["func_name"] = func_name
                 self.modules[module_name][func_name] = ModuleFunction(self, abi)
 
     # ####### Publish
 
-    def replace_toml(self, move_toml: MoveToml, replace_address: dict = None):
+    def replace_toml(self, move_toml: MoveToml, replace_address: dict = None, replace_publish_at: dict = None):
         package_name = move_toml["package"]["name"]
-        if package_name in replace_address:
-            if replace_address[package_name] is not None:
-                move_toml["package"]["published-at"] = replace_address[package_name]
+        if package_name in replace_publish_at:
+            if replace_publish_at[package_name] is not None:
+                move_toml["package"]["published-at"] = replace_publish_at[package_name]
             elif self.project.search_package(package_name) is not None:
                 move_toml["package"]["published-at"] = self.project.search_package(package_name)
             else:
                 assert False, "Replace address not found for published-at"
         for k in list(move_toml.get("addresses", dict()).keys()):
             if k in replace_address:
                 if replace_address[k] is not None:
@@ -1214,43 +1214,50 @@
                 else:
                     assert False, "Replace address is None for addresses"
         return move_toml
 
     def replace_addresses(
             self,
             replace_address: dict = None,
+            replace_publish_at: dict = None,
             output: dict = None
     ) -> dict:
         if replace_address is None:
+            replace_address = {}
+        if replace_publish_at is None:
+            replace_publish_at = {}
+        if len(replace_address) == 0 and len(replace_publish_at) == 0:
             return output
         if output is None:
             output = dict()
         current_move_toml = MoveToml(str(self.move_toml_file))
         package_name = current_move_toml.package_name()
         package_address_name = current_move_toml.package_address_name()
-        if package_address_name in replace_address and package_name not in replace_address:
-            replace_address[package_name] = replace_address[package_address_name]
+        if package_address_name in replace_publish_at and package_name not in replace_publish_at:
+            replace_publish_at[package_name] = replace_publish_at[package_address_name]
+        if package_address_name in replace_address and package_name not in replace_publish_at:
+            replace_publish_at[package_name] = replace_address[package_address_name]
         if current_move_toml["package"]["name"] in output:
             return output
         output[current_move_toml["package"]["name"]] = current_move_toml
 
         # process current move toml
-        self.replace_toml(current_move_toml, replace_address)
+        self.replace_toml(current_move_toml, replace_address, replace_publish_at)
 
         # process dependencies move toml
         for k in list(current_move_toml.keys()):
             if "dependencies" == k:
                 for d in list(current_move_toml[k].keys()):
                     # process local
                     if "local" in current_move_toml[k][d]:
                         local_path = self.package_path \
                             .joinpath(current_move_toml[k][d]["local"])
                         assert local_path.exists(), f"{local_path.absolute()} not found"
                         dep_move_toml = SuiPackage(package_path=local_path)
-                        dep_move_toml.replace_addresses(replace_address, output)
+                        dep_move_toml.replace_addresses(replace_address, replace_publish_at, output)
                     # process remote
                     else:
                         git_index = current_move_toml[k][d]["git"].rfind("/")
                         git_path = current_move_toml[k][d]["git"][:git_index + 1]
                         git_file = current_move_toml[k][d]["git"][git_index + 1:]
                         if "subdir" not in current_move_toml[k][d]:
                             git_file = f"{d}.git"
@@ -1261,15 +1268,15 @@
                             .replace("://", "___") \
                             .replace("/", "_").replace(".", "_")
                         remote_path = Path(f"{os.environ.get('HOME')}/.move") \
                             .joinpath(git_file) \
                             .joinpath(sub_dir)
                         assert remote_path.exists(), f"{remote_path.absolute()} not found"
                         dep_move_toml = SuiPackage(package_path=remote_path)
-                        dep_move_toml.replace_addresses(replace_address, output)
+                        dep_move_toml.replace_addresses(replace_address, replace_publish_at, output)
 
         for k in output:
             output[k].store()
         return output
 
     def format_dict(self, data):
         for k in list(data.keys()):
@@ -1298,19 +1305,22 @@
         return data
 
     @retry(stop_max_attempt_number=3, wait_random_min=500, wait_random_max=1000)
     def publish_package(
             self,
             gas_budget=None,
             replace_address: dict = None,
+            replace_publish_at: dict = None,
             skip_dependency_verification=True
     ):
         if gas_budget is None:
             gas_budget = self.project.gas_budget
-        replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
+        replace_tomls = self.replace_addresses(replace_address=replace_address,
+                                               replace_publish_at=replace_publish_at,
+                                               output=dict())
         view = f"Publish {self.package_name}"
         print("\n" + "-" * 50 + view + "-" * 50)
         try:
             with self.project.cli_config as cof:
                 skip_flag = " --skip-dependency-verification" if skip_dependency_verification else ""
                 cmd = f"sui client --client.config {cof.file.absolute()} publish " \
                       f"{skip_flag} --gas-budget {gas_budget} " \
@@ -1342,22 +1352,25 @@
             traceback.print_exc()
             raise
         return result
 
     def program_publish_package(
             self,
             replace_address: dict = None,
+            replace_publish_at: dict = None,
             gas_price=None,
             gas_budget=None,
     ):
         if gas_budget is None:
             gas_budget = self.project.gas_budget
         if gas_price is None:
             gas_price = self.project.estimate_gas_price()
-        replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
+        replace_tomls = self.replace_addresses(replace_address=replace_address,
+                                               replace_publish_at=replace_publish_at,
+                                               output=dict())
         try:
             cmd = f"sui move build --dump-bytecode-as-base64 --path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
                 result = json.loads(result[result.find("{"):])
             except:
@@ -1391,23 +1404,26 @@
         return result
 
     def program_upgrade_package(
             self,
             upgrade_capability: str,
             upgrade_policy: int,
             replace_address: dict = None,
+            replace_publish_at: dict = None,
             digest=None,
             gas_price=1000,
             gas_budget=100000000,
     ):
         if gas_budget is None:
             gas_budget = self.project.gas_budget
         if gas_price is None:
             gas_price = self.project.estimate_gas_price()
-        replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
+        replace_tomls = self.replace_addresses(replace_address=replace_address,
+                                               replace_publish_at=replace_publish_at,
+                                               output=dict())
         try:
             cmd = f"sui move build --dump-bytecode-as-base64 --legacy-digest " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
                 first_part_start = result.find("{")
@@ -1454,16 +1470,19 @@
             traceback.print_exc()
             raise
         return result
 
     def generate_digest(
             self,
             replace_address: dict = None,
+            replace_publish_at: dict = None,
     ):
-        replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
+        replace_tomls = self.replace_addresses(replace_address=replace_address,
+                                               replace_publish_at=replace_publish_at,
+                                               output=dict())
         try:
             cmd = f"sui move build --legacy-digest " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             return result
         except:
@@ -1475,22 +1494,25 @@
     def program_dola_upgrade_package(
             self,
             proposal_package_id,
             governance_info: str,
             governance_contracts: str,
             proposal: str,
             replace_address: dict = None,
+            replace_publish_at: dict = None,
             gas_price=None,
             gas_budget=None,
     ):
         if gas_budget is None:
             gas_budget = self.project.gas_budget
         if gas_price is None:
             gas_price = self.project.estimate_gas_price()
-        replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
+        replace_tomls = self.replace_addresses(replace_address=replace_address,
+                                               replace_publish_at=replace_publish_at,
+                                               output=dict())
         try:
             cmd = f"sui move build --dump-bytecode-as-base64 --legacy-digest " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
                 first_part_start = result.find("{")
```

## Comparing `sui_brownie-1.0.1.dist-info/METADATA` & `sui_brownie-1.0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -23,7 +24,9 @@
 Requires-Dist: retrying
 Requires-Dist: mnemonic
 Requires-Dist: httpx
 Requires-Dist: python-dotenv
 Requires-Dist: pynacl
 
 This is an sui python tool to quickly implement sui calls
+
+
```

## Comparing `sui_brownie-1.0.1.dist-info/RECORD` & `sui_brownie-1.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=deRHszURKmZ7_kwMayHyRrINQ32RdcEylrowna-WzZM,92661
+sui_brownie/sui_brownie.py,sha256=BJFfSWeL5OW6pZFtObTP0jFR8sbGplab_rKhF5m8BvU,94069
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-1.0.1.dist-info/METADATA,sha256=CXS4GAqyAYdyT_LzEX-Ap4X1zX2gTIPJjkKuTyrZ0Y0,982
-sui_brownie-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-1.0.1.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-1.0.1.dist-info/RECORD,,
+sui_brownie-1.0.2.dist-info/METADATA,sha256=2B0fhuJYYuhyNdY4b9MiK6FDD_H_8N5PIExarSbpDgU,1002
+sui_brownie-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-1.0.2.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-1.0.2.dist-info/RECORD,,
```

