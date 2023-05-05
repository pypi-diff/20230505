# Comparing `tmp/gep3-0.0.9.tar.gz` & `tmp/gep3-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/gep3/gep3/dist/tmpy9fdl784/gep3-0.0.9.tar", last modified: Wed May  4 17:53:35 2022, max compression
+gzip compressed data, was "gep3-0.1.tar", last modified: Fri May  5 19:22:28 2023, max compression
```

## Comparing `gep3-0.0.9.tar` & `gep3-0.1.tar`

### file list

```diff
@@ -1,35 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:35.000000 gep3-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-04 17:53:25.000000 gep3-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-05-04 17:53:35.000000 gep3-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-05-04 17:53:25.000000 gep3-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-04 17:53:25.000000 gep3-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-04 17:53:35.000000 gep3-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:35.000000 gep3-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:35.000000 gep3-0.0.9/src/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:25.000000 gep3-0.0.9/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6004 2022-05-04 17:53:25.000000 gep3-0.0.9/src/common/ber.py
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-05-04 17:53:25.000000 gep3-0.0.9/src/common/bitstr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-05-04 17:53:25.000000 gep3-0.0.9/src/common/hstr.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-05-04 17:53:25.000000 gep3-0.0.9/src/common/intlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-05-04 17:53:25.000000 gep3-0.0.9/src/common/str.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:35.000000 gep3-0.0.9/src/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:25.000000 gep3-0.0.9/src/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19698 2022-05-04 17:53:25.000000 gep3-0.0.9/src/crypto/des.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-05-04 17:53:25.000000 gep3-0.0.9/src/crypto/modes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:35.000000 gep3-0.0.9/src/emv/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:25.000000 gep3-0.0.9/src/emv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-05-04 17:53:25.000000 gep3-0.0.9/src/emv/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-05-04 17:53:25.000000 gep3-0.0.9/src/emv/records.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:35.000000 gep3-0.0.9/src/gep3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-05-04 17:53:35.000000 gep3-0.0.9/src/gep3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-05-04 17:53:35.000000 gep3-0.0.9/src/gep3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 17:53:35.000000 gep3-0.0.9/src/gep3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-04 17:53:35.000000 gep3-0.0.9/src/gep3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-04 17:53:35.000000 gep3-0.0.9/src/gep3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:35.000000 gep3-0.0.9/src/pcsc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:25.000000 gep3-0.0.9/src/pcsc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10759 2022-05-04 17:53:25.000000 gep3-0.0.9/src/pcsc/card.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-05-04 17:53:25.000000 gep3-0.0.9/src/pcsc/emv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:35.000000 gep3-0.0.9/src/shell/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 17:53:25.000000 gep3-0.0.9/src/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-05-04 17:53:25.000000 gep3-0.0.9/src/shell/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.485227 gep3-0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-05-05 19:22:18.000000 gep3-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-05-05 19:22:28.489228 gep3-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-05 19:22:18.000000 gep3-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-05 19:22:18.000000 gep3-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-05 19:22:28.489228 gep3-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.481227 gep3-0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.481227 gep3-0.1/src/ccid/
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-05 19:22:18.000000 gep3-0.1/src/ccid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-05-05 19:22:18.000000 gep3-0.1/src/ccid/bulk_in_messages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4922 2023-05-05 19:22:18.000000 gep3-0.1/src/ccid/bulk_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-05 19:22:18.000000 gep3-0.1/src/ccid/bulk_out_messages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-05-05 19:22:18.000000 gep3-0.1/src/ccid/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8541 2023-05-05 19:22:18.000000 gep3-0.1/src/ccid/pyusb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.481227 gep3-0.1/src/common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:18.000000 gep3-0.1/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-05 19:22:18.000000 gep3-0.1/src/common/ber.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-05-05 19:22:18.000000 gep3-0.1/src/common/bitstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3954 2023-05-05 19:22:18.000000 gep3-0.1/src/common/hstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-05 19:22:18.000000 gep3-0.1/src/common/intlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-05-05 19:22:18.000000 gep3-0.1/src/common/str.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.481227 gep3-0.1/src/crypto/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:18.000000 gep3-0.1/src/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21863 2023-05-05 19:22:18.000000 gep3-0.1/src/crypto/des.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-05 19:22:18.000000 gep3-0.1/src/crypto/modes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.485227 gep3-0.1/src/emv/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-05 19:22:18.000000 gep3-0.1/src/emv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-05-05 19:22:18.000000 gep3-0.1/src/emv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12423 2023-05-05 19:22:18.000000 gep3-0.1/src/emv/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-05-05 19:22:18.000000 gep3-0.1/src/emv/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-05 19:22:18.000000 gep3-0.1/src/emv/key_management.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-05-05 19:22:18.000000 gep3-0.1/src/emv/records.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.485227 gep3-0.1/src/gep3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-05-05 19:22:28.000000 gep3-0.1/src/gep3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-05-05 19:22:28.000000 gep3-0.1/src/gep3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 19:22:28.000000 gep3-0.1/src/gep3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-05 19:22:28.000000 gep3-0.1/src/gep3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-05 19:22:28.000000 gep3-0.1/src/gep3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.485227 gep3-0.1/src/globalplatform/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-05 19:22:18.000000 gep3-0.1/src/globalplatform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3054 2023-05-05 19:22:18.000000 gep3-0.1/src/globalplatform/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6125 2023-05-05 19:22:18.000000 gep3-0.1/src/globalplatform/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.485227 gep3-0.1/src/iso7816/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-05-05 19:22:18.000000 gep3-0.1/src/iso7816/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16012 2023-05-05 19:22:18.000000 gep3-0.1/src/iso7816/apdu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-05 19:22:18.000000 gep3-0.1/src/iso7816/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-05-05 19:22:18.000000 gep3-0.1/src/iso7816/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.485227 gep3-0.1/src/multos/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-05 19:22:18.000000 gep3-0.1/src/multos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-05-05 19:22:18.000000 gep3-0.1/src/multos/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-05-05 19:22:18.000000 gep3-0.1/src/multos/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:28.485227 gep3-0.1/src/pcsc/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 19:22:18.000000 gep3-0.1/src/pcsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-05-05 19:22:18.000000 gep3-0.1/src/pcsc/card.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-05 19:22:18.000000 gep3-0.1/src/pcsc/emv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2262 2023-05-05 19:22:18.000000 gep3-0.1/src/pcsc/gp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-05 19:22:18.000000 gep3-0.1/src/pcsc/ml.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15056 2023-05-05 19:22:18.000000 gep3-0.1/src/pcsc/scard.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gep3-0.0.9/LICENSE` & `gep3-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gep3-0.0.9/PKG-INFO` & `gep3-0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.0.9
+Version: 0.1
 Summary: Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 Home-page: https://github.com/spochic/gep3
 Author: Sebastien Pochic
 Author-email: spochic@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/spochic/gep3/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Smart Card
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gep3
 Generic Encryption Peripheral: various utilities related to cryptography and smart cards 
