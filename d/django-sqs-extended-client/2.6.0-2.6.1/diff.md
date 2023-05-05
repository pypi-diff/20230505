# Comparing `tmp/django-sqs-extended-client-2.6.0.tar.gz` & `tmp/django-sqs-extended-client-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sqs-extended-client-2.6.0.tar", last modified: Wed Feb  1 13:29:10 2023, max compression
+gzip compressed data, was "django-sqs-extended-client-2.6.1.tar", last modified: Fri May  5 10:38:48 2023, max compression
```

## Comparing `django-sqs-extended-client-2.6.0.tar` & `django-sqs-extended-client-2.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.670329 django-sqs-extended-client-2.6.0/
--rw-r--r--   0 tommy      (501) staff       (20)     1066 2021-01-18 13:45:36.000000 django-sqs-extended-client-2.6.0/LICENSE
--rw-r--r--   0 tommy      (501) staff       (20)       44 2021-01-18 13:33:47.000000 django-sqs-extended-client-2.6.0/MANIFEST.in
--rw-r--r--   0 tommy      (501) staff       (20)     5440 2023-02-01 13:29:10.670385 django-sqs-extended-client-2.6.0/PKG-INFO
--rw-r--r--   0 tommy      (501) staff       (20)     4579 2023-01-26 14:41:34.000000 django-sqs-extended-client-2.6.0/README.rst
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.666569 django-sqs-extended-client-2.6.0/django_sqs_extended_client/
--rw-r--r--   0 tommy      (501) staff       (20)        0 2021-01-18 15:17:37.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/__init__.py
--rw-r--r--   0 tommy      (501) staff       (20)      113 2021-01-18 22:31:03.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/apps.py
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.667605 django-sqs-extended-client-2.6.0/django_sqs_extended_client/aws/
--rw-r--r--   0 tommy      (501) staff       (20)        0 2021-01-16 11:01:40.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/aws/__init__.py
--rw-r--r--   0 tommy      (501) staff       (20)    15230 2023-02-01 13:27:58.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/aws/sns_client_extended.py
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.668719 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event/
--rw-r--r--   0 tommy      (501) staff       (20)        0 2021-01-16 11:01:40.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event/__init__.py
--rw-r--r--   0 tommy      (501) staff       (20)      141 2023-01-26 14:39:14.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event/event_base.py
--rw-r--r--   0 tommy      (501) staff       (20)     1148 2023-02-01 13:28:38.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event/event_base_aws.py
--rw-r--r--   0 tommy      (501) staff       (20)      156 2023-01-26 20:51:31.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event/event_dispatcher.py
--rw-r--r--   0 tommy      (501) staff       (20)      165 2023-01-26 14:40:22.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event/event_dispatcher_fifo.py
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.669075 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event_processor/
--rw-r--r--   0 tommy      (501) staff       (20)        0 2021-01-18 22:56:13.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event_processor/__init__.py
--rw-r--r--   0 tommy      (501) staff       (20)      301 2021-04-20 15:53:41.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/event_processor/event_processor.py
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.669321 django-sqs-extended-client-2.6.0/django_sqs_extended_client/management/
--rw-r--r--   0 tommy      (501) staff       (20)        0 2021-01-18 15:17:37.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/management/__init__.py
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.669797 django-sqs-extended-client-2.6.0/django_sqs_extended_client/management/commands/
--rw-r--r--   0 tommy      (501) staff       (20)        0 2021-01-18 15:17:37.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/management/commands/__init__.py
--rw-r--r--   0 tommy      (501) staff       (20)     1241 2021-04-20 13:01:29.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/management/commands/clean_s3_queues.py
--rw-r--r--   0 tommy      (501) staff       (20)     4216 2023-01-23 11:48:38.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/management/commands/process_queue.py
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.670145 django-sqs-extended-client-2.6.0/django_sqs_extended_client/queue/
--rw-r--r--   0 tommy      (501) staff       (20)        0 2021-01-18 15:17:37.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/queue/__init__.py
--rw-r--r--   0 tommy      (501) staff       (20)      403 2021-01-18 09:38:57.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client/queue/common.py
-drwxr-xr-x   0 tommy      (501) staff       (20)        0 2023-02-01 13:29:10.667380 django-sqs-extended-client-2.6.0/django_sqs_extended_client.egg-info/
--rw-r--r--   0 tommy      (501) staff       (20)     5440 2023-02-01 13:29:10.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client.egg-info/PKG-INFO
--rw-r--r--   0 tommy      (501) staff       (20)     1184 2023-02-01 13:29:10.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client.egg-info/SOURCES.txt
--rw-r--r--   0 tommy      (501) staff       (20)        1 2023-02-01 13:29:10.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client.egg-info/dependency_links.txt
--rw-r--r--   0 tommy      (501) staff       (20)       42 2023-02-01 13:29:10.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client.egg-info/requires.txt
--rw-r--r--   0 tommy      (501) staff       (20)       27 2023-02-01 13:29:10.000000 django-sqs-extended-client-2.6.0/django_sqs_extended_client.egg-info/top_level.txt
--rw-r--r--   0 tommy      (501) staff       (20)       86 2023-01-26 20:30:40.000000 django-sqs-extended-client-2.6.0/requirements.txt
--rw-r--r--   0 tommy      (501) staff       (20)      922 2023-02-01 13:29:10.670660 django-sqs-extended-client-2.6.0/setup.cfg
--rw-r--r--   0 tommy      (501) staff       (20)       37 2021-01-18 13:32:39.000000 django-sqs-extended-client-2.6.0/setup.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.390166 django-sqs-extended-client-2.6.1/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     1066 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/LICENSE
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)       44 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/MANIFEST.in
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     5440 2023-05-05 10:38:48.390166 django-sqs-extended-client-2.6.1/PKG-INFO
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     4579 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/README.rst
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.386165 django-sqs-extended-client-2.6.1/django_sqs_extended_client/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/__init__.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      113 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/apps.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.386165 django-sqs-extended-client-2.6.1/django_sqs_extended_client/aws/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/aws/__init__.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)    15381 2023-05-05 10:32:49.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/aws/sns_client_extended.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.390166 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event/__init__.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      141 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event/event_base.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     1148 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event/event_base_aws.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      156 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event/event_dispatcher.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      165 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event/event_dispatcher_fifo.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.390166 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event_processor/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event_processor/__init__.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      301 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/event_processor/event_processor.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.390166 django-sqs-extended-client-2.6.1/django_sqs_extended_client/management/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/management/__init__.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.390166 django-sqs-extended-client-2.6.1/django_sqs_extended_client/management/commands/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/management/commands/__init__.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     1241 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/management/commands/clean_s3_queues.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     4216 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/management/commands/process_queue.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.390166 django-sqs-extended-client-2.6.1/django_sqs_extended_client/queue/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/queue/__init__.py
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      403 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client/queue/common.py
+drwxrwxr-x   0 bruno     (1000) bruno     (1000)        0 2023-05-05 10:38:48.386165 django-sqs-extended-client-2.6.1/django_sqs_extended_client.egg-info/
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     5440 2023-05-05 10:38:48.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)     1184 2023-05-05 10:38:48.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)        1 2023-05-05 10:38:48.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)       42 2023-05-05 10:38:48.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client.egg-info/requires.txt
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)       27 2023-05-05 10:38:48.000000 django-sqs-extended-client-2.6.1/django_sqs_extended_client.egg-info/top_level.txt
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)       86 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/requirements.txt
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)      922 2023-05-05 10:38:48.390166 django-sqs-extended-client-2.6.1/setup.cfg
+-rw-rw-r--   0 bruno     (1000) bruno     (1000)       37 2023-05-05 10:30:55.000000 django-sqs-extended-client-2.6.1/setup.py
```

### Comparing `django-sqs-extended-client-2.6.0/LICENSE` & `django-sqs-extended-client-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sqs-extended-client-2.6.0/PKG-INFO` & `django-sqs-extended-client-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sqs-extended-client
-Version: 2.6.0
+Version: 2.6.1
 Summary: A Django app to easily use AWS Simple Queue Service (SQS) with S3 for messages up to 2 GB.
 Home-page: https://github.com/tommaso-castellani/django-sqs-extended-client
 Author: Tommaso Castellani
 Author-email: castellani.tom@gmail.com
 License: MIT License
 Classifier: Environment :: Other Environment
 Classifier: Framework :: Django
