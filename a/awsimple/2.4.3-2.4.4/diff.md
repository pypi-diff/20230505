# Comparing `tmp/awsimple-2.4.3-py3-none-any.whl.zip` & `tmp/awsimple-2.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 32813 bytes, number of entries: 18
+Zip file size: 32779 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      871 b- defN 23-Apr-12 19:14 awsimple/__init__.py
--rw-rw-rw-  2.0 fat      323 b- defN 23-May-05 04:49 awsimple/__version__.py
+-rw-rw-rw-  2.0 fat      323 b- defN 23-May-05 05:05 awsimple/__version__.py
 -rw-rw-rw-  2.0 fat     6952 b- defN 23-Apr-12 23:17 awsimple/aws.py
 -rw-rw-rw-  2.0 fat     7137 b- defN 23-Mar-14 23:35 awsimple/cache.py
 -rw-rw-rw-  2.0 fat    35834 b- defN 23-May-05 02:27 awsimple/dynamodb.py
 -rw-rw-rw-  2.0 fat     4619 b- defN 23-Mar-14 23:35 awsimple/dynamodb_miv.py
 -rw-rw-rw-  2.0 fat     4278 b- defN 23-Mar-14 23:10 awsimple/logs.py
 -rw-rw-rw-  2.0 fat      199 b- defN 23-Mar-14 23:10 awsimple/mock.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 23:10 awsimple/py.typed
 -rw-rw-rw-  2.0 fat    23243 b- defN 23-Mar-14 23:35 awsimple/s3.py
 -rw-rw-rw-  2.0 fat     3266 b- defN 23-Mar-14 23:10 awsimple/sns.py
--rw-rw-rw-  2.0 fat    14907 b- defN 23-May-05 04:43 awsimple/sqs.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 04:52 awsimple-2.4.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 04:52 awsimple-2.4.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4815 b- defN 23-May-05 04:52 awsimple-2.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 04:52 awsimple-2.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 04:52 awsimple-2.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1376 b- defN 23-May-05 04:52 awsimple-2.4.3.dist-info/RECORD
-18 files, 110107 bytes uncompressed, 30599 bytes compressed:  72.2%
+-rw-rw-rw-  2.0 fat    14871 b- defN 23-May-05 05:04 awsimple/sqs.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4815 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1376 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/RECORD
+18 files, 110071 bytes uncompressed, 30565 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: awsimple/sns.py
 Comment: 
 
 Filename: awsimple/sqs.py
 Comment: 
 
-Filename: awsimple-2.4.3.dist-info/LICENSE
+Filename: awsimple-2.4.4.dist-info/LICENSE
 Comment: 
 
-Filename: awsimple-2.4.3.dist-info/LICENSE.txt
+Filename: awsimple-2.4.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: awsimple-2.4.3.dist-info/METADATA
+Filename: awsimple-2.4.4.dist-info/METADATA
 Comment: 
 
-Filename: awsimple-2.4.3.dist-info/WHEEL
+Filename: awsimple-2.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: awsimple-2.4.3.dist-info/top_level.txt
+Filename: awsimple-2.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: awsimple-2.4.3.dist-info/RECORD
+Filename: awsimple-2.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awsimple/__version__.py

```diff
@@ -1,8 +1,8 @@
 __application_name__ = "awsimple"
 __title__ = __application_name__
 __author__ = "abel"
-__version__ = "2.4.3"
+__version__ = "2.4.4"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/awsimple"
 __download_url__ = "https://github.com/jamesabel/awsimple"
 __description__ = "Simple AWS API for S3, DynamoDB, SNS, and SQS"
```

## awsimple/sqs.py

```diff
@@ -137,16 +137,17 @@
         assert self.resource is not None
         try:
             self.resource.get_queue_by_name(QueueName=self.queue_name)
             queue_exists = True
         except self.client.exceptions.QueueDoesNotExist:
             queue_exists = False
         except self.client.exceptions.ClientError as e:
-            error_code = e.response["Error"]["Code"]
-            queue_exists = not (error_code == "AWS.SimpleQueueService.NonExistentQueue" or error_code == "400")  # 400 is for mock
+            error_code = e.response["Error"].get("Code")
+            log.info(f"{self.queue_name},{error_code=}")
+            queue_exists = False
         return queue_exists
 
     def calculate_nominal_work_time(self) -> int:
         response_times = []
         for begin, end in self.response_history.values():
             if end is not None:
                 response_times.append(end - begin)
```