-
-
```

### Comparing `gep3-0.0.9/setup.cfg` & `gep3-0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gep3
-version = 0.0.9
+version = 0.1
 author = Sebastien Pochic
 author_email = spochic@gmail.com
 description = Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spochic/gep3
 project_urls = 
@@ -17,15 +17,15 @@
 	Topic :: Security :: Cryptography
 	Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Smart Card
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.10
 install_requires = pyscard >2
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `gep3-0.0.9/src/common/ber.py` & `gep3-0.1/src/common/ber.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,36 @@
 def parse_to_dict(tlv_hstr: str):
     """
     """
     tlv_object_list, remainder = parse(tlv_hstr, recursive=True)
 
     return _tlv_object_list_to_dict(tlv_object_list)
 
+def parse_dol(tlv_hstr: str):
+    """parse_dol():
+    """
+    remainder = _hstr.clean(tlv_hstr)
+    output = []
+    while remainder != '':
+        # Ignoring 00 bytes before or after TLV objects
+        while remainder[0:2] == '00':
+            remainder = remainder[2:]
+
+        T, remainder = _decode_tag(remainder)
+        if T == '':
+            break
+
+        L, remainder = _decode_length(remainder)
+        if L == '':
+            break
+
+        output.append((T, L))
+
+    return (output, remainder)
+
 def find(tag, tlv_object):
     """find: finds a specific tag in a list of objects
     """
     tag = _hstr.clean(tag)
     if isinstance(tlv_object, tuple):
         return _find_in_tuple(tag, tlv_object)
     elif isinstance(tlv_object, list):
@@ -74,14 +96,24 @@
         if len(l_value) % 2 != 0:
             # Left pad with 0 to have even number of nibbles
             l_value = F"0{l_value}"
         
         l_header = F"{128+len(l_value)//2:02X}"
 
         return F"{l_header}{l_value}"
+
+def encode(tag: str, data: str) -> str:
+    """encode(): encode tag and data into BER-TLV object
+    """
+    tag = _hstr.clean(tag)
+    data = _hstr.clean(data)
+
+    return F"{tag}{encode_length(data)}{data}"
+
+
 #
 # Helper functions (assume a clean 'hstr' as input)
 #
 
 def _find_in_tuple(tag, tlv_object):
     T, _, V = tlv_object
     if T == tag:
```

