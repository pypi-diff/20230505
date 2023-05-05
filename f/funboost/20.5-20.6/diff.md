# Comparing `tmp/funboost-20.5-py3-none-any.whl.zip` & `tmp/funboost-20.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1883926 bytes, number of entries: 218
+Zip file size: 1884051 bytes, number of entries: 218
 -rw-rw-rw-  2.0 fat    21081 b- defN 23-May-05 03:43 funboost/__init__.py
 -rw-rw-rw-  2.0 fat     5910 b- defN 23-Apr-28 02:46 funboost/constant.py
 -rw-rw-rw-  2.0 fat     7100 b- defN 23-Apr-27 08:42 funboost/funboost_config_deafult.py
 -rw-rw-rw-  2.0 fat    14104 b- defN 23-Apr-14 00:56 funboost/helpers.py
 -rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-13 09:47 funboost/set_frame_config.py
 -rw-rw-rw-  2.0 fat     3930 b- defN 22-Sep-17 06:12 funboost/beggar_version_implementation/beggar_redis_consumer.py
 -rw-rw-rw-  2.0 fat      759 b- defN 22-Dec-19 11:45 funboost/concurrent_pool/__init__.py
@@ -208,13 +208,13 @@
 -rw-rw-rw-  2.0 fat      303 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc
 -rw-rw-rw-  2.0 fat      311 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc
 -rw-rw-rw-  2.0 fat      909 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/__init__.py
 -rw-rw-rw-  2.0 fat     2243 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/pycompat.py
 -rw-rw-rw-  2.0 fat    19131 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/tracer.py
 -rw-rw-rw-  2.0 fat     2753 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/utils.py
 -rw-rw-rw-  2.0 fat     3693 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/variables.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-05 08:56 funboost-20.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    25817 b- defN 23-May-05 08:56 funboost-20.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-05 08:56 funboost-20.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 08:56 funboost-20.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    24059 b- defN 23-May-05 08:56 funboost-20.5.dist-info/RECORD
-218 files, 3237751 bytes uncompressed, 1843914 bytes compressed:  43.1%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-05 11:35 funboost-20.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    26267 b- defN 23-May-05 11:35 funboost-20.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-05 11:35 funboost-20.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 11:34 funboost-20.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    24059 b- defN 23-May-05 11:35 funboost-20.6.dist-info/RECORD
+218 files, 3238201 bytes uncompressed, 1844039 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -633,23 +633,23 @@
 
 Filename: funboost/utils/pysnooper_ydf/utils.py
 Comment: 
 
 Filename: funboost/utils/pysnooper_ydf/variables.py
 Comment: 
 
-Filename: funboost-20.5.dist-info/LICENSE
+Filename: funboost-20.6.dist-info/LICENSE
 Comment: 
 
-Filename: funboost-20.5.dist-info/METADATA
+Filename: funboost-20.6.dist-info/METADATA
 Comment: 
 
-Filename: funboost-20.5.dist-info/WHEEL
+Filename: funboost-20.6.dist-info/WHEEL
 Comment: 
 
-Filename: funboost-20.5.dist-info/top_level.txt
+Filename: funboost-20.6.dist-info/top_level.txt
 Comment: 
 
-Filename: funboost-20.5.dist-info/RECORD
+Filename: funboost-20.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `funboost-20.5.dist-info/LICENSE` & `funboost-20.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funboost-20.5.dist-info/METADATA` & `funboost-20.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funboost
-Version: 20.5
+Version: 20.6
 Summary: pip install funboost，python全功能分布式函数调度框架,。支持python所有类型的并发模式和一切知名消息队列中间件，python函数加速器，框架包罗万象，一统编程思维，兼容50% python业务场景，适用范围广。只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大，相见恨晚 
 Home-page: https://github.com/ydf0509/funboost
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -50,26 +50,34 @@
 Requires-Dist: redis2
 Requires-Dist: redis3
 Requires-Dist: redis
 Requires-Dist: nb-log (>=8.5)
 Requires-Dist: rocketmq
 Requires-Dist: zmq
 Requires-Dist: pyzmq
-Requires-Dist: kombu
 Requires-Dist: paho-mqtt
 Requires-Dist: setuptools-rust
 Requires-Dist: fabric2 (==2.6.0)
 Requires-Dist: nats-python
 Requires-Dist: nb-filelock
 Requires-Dist: aiohttp (==3.8.3)
 Requires-Dist: pysnooper
 Requires-Dist: deprecated
 Requires-Dist: cryptography
 Requires-Dist: auto-run-on-remote
 Requires-Dist: frozenlist
+Provides-Extra: others
+Requires-Dist: confluent-kafka (==1.7.0) ; extra == 'others'
+Requires-Dist: kombu ; extra == 'others'
+Requires-Dist: celery ; extra == 'others'
+Requires-Dist: flower ; extra == 'others'
+Requires-Dist: nameko (==2.14.1) ; extra == 'others'
+Requires-Dist: sqlalchemy (==1.3.10) ; extra == 'others'
+Requires-Dist: sqlalchemy-utils (==0.36.1) ; extra == 'others'
+Requires-Dist: pulsar-client (==3.1.0) ; (python_version >= "3.6") and extra == 'others'
 
 
 # 1.分布式函数调度框架简介
 
 <pre style="color: greenyellow;background-color: #0c1119; font-size: medium;">
 pip install funboost ,python全功能分布式函数调度框架,。 支持python所有类型的并发模式和全球一切知名消息队列中间件，
 同时funboost支持celery整个框架作为核心来发布和消费消息，使用funboost的极简api方式来自动化配置和操作celery,
```

## Comparing `funboost-20.5.dist-info/RECORD` & `funboost-20.6.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -207,12 +207,12 @@
 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc,sha256=67Zqz4tjErzQSm9FM9mGaY3uMHYOUj3QYKtPqJQvQpE,303
 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc,sha256=a1ajayGg3JjQz--IC3-6YQHRFStG9etoieY8mXEdJ6Q,311
 funboost/utils/pysnooper_ydf/__init__.py,sha256=ctbQdJpLVZ5g_PPstj7Xaqcl0sMIgvUGwZXtcogYyHA,909
 funboost/utils/pysnooper_ydf/pycompat.py,sha256=ehsCfjsLdwoK0_o5fwYWDo3WeqCVfHW5lxekrEZxq4Y,2243
 funboost/utils/pysnooper_ydf/tracer.py,sha256=DYxYeRFSH1jXy4OTB5KIAgQm2EHRWEOwq3EXJig7Yrk,19131
 funboost/utils/pysnooper_ydf/utils.py,sha256=evSmGi_Oul7vSP47AJ0DLjFwoCYCfunJZ1mWxAkwPZw,2753
 funboost/utils/pysnooper_ydf/variables.py,sha256=QejRDESBA06KG9OH4sBT4J1M55eaU29EIHg8K_igaXo,3693
-funboost-20.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-funboost-20.5.dist-info/METADATA,sha256=sKm7DNRngKJX8aXAdcf-C-JwQUTu9myQzRFgNe6_cOI,25817
-funboost-20.5.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-funboost-20.5.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
-funboost-20.5.dist-info/RECORD,,
+funboost-20.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+funboost-20.6.dist-info/METADATA,sha256=3upqKjbqcwUJ6kZBnPEdR4VNFLNGjtTwmS-sdOYuZAM,26267
+funboost-20.6.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+funboost-20.6.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
+funboost-20.6.dist-info/RECORD,,
```

