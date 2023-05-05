# Comparing `tmp/ipfs_dict_chain-1.0.5.tar.gz` & `tmp/ipfs_dict_chain-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfs_dict_chain-1.0.5.tar", last modified: Thu May  4 02:16:50 2023, max compression
+gzip compressed data, was "ipfs_dict_chain-1.0.6.tar", last modified: Fri May  5 14:58:40 2023, max compression
```

## Comparing `ipfs_dict_chain-1.0.5.tar` & `ipfs_dict_chain-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 02:16:49.995499 ipfs_dict_chain-1.0.5/
--rw-rw-rw-   0        0        0     1091 2023-04-21 21:22:08.000000 ipfs_dict_chain-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-04 01:15:25.000000 ipfs_dict_chain-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      575 2023-05-04 02:16:49.994967 ipfs_dict_chain-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2392 2023-05-04 02:13:45.000000 ipfs_dict_chain-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 02:16:49.974989 ipfs_dict_chain-1.0.5/ipfs_dict_chain/
--rw-rw-rw-   0        0        0     1774 2023-05-03 22:46:27.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain/CID.py
--rw-rw-rw-   0        0        0     4416 2023-05-03 23:13:55.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain/IPFS.py
--rw-rw-rw-   0        0        0     2409 2023-05-04 02:13:45.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain/IPFSDict.py
--rw-rw-rw-   0        0        0     3474 2023-05-04 01:41:06.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain/IPFSDictChain.py
--rw-rw-rw-   0        0        0        0 2023-05-04 01:46:08.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 02:16:49.984496 ipfs_dict_chain-1.0.5/ipfs_dict_chain.egg-info/
--rw-rw-rw-   0        0        0      575 2023-05-04 02:16:49.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-05-04 02:16:49.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 02:16:49.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-04 02:16:49.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 02:16:49.000000 ipfs_dict_chain-1.0.5/ipfs_dict_chain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 02:16:49.996028 ipfs_dict_chain-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      767 2023-05-04 02:15:37.000000 ipfs_dict_chain-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 02:16:49.992769 ipfs_dict_chain-1.0.5/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 22:39:34.000000 ipfs_dict_chain-1.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-05-04 01:27:56.000000 ipfs_dict_chain-1.0.5/tests/test_CID.py
--rw-rw-rw-   0        0        0     1129 2023-05-04 01:29:17.000000 ipfs_dict_chain-1.0.5/tests/test_IPFS.py
--rw-rw-rw-   0        0        0     1485 2023-05-04 01:44:49.000000 ipfs_dict_chain-1.0.5/tests/test_IPFSDict.py
--rw-rw-rw-   0        0        0     1644 2023-05-04 01:45:04.000000 ipfs_dict_chain-1.0.5/tests/test_IPFSDictChain.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:40.218724 ipfs_dict_chain-1.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-21 21:22:08.000000 ipfs_dict_chain-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-04 01:15:25.000000 ipfs_dict_chain-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      791 2023-05-05 14:58:40.218182 ipfs_dict_chain-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2392 2023-05-04 02:13:45.000000 ipfs_dict_chain-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:40.190779 ipfs_dict_chain-1.0.6/ipfs_dict_chain/
+-rw-rw-rw-   0        0        0     1774 2023-05-03 22:46:27.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain/CID.py
+-rw-rw-rw-   0        0        0     4416 2023-05-03 23:13:55.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain/IPFS.py
+-rw-rw-rw-   0        0        0     3212 2023-05-05 14:41:38.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain/IPFSDict.py
+-rw-rw-rw-   0        0        0     3474 2023-05-04 01:41:06.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain/IPFSDictChain.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 01:46:08.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:40.199442 ipfs_dict_chain-1.0.6/ipfs_dict_chain.egg-info/
+-rw-rw-rw-   0        0        0      791 2023-05-05 14:58:40.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-05-05 14:58:40.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:58:40.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-05 14:58:40.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 14:58:40.000000 ipfs_dict_chain-1.0.6/ipfs_dict_chain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 14:58:40.218724 ipfs_dict_chain-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-05-05 14:55:13.000000 ipfs_dict_chain-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:58:40.216005 ipfs_dict_chain-1.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 22:39:34.000000 ipfs_dict_chain-1.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-05-04 01:27:56.000000 ipfs_dict_chain-1.0.6/tests/test_CID.py
+-rw-rw-rw-   0        0        0     1129 2023-05-04 01:29:17.000000 ipfs_dict_chain-1.0.6/tests/test_IPFS.py
+-rw-rw-rw-   0        0        0     2793 2023-05-05 14:31:39.000000 ipfs_dict_chain-1.0.6/tests/test_IPFSDict.py
+-rw-rw-rw-   0        0        0     1689 2023-05-05 14:36:51.000000 ipfs_dict_chain-1.0.6/tests/test_IPFSDictChain.py
```

### Comparing `ipfs_dict_chain-1.0.5/LICENSE` & `ipfs_dict_chain-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.5/README.md` & `ipfs_dict_chain-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.5/ipfs_dict_chain/CID.py` & `ipfs_dict_chain-1.0.6/ipfs_dict_chain/CID.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.5/ipfs_dict_chain/IPFS.py` & `ipfs_dict_chain-1.0.6/ipfs_dict_chain/IPFS.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.5/ipfs_dict_chain/IPFSDictChain.py` & `ipfs_dict_chain-1.0.6/ipfs_dict_chain/IPFSDictChain.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.5/ipfs_dict_chain.egg-info/PKG-INFO` & `ipfs_dict_chain-1.0.6/ipfs_dict_chain.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Metadata-Version: 2.1
 Name: ipfs-dict-chain
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python package that provides IPFSDict and IPFSDictChain objects, which are dictionary-like data structures that store their state on IPFS and keep track of changes.
 Home-page: https://github.com/ValyrianTech/ipfs_dict_chain
 Author: Wouter Glorieux
 Author-email: info@valyrian.tech
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
```

### Comparing `ipfs_dict_chain-1.0.5/setup.py` & `ipfs_dict_chain-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name='ipfs_dict_chain',
-    version='1.0.5',
+    version='1.0.6',
     description='A Python package that provides IPFSDict and IPFSDictChain objects, which are dictionary-like data structures that store their state on IPFS and keep track of changes.',
     author='Wouter Glorieux',
     author_email='info@valyrian.tech',
     url='https://github.com/ValyrianTech/ipfs_dict_chain',
     packages=['ipfs_dict_chain'],
     install_requires=[
         'aioipfs>=0.6.3',
         'multiaddr>=0.0.9',
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
 )
