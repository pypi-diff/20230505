# Comparing `tmp/awsimple-2.4.4-py3-none-any.whl.zip` & `tmp/awsimple-2.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 32779 bytes, number of entries: 18
+Zip file size: 32817 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      871 b- defN 23-Apr-12 19:14 awsimple/__init__.py
--rw-rw-rw-  2.0 fat      323 b- defN 23-May-05 05:05 awsimple/__version__.py
+-rw-rw-rw-  2.0 fat      323 b- defN 23-May-05 15:59 awsimple/__version__.py
 -rw-rw-rw-  2.0 fat     6952 b- defN 23-Apr-12 23:17 awsimple/aws.py
 -rw-rw-rw-  2.0 fat     7137 b- defN 23-Mar-14 23:35 awsimple/cache.py
 -rw-rw-rw-  2.0 fat    35834 b- defN 23-May-05 02:27 awsimple/dynamodb.py
 -rw-rw-rw-  2.0 fat     4619 b- defN 23-Mar-14 23:35 awsimple/dynamodb_miv.py
 -rw-rw-rw-  2.0 fat     4278 b- defN 23-Mar-14 23:10 awsimple/logs.py
 -rw-rw-rw-  2.0 fat      199 b- defN 23-Mar-14 23:10 awsimple/mock.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 23:10 awsimple/py.typed
 -rw-rw-rw-  2.0 fat    23243 b- defN 23-Mar-14 23:35 awsimple/s3.py
 -rw-rw-rw-  2.0 fat     3266 b- defN 23-Mar-14 23:10 awsimple/sns.py
--rw-rw-rw-  2.0 fat    14871 b- defN 23-May-05 05:04 awsimple/sqs.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4815 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1376 b- defN 23-May-05 05:15 awsimple-2.4.4.dist-info/RECORD
-18 files, 110071 bytes uncompressed, 30565 bytes compressed:  72.2%
+-rw-rw-rw-  2.0 fat    15040 b- defN 23-May-05 16:42 awsimple/sqs.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 16:56 awsimple-2.4.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-May-05 16:56 awsimple-2.4.5.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4815 b- defN 23-May-05 16:56 awsimple-2.4.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 16:56 awsimple-2.4.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 16:56 awsimple-2.4.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1376 b- defN 23-May-05 16:56 awsimple-2.4.5.dist-info/RECORD
+18 files, 110240 bytes uncompressed, 30603 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: awsimple/sns.py
 Comment: 
 
 Filename: awsimple/sqs.py
 Comment: 
 
-Filename: awsimple-2.4.4.dist-info/LICENSE
+Filename: awsimple-2.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: awsimple-2.4.4.dist-info/LICENSE.txt
+Filename: awsimple-2.4.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: awsimple-2.4.4.dist-info/METADATA
+Filename: awsimple-2.4.5.dist-info/METADATA
 Comment: 
 
-Filename: awsimple-2.4.4.dist-info/WHEEL
+Filename: awsimple-2.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: awsimple-2.4.4.dist-info/top_level.txt
+Filename: awsimple-2.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: awsimple-2.4.4.dist-info/RECORD
+Filename: awsimple-2.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awsimple/__version__.py

```diff
@@ -1,8 +1,8 @@
 __application_name__ = "awsimple"
 __title__ = __application_name__
 __author__ = "abel"
-__version__ = "2.4.4"
+__version__ = "2.4.5"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/awsimple"
 __download_url__ = "https://github.com/jamesabel/awsimple"
 __description__ = "Simple AWS API for S3, DynamoDB, SNS, and SQS"
```

## awsimple/sqs.py

```diff
@@ -78,22 +78,37 @@
         self.response_history = {}  # type: Dict[Any, Any]
 
         # We write the history out as a file so don't make this too big. We take the median (for the nominal run time) so make this big enough to tolerate a fair number of outliers.
         self.max_history = 20
 
     def _get_queue(self):
         if self.queue is None:
-            queue = self.resource.get_queue_by_name(QueueName=self.queue_name)
-            queue_type = type(queue)
-            queue_type_string = str(queue_type)
-            log.debug(queue_type_string)
-            if "sqs.Queue" in queue_type_string:
-                self.queue = queue
-            else:
-                log.warning(f"could not get Queue {self.queue_name}")
+            try:
+                queue = self.resource.get_queue_by_name(QueueName=self.queue_name)
+            except self.client.exceptions.QueueDoesNotExist as e:
+                log.debug(f"{self.queue_name},{e=}")
+                queue = None
+            except self.client.exceptions.ClientError as e:
+                error_code = e.response["Error"].get("Code")
+                if "NonExistentQueue" in error_code:
+                    log.debug(f"{self.queue_name},{e=},{error_code=}")
+                    queue = None
+                else:
+                    # other errors (e.g. connection errors, etc.)
+                    raise
+
+            if queue is not None:
+                # kludge so when moto mocking we return None if it can't get the queue
+                queue_type = type(queue)
+                queue_type_string = str(queue_type)
+                if "dict" in queue_type_string:
+                    log.warning(f"could not get Queue {self.queue_name}")
+                else:
+                    self.queue = queue
+
         return self.queue
 
     @typechecked()
     def _get_response_history_file_path(self) -> Path:
         """
         get response history file path
 
@@ -114,41 +129,27 @@
         url = response.get("QueueUrl", "")
         return url
 
     def delete_queue(self):
         """
         delete queue
         """
-        queue = self.resource.get_queue_by_name(QueueName=self.queue_name)
-        queue_type = type(queue)
-        queue_type_string = str(queue_type)
-        log.debug(queue_type_string)
-        if "sqs.Queue" in queue_type_string:
-            queue.delete()
-        else:
+        if (queue := self._get_queue()) is None:
             log.warning(f"could not get queue {self.queue_name}")
+        else:
+            queue.delete()
 
     @typechecked()
     def exists(self) -> bool:
         """
         test if SQS queue exists
 
         :return: True if exists
         """
-        assert self.resource is not None
-        try:
-            self.resource.get_queue_by_name(QueueName=self.queue_name)
-            queue_exists = True
-        except self.client.exceptions.QueueDoesNotExist:
-            queue_exists = False
-        except self.client.exceptions.ClientError as e:
-            error_code = e.response["Error"].get("Code")
-            log.info(f"{self.queue_name},{error_code=}")
-            queue_exists = False
-        return queue_exists
+        return self._get_queue() is not None
 
     def calculate_nominal_work_time(self) -> int:
         response_times = []
         for begin, end in self.response_history.values():
             if end is not None:
                 response_times.append(end - begin)
         nominal_work_time = max(statistics.median(response_times), self.minimum_nominal_work_time)  # tolerate in case the measured work is very short
@@ -333,15 +334,18 @@
         else:
             self.client.set_queue_attributes(QueueUrl=queue.url, Attributes={"Policy": policy_string})
 
     def purge(self):
         """
         purge all messages in the queue
         """
-        self.client.purge_queue(QueueUrl=self._get_queue().url)
+        if (queue := self._get_queue()) is None:
+            log.warning(f"could not get queue {self.queue_name}")
+        else:
+            self.client.purge_queue(QueueUrl=queue.url)
 
     def messages_available(self) -> int:
         """
         return number of messages available
         :return: number of messages available
         """
         key = "ApproximateNumberOfMessages"
```