### Comparing `gep3-0.0.9/src/common/bitstr.py` & `gep3-0.1/src/common/bitstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.0.9/src/common/hstr.py` & `gep3-0.1/src/common/hstr.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Standard library imports
 
 # Third party imports
 
 # Local application imports
 from common.str import clean as _clean
 
+
 def clean(hstr_in: str, command_name='()', hstr_name='') -> str:
     """clean(hstr)
 
     - Capitalizes hexadecimal digits
     - Removes '_' characters
     - Raises exceptions on illegal characters
     """
@@ -30,14 +31,30 @@
 
     for nibble in clean(hstr, command_name, hstr_name):
         bstr += F"{int(nibble, 16):04b}"
 
     return bstr
 
 
+def or_(hstr_a: str, hstr_b: str, command_name='()', hstr_name='') -> str:
+    """or_(hstr_a, hstr_b):
+    """
+    hstr_a = clean(hstr_a, command_name, hstr_name)
+    hstr_b = clean(hstr_b, command_name, hstr_name)
+    length = max(len(hstr_a), len(hstr_b))
+    hstr_a = hstr_a.rjust(length, '0')
+    hstr_b = hstr_b.rjust(length, '0')
+    or_hstr = ''
+
+    for (nibble_a, nibble_b) in zip(hstr_a, hstr_b):
+        or_hstr += F"{int(nibble_a, 16)|int(nibble_b, 16):X}"
+
+    return or_hstr
+
+
 def xor(hstr_a: str, hstr_b: str, command_name='()', hstr_name='') -> str:
     """xor(hstr_a, hstr_b):
     """
     hstr_a = clean(hstr_a, command_name, hstr_name)
     hstr_b = clean(hstr_b, command_name, hstr_name)
     length = max(len(hstr_a), len(hstr_b))
     hstr_a = hstr_a.rjust(length, '0')
@@ -45,14 +62,15 @@
     xor_hstr = ''
 
     for (nibble_a, nibble_b) in zip(hstr_a, hstr_b):
         xor_hstr += F"{int(nibble_a, 16)^int(nibble_b, 16):X}"
 
     return xor_hstr
 
+
 def and_(hstr_a: str, hstr_b: str, command_name='()', hstr_name='') -> str:
     """and_(hstr_a, hstr_b):
     """
     hstr_a = clean(hstr_a, command_name, hstr_name)
     hstr_b = clean(hstr_b, command_name, hstr_name)
     length = max(len(hstr_a), len(hstr_b))
     hstr_a = hstr_a.rjust(length, '0')
@@ -60,15 +78,16 @@
     and_hstr = ''
 
     for (nibble_a, nibble_b) in zip(hstr_a, hstr_b):
         and_hstr += F"{int(nibble_a, 16)&int(nibble_b, 16):X}"
 
     return and_hstr
 
-def not_hstr(hstr_in: str, command_name='()', hstr_name='') -> str:
+
+def not_(hstr_in: str, command_name='()', hstr_name='') -> str:
     """not(hstr):
     """
     hstr_in = clean(hstr_in, command_name, hstr_name)
     hstr_out = ''
 
     for nibble in hstr_in:
         hstr_out += xor(nibble, 'F')
@@ -83,16 +102,15 @@
 
 
 def to_intlist(hstr: str, command_name='()', hstr_name='') -> list[int]:
     """to_intlist():
     """
     hstr = clean(hstr, command_name, hstr_name)
     if (len(hstr) % 2) != 0:
