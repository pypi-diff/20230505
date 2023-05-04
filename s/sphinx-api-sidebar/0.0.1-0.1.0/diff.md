# Comparing `tmp/sphinx-api-sidebar-0.0.1.tar.gz` & `tmp/sphinx_api_sidebar-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-api-sidebar-0.0.1.tar", last modified: Thu May  4 16:44:32 2023, max compression
+gzip compressed data, was "sphinx_api_sidebar-0.1.0.tar", last modified: Thu May  4 23:27:13 2023, max compression
```

## Comparing `sphinx-api-sidebar-0.0.1.tar` & `sphinx_api_sidebar-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 16:44:32.142057 sphinx-api-sidebar-0.0.1/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-05-04 06:26:37.000000 sphinx-api-sidebar-0.0.1/LICENSE
--rw-r--r--   0 yihengxiong   (501) staff       (20)        0 2023-05-04 06:32:13.000000 sphinx-api-sidebar-0.0.1/MANIFEST.in
--rw-r--r--   0 yihengxiong   (501) staff       (20)     4163 2023-05-04 16:44:32.141757 sphinx-api-sidebar-0.0.1/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)     2238 2023-05-04 16:40:41.000000 sphinx-api-sidebar-0.0.1/README.md
--rw-r--r--   0 yihengxiong   (501) staff       (20)      358 2023-05-04 16:44:20.000000 sphinx-api-sidebar-0.0.1/pyproject.toml
--rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-04 16:44:32.142175 sphinx-api-sidebar-0.0.1/setup.cfg
--rw-r--r--   0 yihengxiong   (501) staff       (20)      934 2023-05-04 16:40:41.000000 sphinx-api-sidebar-0.0.1/setup.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 16:44:32.138192 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar/
--rw-r--r--   0 yihengxiong   (501) staff       (20)       37 2023-05-04 06:28:19.000000 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar/__init__.py
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1520 2023-05-04 06:30:13.000000 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar/sphinx_api_sidebar.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 16:44:32.140964 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar.egg-info/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     4163 2023-05-04 16:44:32.000000 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar.egg-info/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)      412 2023-05-04 16:44:32.000000 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar.egg-info/SOURCES.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-05-04 16:44:32.000000 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar.egg-info/dependency_links.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       66 2023-05-04 16:44:32.000000 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar.egg-info/entry_points.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       12 2023-05-04 16:44:32.000000 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar.egg-info/requires.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       19 2023-05-04 16:44:32.000000 sphinx-api-sidebar-0.0.1/sphinx_api_sidebar.egg-info/top_level.txt
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 16:44:32.141354 sphinx-api-sidebar-0.0.1/tests/
--rw-r--r--   0 yihengxiong   (501) staff       (20)      555 2023-05-04 16:40:41.000000 sphinx-api-sidebar-0.0.1/tests/test_sphinx_api_sidebar.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:27:13.662619 sphinx_api_sidebar-0.1.0/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-05-04 06:26:37.000000 sphinx_api_sidebar-0.1.0/LICENSE
+-rw-r--r--   0 yihengxiong   (501) staff       (20)        0 2023-05-04 06:32:13.000000 sphinx_api_sidebar-0.1.0/MANIFEST.in
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     4729 2023-05-04 23:27:13.661896 sphinx_api_sidebar-0.1.0/PKG-INFO
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     2804 2023-05-04 23:16:02.000000 sphinx_api_sidebar-0.1.0/README.md
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      358 2023-05-04 23:26:35.000000 sphinx_api_sidebar-0.1.0/pyproject.toml
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-04 23:27:13.662800 sphinx_api_sidebar-0.1.0/setup.cfg
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      934 2023-05-04 16:40:41.000000 sphinx_api_sidebar-0.1.0/setup.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:27:13.654517 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       37 2023-05-04 06:28:19.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar/__init__.py
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     1526 2023-05-04 23:02:49.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar/sphinx_api_sidebar.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:27:13.660058 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     4729 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/PKG-INFO
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      412 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/SOURCES.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/dependency_links.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       66 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/entry_points.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       12 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/requires.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       19 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/top_level.txt
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:27:13.660824 sphinx_api_sidebar-0.1.0/tests/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      555 2023-05-04 16:40:41.000000 sphinx_api_sidebar-0.1.0/tests/test_sphinx_api_sidebar.py
```

### Comparing `sphinx-api-sidebar-0.0.1/LICENSE` & `sphinx_api_sidebar-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-api-sidebar-0.0.1/PKG-INFO` & `sphinx_api_sidebar-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7370 6869  : 2.1.Name: sphi
-00000020: 6e78 2d61 7069 2d73 6964 6562 6172 0a56  nx-api-sidebar.V
-00000030: 6572 7369 6f6e 3a20 302e 302e 310a 5375  ersion: 0.0.1.Su
+00000020: 6e78 5f61 7069 5f73 6964 6562 6172 0a56  nx_api_sidebar.V
+00000030: 6572 7369 6f6e 3a20 302e 312e 300a 5375  ersion: 0.1.0.Su
 00000040: 6d6d 6172 793a 2044 6973 706c 6179 2061  mmary: Display a
 00000050: 6e79 2067 656e 6572 6174 6564 2073 7461  ny generated sta
 00000060: 7469 6320 4150 4920 646f 6375 6d65 6e74  tic API document
 00000070: 6174 696f 6e20 696e 2061 2073 6964 6562  ation in a sideb
 00000080: 6172 0a48 6f6d 652d 7061 6765 3a20 6874  ar.Home-page: ht
 00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000a0: 2f59 6968 656e 6778 696f 6e67 362f 7370  /Yihengxiong6/sp
@@ -124,138 +124,173 @@
 000007b0: 7220 6469 7370 6c61 7969 6e67 2061 6e79  r displaying any
 000007c0: 2067 656e 6572 6174 6564 2073 7461 7469   generated stati
 000007d0: 6320 4150 4920 646f 6375 6d65 6e74 6174  c API documentat
 000007e0: 696f 6e20 696e 2061 2073 6964 6562 6172  ion in a sidebar
 000007f0: 2e0a 0a23 2320 4f76 6572 7669 6577 0a0a  ...## Overview..
 00000800: 5468 6973 2053 7068 696e 7820 6578 7465  This Sphinx exte
 00000810: 6e73 696f 6e20 616c 6c6f 7773 2079 6f75  nsion allows you
