# Comparing `tmp/monopay-0.0.4.tar.gz` & `tmp/monopay-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monopay-0.0.4.tar", max compression
+gzip compressed data, was "monopay-0.0.5.tar", max compression
```

## Comparing `monopay-0.0.4.tar` & `monopay-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1099 2023-05-05 09:56:02.301351 monopay-0.0.4/README.md
--rw-r--r--   0        0        0      350 2023-05-05 09:01:58.594876 monopay-0.0.4/monopay/__init__.py
--rw-r--r--   0        0        0      872 2023-05-05 10:00:07.251026 monopay-0.0.4/monopay/__main__.py
--rw-r--r--   0        0        0      882 2023-05-05 08:27:01.547325 monopay-0.0.4/monopay/asyncmonopay.py
--rw-r--r--   0        0        0       26 2023-05-05 08:44:34.723134 monopay-0.0.4/monopay/decorators/__init__.py
--rw-r--r--   0        0        0      224 2023-05-05 08:50:32.573715 monopay-0.0.4/monopay/decorators/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1698 2023-05-05 08:54:47.552672 monopay-0.0.4/monopay/decorators/__pycache__/decorators.cpython-38.pyc
--rw-r--r--   0        0        0     1526 2023-05-05 09:56:02.693355 monopay-0.0.4/monopay/decorators/decorators.py
--rw-r--r--   0        0        0      163 2023-05-01 23:28:55.360959 monopay-0.0.4/monopay/exceptions/__init__.py
--rw-r--r--   0        0        0      307 2023-05-02 03:50:57.353116 monopay-0.0.4/monopay/exceptions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      443 2023-05-02 03:50:57.353116 monopay-0.0.4/monopay/exceptions/__pycache__/base_exception.cpython-38.pyc
--rw-r--r--   0        0        0      448 2023-05-02 03:50:57.365116 monopay-0.0.4/monopay/exceptions/__pycache__/invalidated_token.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-05-01 23:18:51.526024 monopay-0.0.4/monopay/exceptions/bad_request.py
--rw-r--r--   0        0        0      111 2023-05-02 03:48:57.753736 monopay-0.0.4/monopay/exceptions/base_exception.py
--rw-r--r--   0        0        0      157 2023-05-01 23:28:02.621330 monopay-0.0.4/monopay/exceptions/invalidated_token.py
--rw-r--r--   0        0        0       25 2023-05-02 04:19:44.707064 monopay-0.0.4/monopay/instances/__init__.py
--rw-r--r--   0        0        0      182 2023-05-02 04:26:39.090598 monopay-0.0.4/monopay/instances/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1657 2023-05-02 06:16:41.942151 monopay-0.0.4/monopay/instances/__pycache__/instances.cpython-38.pyc
--rw-r--r--   0        0        0      928 2023-05-02 06:14:02.034741 monopay-0.0.4/monopay/instances/instances.py
--rw-r--r--   0        0        0      106 2023-05-05 06:24:50.221954 monopay-0.0.4/monopay/methods/__init__.py
--rw-r--r--   0        0        0      340 2023-05-05 07:11:36.402630 monopay-0.0.4/monopay/methods/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4287 2023-05-05 02:47:23.823939 monopay-0.0.4/monopay/methods/__pycache__/invoice.cpython-38.pyc
--rw-r--r--   0        0        0     2828 2023-05-05 08:50:32.573715 monopay-0.0.4/monopay/methods/__pycache__/merchant.cpython-38.pyc
--rw-r--r--   0        0        0     2031 2023-05-05 08:53:44.000934 monopay-0.0.4/monopay/methods/__pycache__/qr.cpython-38.pyc
--rw-r--r--   0        0        0     2081 2023-05-05 02:47:24.079938 monopay-0.0.4/monopay/methods/__pycache__/wallet.cpython-38.pyc
--rw-r--r--   0        0        0     5981 2023-05-05 08:56:30.560245 monopay-0.0.4/monopay/methods/invoice.py
--rw-r--r--   0        0        0     2868 2023-05-05 09:56:02.429352 monopay-0.0.4/monopay/methods/merchant.py
--rw-r--r--   0        0        0     1829 2023-05-05 08:53:41.916942 monopay-0.0.4/monopay/methods/qr.py
--rw-r--r--   0        0        0     1985 2023-05-02 07:30:47.349960 monopay-0.0.4/monopay/methods/wallet.py
--rw-r--r--   0        0        0       25 2023-05-02 03:31:07.823707 monopay-0.0.4/monopay/responses/__init__.py
--rw-r--r--   0        0        0      182 2023-05-02 03:50:57.369116 monopay-0.0.4/monopay/responses/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2819 2023-05-05 02:47:24.027938 monopay-0.0.4/monopay/responses/__pycache__/responses.cpython-38.pyc
--rw-r--r--   0        0        0     1464 2023-05-02 07:30:20.798074 monopay-0.0.4/monopay/responses/responses.py
--rw-r--r--   0        0        0      279 2023-05-05 08:42:46.499546 monopay-0.0.4/monopay/utils/__init__.py
--rw-r--r--   0        0        0      404 2023-05-05 08:43:25.335399 monopay-0.0.4/monopay/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      493 2023-05-05 08:43:25.431399 monopay-0.0.4/monopay/utils/__pycache__/builders.cpython-38.pyc
--rw-r--r--   0        0        0      375 2023-05-02 03:52:12.988736 monopay-0.0.4/monopay/utils/__pycache__/is_exception.cpython-38.pyc
--rw-r--r--   0        0        0      441 2023-05-05 08:43:25.431399 monopay-0.0.4/monopay/utils/__pycache__/to_camel_case.cpython-38.pyc
--rw-r--r--   0        0        0      693 2023-05-02 03:50:57.305116 monopay-0.0.4/monopay/utils/__pycache__/webhook_authentication.cpython-38.pyc
--rw-r--r--   0        0        0      265 2023-05-05 09:56:02.553354 monopay-0.0.4/monopay/utils/builders.py
--rw-r--r--   0        0        0      152 2023-05-02 03:51:46.648867 monopay-0.0.4/monopay/utils/is_exception.py
--rw-r--r--   0        0        0      140 2023-05-05 08:40:20.548084 monopay-0.0.4/monopay/utils/to_camel_case.py
--rw-r--r--   0        0        0      505 2023-05-01 23:52:09.567523 monopay-0.0.4/monopay/utils/webhook_authentication.py
--rw-r--r--   0        0        0      402 2023-05-05 10:09:33.620156 monopay-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1664 1970-01-01 00:00:00.000000 monopay-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-05 09:56:02.301351 monopay-0.0.5/README.md
+-rw-r--r--   0        0        0      348 2023-05-05 10:16:09.831888 monopay-0.0.5/monopay/__init__.py
+-rw-r--r--   0        0        0      872 2023-05-05 10:00:07.251026 monopay-0.0.5/monopay/__main__.py
+-rw-r--r--   0        0        0      882 2023-05-05 08:27:01.547325 monopay-0.0.5/monopay/asyncmonopay.py
+-rw-r--r--   0        0        0       26 2023-05-05 08:44:34.723134 monopay-0.0.5/monopay/decorators/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-05 08:50:32.573715 monopay-0.0.5/monopay/decorators/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1698 2023-05-05 08:54:47.552672 monopay-0.0.5/monopay/decorators/__pycache__/decorators.cpython-38.pyc
+-rw-r--r--   0        0        0     1526 2023-05-05 09:56:02.693355 monopay-0.0.5/monopay/decorators/decorators.py
+-rw-r--r--   0        0        0      163 2023-05-01 23:28:55.360959 monopay-0.0.5/monopay/exceptions/__init__.py
+-rw-r--r--   0        0        0      307 2023-05-02 03:50:57.353116 monopay-0.0.5/monopay/exceptions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      443 2023-05-02 03:50:57.353116 monopay-0.0.5/monopay/exceptions/__pycache__/base_exception.cpython-38.pyc
+-rw-r--r--   0        0        0      448 2023-05-02 03:50:57.365116 monopay-0.0.5/monopay/exceptions/__pycache__/invalidated_token.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-05-01 23:18:51.526024 monopay-0.0.5/monopay/exceptions/bad_request.py
+-rw-r--r--   0        0        0      111 2023-05-02 03:48:57.753736 monopay-0.0.5/monopay/exceptions/base_exception.py
+-rw-r--r--   0        0        0      157 2023-05-01 23:28:02.621330 monopay-0.0.5/monopay/exceptions/invalidated_token.py
+-rw-r--r--   0        0        0       25 2023-05-02 04:19:44.707064 monopay-0.0.5/monopay/instances/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-02 04:26:39.090598 monopay-0.0.5/monopay/instances/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1657 2023-05-02 06:16:41.942151 monopay-0.0.5/monopay/instances/__pycache__/instances.cpython-38.pyc
+-rw-r--r--   0        0        0      928 2023-05-02 06:14:02.034741 monopay-0.0.5/monopay/instances/instances.py
+-rw-r--r--   0        0        0      106 2023-05-05 06:24:50.221954 monopay-0.0.5/monopay/methods/__init__.py
+-rw-r--r--   0        0        0      340 2023-05-05 07:11:36.402630 monopay-0.0.5/monopay/methods/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4287 2023-05-05 02:47:23.823939 monopay-0.0.5/monopay/methods/__pycache__/invoice.cpython-38.pyc
+-rw-r--r--   0        0        0     2828 2023-05-05 08:50:32.573715 monopay-0.0.5/monopay/methods/__pycache__/merchant.cpython-38.pyc
+-rw-r--r--   0        0        0     2031 2023-05-05 08:53:44.000934 monopay-0.0.5/monopay/methods/__pycache__/qr.cpython-38.pyc
+-rw-r--r--   0        0        0     2081 2023-05-05 02:47:24.079938 monopay-0.0.5/monopay/methods/__pycache__/wallet.cpython-38.pyc
+-rw-r--r--   0        0        0     5981 2023-05-05 08:56:30.560245 monopay-0.0.5/monopay/methods/invoice.py
+-rw-r--r--   0        0        0     2868 2023-05-05 09:56:02.429352 monopay-0.0.5/monopay/methods/merchant.py
+-rw-r--r--   0        0        0     1829 2023-05-05 08:53:41.916942 monopay-0.0.5/monopay/methods/qr.py
+-rw-r--r--   0        0        0     1985 2023-05-02 07:30:47.349960 monopay-0.0.5/monopay/methods/wallet.py
+-rw-r--r--   0        0        0       25 2023-05-02 03:31:07.823707 monopay-0.0.5/monopay/responses/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-02 03:50:57.369116 monopay-0.0.5/monopay/responses/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2819 2023-05-05 02:47:24.027938 monopay-0.0.5/monopay/responses/__pycache__/responses.cpython-38.pyc
+-rw-r--r--   0        0        0     1464 2023-05-02 07:30:20.798074 monopay-0.0.5/monopay/responses/responses.py
+-rw-r--r--   0        0        0      279 2023-05-05 08:42:46.499546 monopay-0.0.5/monopay/utils/__init__.py
+-rw-r--r--   0        0        0      404 2023-05-05 08:43:25.335399 monopay-0.0.5/monopay/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      493 2023-05-05 08:43:25.431399 monopay-0.0.5/monopay/utils/__pycache__/builders.cpython-38.pyc
+-rw-r--r--   0        0        0      375 2023-05-02 03:52:12.988736 monopay-0.0.5/monopay/utils/__pycache__/is_exception.cpython-38.pyc
+-rw-r--r--   0        0        0      441 2023-05-05 08:43:25.431399 monopay-0.0.5/monopay/utils/__pycache__/to_camel_case.cpython-38.pyc
+-rw-r--r--   0        0        0      693 2023-05-02 03:50:57.305116 monopay-0.0.5/monopay/utils/__pycache__/webhook_authentication.cpython-38.pyc
+-rw-r--r--   0        0        0      265 2023-05-05 09:56:02.553354 monopay-0.0.5/monopay/utils/builders.py
+-rw-r--r--   0        0        0      152 2023-05-02 03:51:46.648867 monopay-0.0.5/monopay/utils/is_exception.py
+-rw-r--r--   0        0        0      140 2023-05-05 08:40:20.548084 monopay-0.0.5/monopay/utils/to_camel_case.py
+-rw-r--r--   0        0        0      505 2023-05-01 23:52:09.567523 monopay-0.0.5/monopay/utils/webhook_authentication.py
+-rw-r--r--   0        0        0      402 2023-05-05 10:16:15.931880 monopay-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1664 1970-01-01 00:00:00.000000 monopay-0.0.5/PKG-INFO
```

### Comparing `monopay-0.0.4/README.md` & `monopay-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/__main__.py` & `monopay-0.0.5/monopay/__main__.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/asyncmonopay.py` & `monopay-0.0.5/monopay/asyncmonopay.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/decorators/__pycache__/decorators.cpython-38.pyc` & `monopay-0.0.5/monopay/decorators/__pycache__/decorators.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/decorators/decorators.py` & `monopay-0.0.5/monopay/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/instances/__pycache__/instances.cpython-38.pyc` & `monopay-0.0.5/monopay/instances/__pycache__/instances.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/instances/instances.py` & `monopay-0.0.5/monopay/instances/instances.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/methods/__pycache__/invoice.cpython-38.pyc` & `monopay-0.0.5/monopay/methods/__pycache__/invoice.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/methods/__pycache__/merchant.cpython-38.pyc` & `monopay-0.0.5/monopay/methods/__pycache__/merchant.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/methods/__pycache__/qr.cpython-38.pyc` & `monopay-0.0.5/monopay/methods/__pycache__/qr.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/methods/__pycache__/wallet.cpython-38.pyc` & `monopay-0.0.5/monopay/methods/__pycache__/wallet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/methods/invoice.py` & `monopay-0.0.5/monopay/methods/invoice.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/methods/merchant.py` & `monopay-0.0.5/monopay/methods/merchant.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/methods/qr.py` & `monopay-0.0.5/monopay/methods/qr.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/methods/wallet.py` & `monopay-0.0.5/monopay/methods/wallet.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/responses/__pycache__/responses.cpython-38.pyc` & `monopay-0.0.5/monopay/responses/__pycache__/responses.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/responses/responses.py` & `monopay-0.0.5/monopay/responses/responses.py`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/monopay/utils/__pycache__/webhook_authentication.cpython-38.pyc` & `monopay-0.0.5/monopay/utils/__pycache__/webhook_authentication.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `monopay-0.0.4/PKG-INFO` & `monopay-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monopay
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Sync/Async library for work with Monobank acquiring api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