```

### Comparing `ipfs_dict_chain-1.0.5/tests/test_CID.py` & `ipfs_dict_chain-1.0.6/tests/test_CID.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.5/tests/test_IPFS.py` & `ipfs_dict_chain-1.0.6/tests/test_IPFS.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.5/tests/test_IPFSDictChain.py` & `ipfs_dict_chain-1.0.6/tests/test_IPFSDictChain.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def test_changes(self):
         ipfs_dict_chain = IPFSDictChain()
         ipfs_dict_chain['key'] = 'value'
         ipfs_dict_chain.save()
         ipfs_dict_chain['key'] = 'new_value'
         ipfs_dict_chain.save()
         changes = ipfs_dict_chain.changes()
-        self.assertEqual(changes, {'previous_cid': {'old': None, 'new': 'QmQDvMjHHichd3EERWyzmRFdEe2m3ZoKq6HgFynSn9UW1C'}})
+        self.assertEqual(changes, {'previous_cid': {'old': None, 'new': 'QmNqXUYiiNMFXKy5rYFfs1tFASH6kgMA4fA1JwRoGuam8D'}, 'key': {'old': 'value', 'new': 'new_value'}})
 
     def test_get_previous_states(self):
         ipfs_dict_chain = IPFSDictChain()
         ipfs_dict_chain['key'] = 'value'
         ipfs_dict_chain.save()
         dict1 = dict(ipfs_dict_chain.items())
         ipfs_dict_chain['key'] = 'new_value'
```