-00000820: 2074 6f20 6175 746f 6d61 7469 6361 6c6c   to automaticall
-00000830: 7920 696e 636c 7564 6520 616e 6420 6469  y include and di
-00000840: 7370 6c61 7920 7374 6174 6963 2041 5049  splay static API
-00000850: 2064 6f63 756d 656e 7461 7469 6f6e 2028   documentation (
-00000860: 652e 672e 2c20 4a61 7661 446f 632c 2050  e.g., JavaDoc, P
-00000870: 7974 686f 6e27 7320 5370 6869 6e78 2d67  ython's Sphinx-g
-00000880: 656e 6572 6174 6564 2048 544d 4c29 2069  enerated HTML) i
-00000890: 6e20 7468 6520 7369 6465 6261 7220 6f66  n the sidebar of
-000008a0: 2079 6f75 7220 5370 6869 6e78 2064 6f63   your Sphinx doc
-000008b0: 756d 656e 7461 7469 6f6e 2e20 4974 2075  umentation. It u
-000008c0: 7064 6174 6573 2074 6865 2060 6874 6d6c  pdates the `html
-000008d0: 5f63 6f6e 7465 7874 6020 7769 7468 2074  _context` with t
-000008e0: 6865 2041 5049 2064 6f63 756d 656e 7461  he API documenta
-000008f0: 7469 6f6e 2070 6174 6873 2c20 7768 6963  tion paths, whic
-00000900: 6820 6361 6e20 7468 656e 2062 6520 7573  h can then be us
-00000910: 6564 2069 6e20 7468 6520 7369 6465 6261  ed in the sideba
-00000920: 722e 0a0a 2323 2049 6e73 7461 6c6c 6174  r...## Installat
-00000930: 696f 6e0a 0a54 6f20 696e 7374 616c 6c20  ion..To install 
-00000940: 7468 6520 6073 7068 696e 782d 6170 692d  the `sphinx-api-
-00000950: 7369 6465 6261 7260 2065 7874 656e 7369  sidebar` extensi
-00000960: 6f6e 2c20 796f 7520 6361 6e20 7573 6520  on, you can use 
-00000970: 7069 703a 0a0a 6060 6073 680a 7069 7020  pip:..```sh.pip 
-00000980: 696e 7374 616c 6c20 7370 6869 6e78 2d61  install sphinx-a
-00000990: 7069 2d73 6964 6562 6172 0a60 6060 0a0a  pi-sidebar.```..
-000009a0: 2323 2055 7361 6765 0a31 2e20 546f 2065  ## Usage.1. To e
-000009b0: 6e61 626c 6520 7468 6520 7370 6869 6e78  nable the sphinx
-000009c0: 2d61 7069 2d73 6964 6562 6172 2065 7874  -api-sidebar ext
-000009d0: 656e 7369 6f6e 2069 6e20 796f 7572 2053  ension in your S
-000009e0: 7068 696e 7820 646f 6375 6d65 6e74 6174  phinx documentat
-000009f0: 696f 6e20 7072 6f6a 6563 742c 2061 6464  ion project, add
-00000a00: 2069 7420 746f 2074 6865 2065 7874 656e   it to the exten
-00000a10: 7369 6f6e 7320 6c69 7374 2069 6e20 796f  sions list in yo
-00000a20: 7572 2063 6f6e 662e 7079 2066 696c 653a  ur conf.py file:
-00000a30: 0a0a 6060 6070 7974 686f 6e0a 6578 7465  ..```python.exte
-00000a40: 6e73 696f 6e73 203d 205b 0a20 2020 2027  nsions = [.    '
-00000a50: 7370 6869 6e78 5f61 7069 5f73 6964 6562  sphinx_api_sideb
-00000a60: 6172 272c 0a20 2020 2023 204f 7468 6572  ar',.    # Other
-00000a70: 2065 7874 656e 7369 6f6e 732e 2e2e 0a5d   extensions....]
-00000a80: 0a60 6060 0a0a 322e 2054 6f20 7573 6520  .```..2. To use 
-00000a90: 6120 6375 7374 6f6d 2063 6f6d 6d61 6e64  a custom command
-00000aa0: 2074 6f20 6765 6e65 7261 7465 2079 6f75   to generate you
-00000ab0: 7220 4150 4920 646f 6375 6d65 6e74 6174  r API documentat
-00000ac0: 696f 6e20 6f72 2073 7065 6369 6679 2064  ion or specify d
-00000ad0: 6966 6665 7265 6e74 2064 6972 6563 746f  ifferent directo
-00000ae0: 7269 6573 2c20 796f 7520 6361 6e20 7365  ries, you can se
-00000af0: 7420 7468 6520 6170 695f 646f 6373 5f67  t the api_docs_g
-00000b00: 656e 6572 6174 6f72 2063 6f6e 6669 6775  enerator configu
-00000b10: 7261 7469 6f6e 2076 616c 7565 2069 6e20  ration value in 
-00000b20: 796f 7572 2063 6f6e 662e 7079 2066 696c  your conf.py fil
-00000b30: 653a 0a0a 6060 6070 7974 686f 6e0a 6170  e:..```python.ap
-00000b40: 695f 646f 6373 5f67 656e 6572 6174 6f72  i_docs_generator
-00000b50: 203d 205b 0a20 2020 2027 3c79 6f75 725f   = [.    '<your_
-00000b60: 6375 7374 6f6d 5f62 7569 6c64 5f63 6f6d  custom_build_com
-00000b70: 6d61 6e64 3e27 2c0a 2020 2020 5b0a 2020  mand>',.    [.  
-00000b80: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00000b90: 2020 2020 276e 616d 6527 3a20 273c 6765      'name': '<ge
-00000ba0: 6e65 7261 7465 645f 6170 695f 646f 635f  nerated_api_doc_
-00000bb0: 6e61 6d65 3e27 2c0a 2020 2020 2020 2020  name>',.        
-00000bc0: 2020 2020 2770 6174 6827 3a20 273c 7061      'path': '<pa
-00000bd0: 7468 5f74 6f5f 6765 6e65 7261 7465 645f  th_to_generated_
-00000be0: 6170 695f 646f 633e 270a 2020 2020 2020  api_doc>'.      
-00000bf0: 2020 7d2c 0a20 2020 2020 2020 2023 2041    },.        # A
-00000c00: 6464 206d 6f72 6520 6469 6374 696f 6e61  dd more dictiona
-00000c10: 7269 6573 2066 6f72 2065 6163 6820 6164  ries for each ad
-00000c20: 6469 7469 6f6e 616c 2041 5049 2064 6f63  ditional API doc
-00000c30: 0a20 2020 205d 0a5d 0a60 6060 0a0a 5265  .    ].].```..Re
-00000c40: 706c 6163 6520 3c79 6f75 725f 6375 7374  place <your_cust
-00000c50: 6f6d 5f62 7569 6c64 5f63 6f6d 6d61 6e64  om_build_command
-00000c60: 3e2c 203c 6765 6e65 7261 7465 645f 6170  >, <generated_ap
-00000c70: 695f 646f 635f 6e61 6d65 3e2c 2061 6e64  i_doc_name>, and
-00000c80: 203c 7061 7468 5f74 6f5f 6765 6e65 7261   <path_to_genera
-00000c90: 7465 645f 6170 695f 646f 633e 2077 6974  ted_api_doc> wit
-00000ca0: 6820 7468 6520 6170 7072 6f70 7269 6174  h the appropriat
-00000cb0: 6520 7661 6c75 6573 2066 6f72 2079 6f75  e values for you
-00000cc0: 7220 7072 6f6a 6563 742e 0a0a 0a33 2e20  r project....3. 
-00000cd0: 546f 206d 616b 6520 7468 6520 6469 6666  To make the diff
-00000ce0: 6572 656e 7420 6170 6920 646f 6375 6d65  erent api docume
-00000cf0: 6e74 6174 696f 6e20 7368 6f77 2075 7020  ntation show up 
-00000d00: 696e 2074 6865 2073 6964 6562 6172 2c20  in the sidebar, 
-00000d10: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
-00000d20: 2063 6f70 7920 7468 6520 6061 7069 5f64   copy the `api_d
-00000d30: 6f63 735f 7369 6465 6261 722e 6874 6d6c  ocs_sidebar.html
-00000d40: 6020 7465 6d70 6c61 7465 2066 696c 6520  ` template file 
-00000d50: 6672 6f6d 2074 6865 2060 7370 6869 6e78  from the `sphinx
-00000d60: 5f61 7069 5f73 6964 6562 6172 2f74 656d  _api_sidebar/tem
-00000d70: 706c 6174 6573 6020 666f 6c64 6572 206f  plates` folder o
-00000d80: 6620 7468 6520 696e 7374 616c 6c65 6420  f the installed 
-00000d90: 7061 636b 6167 6520 746f 2079 6f75 7220  package to your 
-00000da0: 5370 6869 6e78 2070 726f 6a65 6374 2773  Sphinx project's
-00000db0: 205f 7465 6d70 6c61 7465 7320 666f 6c64   _templates fold
-00000dc0: 6572 2e20 416c 7465 726e 6174 6976 656c  er. Alternativel
-00000dd0: 792c 2079 6f75 2063 616e 2063 7265 6174  y, you can creat
-00000de0: 6520 6120 6e65 7720 6669 6c65 2069 6e20  e a new file in 
-00000df0: 796f 7572 2070 726f 6a65 6374 2773 205f  your project's _
-00000e00: 7465 6d70 6c61 7465 7320 666f 6c64 6572  templates folder
-00000e10: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
-00000e20: 696e 6720 636f 6e74 656e 743a 0a0a 6060  ing content:..``
-00000e30: 6068 746d 6c0a 7b25 2069 6620 6170 695f  `html.{% if api_
-00000e40: 646f 6373 2025 7d0a 2020 3c68 333e 7b7b  docs %}.  <h3>{{
-00000e50: 205f 2827 4150 4920 446f 6375 6d65 6e74   _('API Document
-00000e60: 6174 696f 6e27 2920 7d7d 3c2f 6833 3e0a  ation') }}</h3>.
-00000e70: 2020 3c75 6c20 7374 796c 653d 226c 6973    <ul style="lis
-00000e80: 742d 7374 796c 652d 7479 7065 3a20 6e6f  t-style-type: no
-00000e90: 6e65 3b22 3e0a 2020 2020 7b25 2d20 666f  ne;">.    {%- fo
-00000ea0: 7220 6974 656d 2069 6e20 6170 695f 646f  r item in api_do
-00000eb0: 6373 2025 7d0a 2020 2020 2020 3c6c 6920  cs %}.      <li 
-00000ec0: 7374 796c 653d 226d 6172 6769 6e2d 626f  style="margin-bo
-00000ed0: 7474 6f6d 3a20 3130 7078 3b22 3e3c 6120  ttom: 10px;"><a 
-00000ee0: 6872 6566 3d22 7b7b 2070 6174 6874 6f28  href="{{ pathto(
-00000ef0: 275f 7374 6174 6963 2f61 7069 2d64 6f63  '_static/api-doc
-00000f00: 732f 7b7d 272e 666f 726d 6174 2869 7465  s/{}'.format(ite
-00000f10: 6d29 2c20 3129 207d 7d22 3e7b 7b20 6974  m), 1) }}">{{ it
-00000f20: 656d 207d 7d3c 2f61 3e3c 2f6c 693e 0a20  em }}</a></li>. 
-00000f30: 2020 207b 252d 2065 6e64 666f 7220 257d     {%- endfor %}
-00000f40: 0a20 203c 2f75 6c3e 0a7b 2520 656e 6469  .  </ul>.{% endi
-00000f50: 6620 257d 0a60 6060 0a0a 342e 2055 7064  f %}.```..4. Upd
-00000f60: 6174 6520 796f 7572 2060 636f 6e66 2e70  ate your `conf.p
-00000f70: 7960 2066 696c 6520 746f 2069 6e63 6c75  y` file to inclu
-00000f80: 6465 2074 6865 2060 6170 695f 646f 6373  de the `api_docs
-00000f90: 5f73 6964 6562 6172 2e68 746d 6c60 2074  _sidebar.html` t
-00000fa0: 656d 706c 6174 6520 696e 2074 6865 2068  emplate in the h
-00000fb0: 746d 6c5f 7369 6465 6261 7273 2063 6f6e  tml_sidebars con
-00000fc0: 6669 6775 7261 7469 6f6e 3a0a 0a60 6060  figuration:..```
-00000fd0: 7079 7468 6f6e 0a68 746d 6c5f 7369 6465  python.html_side
-00000fe0: 6261 7273 203d 207b 0a20 2020 2027 2a2a  bars = {.    '**
-00000ff0: 273a 205b 0a20 2020 2020 2020 2023 202e  ': [.        # .
-00001000: 2e2e 206f 7468 6572 2073 6964 6562 6172  .. other sidebar
-00001010: 7320 2e2e 2e0a 2020 2020 2020 2020 2761  s ....        'a
-00001020: 7069 5f64 6f63 735f 7369 6465 6261 722e  pi_docs_sidebar.
-00001030: 6874 6d6c 272c 0a20 2020 205d 0a7d 0a60  html',.    ].}.`
-00001040: 6060 0a                                  ``.
+00000820: 2074 6f20 696e 636c 7564 6520 616e 6420   to include and 
+00000830: 6469 7370 6c61 7920 7374 6174 6963 2041  display static A
+00000840: 5049 2064 6f63 756d 656e 7461 7469 6f6e  PI documentation
+00000850: 2028 652e 672e 2c20 604a 6176 6144 6f63   (e.g., `JavaDoc
+00000860: 602c 2060 446f 7879 6765 6e60 2920 696e  `, `Doxygen`) in
+00000870: 2074 6865 2073 6964 6562 6172 206f 6620   the sidebar of 
+00000880: 796f 7572 2053 7068 696e 7820 646f 6375  your Sphinx docu
+00000890: 6d65 6e74 6174 696f 6e2e 2049 7420 7570  mentation. It up
+000008a0: 6461 7465 7320 7468 6520 6068 746d 6c5f  dates the `html_
+000008b0: 636f 6e74 6578 7460 2077 6974 6820 7468  context` with th
+000008c0: 6520 4150 4920 646f 6375 6d65 6e74 6174  e API documentat
+000008d0: 696f 6e20 7061 7468 732c 2077 6869 6368  ion paths, which
+000008e0: 2063 616e 2074 6865 6e20 6265 2075 7365   can then be use
+000008f0: 6420 696e 2074 6865 2041 5049 2073 6964  d in the API sid
+00000900: 6562 6172 2074 656d 706c 6174 652e 0a0a  ebar template...
+00000910: 5468 6973 2065 7874 656e 7369 6f6e 2073  This extension s
+00000920: 6572 7665 7320 6173 2061 6e20 696d 6d65  erves as an imme
+00000930: 6469 6174 6520 776f 726b 6172 6f75 6e64  diate workaround
+00000940: 2074 6f20 6d61 6b65 2053 7068 696e 7820   to make Sphinx 
+00000950: 636f 6e73 756d 6520 4150 4920 646f 6373  consume API docs
+00000960: 2066 726f 6d20 7661 7269 6f75 7320 6c61   from various la
+00000970: 6e67 7561 6765 7320 7769 7468 6f75 7420  nguages without 
+00000980: 6275 696c 6469 6e67 2061 6464 6974 696f  building additio
+00000990: 6e61 6c20 6578 7465 6e73 696f 6e73 2e0a  nal extensions..
+000009a0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+000009b0: 0a0a 546f 2069 6e73 7461 6c6c 2074 6865  ..To install the
+000009c0: 2060 7370 6869 6e78 2d61 7069 2d73 6964   `sphinx-api-sid
+000009d0: 6562 6172 6020 6578 7465 6e73 696f 6e2c  ebar` extension,
+000009e0: 2079 6f75 2063 616e 2075 7365 2070 6970   you can use pip
+000009f0: 3a0a 0a60 6060 7368 0a70 6970 2069 6e73  :..```sh.pip ins
+00000a00: 7461 6c6c 2073 7068 696e 782d 6170 692d  tall sphinx-api-
+00000a10: 7369 6465 6261 720a 6060 600a 0a23 2320  sidebar.```..## 
+00000a20: 5573 6167 650a 312e 2054 6f20 656e 6162  Usage.1. To enab
+00000a30: 6c65 2074 6865 2073 7068 696e 782d 6170  le the sphinx-ap
+00000a40: 692d 7369 6465 6261 7220 6578 7465 6e73  i-sidebar extens
+00000a50: 696f 6e20 696e 2079 6f75 7220 5370 6869  ion in your Sphi
+00000a60: 6e78 2064 6f63 756d 656e 7461 7469 6f6e  nx documentation
+00000a70: 2070 726f 6a65 6374 2c20 6164 6420 6974   project, add it
+00000a80: 2074 6f20 7468 6520 6578 7465 6e73 696f   to the extensio
+00000a90: 6e73 206c 6973 7420 696e 2079 6f75 7220  ns list in your 
+00000aa0: 636f 6e66 2e70 7920 6669 6c65 3a0a 0a60  conf.py file:..`
+00000ab0: 6060 7079 7468 6f6e 0a65 7874 656e 7369  ``python.extensi
+00000ac0: 6f6e 7320 3d20 5b0a 2020 2020 2773 7068  ons = [.    'sph
+00000ad0: 696e 785f 6170 695f 7369 6465 6261 7227  inx_api_sidebar'
+00000ae0: 2c0a 2020 2020 2320 4f74 6865 7220 6578  ,.    # Other ex
+00000af0: 7465 6e73 696f 6e73 2e2e 2e0a 5d0a 6060  tensions....].``
+00000b00: 600a 0a32 2e20 546f 2075 7365 2061 2063  `..2. To use a c
+00000b10: 7573 746f 6d20 636f 6d6d 616e 6420 746f  ustom command to
+00000b20: 2067 656e 6572 6174 6520 796f 7572 2041   generate your A
+00000b30: 5049 2064 6f63 756d 656e 7461 7469 6f6e  PI documentation
+00000b40: 206f 7220 7370 6563 6966 7920 6469 6666   or specify diff
+00000b50: 6572 656e 7420 6469 7265 6374 6f72 6965  erent directorie
+00000b60: 732c 2079 6f75 2063 616e 2073 6574 2074  s, you can set t
+00000b70: 6865 2061 7069 5f64 6f63 735f 6765 6e65  he api_docs_gene
+00000b80: 7261 746f 7220 636f 6e66 6967 7572 6174  rator configurat
+00000b90: 696f 6e20 7661 6c75 6520 696e 2079 6f75  ion value in you
+00000ba0: 7220 636f 6e66 2e70 7920 6669 6c65 3a0a  r conf.py file:.
+00000bb0: 0a60 6060 7079 7468 6f6e 0a61 7069 5f64  .```python.api_d
+00000bc0: 6f63 735f 6765 6e65 7261 746f 7220 3d20  ocs_generator = 
+00000bd0: 5b0a 2020 7b0a 2020 2020 2763 6f6d 6d61  [.  {.    'comma
+00000be0: 6e64 273a 2027 3c79 6f75 725f 6170 695f  nd': '<your_api_
+00000bf0: 646f 6373 5f62 7569 6c64 5f63 6f6d 6d61  docs_build_comma
+00000c00: 6e64 5f31 3e27 2c0a 2020 2020 276f 7574  nd_1>',.    'out
+00000c10: 7075 7473 273a 205b 0a20 2020 2020 2020  puts': [.       
+00000c20: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000c30: 2020 2020 2020 2027 6e61 6d65 273a 2027         'name': '
+00000c40: 3c67 656e 6572 6174 6564 5f61 7069 5f64  <generated_api_d
+00000c50: 6f63 5f6e 616d 655f 313e 272c 0a20 2020  oc_name_1>',.   
+00000c60: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
+00000c70: 7468 273a 2027 3c70 6174 685f 746f 5f67  th': '<path_to_g
+00000c80: 656e 6572 6174 6564 5f61 7069 5f64 6f63  enerated_api_doc
+00000c90: 5f31 3e27 0a20 2020 2020 2020 2020 2020  _1>'.           
+00000ca0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00000cb0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000cc0: 2020 276e 616d 6527 3a20 273c 6765 6e65    'name': '<gene
+00000cd0: 7261 7465 645f 6170 695f 646f 635f 6e61  rated_api_doc_na
+00000ce0: 6d65 5f32 3e27 2c0a 2020 2020 2020 2020  me_2>',.        
+00000cf0: 2020 2020 2020 2020 2770 6174 6827 3a20          'path': 
+00000d00: 273c 7061 7468 5f74 6f5f 6765 6e65 7261  '<path_to_genera
+00000d10: 7465 645f 6170 695f 646f 635f 323e 270a  ted_api_doc_2>'.
+00000d20: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000d30: 2020 2020 2020 2020 2020 2023 202e 2e2e             # ...
+00000d40: 0a20 2020 2020 2020 205d 0a20 207d 2c0a  .        ].  },.
+00000d50: 2020 7b0a 2020 2020 2763 6f6d 6d61 6e64    {.    'command
+00000d60: 273a 2027 3c79 6f75 725f 6375 7374 6f6d  ': '<your_custom
+00000d70: 5f62 7569 6c64 5f63 6f6d 6d61 6e64 5f32  _build_command_2
+00000d80: 3e27 2c0a 2020 2020 276f 7574 7075 7473  >',.    'outputs
+00000d90: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
+00000da0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000db0: 2020 2027 6e61 6d65 273a 2027 3c67 656e     'name': '<gen
+00000dc0: 6572 6174 6564 5f61 7069 5f64 6f63 5f6e  erated_api_doc_n
+00000dd0: 616d 655f 333e 272c 0a20 2020 2020 2020  ame_3>',.       
+00000de0: 2020 2020 2020 2020 2027 7061 7468 273a           'path':
+00000df0: 2027 3c70 6174 685f 746f 5f67 656e 6572   '<path_to_gener
+00000e00: 6174 6564 5f61 7069 5f64 6f63 5f33 3e27  ated_api_doc_3>'
+00000e10: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00000e20: 2020 2020 2020 2020 2020 2020 2320 2e2e              # ..
+00000e30: 2e0a 2020 2020 2020 2020 5d0a 2020 7d2c  ..        ].  },
+00000e40: 0a20 2023 206d 6f72 6520 6772 6f75 7073  .  # more groups
+00000e50: 206f 6620 6765 6e65 7261 7465 6420 6170   of generated ap
+00000e60: 6920 646f 6373 0a5d 0a60 6060 0a0a 5265  i docs.].```..Re
+00000e70: 706c 6163 6520 3c79 6f75 725f 6375 7374  place <your_cust
+00000e80: 6f6d 5f62 7569 6c64 5f63 6f6d 6d61 6e64  om_build_command
+00000e90: 5f2a 3e2c 203c 6765 6e65 7261 7465 645f  _*>, <generated_
+00000ea0: 6170 695f 646f 635f 6e61 6d65 5f2a 3e2c  api_doc_name_*>,
+00000eb0: 2061 6e64 203c 7061 7468 5f74 6f5f 6765   and <path_to_ge
+00000ec0: 6e65 7261 7465 645f 6170 695f 646f 635f  nerated_api_doc_
+00000ed0: 2a3e 2077 6974 6820 7468 6520 6170 7072  *> with the appr
+00000ee0: 6f70 7269 6174 6520 7661 6c75 6573 2066  opriate values f
+00000ef0: 6f72 2079 6f75 7220 7072 6f6a 6563 742e  or your project.
+00000f00: 0a0a 0a33 2e20 546f 206d 616b 6520 7468  ...3. To make th
+00000f10: 6520 6469 6666 6572 656e 7420 6170 6920  e different api 
+00000f20: 646f 6375 6d65 6e74 6174 696f 6e20 7368  documentation sh
+00000f30: 6f77 2075 7020 696e 2074 6865 2073 6964  ow up in the sid
+00000f40: 6562 6172 2c20 796f 7520 7769 6c6c 206e  ebar, you will n
+00000f50: 6565 6420 746f 2063 6f70 7920 7468 6520  eed to copy the 
+00000f60: 6061 7069 5f64 6f63 735f 7369 6465 6261  `api_docs_sideba
+00000f70: 722e 6874 6d6c 6020 7465 6d70 6c61 7465  r.html` template
+00000f80: 2066 696c 6520 6672 6f6d 2074 6865 2060   file from the `
+00000f90: 7370 6869 6e78 5f61 7069 5f73 6964 6562  sphinx_api_sideb
+00000fa0: 6172 2f74 656d 706c 6174 6573 6020 666f  ar/templates` fo
+00000fb0: 6c64 6572 206f 6620 7468 6520 696e 7374  lder of the inst
+00000fc0: 616c 6c65 6420 7061 636b 6167 6520 746f  alled package to
+00000fd0: 2079 6f75 7220 5370 6869 6e78 2070 726f   your Sphinx pro
+00000fe0: 6a65 6374 2773 205f 7465 6d70 6c61 7465  ject's _template
+00000ff0: 7320 666f 6c64 6572 2e20 416c 7465 726e  s folder. Altern
+00001000: 6174 6976 656c 792c 2079 6f75 2063 616e  atively, you can
+00001010: 2063 7265 6174 6520 6120 6e65 7720 6669   create a new fi
+00001020: 6c65 2069 6e20 796f 7572 2070 726f 6a65  le in your proje
+00001030: 6374 2773 205f 7465 6d70 6c61 7465 7320  ct's _templates 
+00001040: 666f 6c64 6572 2077 6974 6820 7468 6520  folder with the 
+00001050: 666f 6c6c 6f77 696e 6720 636f 6e74 656e  following conten
+00001060: 743a 0a0a 6060 6068 746d 6c0a 7b25 2069  t:..```html.{% i
+00001070: 6620 6170 695f 646f 6373 2025 7d0a 2020  f api_docs %}.  
+00001080: 3c68 333e 7b7b 205f 2827 4150 4920 446f  <h3>{{ _('API Do
+00001090: 6375 6d65 6e74 6174 696f 6e27 2920 7d7d  cumentation') }}
+000010a0: 3c2f 6833 3e0a 2020 3c75 6c20 7374 796c  </h3>.  <ul styl
+000010b0: 653d 226c 6973 742d 7374 796c 652d 7479  e="list-style-ty
+000010c0: 7065 3a20 6e6f 6e65 3b22 3e0a 2020 2020  pe: none;">.    
+000010d0: 7b25 2d20 666f 7220 6974 656d 2069 6e20  {%- for item in 
+000010e0: 6170 695f 646f 6373 2025 7d0a 2020 2020  api_docs %}.    
+000010f0: 2020 3c6c 6920 7374 796c 653d 226d 6172    <li style="mar
+00001100: 6769 6e2d 626f 7474 6f6d 3a20 3130 7078  gin-bottom: 10px
+00001110: 3b22 3e3c 6120 6872 6566 3d22 7b7b 2070  ;"><a href="{{ p
+00001120: 6174 6874 6f28 275f 7374 6174 6963 2f61  athto('_static/a
+00001130: 7069 2d64 6f63 732f 7b7d 272e 666f 726d  pi-docs/{}'.form
+00001140: 6174 2869 7465 6d29 2c20 3129 207d 7d22  at(item), 1) }}"
+00001150: 3e7b 7b20 6974 656d 207d 7d3c 2f61 3e3c  >{{ item }}</a><
+00001160: 2f6c 693e 0a20 2020 207b 252d 2065 6e64  /li>.    {%- end
+00001170: 666f 7220 257d 0a20 203c 2f75 6c3e 0a7b  for %}.  </ul>.{
+00001180: 2520 656e 6469 6620 257d 0a60 6060 0a0a  % endif %}.```..
+00001190: 342e 2055 7064 6174 6520 796f 7572 2060  4. Update your `
+000011a0: 636f 6e66 2e70 7960 2066 696c 6520 746f  conf.py` file to
+000011b0: 2069 6e63 6c75 6465 2074 6865 2060 6170   include the `ap
+000011c0: 695f 646f 6373 5f73 6964 6562 6172 2e68  i_docs_sidebar.h
+000011d0: 746d 6c60 2074 656d 706c 6174 6520 696e  tml` template in
+000011e0: 2074 6865 2068 746d 6c5f 7369 6465 6261   the html_sideba
+000011f0: 7273 2063 6f6e 6669 6775 7261 7469 6f6e  rs configuration
+00001200: 3a0a 0a60 6060 7079 7468 6f6e 0a68 746d  :..```python.htm
+00001210: 6c5f 7369 6465 6261 7273 203d 207b 0a20  l_sidebars = {. 
+00001220: 2020 2027 2a2a 273a 205b 0a20 2020 2020     '**': [.     
+00001230: 2020 2023 202e 2e2e 206f 7468 6572 2073     # ... other s
+00001240: 6964 6562 6172 7320 2e2e 2e0a 2020 2020  idebars ....    
+00001250: 2020 2020 2761 7069 5f64 6f63 735f 7369      'api_docs_si
+00001260: 6465 6261 722e 6874 6d6c 272c 0a20 2020  debar.html',.   
+00001270: 205d 0a7d 0a60 6060 0a                    ].}.```.
```

### Comparing `sphinx-api-sidebar-0.0.1/README.md` & `sphinx_api_sidebar-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Sphinx API Sidebar
 
 A Sphinx extension for displaying any generated static API documentation in a sidebar.
 
 ## Overview
 