## Comparing `awsimple-2.4.3.dist-info/LICENSE` & `awsimple-2.4.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awsimple-2.4.3.dist-info/LICENSE.txt` & `awsimple-2.4.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `awsimple-2.4.3.dist-info/METADATA` & `awsimple-2.4.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsimple
-Version: 2.4.3
+Version: 2.4.4
 Summary: Simple AWS API for S3, DynamoDB, SNS, and SQS
 Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple
 Author: abel
 Author-email: j@abel.co
 License: MIT License
 Project-URL: Documentation, https://awsimple.readthedocs.io/
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awsimple Version: 2.4.3 Summary: Simple AWS API for
+Metadata-Version: 2.1 Name: awsimple Version: 2.4.4 Summary: Simple AWS API for
 S3, DynamoDB, SNS, and SQS Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple Author: abel Author-email:
 j@abel.co License: MIT License Project-URL: Documentation, https://
 awsimple.readthedocs.io/ Keywords: aws,cloud,storage,database,dynamodb,s3
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 LICENSE.txt Requires-Dist: boto3 Requires-Dist: typeguard (<3) Requires-Dist:
 hashy (>=0.1.1) Requires-Dist: dictim Requires-Dist: appdirs Requires-Dist:
```

## Comparing `awsimple-2.4.3.dist-info/RECORD` & `awsimple-2.4.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 awsimple/__init__.py,sha256=HIEMxWrkMoIAC6m_PGv0_OgyJ5vfOhuAVJgRmRbT0eg,871
-awsimple/__version__.py,sha256=zdQ5Woi_pdM-06kykZvsI4yrRPpj0qH96Kvy4U40tEI,323
+awsimple/__version__.py,sha256=6tAW_q6Vbj55Iv7AJtK4m7Vqp-aHcjvuFjENc6R87eQ,323
 awsimple/aws.py,sha256=4RYd-BmzFx02wCNTb4md9Z59M6okhFK5zIP9NpoqXoU,6952
 awsimple/cache.py,sha256=5dYf7bh1Dr_pFbkHck4Ym8zrffctv0ERhGJwieRHQH8,7137
 awsimple/dynamodb.py,sha256=giwvkmxJidMEOYSTaAj2BFERzfPm92vg2lmaOQoDbzo,35834
 awsimple/dynamodb_miv.py,sha256=FcbEn2VbrYxQcgQKqFoWFqVwAkoqJpwZ4Nr5guXgGXM,4619
 awsimple/logs.py,sha256=A2RmTT90pfFTthfENd7GSsEHSIBJXO8ICHPdA7sEsHY,4278
 awsimple/mock.py,sha256=32CNU656uC3PBhjCJ4R-WBTtHbSl6VNVkpN8G8XDvsQ,199
 awsimple/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awsimple/s3.py,sha256=uMEz6NN9hXOfsQNUNJ2YOuKGKlT2xqZ5btJ9zsCHBrY,23243
 awsimple/sns.py,sha256=LjKj-UxPdfRDQfN10jU_ULjnlEqLmHcuqfRIKX9lkZo,3266
-awsimple/sqs.py,sha256=OXh1bUVy8hXOIIUmUZqLGG9-ia02UYLDVRCow7mb7Z8,14907
-awsimple-2.4.3.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.4.3.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.4.3.dist-info/METADATA,sha256=9ob1GeH_KfGgvOebrLDWFuESZKM6iM7lXqMMAiMlN3g,4815
-awsimple-2.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-awsimple-2.4.3.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
-awsimple-2.4.3.dist-info/RECORD,,
+awsimple/sqs.py,sha256=JRGxF4pxLHQtz5bwspjuVe7Py7ITDpAW93-35cwKypA,14871
+awsimple-2.4.4.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.4.4.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.4.4.dist-info/METADATA,sha256=_5KdvdwaWzTSkMtwRN7g0ZWnFf8i3nfxvY2YsO4X684,4815
+awsimple-2.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+awsimple-2.4.4.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
+awsimple-2.4.4.dist-info/RECORD,,
```