## Comparing `awsimple-2.4.4.dist-info/LICENSE` & `awsimple-2.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awsimple-2.4.4.dist-info/LICENSE.txt` & `awsimple-2.4.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `awsimple-2.4.4.dist-info/METADATA` & `awsimple-2.4.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsimple
-Version: 2.4.4
+Version: 2.4.5
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
-Metadata-Version: 2.1 Name: awsimple Version: 2.4.4 Summary: Simple AWS API for
+Metadata-Version: 2.1 Name: awsimple Version: 2.4.5 Summary: Simple AWS API for
 S3, DynamoDB, SNS, and SQS Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple Author: abel Author-email:
 j@abel.co License: MIT License Project-URL: Documentation, https://
 awsimple.readthedocs.io/ Keywords: aws,cloud,storage,database,dynamodb,s3
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 LICENSE.txt Requires-Dist: boto3 Requires-Dist: typeguard (<3) Requires-Dist:
 hashy (>=0.1.1) Requires-Dist: dictim Requires-Dist: appdirs Requires-Dist:
```

## Comparing `awsimple-2.4.4.dist-info/RECORD` & `awsimple-2.4.5.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 awsimple/__init__.py,sha256=HIEMxWrkMoIAC6m_PGv0_OgyJ5vfOhuAVJgRmRbT0eg,871
-awsimple/__version__.py,sha256=6tAW_q6Vbj55Iv7AJtK4m7Vqp-aHcjvuFjENc6R87eQ,323
+awsimple/__version__.py,sha256=8SGXrMStlNQAdTn0phWqAWb9Q2Hx02Ai1zwTpVicVNk,323
 awsimple/aws.py,sha256=4RYd-BmzFx02wCNTb4md9Z59M6okhFK5zIP9NpoqXoU,6952
 awsimple/cache.py,sha256=5dYf7bh1Dr_pFbkHck4Ym8zrffctv0ERhGJwieRHQH8,7137
 awsimple/dynamodb.py,sha256=giwvkmxJidMEOYSTaAj2BFERzfPm92vg2lmaOQoDbzo,35834
 awsimple/dynamodb_miv.py,sha256=FcbEn2VbrYxQcgQKqFoWFqVwAkoqJpwZ4Nr5guXgGXM,4619
 awsimple/logs.py,sha256=A2RmTT90pfFTthfENd7GSsEHSIBJXO8ICHPdA7sEsHY,4278
 awsimple/mock.py,sha256=32CNU656uC3PBhjCJ4R-WBTtHbSl6VNVkpN8G8XDvsQ,199
 awsimple/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awsimple/s3.py,sha256=uMEz6NN9hXOfsQNUNJ2YOuKGKlT2xqZ5btJ9zsCHBrY,23243
 awsimple/sns.py,sha256=LjKj-UxPdfRDQfN10jU_ULjnlEqLmHcuqfRIKX9lkZo,3266
-awsimple/sqs.py,sha256=JRGxF4pxLHQtz5bwspjuVe7Py7ITDpAW93-35cwKypA,14871
-awsimple-2.4.4.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.4.4.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.4.4.dist-info/METADATA,sha256=_5KdvdwaWzTSkMtwRN7g0ZWnFf8i3nfxvY2YsO4X684,4815
-awsimple-2.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-awsimple-2.4.4.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
-awsimple-2.4.4.dist-info/RECORD,,
+awsimple/sqs.py,sha256=d2228qH_jwNRo8XXXL8Pmng47yx5IwzwRNA-k_jWe-g,15040
+awsimple-2.4.5.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.4.5.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.4.5.dist-info/METADATA,sha256=0dK-Mt0OUkDT8TjKn1slO-Rgt-rByUhtulhAtKYQXfw,4815
+awsimple-2.4.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+awsimple-2.4.5.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
+awsimple-2.4.5.dist-info/RECORD,,
```