-        raise ValueError(
-            F"{command_name}: uneven length for {hstr_name}: {len(hstr)}")
+        hstr = '0' + hstr
 
     bytelist = []
     for i in range(len(hstr)//2):
         bytelist.append(int(hstr[i*2:(i+1)*2], 16))
 
     return bytelist
 
@@ -104,17 +122,32 @@
     hstr_b = clean(hstr_b)
 
     if int(hstr_a, 16) == min(int(hstr_a, 16), int(hstr_b, 16)):
         return hstr_a
 
     return hstr_b
 
-def split_by_length(hstr:str, length:int) -> list[str]:
+
+def split_by_length(hstr: str, length: int) -> list[str]:
     """split_by(): 
     """
     if len(hstr) % length != 0:
         # Error if the string is not a multiple of the length divider
         return []
-    
+
     nr_splits = len(hstr)//length
 
-    return [hstr[i*length:(i+1)*length] for i in range(nr_splits)]
+    return [hstr[i*length:(i+1)*length] for i in range(nr_splits)]
+
+
+def dscan_decimalize(hstr: str) -> str:
+    """dscan_decimalize(): double scan decimalization
+    """
+    dstr1 = ''
+    dstr2 = ''
+    for h in clean(hstr):
+        if h.isdigit():
+            dstr1 = dstr1 + h
+        else:
+            dstr2 = dstr2 + F"{int(h, 16)-10}"
+
+    return dstr1 + dstr2
```

### Comparing `gep3-0.0.9/src/common/str.py` & `gep3-0.1/src/common/str.py`

 * *Files identical despite different names*

### Comparing `gep3-0.0.9/src/crypto/des.py` & `gep3-0.1/src/crypto/des.py`

 * *Files 12% similar despite different names*

```diff
@@ -236,14 +236,34 @@
 
     # applying the inversed initial permutation
     block_64 = _str.perm(R_32 + L_32, _IPINV)
 
     return _bitstr.to_hstr(block_64)
 
 
+def tdea_2_ede_ecb(key_32h: str, block_16h_n: str) -> str:
+    """tdea_2_ede_ecb: Triple DES encryption algorithm in ECB mnode
+    """
+    # cleaning inputs
+    key_32h = _clean_key(key_32h, 32)
+    block_16h_n = _clean_n_blocks(block_16h_n, 16)
+
+    return modes.ecb_encryption(tdea_2_ede, key_32h, block_16h_n)
+
+
+def tdea_2_ded_ecb(key_32h: str, block_16h_n: str) -> str:
+    """tdea_2_ded_ecb: Triple DES decryption algorithm in ECB mode
+    """
+    # cleaning inputs
+    key_32h = _clean_key(key_32h, 32)
+    block_16h_n = _clean_n_blocks(block_16h_n, 16)
+
+    return modes.ecb_decryption(tdea_2_ded, key_32h, block_16h_n)
+
+
 def tdea_2_ede_cbc(key_32h: str, block_16h_n: str, iv_16h: str) -> str:
     """tdea_2_ede_cbc: Triple DES encryption algorithm in CBC mnode
     """
     # cleaning inputs
     key_32h = _clean_key(key_32h, 32)
     block_16h_n = _clean_n_blocks(block_16h_n, 16)
     iv_16h = _clean_block(iv_16h, 16)
@@ -290,19 +310,68 @@
     if len(key_h) == 32:
         return tdea_2_ded(key_h, block_16h)
 
     if len(key_h) == 48:
         return ''
 
 
-def kcv(key_h: str) -> str:
+def kcv(key_h: str, len = 3) -> str:
     """kcv(): Key Check Value
     """
-    return encrypt(key_h, '00' * 8)[0:6]
+    return encrypt(key_h, '00' * 8)[0:2*len]
 
+def mac_1_e(key_h: str, hstr: str):
+    """mac_1_e(): single DES MAC generation
+    """
+    key_h = _hstr.clean(key_h)
+    hstr = _hstr.clean(hstr)
+    temp = '0' * 16
+    for i in range(len(hstr)//16):
+        block = hstr[i*16:i*16+16]
+        temp = dea_e(key_h, _hstr.xor(temp, block))
+    return temp
+
+def mac_2_ede(key_h: str, hstr: str):
+    """mac_2_ede(): double DES MAC generation
+    """
+    key_h = _hstr.clean(key_h)
+    hstr = _hstr.clean(hstr)
+    key__key_1 = key_h[0:16]
+    key__key_2 = key_h[16:32]
+    
+    mac = mac_1_e(key__key_1, hstr)
+    mac = dea_d(key__key_2, mac)
+    mac = dea_e(key__key_1, mac)
+    
+    return mac
+
+def adjust_parity(key_h: str):
+    """
+    """
+    key_h = _hstr.clean(key_h)
+    if len(key_h) % 16 != 0:
+        return ''
+
+    return ''.join([_adjust_parity_byte(key_h[2*i:2*i+2]) for i in range(len(key_h)//2)])
+
+def combine_keys_xor(combined_kcv: str, components: list) -> str:
+    """combine_keys_xor(): combine two or more key components with kcv checking
+    """
+    combined_key = '00'
+
+    for _value, _kcv in components:
+        if kcv(_value, len(_kcv)//2) != _kcv:
+            return None
+        else:
+            combined_key = _hstr.xor(combined_key,_value)
+
+    if kcv(combined_key, len(combined_kcv)//2) != combined_kcv:
+        return None
+    else:
+        return combined_key
 
 #
 # DEA inner functions
 #
 
 
 def _roundkeys(rootkey_64):
@@ -375,8 +444,13 @@
                 F"Wrong number of blocks: 0x{_math.ceil(len(block_lh_n) / length):X}h")
     else:
         if len(block_lh_n) != length * n:
             raise TypeError(F"Wrong block length: 0x{len(block_lh_n):X}h")
 
     return block_lh_n
 
-
+def _adjust_parity_byte(byte_h: str):
+    byte_b = F"{int(byte_h, 16):08b}"
+    if byte_b.count('1') % 2 == 0:
+        return _hstr.xor(byte_h, '01')
+    else:
+        return byte_h
```

### Comparing `gep3-0.0.9/src/emv/records.py` & `gep3-0.1/src/emv/records.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,23 @@
     """decode_afl(): 
     """
     AFL = _hstr.clean(AFL)
     if len(AFL) % 8 != 0:
         # Error if the AFL is not a multiple of 4 bytes
         return None, "AFL is not a multiple of 4 bytes"
     
-    return list(map(_decode_afl_element, _hstr.split_by_length(AFL, 8)))
+    afl = []
+    for afl_element in _hstr.split_by_length(AFL, 8):
+        r, err = _decode_afl_element(afl_element)
+        if err is not None:
+            return None, err
+        else:
+            afl.append(r)
+    
+    return afl, None
 
 #
 # Helper functions (assume a clean 'hstr' as input)
 #
 
 
 def _decode_afl_element(e:str):
@@ -43,8 +51,8 @@
         return None, "AFL Byte 3 is smaller than Byte 2"
     
     oda_records = int(byte4, 16)
     if oda_records > (last_record - first_record + 1):
         # Error if the number of records used for ODA is greater than the total number of records
         return None, "AFL Byte 4 is greater than total number of records"
     
-    return (SFI, first_record, last_record, oda_records)
+    return (SFI, first_record, last_record, oda_records), None
```

### Comparing `gep3-0.0.9/src/gep3.egg-info/PKG-INFO` & `gep3-0.1/src/gep3.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.0.9
+Version: 0.1
 Summary: Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 Home-page: https://github.com/spochic/gep3
 Author: Sebastien Pochic
 Author-email: spochic@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/spochic/gep3/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Smart Card
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gep3
 Generic Encryption Peripheral: various utilities related to cryptography and smart cards 
-
-
```

### Comparing `gep3-0.0.9/src/pcsc/emv.py` & `gep3-0.1/src/pcsc/emv.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 
 def READ_RECORD(card_service: card._CardService, sfi: int, record:int, trace=None):
     return card.send_apdu(card_service, command.READ_RECORD(sfi, record), trace=trace)
 
 def READ_RECORDs(card_service: card._CardService, AFL: str, trace=None):
     output = []
 
-    for (sfi, first, last, _) in records.decode_afl(AFL):
-        for n in range(first, last+1):
-            r, err = READ_RECORD(card_service, sfi, n, trace=trace)
-            output.append((r, err))
-            if err != '':
-                return output
-    
-    return output
-
+    r, err = records.decode_afl(AFL)
+    if err is not None:
+        return []
+    else:
+        for (sfi, first, last, _) in r:
+            for n in range(first, last+1):
+                r, err = READ_RECORD(card_service, sfi, n, trace=trace)
+                output.append((r, err))
+                if err != '':
+                    return output
+        return output
 
 def GET_DATA(card_service: card._CardService, tag: str, trace=None):
     return card.send_apdu(card_service, command.GET_DATA(tag), trace=trace)
```

