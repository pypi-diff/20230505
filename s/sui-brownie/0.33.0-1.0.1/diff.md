# Comparing `tmp/sui_brownie-0.33.0-py3-none-any.whl.zip` & `tmp/sui_brownie-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27684 bytes, number of entries: 16
+Zip file size: 27695 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-21 09:58 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    92540 b- defN 23-Apr-27 03:16 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    92661 b- defN 23-May-05 08:03 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx      983 b- defN 23-Apr-27 03:18 sui_brownie-0.33.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 03:18 sui_brownie-0.33.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-27 03:18 sui_brownie-0.33.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-27 03:18 sui_brownie-0.33.0.dist-info/RECORD
-16 files, 158348 bytes uncompressed, 25542 bytes compressed:  83.9%
+-rw-r--r--  2.0 unx      982 b- defN 23-May-05 08:05 sui_brownie-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 08:05 sui_brownie-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-05 08:05 sui_brownie-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1296 b- defN 23-May-05 08:05 sui_brownie-1.0.1.dist-info/RECORD
+16 files, 158464 bytes uncompressed, 25561 bytes compressed:  83.9%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-0.33.0.dist-info/METADATA
+Filename: sui_brownie-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-0.33.0.dist-info/WHEEL
+Filename: sui_brownie-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-0.33.0.dist-info/top_level.txt
+Filename: sui_brownie-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-0.33.0.dist-info/RECORD
+Filename: sui_brownie-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -1391,37 +1391,39 @@
         return result
 
     def program_upgrade_package(
             self,
             upgrade_capability: str,
             upgrade_policy: int,
             replace_address: dict = None,
-            gas_price=None,
-            gas_budget=None,
-            hex_digest=None
+            digest=None,
+            gas_price=1000,
+            gas_budget=100000000,
     ):
         if gas_budget is None:
             gas_budget = self.project.gas_budget
         if gas_price is None:
             gas_price = self.project.estimate_gas_price()
         replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
         try:
-            cmd = f"sui move build --dump-bytecode-as-base64 --dump-package-digest " \
+            cmd = f"sui move build --dump-bytecode-as-base64 --legacy-digest " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
                 first_part_start = result.find("{")
                 first_part_end = result.find("}") + 1
-                if hex_digest is None:
-                    hex_digest = result[first_part_end:]
-                else:
-                    hex_digest = hex_digest.replace("0x", "")
-                digest = list(bytes.fromhex(hex_digest))
                 result = json.loads(result[first_part_start:first_part_end])
+                if digest is None:
+                    digest = result["digest"]
+                    hex_digest = bytes(digest).hex()
+                else:
+                    if isinstance(digest, str):
+                        digest = list(bytes.fromhex(digest.replace("0x", "")))
+                    hex_digest = bytes(digest).hex()
                 print(f"Upgrade digest: {hex_digest}")
             except:
                 print(f"Build error:\n{cmd}\n{result}")
                 raise
             move_modules = []
             for m in result["modules"]:
                 move_modules.append(list(base64.b64decode(m)))
@@ -1455,15 +1457,15 @@
 
     def generate_digest(
             self,
             replace_address: dict = None,
     ):
         replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
         try:
-            cmd = f"sui move build --dump-package-digest " \
+            cmd = f"sui move build --legacy-digest " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             return result
         except:
             traceback.print_exc()
 
@@ -1482,23 +1484,24 @@
     ):
         if gas_budget is None:
             gas_budget = self.project.gas_budget
         if gas_price is None:
             gas_price = self.project.estimate_gas_price()
         replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
         try:
-            cmd = f"sui move build --dump-bytecode-as-base64 --dump-package-digest " \
+            cmd = f"sui move build --dump-bytecode-as-base64 --legacy-digest " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
                 first_part_start = result.find("{")
                 first_part_end = result.find("}") + 1
-                hex_digest = result[first_part_end:]
                 result = json.loads(result[first_part_start:first_part_end])
+                digest = result["digest"]
+                hex_digest = bytes(digest).hex()
                 print(f"Upgrade digest: {hex_digest}")
             except:
                 pprint(f"Build error:\n{result}")
                 raise
             move_modules = []
             for m in result["modules"]:
                 move_modules.append(list(base64.b64decode(m)))
```

## Comparing `sui_brownie-0.33.0.dist-info/METADATA` & `sui_brownie-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 0.33.0
+Version: 1.0.1
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `sui_brownie-0.33.0.dist-info/RECORD` & `sui_brownie-1.0.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=bBhL1lGDnqsEYOywFtnZHxnKx2AdjiDsvSMyEZFgyN0,92540
+sui_brownie/sui_brownie.py,sha256=deRHszURKmZ7_kwMayHyRrINQ32RdcEylrowna-WzZM,92661
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-0.33.0.dist-info/METADATA,sha256=ruFnRIyhW3nXLTUwekQ3JyBVKSOA_dRr9Dqe2oXEfxo,983
-sui_brownie-0.33.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-0.33.0.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-0.33.0.dist-info/RECORD,,
+sui_brownie-1.0.1.dist-info/METADATA,sha256=CXS4GAqyAYdyT_LzEX-Ap4X1zX2gTIPJjkKuTyrZ0Y0,982
+sui_brownie-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-1.0.1.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-1.0.1.dist-info/RECORD,,
```

