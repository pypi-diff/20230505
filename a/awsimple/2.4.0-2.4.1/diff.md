# Comparing `tmp/awsimple-2.4.0-py3-none-any.whl.zip` & `tmp/awsimple-2.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 32561 bytes, number of entries: 18
+Zip file size: 32570 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      871 b- defN 23-Apr-12 19:14 awsimple/__init__.py
--rw-rw-rw-  2.0 fat      323 b- defN 23-Apr-12 19:14 awsimple/__version__.py
+-rw-rw-rw-  2.0 fat      323 b- defN 23-May-05 02:25 awsimple/__version__.py
 -rw-rw-rw-  2.0 fat     6952 b- defN 23-Apr-12 23:17 awsimple/aws.py
 -rw-rw-rw-  2.0 fat     7137 b- defN 23-Mar-14 23:35 awsimple/cache.py
--rw-rw-rw-  2.0 fat    35771 b- defN 23-Apr-10 06:56 awsimple/dynamodb.py
+-rw-rw-rw-  2.0 fat    35834 b- defN 23-May-05 02:27 awsimple/dynamodb.py
 -rw-rw-rw-  2.0 fat     4619 b- defN 23-Mar-14 23:35 awsimple/dynamodb_miv.py
 -rw-rw-rw-  2.0 fat     4278 b- defN 23-Mar-14 23:10 awsimple/logs.py
 -rw-rw-rw-  2.0 fat      199 b- defN 23-Mar-14 23:10 awsimple/mock.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 23:10 awsimple/py.typed
 -rw-rw-rw-  2.0 fat    23243 b- defN 23-Mar-14 23:35 awsimple/s3.py
 -rw-rw-rw-  2.0 fat     3266 b- defN 23-Mar-14 23:10 awsimple/sns.py
 -rw-rw-rw-  2.0 fat    13260 b- defN 23-Apr-12 23:34 awsimple/sqs.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4815 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1376 b- defN 23-Apr-13 00:13 awsimple-2.4.0.dist-info/RECORD
-18 files, 108397 bytes uncompressed, 30347 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 02:28 awsimple-2.4.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 02:28 awsimple-2.4.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4815 b- defN 23-May-05 02:28 awsimple-2.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 02:28 awsimple-2.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 02:28 awsimple-2.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1376 b- defN 23-May-05 02:28 awsimple-2.4.1.dist-info/RECORD
+18 files, 108460 bytes uncompressed, 30356 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: awsimple/sns.py
 Comment: 
 
 Filename: awsimple/sqs.py
 Comment: 
 
-Filename: awsimple-2.4.0.dist-info/LICENSE
+Filename: awsimple-2.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: awsimple-2.4.0.dist-info/LICENSE.txt
+Filename: awsimple-2.4.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: awsimple-2.4.0.dist-info/METADATA
+Filename: awsimple-2.4.1.dist-info/METADATA
 Comment: 
 
-Filename: awsimple-2.4.0.dist-info/WHEEL
+Filename: awsimple-2.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: awsimple-2.4.0.dist-info/top_level.txt
+Filename: awsimple-2.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: awsimple-2.4.0.dist-info/RECORD
+Filename: awsimple-2.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awsimple/__version__.py

```diff
@@ -1,8 +1,8 @@
 __application_name__ = "awsimple"
 __title__ = __application_name__
 __author__ = "abel"
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/awsimple"
 __download_url__ = "https://github.com/jamesabel/awsimple"
 __description__ = "Simple AWS API for S3, DynamoDB, SNS, and SQS"
```

## awsimple/dynamodb.py

```diff
@@ -451,14 +451,16 @@
                 ts = "B"
             else:
                 raise ValueError(t)
             return ts
 
         created = False
         if not self.table_exists():
+            log.info(f'creating table "{self.table_name}"')
+
             client = self.client
 
             # https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.CoreComponents.html#HowItWorks.CoreComponents.PrimaryKey
 
             partition_definition, partition_schema = add_key(partition_key, type_to_attribute_type(partition_key_type), "HASH")  # required
             attribute_definitions = [partition_definition]
             key_schema = [partition_schema]
```