-This Sphinx extension allows you to automatically include and display static API documentation (e.g., JavaDoc, Python's Sphinx-generated HTML) in the sidebar of your Sphinx documentation. It updates the `html_context` with the API documentation paths, which can then be used in the sidebar.
+This Sphinx extension allows you to include and display static API documentation (e.g., `JavaDoc`, `Doxygen`) in the sidebar of your Sphinx documentation. It updates the `html_context` with the API documentation paths, which can then be used in the API sidebar template.
+
+This extension serves as an immediate workaround to make Sphinx consume API docs from various languages without building additional extensions.
 
 ## Installation
 
 To install the `sphinx-api-sidebar` extension, you can use pip:
 
 ```sh
 pip install sphinx-api-sidebar
@@ -24,26 +26,43 @@
 ]
 ```
 
 2. To use a custom command to generate your API documentation or specify different directories, you can set the api_docs_generator configuration value in your conf.py file:
 
 ```python
 api_docs_generator = [
-    '<your_custom_build_command>',
-    [
-        {
-            'name': '<generated_api_doc_name>',
-            'path': '<path_to_generated_api_doc>'
-        },
-        # Add more dictionaries for each additional API doc
-    ]
+  {
+    'command': '<your_api_docs_build_command_1>',
+    'outputs': [
+            {
+                'name': '<generated_api_doc_name_1>',
+                'path': '<path_to_generated_api_doc_1>'
+            },
+            {
+                'name': '<generated_api_doc_name_2>',
+                'path': '<path_to_generated_api_doc_2>'
+            },
+            # ...
+        ]
+  },
+  {
+    'command': '<your_custom_build_command_2>',
+    'outputs': [
+            {
+                'name': '<generated_api_doc_name_3>',
+                'path': '<path_to_generated_api_doc_3>'
+            },
+            # ...
+        ]
+  },
+  # more groups of generated api docs
 ]
 ```
 
-Replace <your_custom_build_command>, <generated_api_doc_name>, and <path_to_generated_api_doc> with the appropriate values for your project.
+Replace <your_custom_build_command_*>, <generated_api_doc_name_*>, and <path_to_generated_api_doc_*> with the appropriate values for your project.
 
 
 3. To make the different api documentation show up in the sidebar, you will need to copy the `api_docs_sidebar.html` template file from the `sphinx_api_sidebar/templates` folder of the installed package to your Sphinx project's _templates folder. Alternatively, you can create a new file in your project's _templates folder with the following content:
 
 ```html
 {% if api_docs %}
   <h3>{{ _('API Documentation') }}</h3>
```

#### html2text {}

```diff
@@ -1,22 +1,28 @@
 # Sphinx API Sidebar A Sphinx extension for displaying any generated static API
 documentation in a sidebar. ## Overview This Sphinx extension allows you to
-automatically include and display static API documentation (e.g., JavaDoc,
-Python's Sphinx-generated HTML) in the sidebar of your Sphinx documentation. It
-updates the `html_context` with the API documentation paths, which can then be
-used in the sidebar. ## Installation To install the `sphinx-api-sidebar`
-extension, you can use pip: ```sh pip install sphinx-api-sidebar ``` ## Usage
-1. To enable the sphinx-api-sidebar extension in your Sphinx documentation
-project, add it to the extensions list in your conf.py file: ```python
-extensions = [ 'sphinx_api_sidebar', # Other extensions... ] ``` 2. To use a
-custom command to generate your API documentation or specify different
-directories, you can set the api_docs_generator configuration value in your
-conf.py file: ```python api_docs_generator = [ '', [ { 'name': '', 'path': ''
-}, # Add more dictionaries for each additional API doc ] ] ``` Replace , , and
-with the appropriate values for your project. 3. To make the different api
+include and display static API documentation (e.g., `JavaDoc`, `Doxygen`) in
+the sidebar of your Sphinx documentation. It updates the `html_context` with
+the API documentation paths, which can then be used in the API sidebar
+template. This extension serves as an immediate workaround to make Sphinx
+consume API docs from various languages without building additional extensions.
+## Installation To install the `sphinx-api-sidebar` extension, you can use pip:
+```sh pip install sphinx-api-sidebar ``` ## Usage 1. To enable the sphinx-api-
+sidebar extension in your Sphinx documentation project, add it to the
+extensions list in your conf.py file: ```python extensions =
+[ 'sphinx_api_sidebar', # Other extensions... ] ``` 2. To use a custom command
+to generate your API documentation or specify different directories, you can
+set the api_docs_generator configuration value in your conf.py file: ```python
+api_docs_generator = [ { 'command': '', 'outputs': [ { 'name': '', 'path': ''
+}, { 'name': '', 'path': '' }, # ... ] }, { 'command': '', 'outputs': [
+{ 'name': '', 'path': '' }, # ... ] }, # more groups of generated api docs ]
+``` Replace
+>,
+>, and
+> with the appropriate values for your project. 3. To make the different api
 documentation show up in the sidebar, you will need to copy the
 `api_docs_sidebar.html` template file from the `sphinx_api_sidebar/templates`
 folder of the installed package to your Sphinx project's _templates folder.
 Alternatively, you can create a new file in your project's _templates folder
 with the following content: ```html {% if api_docs %}
 **** {{ _('API Documentation') }} ****
     * {%- for item in api_docs %}
```

### Comparing `sphinx-api-sidebar-0.0.1/setup.py` & `sphinx_api_sidebar-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-api-sidebar-0.0.1/sphinx_api_sidebar/sphinx_api_sidebar.py` & `sphinx_api_sidebar-0.1.0/sphinx_api_sidebar/sphinx_api_sidebar.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,34 +19,35 @@
     # get the path to the _static/api-docs directory
     api_docs_dir = os.path.join(app.srcdir, '_static/api-docs')
 
     # delete the directory if it exists
     if os.path.exists(api_docs_dir):
         shutil.rmtree(api_docs_dir)
 
-    # api_docs = config.html_context['api_docs']
     api_docs = []
 
-    # get the customized command from conf.py and run it
-    customized_build_command = config.api_docs_generator[0]
+    # iterate through the list of dictionaries and run the customized command
+    for api_docs_generator in config.api_docs_generators:
+        # get the build command from conf.py and run it
+        command = api_docs_generator['command']
 
-    subprocess.run([f'{customized_build_command}'], text=True, shell=True, capture_output=True)
+        subprocess.run([f'{command}'], text=True, shell=True, capture_output=True)
 
-    # iterate through the list of dictionaries and copy the generated API docs to the static/api-docs directory
-    for generated_api_doc in config.api_docs_generator[1]:
+        # iterate through the list of dictionaries and copy the generated API docs to the static/api-docs directory
+        for output in api_docs_generator['outputs']:
 
-        generated_api_doc_name = generated_api_doc['name']
+            api_doc_name = output['name']
 
-        generated_api_doc_path = generated_api_doc['path']
-        
-        shutil.copytree(generated_api_doc_path, os.path.join(api_docs_dir, generated_api_doc_name))
+            output_path = output['path']
+            
+            shutil.copytree(output_path, os.path.join(api_docs_dir, api_doc_name))
 
-        api_docs.append(generated_api_doc_name)
+            api_docs.append(api_doc_name)
 
     # update html_context with api_docs
     update_html_context(config, api_docs)
 
 
 def setup(app):
-    app.add_config_value('api_docs_generator', [], 'env')
+    app.add_config_value('api_docs_generators', [], 'env')
 
     app.connect('config-inited', generate_api_docs)
```

### Comparing `sphinx-api-sidebar-0.0.1/sphinx_api_sidebar.egg-info/PKG-INFO` & `sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7370 6869  : 2.1.Name: sphi
 00000020: 6e78 2d61 7069 2d73 6964 6562 6172 0a56  nx-api-sidebar.V
-00000030: 6572 7369 6f6e 3a20 302e 302e 310a 5375  ersion: 0.0.1.Su
+00000030: 6572 7369 6f6e 3a20 302e 312e 300a 5375  ersion: 0.1.0.Su
 00000040: 6d6d 6172 793a 2044 6973 706c 6179 2061  mmary: Display a
 00000050: 6e79 2067 656e 6572 6174 6564 2073 7461  ny generated sta
 00000060: 7469 6320 4150 4920 646f 6375 6d65 6e74  tic API document
 00000070: 6174 696f 6e20 696e 2061 2073 6964 6562  ation in a sideb
 00000080: 6172 0a48 6f6d 652d 7061 6765 3a20 6874  ar.Home-page: ht
 00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000a0: 2f59 6968 656e 6778 696f 6e67 362f 7370  /Yihengxiong6/sp
@@ -124,138 +124,173 @@
 000007b0: 7220 6469 7370 6c61 7969 6e67 2061 6e79  r displaying any
 000007c0: 2067 656e 6572 6174 6564 2073 7461 7469   generated stati
 000007d0: 6320 4150 4920 646f 6375 6d65 6e74 6174  c API documentat
 000007e0: 696f 6e20 696e 2061 2073 6964 6562 6172  ion in a sidebar
 000007f0: 2e0a 0a23 2320 4f76 6572 7669 6577 0a0a  ...## Overview..
 00000800: 5468 6973 2053 7068 696e 7820 6578 7465  This Sphinx exte
 00000810: 6e73 696f 6e20 616c 6c6f 7773 2079 6f75  nsion allows you
-00000820: 2074 6f20 6175 746f 6d61 7469 6361 6c6c   to automaticall
-00000830: 7920 696e 636c 7564 6520 616e 6420 6469  y include and di
-00000840: 7370 6c61 7920 7374 6174 6963 2041 5049  splay static API
-00000850: 2064 6f63 756d 656e 7461 7469 6f6e 2028   documentation (
-00000860: 652e 672e 2c20 4a61 7661 446f 632c 2050  e.g., JavaDoc, P
-00000870: 7974 686f 6e27 7320 5370 6869 6e78 2d67  ython's Sphinx-g
-00000880: 656e 6572 6174 6564 2048 544d 4c29 2069  enerated HTML) i
-00000890: 6e20 7468 6520 7369 6465 6261 7220 6f66  n the sidebar of
-000008a0: 2079 6f75 7220 5370 6869 6e78 2064 6f63   your Sphinx doc
-000008b0: 756d 656e 7461 7469 6f6e 2e20 4974 2075  umentation. It u
-000008c0: 7064 6174 6573 2074 6865 2060 6874 6d6c  pdates the `html
-000008d0: 5f63 6f6e 7465 7874 6020 7769 7468 2074  _context` with t
-000008e0: 6865 2041 5049 2064 6f63 756d 656e 7461  he API documenta
-000008f0: 7469 6f6e 2070 6174 6873 2c20 7768 6963  tion paths, whic
-00000900: 6820 6361 6e20 7468 656e 2062 6520 7573  h can then be us
-00000910: 6564 2069 6e20 7468 6520 7369 6465 6261  ed in the sideba
-00000920: 722e 0a0a 2323 2049 6e73 7461 6c6c 6174  r...## Installat
-00000930: 696f 6e0a 0a54 6f20 696e 7374 616c 6c20  ion..To install 
-00000940: 7468 6520 6073 7068 696e 782d 6170 692d  the `sphinx-api-
-00000950: 7369 6465 6261 7260 2065 7874 656e 7369  sidebar` extensi
-00000960: 6f6e 2c20 796f 7520 6361 6e20 7573 6520  on, you can use 
-00000970: 7069 703a 0a0a 6060 6073 680a 7069 7020  pip:..```sh.pip 
-00000980: 696e 7374 616c 6c20 7370 6869 6e78 2d61  install sphinx-a
-00000990: 7069 2d73 6964 6562 6172 0a60 6060 0a0a  pi-sidebar.```..
-000009a0: 2323 2055 7361 6765 0a31 2e20 546f 2065  ## Usage.1. To e
-000009b0: 6e61 626c 6520 7468 6520 7370 6869 6e78  nable the sphinx
-000009c0: 2d61 7069 2d73 6964 6562 6172 2065 7874  -api-sidebar ext
-000009d0: 656e 7369 6f6e 2069 6e20 796f 7572 2053  ension in your S
-000009e0: 7068 696e 7820 646f 6375 6d65 6e74 6174  phinx documentat
-000009f0: 696f 6e20 7072 6f6a 6563 742c 2061 6464  ion project, add
-00000a00: 2069 7420 746f 2074 6865 2065 7874 656e   it to the exten
-00000a10: 7369 6f6e 7320 6c69 7374 2069 6e20 796f  sions list in yo
-00000a20: 7572 2063 6f6e 662e 7079 2066 696c 653a  ur conf.py file:
-00000a30: 0a0a 6060 6070 7974 686f 6e0a 6578 7465  ..```python.exte
-00000a40: 6e73 696f 6e73 203d 205b 0a20 2020 2027  nsions = [.    '
-00000a50: 7370 6869 6e78 5f61 7069 5f73 6964 6562  sphinx_api_sideb
-00000a60: 6172 272c 0a20 2020 2023 204f 7468 6572  ar',.    # Other
-00000a70: 2065 7874 656e 7369 6f6e 732e 2e2e 0a5d   extensions....]
-00000a80: 0a60 6060 0a0a 322e 2054 6f20 7573 6520  .```..2. To use 
-00000a90: 6120 6375 7374 6f6d 2063 6f6d 6d61 6e64  a custom command
-00000aa0: 2074 6f20 6765 6e65 7261 7465 2079 6f75   to generate you
-00000ab0: 7220 4150 4920 646f 6375 6d65 6e74 6174  r API documentat
-00000ac0: 696f 6e20 6f72 2073 7065 6369 6679 2064  ion or specify d
-00000ad0: 6966 6665 7265 6e74 2064 6972 6563 746f  ifferent directo
-00000ae0: 7269 6573 2c20 796f 7520 6361 6e20 7365  ries, you can se
-00000af0: 7420 7468 6520 6170 695f 646f 6373 5f67  t the api_docs_g
-00000b00: 656e 6572 6174 6f72 2063 6f6e 6669 6775  enerator configu
-00000b10: 7261 7469 6f6e 2076 616c 7565 2069 6e20  ration value in 
-00000b20: 796f 7572 2063 6f6e 662e 7079 2066 696c  your conf.py fil
-00000b30: 653a 0a0a 6060 6070 7974 686f 6e0a 6170  e:..```python.ap
-00000b40: 695f 646f 6373 5f67 656e 6572 6174 6f72  i_docs_generator
-00000b50: 203d 205b 0a20 2020 2027 3c79 6f75 725f   = [.    '<your_
-00000b60: 6375 7374 6f6d 5f62 7569 6c64 5f63 6f6d  custom_build_com
-00000b70: 6d61 6e64 3e27 2c0a 2020 2020 5b0a 2020  mand>',.    [.  
-00000b80: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00000b90: 2020 2020 276e 616d 6527 3a20 273c 6765      'name': '<ge
-00000ba0: 6e65 7261 7465 645f 6170 695f 646f 635f  nerated_api_doc_
-00000bb0: 6e61 6d65 3e27 2c0a 2020 2020 2020 2020  name>',.        
-00000bc0: 2020 2020 2770 6174 6827 3a20 273c 7061      'path': '<pa
-00000bd0: 7468 5f74 6f5f 6765 6e65 7261 7465 645f  th_to_generated_
-00000be0: 6170 695f 646f 633e 270a 2020 2020 2020  api_doc>'.      
-00000bf0: 2020 7d2c 0a20 2020 2020 2020 2023 2041    },.        # A
-00000c00: 6464 206d 6f72 6520 6469 6374 696f 6e61  dd more dictiona
-00000c10: 7269 6573 2066 6f72 2065 6163 6820 6164  ries for each ad
-00000c20: 6469 7469 6f6e 616c 2041 5049 2064 6f63  ditional API doc
-00000c30: 0a20 2020 205d 0a5d 0a60 6060 0a0a 5265  .    ].].```..Re
-00000c40: 706c 6163 6520 3c79 6f75 725f 6375 7374  place <your_cust
-00000c50: 6f6d 5f62 7569 6c64 5f63 6f6d 6d61 6e64  om_build_command
-00000c60: 3e2c 203c 6765 6e65 7261 7465 645f 6170  >, <generated_ap
-00000c70: 695f 646f 635f 6e61 6d65 3e2c 2061 6e64  i_doc_name>, and
-00000c80: 203c 7061 7468 5f74 6f5f 6765 6e65 7261   <path_to_genera
-00000c90: 7465 645f 6170 695f 646f 633e 2077 6974  ted_api_doc> wit
-00000ca0: 6820 7468 6520 6170 7072 6f70 7269 6174  h the appropriat
-00000cb0: 6520 7661 6c75 6573 2066 6f72 2079 6f75  e values for you
-00000cc0: 7220 7072 6f6a 6563 742e 0a0a 0a33 2e20  r project....3. 
-00000cd0: 546f 206d 616b 6520 7468 6520 6469 6666  To make the diff
-00000ce0: 6572 656e 7420 6170 6920 646f 6375 6d65  erent api docume
-00000cf0: 6e74 6174 696f 6e20 7368 6f77 2075 7020  ntation show up 
-00000d00: 696e 2074 6865 2073 6964 6562 6172 2c20  in the sidebar, 
-00000d10: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
-00000d20: 2063 6f70 7920 7468 6520 6061 7069 5f64   copy the `api_d
-00000d30: 6f63 735f 7369 6465 6261 722e 6874 6d6c  ocs_sidebar.html
-00000d40: 6020 7465 6d70 6c61 7465 2066 696c 6520  ` template file 
-00000d50: 6672 6f6d 2074 6865 2060 7370 6869 6e78  from the `sphinx
-00000d60: 5f61 7069 5f73 6964 6562 6172 2f74 656d  _api_sidebar/tem
-00000d70: 706c 6174 6573 6020 666f 6c64 6572 206f  plates` folder o
-00000d80: 6620 7468 6520 696e 7374 616c 6c65 6420  f the installed 
-00000d90: 7061 636b 6167 6520 746f 2079 6f75 7220  package to your 
-00000da0: 5370 6869 6e78 2070 726f 6a65 6374 2773  Sphinx project's
-00000db0: 205f 7465 6d70 6c61 7465 7320 666f 6c64   _templates fold
-00000dc0: 6572 2e20 416c 7465 726e 6174 6976 656c  er. Alternativel
-00000dd0: 792c 2079 6f75 2063 616e 2063 7265 6174  y, you can creat
-00000de0: 6520 6120 6e65 7720 6669 6c65 2069 6e20  e a new file in 
-00000df0: 796f 7572 2070 726f 6a65 6374 2773 205f  your project's _
-00000e00: 7465 6d70 6c61 7465 7320 666f 6c64 6572  templates folder
-00000e10: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
-00000e20: 696e 6720 636f 6e74 656e 743a 0a0a 6060  ing content:..``
-00000e30: 6068 746d 6c0a 7b25 2069 6620 6170 695f  `html.{% if api_
-00000e40: 646f 6373 2025 7d0a 2020 3c68 333e 7b7b  docs %}.  <h3>{{
-00000e50: 205f 2827 4150 4920 446f 6375 6d65 6e74   _('API Document
-00000e60: 6174 696f 6e27 2920 7d7d 3c2f 6833 3e0a  ation') }}</h3>.
-00000e70: 2020 3c75 6c20 7374 796c 653d 226c 6973    <ul style="lis
-00000e80: 742d 7374 796c 652d 7479 7065 3a20 6e6f  t-style-type: no
-00000e90: 6e65 3b22 3e0a 2020 2020 7b25 2d20 666f  ne;">.    {%- fo
-00000ea0: 7220 6974 656d 2069 6e20 6170 695f 646f  r item in api_do
-00000eb0: 6373 2025 7d0a 2020 2020 2020 3c6c 6920  cs %}.      <li 
-00000ec0: 7374 796c 653d 226d 6172 6769 6e2d 626f  style="margin-bo
-00000ed0: 7474 6f6d 3a20 3130 7078 3b22 3e3c 6120  ttom: 10px;"><a 
-00000ee0: 6872 6566 3d22 7b7b 2070 6174 6874 6f28  href="{{ pathto(
-00000ef0: 275f 7374 6174 6963 2f61 7069 2d64 6f63  '_static/api-doc
-00000f00: 732f 7b7d 272e 666f 726d 6174 2869 7465  s/{}'.format(ite
-00000f10: 6d29 2c20 3129 207d 7d22 3e7b 7b20 6974  m), 1) }}">{{ it
-00000f20: 656d 207d 7d3c 2f61 3e3c 2f6c 693e 0a20  em }}</a></li>. 
-00000f30: 2020 207b 252d 2065 6e64 666f 7220 257d     {%- endfor %}
-00000f40: 0a20 203c 2f75 6c3e 0a7b 2520 656e 6469  .  </ul>.{% endi
-00000f50: 6620 257d 0a60 6060 0a0a 342e 2055 7064  f %}.```..4. Upd
-00000f60: 6174 6520 796f 7572 2060 636f 6e66 2e70  ate your `conf.p
-00000f70: 7960 2066 696c 6520 746f 2069 6e63 6c75  y` file to inclu
-00000f80: 6465 2074 6865 2060 6170 695f 646f 6373  de the `api_docs
-00000f90: 5f73 6964 6562 6172 2e68 746d 6c60 2074  _sidebar.html` t
-00000fa0: 656d 706c 6174 6520 696e 2074 6865 2068  emplate in the h
-00000fb0: 746d 6c5f 7369 6465 6261 7273 2063 6f6e  tml_sidebars con
-00000fc0: 6669 6775 7261 7469 6f6e 3a0a 0a60 6060  figuration:..```
-00000fd0: 7079 7468 6f6e 0a68 746d 6c5f 7369 6465  python.html_side
-00000fe0: 6261 7273 203d 207b 0a20 2020 2027 2a2a  bars = {.    '**
-00000ff0: 273a 205b 0a20 2020 2020 2020 2023 202e  ': [.        # .
-00001000: 2e2e 206f 7468 6572 2073 6964 6562 6172  .. other sidebar
-00001010: 7320 2e2e 2e0a 2020 2020 2020 2020 2761  s ....        'a
-00001020: 7069 5f64 6f63 735f 7369 6465 6261 722e  pi_docs_sidebar.
-00001030: 6874 6d6c 272c 0a20 2020 205d 0a7d 0a60  html',.    ].}.`
-00001040: 6060 0a                                  ``.
+00000820: 2074 6f20 696e 636c 7564 6520 616e 6420   to include and 
+00000830: 6469 7370 6c61 7920 7374 6174 6963 2041  display static A
+00000840: 5049 2064 6f63 756d 656e 7461 7469 6f6e  PI documentation
+00000850: 2028 652e 672e 2c20 604a 6176 6144 6f63   (e.g., `JavaDoc
+00000860: 602c 2060 446f 7879 6765 6e60 2920 696e  `, `Doxygen`) in
+00000870: 2074 6865 2073 6964 6562 6172 206f 6620   the sidebar of 
+00000880: 796f 7572 2053 7068 696e 7820 646f 6375  your Sphinx docu
+00000890: 6d65 6e74 6174 696f 6e2e 2049 7420 7570  mentation. It up
+000008a0: 6461 7465 7320 7468 6520 6068 746d 6c5f  dates the `html_
+000008b0: 636f 6e74 6578 7460 2077 6974 6820 7468  context` with th
+000008c0: 6520 4150 4920 646f 6375 6d65 6e74 6174  e API documentat
+000008d0: 696f 6e20 7061 7468 732c 2077 6869 6368  ion paths, which
+000008e0: 2063 616e 2074 6865 6e20 6265 2075 7365   can then be use
+000008f0: 6420 696e 2074 6865 2041 5049 2073 6964  d in the API sid
+00000900: 6562 6172 2074 656d 706c 6174 652e 0a0a  ebar template...
+00000910: 5468 6973 2065 7874 656e 7369 6f6e 2073  This extension s
+00000920: 6572 7665 7320 6173 2061 6e20 696d 6d65  erves as an imme
+00000930: 6469 6174 6520 776f 726b 6172 6f75 6e64  diate workaround
+00000940: 2074 6f20 6d61 6b65 2053 7068 696e 7820   to make Sphinx 
+00000950: 636f 6e73 756d 6520 4150 4920 646f 6373  consume API docs
+00000960: 2066 726f 6d20 7661 7269 6f75 7320 6c61   from various la
+00000970: 6e67 7561 6765 7320 7769 7468 6f75 7420  nguages without 
+00000980: 6275 696c 6469 6e67 2061 6464 6974 696f  building additio
+00000990: 6e61 6c20 6578 7465 6e73 696f 6e73 2e0a  nal extensions..
+000009a0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+000009b0: 0a0a 546f 2069 6e73 7461 6c6c 2074 6865  ..To install the
+000009c0: 2060 7370 6869 6e78 2d61 7069 2d73 6964   `sphinx-api-sid
+000009d0: 6562 6172 6020 6578 7465 6e73 696f 6e2c  ebar` extension,
+000009e0: 2079 6f75 2063 616e 2075 7365 2070 6970   you can use pip
+000009f0: 3a0a 0a60 6060 7368 0a70 6970 2069 6e73  :..```sh.pip ins
+00000a00: 7461 6c6c 2073 7068 696e 782d 6170 692d  tall sphinx-api-
+00000a10: 7369 6465 6261 720a 6060 600a 0a23 2320  sidebar.```..## 
+00000a20: 5573 6167 650a 312e 2054 6f20 656e 6162  Usage.1. To enab
+00000a30: 6c65 2074 6865 2073 7068 696e 782d 6170  le the sphinx-ap
+00000a40: 692d 7369 6465 6261 7220 6578 7465 6e73  i-sidebar extens
+00000a50: 696f 6e20 696e 2079 6f75 7220 5370 6869  ion in your Sphi
+00000a60: 6e78 2064 6f63 756d 656e 7461 7469 6f6e  nx documentation
+00000a70: 2070 726f 6a65 6374 2c20 6164 6420 6974   project, add it
+00000a80: 2074 6f20 7468 6520 6578 7465 6e73 696f   to the extensio
+00000a90: 6e73 206c 6973 7420 696e 2079 6f75 7220  ns list in your 
+00000aa0: 636f 6e66 2e70 7920 6669 6c65 3a0a 0a60  conf.py file:..`
+00000ab0: 6060 7079 7468 6f6e 0a65 7874 656e 7369  ``python.extensi
+00000ac0: 6f6e 7320 3d20 5b0a 2020 2020 2773 7068  ons = [.    'sph
+00000ad0: 696e 785f 6170 695f 7369 6465 6261 7227  inx_api_sidebar'
+00000ae0: 2c0a 2020 2020 2320 4f74 6865 7220 6578  ,.    # Other ex
+00000af0: 7465 6e73 696f 6e73 2e2e 2e0a 5d0a 6060  tensions....].``
+00000b00: 600a 0a32 2e20 546f 2075 7365 2061 2063  `..2. To use a c
+00000b10: 7573 746f 6d20 636f 6d6d 616e 6420 746f  ustom command to
+00000b20: 2067 656e 6572 6174 6520 796f 7572 2041   generate your A
+00000b30: 5049 2064 6f63 756d 656e 7461 7469 6f6e  PI documentation
+00000b40: 206f 7220 7370 6563 6966 7920 6469 6666   or specify diff
+00000b50: 6572 656e 7420 6469 7265 6374 6f72 6965  erent directorie
+00000b60: 732c 2079 6f75 2063 616e 2073 6574 2074  s, you can set t
+00000b70: 6865 2061 7069 5f64 6f63 735f 6765 6e65  he api_docs_gene
+00000b80: 7261 746f 7220 636f 6e66 6967 7572 6174  rator configurat
+00000b90: 696f 6e20 7661 6c75 6520 696e 2079 6f75  ion value in you
+00000ba0: 7220 636f 6e66 2e70 7920 6669 6c65 3a0a  r conf.py file:.
+00000bb0: 0a60 6060 7079 7468 6f6e 0a61 7069 5f64  .```python.api_d
+00000bc0: 6f63 735f 6765 6e65 7261 746f 7220 3d20  ocs_generator = 
+00000bd0: 5b0a 2020 7b0a 2020 2020 2763 6f6d 6d61  [.  {.    'comma
+00000be0: 6e64 273a 2027 3c79 6f75 725f 6170 695f  nd': '<your_api_
+00000bf0: 646f 6373 5f62 7569 6c64 5f63 6f6d 6d61  docs_build_comma
+00000c00: 6e64 5f31 3e27 2c0a 2020 2020 276f 7574  nd_1>',.    'out
+00000c10: 7075 7473 273a 205b 0a20 2020 2020 2020  puts': [.       
+00000c20: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000c30: 2020 2020 2020 2027 6e61 6d65 273a 2027         'name': '
+00000c40: 3c67 656e 6572 6174 6564 5f61 7069 5f64  <generated_api_d
+00000c50: 6f63 5f6e 616d 655f 313e 272c 0a20 2020  oc_name_1>',.   
+00000c60: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
+00000c70: 7468 273a 2027 3c70 6174 685f 746f 5f67  th': '<path_to_g
+00000c80: 656e 6572 6174 6564 5f61 7069 5f64 6f63  enerated_api_doc
+00000c90: 5f31 3e27 0a20 2020 2020 2020 2020 2020  _1>'.           
+00000ca0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00000cb0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000cc0: 2020 276e 616d 6527 3a20 273c 6765 6e65    'name': '<gene
+00000cd0: 7261 7465 645f 6170 695f 646f 635f 6e61  rated_api_doc_na
+00000ce0: 6d65 5f32 3e27 2c0a 2020 2020 2020 2020  me_2>',.        
+00000cf0: 2020 2020 2020 2020 2770 6174 6827 3a20          'path': 
+00000d00: 273c 7061 7468 5f74 6f5f 6765 6e65 7261  '<path_to_genera
+00000d10: 7465 645f 6170 695f 646f 635f 323e 270a  ted_api_doc_2>'.
+00000d20: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000d30: 2020 2020 2020 2020 2020 2023 202e 2e2e             # ...
+00000d40: 0a20 2020 2020 2020 205d 0a20 207d 2c0a  .        ].  },.
+00000d50: 2020 7b0a 2020 2020 2763 6f6d 6d61 6e64    {.    'command
+00000d60: 273a 2027 3c79 6f75 725f 6375 7374 6f6d  ': '<your_custom
+00000d70: 5f62 7569 6c64 5f63 6f6d 6d61 6e64 5f32  _build_command_2
+00000d80: 3e27 2c0a 2020 2020 276f 7574 7075 7473  >',.    'outputs
+00000d90: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
+00000da0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000db0: 2020 2027 6e61 6d65 273a 2027 3c67 656e     'name': '<gen
+00000dc0: 6572 6174 6564 5f61 7069 5f64 6f63 5f6e  erated_api_doc_n
+00000dd0: 616d 655f 333e 272c 0a20 2020 2020 2020  ame_3>',.       
+00000de0: 2020 2020 2020 2020 2027 7061 7468 273a           'path':
+00000df0: 2027 3c70 6174 685f 746f 5f67 656e 6572   '<path_to_gener
+00000e00: 6174 6564 5f61 7069 5f64 6f63 5f33 3e27  ated_api_doc_3>'
+00000e10: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00000e20: 2020 2020 2020 2020 2020 2020 2320 2e2e              # ..
+00000e30: 2e0a 2020 2020 2020 2020 5d0a 2020 7d2c  ..        ].  },
+00000e40: 0a20 2023 206d 6f72 6520 6772 6f75 7073  .  # more groups
+00000e50: 206f 6620 6765 6e65 7261 7465 6420 6170   of generated ap
+00000e60: 6920 646f 6373 0a5d 0a60 6060 0a0a 5265  i docs.].```..Re
+00000e70: 706c 6163 6520 3c79 6f75 725f 6375 7374  place <your_cust
+00000e80: 6f6d 5f62 7569 6c64 5f63 6f6d 6d61 6e64  om_build_command
+00000e90: 5f2a 3e2c 203c 6765 6e65 7261 7465 645f  _*>, <generated_
+00000ea0: 6170 695f 646f 635f 6e61 6d65 5f2a 3e2c  api_doc_name_*>,
+00000eb0: 2061 6e64 203c 7061 7468 5f74 6f5f 6765   and <path_to_ge
+00000ec0: 6e65 7261 7465 645f 6170 695f 646f 635f  nerated_api_doc_
+00000ed0: 2a3e 2077 6974 6820 7468 6520 6170 7072  *> with the appr
+00000ee0: 6f70 7269 6174 6520 7661 6c75 6573 2066  opriate values f
+00000ef0: 6f72 2079 6f75 7220 7072 6f6a 6563 742e  or your project.
+00000f00: 0a0a 0a33 2e20 546f 206d 616b 6520 7468  ...3. To make th
+00000f10: 6520 6469 6666 6572 656e 7420 6170 6920  e different api 
+00000f20: 646f 6375 6d65 6e74 6174 696f 6e20 7368  documentation sh
+00000f30: 6f77 2075 7020 696e 2074 6865 2073 6964  ow up in the sid
+00000f40: 6562 6172 2c20 796f 7520 7769 6c6c 206e  ebar, you will n
+00000f50: 6565 6420 746f 2063 6f70 7920 7468 6520  eed to copy the 
+00000f60: 6061 7069 5f64 6f63 735f 7369 6465 6261  `api_docs_sideba
+00000f70: 722e 6874 6d6c 6020 7465 6d70 6c61 7465  r.html` template
+00000f80: 2066 696c 6520 6672 6f6d 2074 6865 2060   file from the `
+00000f90: 7370 6869 6e78 5f61 7069 5f73 6964 6562  sphinx_api_sideb
+00000fa0: 6172 2f74 656d 706c 6174 6573 6020 666f  ar/templates` fo
+00000fb0: 6c64 6572 206f 6620 7468 6520 696e 7374  lder of the inst
+00000fc0: 616c 6c65 6420 7061 636b 6167 6520 746f  alled package to
+00000fd0: 2079 6f75 7220 5370 6869 6e78 2070 726f   your Sphinx pro
+00000fe0: 6a65 6374 2773 205f 7465 6d70 6c61 7465  ject's _template
+00000ff0: 7320 666f 6c64 6572 2e20 416c 7465 726e  s folder. Altern
+00001000: 6174 6976 656c 792c 2079 6f75 2063 616e  atively, you can
+00001010: 2063 7265 6174 6520 6120 6e65 7720 6669   create a new fi
+00001020: 6c65 2069 6e20 796f 7572 2070 726f 6a65  le in your proje
+00001030: 6374 2773 205f 7465 6d70 6c61 7465 7320  ct's _templates 
+00001040: 666f 6c64 6572 2077 6974 6820 7468 6520  folder with the 
+00001050: 666f 6c6c 6f77 696e 6720 636f 6e74 656e  following conten
+00001060: 743a 0a0a 6060 6068 746d 6c0a 7b25 2069  t:..```html.{% i
+00001070: 6620 6170 695f 646f 6373 2025 7d0a 2020  f api_docs %}.  
+00001080: 3c68 333e 7b7b 205f 2827 4150 4920 446f  <h3>{{ _('API Do
+00001090: 6375 6d65 6e74 6174 696f 6e27 2920 7d7d  cumentation') }}
+000010a0: 3c2f 6833 3e0a 2020 3c75 6c20 7374 796c  </h3>.  <ul styl
+000010b0: 653d 226c 6973 742d 7374 796c 652d 7479  e="list-style-ty
+000010c0: 7065 3a20 6e6f 6e65 3b22 3e0a 2020 2020  pe: none;">.    
+000010d0: 7b25 2d20 666f 7220 6974 656d 2069 6e20  {%- for item in 
+000010e0: 6170 695f 646f 6373 2025 7d0a 2020 2020  api_docs %}.    
+000010f0: 2020 3c6c 6920 7374 796c 653d 226d 6172    <li style="mar
+00001100: 6769 6e2d 626f 7474 6f6d 3a20 3130 7078  gin-bottom: 10px
+00001110: 3b22 3e3c 6120 6872 6566 3d22 7b7b 2070  ;"><a href="{{ p
+00001120: 6174 6874 6f28 275f 7374 6174 6963 2f61  athto('_static/a
+00001130: 7069 2d64 6f63 732f 7b7d 272e 666f 726d  pi-docs/{}'.form
+00001140: 6174 2869 7465 6d29 2c20 3129 207d 7d22  at(item), 1) }}"
+00001150: 3e7b 7b20 6974 656d 207d 7d3c 2f61 3e3c  >{{ item }}</a><
+00001160: 2f6c 693e 0a20 2020 207b 252d 2065 6e64  /li>.    {%- end
+00001170: 666f 7220 257d 0a20 203c 2f75 6c3e 0a7b  for %}.  </ul>.{
+00001180: 2520 656e 6469 6620 257d 0a60 6060 0a0a  % endif %}.```..
+00001190: 342e 2055 7064 6174 6520 796f 7572 2060  4. Update your `
+000011a0: 636f 6e66 2e70 7960 2066 696c 6520 746f  conf.py` file to
+000011b0: 2069 6e63 6c75 6465 2074 6865 2060 6170   include the `ap
+000011c0: 695f 646f 6373 5f73 6964 6562 6172 2e68  i_docs_sidebar.h
+000011d0: 746d 6c60 2074 656d 706c 6174 6520 696e  tml` template in
+000011e0: 2074 6865 2068 746d 6c5f 7369 6465 6261   the html_sideba
+000011f0: 7273 2063 6f6e 6669 6775 7261 7469 6f6e  rs configuration
+00001200: 3a0a 0a60 6060 7079 7468 6f6e 0a68 746d  :..```python.htm
+00001210: 6c5f 7369 6465 6261 7273 203d 207b 0a20  l_sidebars = {. 
+00001220: 2020 2027 2a2a 273a 205b 0a20 2020 2020     '**': [.     
+00001230: 2020 2023 202e 2e2e 206f 7468 6572 2073     # ... other s
+00001240: 6964 6562 6172 7320 2e2e 2e0a 2020 2020  idebars ....    
+00001250: 2020 2020 2761 7069 5f64 6f63 735f 7369      'api_docs_si
+00001260: 6465 6261 722e 6874 6d6c 272c 0a20 2020  debar.html',.   
+00001270: 205d 0a7d 0a60 6060 0a                    ].}.```.
```

### Comparing `sphinx-api-sidebar-0.0.1/tests/test_sphinx_api_sidebar.py` & `sphinx_api_sidebar-0.1.0/tests/test_sphinx_api_sidebar.py`

 * *Files identical despite different names*

