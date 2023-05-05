# Comparing `tmp/sybil-scorer-0.1.0.tar.gz` & `tmp/sybil-scorer-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-scorer-0.1.0.tar", last modified: Fri May  5 21:16:49 2023, max compression
+gzip compressed data, was "sybil-scorer-0.1.0rc1.tar", last modified: Fri May  5 19:45:13 2023, max compression
```

## Comparing `sybil-scorer-0.1.0.tar` & `sybil-scorer-0.1.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 21:16:49.866988 sybil-scorer-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     9689 2023-05-05 21:16:49.866988 sybil-scorer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.1.0/README.md
--rw-rw-rw-   0        0        0     1121 2023-05-05 20:56:17.000000 sybil-scorer-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-05 21:16:49.821758 sybil-scorer-0.1.0/sbscorer/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:16:49.833716 sybil-scorer-0.1.0/sbscorer/sbdata/
--rw-rw-rw-   0        0        0    23148 2023-05-05 20:56:17.000000 sybil-scorer-0.1.0/sbscorer/sbdata/FlipsideApi.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.0/sbscorer/sbdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:16:49.836714 sybil-scorer-0.1.0/sbscorer/sblegos/
--rw-rw-rw-   0        0        0    30403 2023-02-16 10:48:13.000000 sybil-scorer-0.1.0/sbscorer/sblegos/TransactionAnalyser.py
--rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.1.0/sbscorer/sblegos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:16:49.839714 sybil-scorer-0.1.0/sbscorer/sbutils/
--rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.1.0/sbscorer/sbutils/LoadData.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.0/sbscorer/sbutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:16:49.866042 sybil-scorer-0.1.0/sbscorer/sybil_scorer.egg-info/
--rw-rw-rw-   0        0        0     9689 2023-05-05 21:16:49.000000 sybil-scorer-0.1.0/sbscorer/sybil_scorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-05-05 21:16:49.000000 sybil-scorer-0.1.0/sbscorer/sybil_scorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 21:16:49.000000 sybil-scorer-0.1.0/sbscorer/sybil_scorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-05-05 21:16:49.000000 sybil-scorer-0.1.0/sbscorer/sybil_scorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-05 21:16:49.000000 sybil-scorer-0.1.0/sbscorer/sybil_scorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      748 2023-05-05 21:16:49.873988 sybil-scorer-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.888712 sybil-scorer-0.1.0rc1/
+-rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.1.0rc1/LICENSE
+-rw-rw-rw-   0        0        0     9692 2023-05-05 19:45:13.889712 sybil-scorer-0.1.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.1.0rc1/README.md
+-rw-rw-rw-   0        0        0     1125 2023-05-05 19:43:51.000000 sybil-scorer-0.1.0rc1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.811535 sybil-scorer-0.1.0rc1/sbscorer/
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.831405 sybil-scorer-0.1.0rc1/sbscorer/sbdata/
+-rw-rw-rw-   0        0        0    23088 2023-05-05 19:25:03.000000 sybil-scorer-0.1.0rc1/sbscorer/sbdata/FlipsideApi.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.0rc1/sbscorer/sbdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.836444 sybil-scorer-0.1.0rc1/sbscorer/sblegos/
+-rw-rw-rw-   0        0        0    30403 2023-02-16 10:48:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sblegos/TransactionAnalyser.py
+-rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.1.0rc1/sbscorer/sblegos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.840757 sybil-scorer-0.1.0rc1/sbscorer/sbutils/
+-rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.1.0rc1/sbscorer/sbutils/LoadData.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.0rc1/sbscorer/sbutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:45:13.887354 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/
+-rw-rw-rw-   0        0        0     9692 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-05 19:45:13.000000 sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      752 2023-05-05 19:45:13.891710 sybil-scorer-0.1.0rc1/setup.cfg
```

### Comparing `sybil-scorer-0.1.0/LICENSE` & `sybil-scorer-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.0/PKG-INFO` & `sybil-scorer-0.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
```

### Comparing `sybil-scorer-0.1.0/README.md` & `sybil-scorer-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.0/pyproject.toml` & `sybil-scorer-0.1.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0.0', "wheel"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "sybil-scorer"
-version = "0.1.0"
+version = "0.1.0-rc1"
 description = "A sybil scoring tool"
 readme = "README.md"
 authors = [{ name = "Poupou", email = "poupou-web3@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sybil-scorer-0.1.0/sbscorer/sbdata/FlipsideApi.py` & `sybil-scorer-0.1.0rc1/sbscorer/sbdata/FlipsideApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,14 @@
         network : str
             Network of the transactions
 
         Returns
         -------
 
         """
-        np_address = np.char.lower(np_address.astype(str))
         for address in np_address:
             df_address_transactions = df[np.logical_or(
                 df.from_address == address, df.to_address == address)]
             path_to_export = os.path.join(extract_dir, network)
             csv_file = os.path.join(path_to_export, f"{address}_tx.csv")
             if df_address_transactions.shape[0] > 0:
                 save_csv(df_address_transactions, path_to_export, csv_file)
```

### Comparing `sybil-scorer-0.1.0/sbscorer/sblegos/TransactionAnalyser.py` & `sybil-scorer-0.1.0rc1/sbscorer/sblegos/TransactionAnalyser.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.0/sbscorer/sbutils/LoadData.py` & `sybil-scorer-0.1.0rc1/sbscorer/sbutils/LoadData.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.0/sbscorer/sybil_scorer.egg-info/PKG-INFO` & `sybil-scorer-0.1.0rc1/sbscorer/sybil_scorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
```

### Comparing `sybil-scorer-0.1.0/setup.cfg` & `sybil-scorer-0.1.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7962 696c 2d73 636f 7265 720d   = sybil-scorer.
 00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e30  .version = 0.1.0
-00000030: 0d0a 6175 7468 6f72 203d 2050 6f75 706f  ..author = Poupo
-00000040: 750d 0a61 7574 686f 725f 656d 6169 6c20  u..author_email 
-00000050: 3d20 706f 7570 6f75 2d77 6562 3340 7072  = poupou-web3@pr
-00000060: 6f74 6f6e 6d61 696c 2e63 6f6d 0d0a 6465  otonmail.com..de
-00000070: 7363 7269 7074 696f 6e20 3d20 4120 7379  scription = A sy
-00000080: 6269 6c20 7363 6f72 696e 6720 746f 6f6c  bil scoring tool
-00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000a0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000b0: 452e 6d64 2c20 4c49 4345 4e53 452e 7478  E.md, LICENSE.tx
-000000c0: 740d 0a6c 6f6e 675f 6465 7363 7269 7074  t..long_descript
-000000d0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000e0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000f0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000100: 6769 7468 7562 2e63 6f6d 2f70 6f75 706f  github.com/poupo
-00000110: 752d 7765 6233 2f63 6c75 7374 6572 2d73  u-web3/cluster-s
-00000120: 636f 7265 720d 0a70 726f 6a65 6374 5f75  corer..project_u
-00000130: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000140: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000150: 6974 6875 622e 636f 6d2f 706f 7570 6f75  ithub.com/poupou
-00000160: 2d77 6562 332f 7379 6269 6c2d 7363 6f72  -web3/sybil-scor
-00000170: 6572 2f69 7373 7565 730d 0a09 7265 706f  er/issues...repo
-00000180: 7369 746f 7279 203d 2068 7474 7073 3a2f  sitory = https:/
-00000190: 2f67 6974 6875 622e 636f 6d2f 706f 7570  /github.com/poup
-000001a0: 6f75 2d77 6562 332f 7379 6269 6c2d 7363  ou-web3/sybil-sc
-000001b0: 6f72 6572 0d0a 636c 6173 7369 6669 6572  orer..classifier
-000001c0: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
-000001d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001e0: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-000001f0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000200: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-00000210: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-00000220: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000230: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-00000240: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-00000250: 6972 203d 200d 0a09 3d20 7362 7363 6f72  ir = ...= sbscor
-00000260: 6572 0d0a 7061 636b 6167 6573 203d 2066  er..packages = f
-00000270: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000280: 7569 7265 7320 3d20 3e3d 332e 3130 0d0a  uires = >=3.10..
-00000290: 0d0a 5b73 6264 6174 612c 2073 626c 6567  ..[sbdata, sbleg
-000002a0: 6f73 2c20 7362 7574 696c 735d 0d0a 7768  os, sbutils]..wh
-000002b0: 6572 6520 3d20 7362 7363 6f72 6572 0d0a  ere = sbscorer..
-000002c0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002d0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000002e0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000030: 2d72 6331 0d0a 6175 7468 6f72 203d 2050  -rc1..author = P
+00000040: 6f75 706f 750d 0a61 7574 686f 725f 656d  oupou..author_em
+00000050: 6169 6c20 3d20 706f 7570 6f75 2d77 6562  ail = poupou-web
+00000060: 3340 7072 6f74 6f6e 6d61 696c 2e63 6f6d  3@protonmail.com
+00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+00000080: 4120 7379 6269 6c20 7363 6f72 696e 6720  A sybil scoring 
+00000090: 746f 6f6c 0d0a 6c6f 6e67 5f64 6573 6372  tool..long_descr
+000000a0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000b0: 4541 444d 452e 6d64 2c20 4c49 4345 4e53  EADME.md, LICENS
+000000c0: 452e 7478 740d 0a6c 6f6e 675f 6465 7363  E.txt..long_desc
+000000d0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+000000e0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+000000f0: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+00000100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00000110: 6f75 706f 752d 7765 6233 2f63 6c75 7374  oupou-web3/clust
+00000120: 6572 2d73 636f 7265 720d 0a70 726f 6a65  er-scorer..proje
+00000130: 6374 5f75 726c 7320 3d20 0d0a 0942 7567  ct_urls = ...Bug
+00000140: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
+00000150: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
+00000160: 7570 6f75 2d77 6562 332f 7379 6269 6c2d  upou-web3/sybil-
+00000170: 7363 6f72 6572 2f69 7373 7565 730d 0a09  scorer/issues...
+00000180: 7265 706f 7369 746f 7279 203d 2068 7474  repository = htt
+00000190: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001a0: 706f 7570 6f75 2d77 6562 332f 7379 6269  poupou-web3/sybi
+000001b0: 6c2d 7363 6f72 6572 0d0a 636c 6173 7369  l-scorer..classi
+000001c0: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
+000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+000001f0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+00000200: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000210: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000220: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000230: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
+00000240: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+00000250: 6765 5f64 6972 203d 200d 0a09 3d20 7362  ge_dir = ...= sb
+00000260: 7363 6f72 6572 0d0a 7061 636b 6167 6573  scorer..packages
+00000270: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+00000280: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+00000290: 3130 0d0a 0d0a 5b73 6264 6174 612c 2073  10....[sbdata, s
+000002a0: 626c 6567 6f73 2c20 7362 7574 696c 735d  blegos, sbutils]
+000002b0: 0d0a 7768 6572 6520 3d20 7362 7363 6f72  ..where = sbscor
+000002c0: 6572 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  er....[egg_info]
+000002d0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000002e0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