## Comparing `awsimple-2.4.0.dist-info/LICENSE` & `awsimple-2.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awsimple-2.4.0.dist-info/LICENSE.txt` & `awsimple-2.4.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `awsimple-2.4.0.dist-info/METADATA` & `awsimple-2.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsimple
-Version: 2.4.0
+Version: 2.4.1
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
-Metadata-Version: 2.1 Name: awsimple Version: 2.4.0 Summary: Simple AWS API for
+Metadata-Version: 2.1 Name: awsimple Version: 2.4.1 Summary: Simple AWS API for
 S3, DynamoDB, SNS, and SQS Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple Author: abel Author-email:
 j@abel.co License: MIT License Project-URL: Documentation, https://
 awsimple.readthedocs.io/ Keywords: aws,cloud,storage,database,dynamodb,s3
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 LICENSE.txt Requires-Dist: boto3 Requires-Dist: typeguard (<3) Requires-Dist:
 hashy (>=0.1.1) Requires-Dist: dictim Requires-Dist: appdirs Requires-Dist:
```

## Comparing `awsimple-2.4.0.dist-info/RECORD` & `awsimple-2.4.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 awsimple/__init__.py,sha256=HIEMxWrkMoIAC6m_PGv0_OgyJ5vfOhuAVJgRmRbT0eg,871
-awsimple/__version__.py,sha256=9WJKdgEJMHlcFb4xOsMNQZ8kjtrjx67eHypJb7yexds,323
+awsimple/__version__.py,sha256=Ye286vNj1HCa2JcUEUN7TIFw75tYxKPYsYYj3NfmO9Q,323
 awsimple/aws.py,sha256=4RYd-BmzFx02wCNTb4md9Z59M6okhFK5zIP9NpoqXoU,6952
 awsimple/cache.py,sha256=5dYf7bh1Dr_pFbkHck4Ym8zrffctv0ERhGJwieRHQH8,7137
-awsimple/dynamodb.py,sha256=sogLid9dYOEQ4dLswcsDNvTdo0RqWhJD05k3gQlkBRY,35771
+awsimple/dynamodb.py,sha256=giwvkmxJidMEOYSTaAj2BFERzfPm92vg2lmaOQoDbzo,35834
 awsimple/dynamodb_miv.py,sha256=FcbEn2VbrYxQcgQKqFoWFqVwAkoqJpwZ4Nr5guXgGXM,4619
 awsimple/logs.py,sha256=A2RmTT90pfFTthfENd7GSsEHSIBJXO8ICHPdA7sEsHY,4278
 awsimple/mock.py,sha256=32CNU656uC3PBhjCJ4R-WBTtHbSl6VNVkpN8G8XDvsQ,199
 awsimple/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awsimple/s3.py,sha256=uMEz6NN9hXOfsQNUNJ2YOuKGKlT2xqZ5btJ9zsCHBrY,23243
 awsimple/sns.py,sha256=LjKj-UxPdfRDQfN10jU_ULjnlEqLmHcuqfRIKX9lkZo,3266
 awsimple/sqs.py,sha256=g7vHwXHpypu_0yWVlfYCEApcRBp9J6zKC9XywKJenTU,13260
-awsimple-2.4.0.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.4.0.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.4.0.dist-info/METADATA,sha256=KyNWdX6CeynN5D1UY1JxoTjIpsAzHEe1bXbVrkdJr_I,4815
-awsimple-2.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-awsimple-2.4.0.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
-awsimple-2.4.0.dist-info/RECORD,,
+awsimple-2.4.1.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.4.1.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.4.1.dist-info/METADATA,sha256=oDBgIUryE-89nNfSKhHiLtHUXfvaFb5ZaDK4TujS7k8,4815
+awsimple-2.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+awsimple-2.4.1.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
+awsimple-2.4.1.dist-info/RECORD,,
```