```

### Comparing `django-sqs-extended-client-2.6.0/README.rst` & `django-sqs-extended-client-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-sqs-extended-client-2.6.0/django_sqs_extended_client/aws/sns_client_extended.py` & `django-sqs-extended-client-2.6.1/django_sqs_extended_client/aws/sns_client_extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,19 @@
 
         Additionally to purging the queue of the message any s3 referenced object will be deleted
         """
         if self.__is_s3_receipt_handle(receipt_handle):
             self.__delete_message_payload_from_s3(receipt_handle, flush_s3)
             receipt_handle = self.__get_orig_receipt_handle(receipt_handle)
         print("receipt_handle={}".format(receipt_handle))
-        self.sqs.delete_message(QueueUrl=queue_url, ReceiptHandle=receipt_handle)
+        try:
+            self.sqs.delete_message(QueueUrl=queue_url, ReceiptHandle=receipt_handle)
+        except Exception:
+            #  silence exception as it happens randomly when AWS deleted it automatically.
+            pass
 
     def send_message(self, topic, message, message_attributes: dict, message_deduplication_id, message_group_id):
         """
         Delivers a message to the specified queue and uploads the message payload
         to Amazon S3 if necessary.
         """
         if message is None:
```

### Comparing `django-sqs-extended-client-2.6.0/django_sqs_extended_client/event/event_base_aws.py` & `django-sqs-extended-client-2.6.1/django_sqs_extended_client/event/event_base_aws.py`

 * *Files identical despite different names*

### Comparing `django-sqs-extended-client-2.6.0/django_sqs_extended_client/management/commands/clean_s3_queues.py` & `django-sqs-extended-client-2.6.1/django_sqs_extended_client/management/commands/clean_s3_queues.py`

 * *Files identical despite different names*

### Comparing `django-sqs-extended-client-2.6.0/django_sqs_extended_client/management/commands/process_queue.py` & `django-sqs-extended-client-2.6.1/django_sqs_extended_client/management/commands/process_queue.py`

 * *Files identical despite different names*

### Comparing `django-sqs-extended-client-2.6.0/django_sqs_extended_client.egg-info/PKG-INFO` & `django-sqs-extended-client-2.6.1/django_sqs_extended_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sqs-extended-client
-Version: 2.6.0
+Version: 2.6.1
 Summary: A Django app to easily use AWS Simple Queue Service (SQS) with S3 for messages up to 2 GB.
 Home-page: https://github.com/tommaso-castellani/django-sqs-extended-client
 Author: Tommaso Castellani
 Author-email: castellani.tom@gmail.com
 License: MIT License
 Classifier: Environment :: Other Environment
 Classifier: Framework :: Django
```

### Comparing `django-sqs-extended-client-2.6.0/django_sqs_extended_client.egg-info/SOURCES.txt` & `django-sqs-extended-client-2.6.1/django_sqs_extended_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sqs-extended-client-2.6.0/setup.cfg` & `django-sqs-extended-client-2.6.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-sqs-extended-client
-version = 2.6.0
+version = 2.6.1
 description = A Django app to easily use AWS Simple Queue Service (SQS) with S3 for messages up to 2 GB.
 long_description = file: README.rst
 url = https://github.com/tommaso-castellani/django-sqs-extended-client
 author = Tommaso Castellani
 author_email = castellani.tom@gmail.com
 license = MIT License
 classifiers =
```

