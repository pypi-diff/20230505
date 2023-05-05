# Comparing `tmp/spine_aws_common-0.2.8.tar.gz` & `tmp/spine_aws_common-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_aws_common-0.2.8.tar", last modified: Wed Nov 16 15:34:45 2022, max compression
+gzip compressed data, was "spine_aws_common-0.2.9.tar", last modified: Thu Dec  1 15:51:40 2022, max compression
```

## Comparing `spine_aws_common-0.2.8.tar` & `spine_aws_common-0.2.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:34:45.737287 spine_aws_common-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-11-16 15:34:45.737287 spine_aws_common-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:34:45.733287 spine_aws_common-0.2.8/mesh_aws_client/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/mesh_aws_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5506 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/mesh_aws_client/mesh_check_send_parameters_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     4228 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/mesh_aws_client/mesh_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    11490 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/mesh_aws_client/mesh_fetch_message_chunk_application.py
--rw-r--r--   0 runner    (1001) docker     (121)    11079 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/mesh_aws_client/mesh_mailbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/mesh_aws_client/mesh_poll_mailbox_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     6680 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/mesh_aws_client/mesh_send_message_chunk_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-11-16 15:34:45.737287 spine_aws_common-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:34:45.737287 spine_aws_common-0.2.8/spine_aws_common/
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/alb_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/api_gateway_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/api_gateway_v2_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/batch_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     4731 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/cloudlogbase.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/cloudwatch_logs_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/dynamodb_streams_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/eventbridge_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/kinesis_stream_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     6009 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/lambda_application.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:34:45.737287 spine_aws_common-0.2.8/spine_aws_common/log/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4925 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/details.py
--rw-r--r--   0 runner    (1001) docker     (121)     3665 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/log_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3616 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/loglineprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4305 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/logutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/masking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5196 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/spinelogging.py
--rw-r--r--   0 runner    (1001) docker     (121)     5510 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/thirdpartylogging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/log/writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9147 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/s3_event_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/s3_object_event_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/ses_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/sns_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/sqs_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-11-16 15:34:03.000000 spine_aws_common-0.2.8/spine_aws_common/web_application.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 15:34:45.737287 spine_aws_common-0.2.8/spine_aws_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-11-16 15:34:45.000000 spine_aws_common-0.2.8/spine_aws_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-11-16 15:34:45.000000 spine_aws_common-0.2.8/spine_aws_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 15:34:45.000000 spine_aws_common-0.2.8/spine_aws_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-16 15:34:45.000000 spine_aws_common-0.2.8/spine_aws_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-16 15:34:45.000000 spine_aws_common-0.2.8/spine_aws_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:51:40.140188 spine_aws_common-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3257 2022-12-01 15:51:40.140188 spine_aws_common-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2737 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:51:40.132188 spine_aws_common-0.2.9/mesh_aws_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/mesh_aws_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5506 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/mesh_aws_client/mesh_check_send_parameters_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4228 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/mesh_aws_client/mesh_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13852 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/mesh_aws_client/mesh_fetch_message_chunk_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11079 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/mesh_aws_client/mesh_mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3127 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/mesh_aws_client/mesh_poll_mailbox_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6680 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/mesh_aws_client/mesh_send_message_chunk_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2022-12-01 15:51:40.140188 spine_aws_common-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:51:40.136188 spine_aws_common-0.2.9/spine_aws_common/
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/alb_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/api_gateway_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/api_gateway_v2_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/batch_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6006 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/cloudlogbase.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/cloudwatch_logs_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/dynamodb_streams_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/eventbridge_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/kinesis_stream_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6009 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/lambda_application.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:51:40.140188 spine_aws_common-0.2.9/spine_aws_common/log/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4925 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3665 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/log_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/loglineprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4305 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/logutil.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3091 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/masking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5196 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/spinelogging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5510 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/thirdpartylogging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/log/writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9147 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/s3_event_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/s3_object_event_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/ses_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/sns_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/sqs_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2701 2022-12-01 15:51:00.000000 spine_aws_common-0.2.9/spine_aws_common/web_application.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:51:40.136188 spine_aws_common-0.2.9/spine_aws_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3257 2022-12-01 15:51:39.000000 spine_aws_common-0.2.9/spine_aws_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1683 2022-12-01 15:51:40.000000 spine_aws_common-0.2.9/spine_aws_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:51:39.000000 spine_aws_common-0.2.9/spine_aws_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2022-12-01 15:51:39.000000 spine_aws_common-0.2.9/spine_aws_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2022-12-01 15:51:39.000000 spine_aws_common-0.2.9/spine_aws_common.egg-info/top_level.txt
```

### Comparing `spine_aws_common-0.2.8/PKG-INFO` & `spine_aws_common-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spine_aws_common
-Version: 0.2.8
+Version: 0.2.9
 Summary: NHS Digital Spine Core common AWS code
 Home-page: https://github.com/NHSDigital/spine-core-aws-common
 Author: NHS Digital
 Author-email: devops.core@nhs.net
 Project-URL: Bug Tracker, https://github.com/NHSDigital/spine-core-aws-common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spine_aws_common-0.2.8/README.md` & `spine_aws_common-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/mesh_aws_client/mesh_check_send_parameters_application.py` & `spine_aws_common-0.2.9/mesh_aws_client/mesh_check_send_parameters_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/mesh_aws_client/mesh_common.py` & `spine_aws_common-0.2.9/mesh_aws_client/mesh_common.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/mesh_aws_client/mesh_fetch_message_chunk_application.py` & `spine_aws_common-0.2.9/mesh_aws_client/mesh_fetch_message_chunk_application.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,42 +32,125 @@
         self.input = {}
         self.environment = os.environ.get("Environment", "default")
         self.chunk_size = os.environ.get("CHUNK_SIZE", MeshCommon.DEFAULT_CHUNK_SIZE)
         self.http_response = None
         self.response = {}
         self.internal_id = None
         self.aws_upload_id = None
-        self.aws_current_part_id = 1
+        self.aws_current_part_id = 0
         self.aws_part_etags = []
         self.chunked = False
-        self.current_chunk = 1
+        self.number_of_chunks = 0
+        self.current_chunk = 0
         self.message_id = None
         self.region = os.environ.get("AWS_REGION", "eu-west-2")
         self.s3_client = None
         self.s3_bucket = ""
-        self.http_headers_bytes_read = None
+        self.http_headers_bytes_read = 0
         self.s3_key = ""
+        self.s3_tempfile_key = None
 
     def initialise(self):
         """decode input event"""
         self.input = self.event.get("body")
         self.internal_id = self.input.get("internal_id", "Not Provided")
-        self.aws_upload_id = self.input.get("aws_upload_id", None)
+        self.aws_upload_id = self.input.get("aws_upload_id", "Not Provided")
         self.aws_current_part_id = self.input.get("aws_current_part_id", 1)
         self.aws_part_etags = self.input.get("aws_part_etags", [])
         self.chunked = self.input.get("chunked")
         self.current_chunk = self.input.get("chunk_num", 1)
         self.message_id = self.input["message_id"]
         self.response = self.event.raw_event
+        self.s3_client = boto3.client("s3", region_name=self.region)
+        self.log_object.internal_id = self.internal_id
+        self._setup_mailbox()
 
     def _setup_mailbox(self):
         self.mailbox = MeshMailbox(
             self.log_object, self.input["dest_mailbox"], self.environment
         )
 
+    def start(self):
+        self.log_object.write_log(
+            "MESHFETCH0001",
+            None,
+            {
+                "message_id": self.message_id,
+            },
+        )
+        # get stream for this chunk
+        self.http_response = self.mailbox.get_chunk(
+            self.message_id, chunk_num=self.current_chunk
+        )
+        self.number_of_chunks = self._get_number_of_chunks()
+        self.http_response.raise_for_status()
+        self.chunked = (
+            self.http_response.status_code == HTTPStatus.PARTIAL_CONTENT.value
+        )
+        self._get_aws_bucket_and_key()
+
+        if self.http_response.headers.get("Mex-Messagetype") == "REPORT":
+            self._handle_report_message()
+        elif self.number_of_chunks == 1:
+            self._handle_single_chunk_message()
+        else:
+            self._handle_multiple_chunk_message()
+
+    def _handle_multiple_chunk_message(self):
+        self.log_object.write_log(
+            "MESHFETCH0013", None, {"message_id": self.message_id}
+        )
+        if self.current_chunk == 1:
+            self._create_multipart_upload()
+        self._read_bytes_into_buffer()
+        self.log_object.write_log(
+            "MESHFETCH0001a",
+            None,
+            {
+                "length": self.http_headers_bytes_read,
+                "message_id": self.message_id,
+            },
+        )
+        last_chunk = self._is_last_chunk(self.current_chunk)
+        if last_chunk:
+            self._finish_multipart_upload()
+            self.mailbox.acknowledge_message(self.message_id)
+            self.log_object.write_log(
+                "MESHFETCH0004", None, {"message_id": self.message_id}
+            )
+        else:
+            self.current_chunk += 1
+            self.log_object.write_log(
+                "MESHFETCH0003",
+                None,
+                {"chunk": self.current_chunk, "message_id": self.message_id},
+            )
+        self._update_response_and_mailbox_cleanup(complete=last_chunk)
+
+    def _handle_single_chunk_message(self):
+        self.log_object.write_log(
+            "MESHFETCH0011", None, {"message_id": self.message_id}
+        )
+        chunk_data = self.http_response.raw.read(decode_content=True)
+        self._upload_to_s3(chunk_data, s3_key=self.s3_key)
+        self.mailbox.acknowledge_message(self.message_id)
+        self._update_response_and_mailbox_cleanup(complete=True)
+        self.log_object.write_log(
+            "MESHFETCH0012", None, {"message_id": self.message_id}
+        )
+
+    def _handle_report_message(self):
+        self.log_object.write_log(
+            "MESHFETCH0010", None, {"message_id": self.message_id}
+        )
+        buffer = json.dumps(dict(self.http_response.headers)).encode("utf-8")
+        self.http_headers_bytes_read = len(buffer)
+        self._upload_to_s3(buffer, s3_key=self.s3_key)
+        self.mailbox.acknowledge_message(self.message_id)
+
     def _get_filename(self):
         file_name = self.http_response.headers.get("Mex-Filename", "")
         if len(file_name) == 0:
             if self.http_response.headers.get("Mex-Messagetype") == "REPORT":
                 file_name = self.message_id + ".ctl"
             else:
                 file_name = self.message_id + ".dat"
@@ -79,67 +162,64 @@
         if len(s3_folder) > 0:
             s3_folder += "/"
         file_name = self._get_filename()
         self.s3_key = s3_folder + (
             file_name if len(file_name) > 0 else self.message_id + ".dat"
         )
 
-    def _is_last_chunk(self, chunk_num):
+    def _is_last_chunk(self, chunk_num) -> bool:
+        chunk_range = self.http_response.headers.get("Mex-Chunk-Range", "1:1")
+        self.number_of_chunks = int(chunk_range.split(":")[1])
+        return chunk_num == self.number_of_chunks
+
+    def _get_number_of_chunks(self) -> int:
         chunk_range = self.http_response.headers.get("Mex-Chunk-Range", "1:1")
         number_of_chunks = int(chunk_range.split(":")[1])
-        last_chunk = chunk_num == number_of_chunks
-        return last_chunk
+        return number_of_chunks
 
-    def _upload_part_to_s3(self, buffer, last_chunk):
+    def _upload_part_to_s3(self, buffer):
         """Upload a part to S3 and check response"""
+        overflow_filename = f"part_overflow_{self.message_id}.tmp"
+        self.s3_tempfile_key = os.path.basename(self.s3_key) + overflow_filename
 
         # check if part_overflow_{message_id}.tmp exists and pre-pend to buffer
-        filename = f"part_overflow_{self.message_id}.tmp"
-        s3_tempfile_key = os.path.basename(self.s3_key) + filename
         try:
             s3_response = self.s3_client.get_object(
-                Bucket=self.s3_bucket, Key=s3_tempfile_key
+                Bucket=self.s3_bucket, Key=self.s3_tempfile_key
             )
             if s3_response["ResponseMetadata"]["HTTPStatusCode"] == HTTPStatus.OK.value:
                 pre_buffer = s3_response["Body"].read()
                 buffer = pre_buffer + buffer
+
                 self.log_object.write_log(
                     "MESHFETCH0002b",
                     None,
                     {
+                        "number_of_chunks": self.number_of_chunks,
                         "aws_part_size": len(pre_buffer),
                         "aws_upload_id": self.aws_upload_id,
                     },
                 )
+
             self.s3_client.delete_object(
                 Bucket=self.s3_bucket,
-                Key=s3_tempfile_key,
+                Key=self.s3_tempfile_key,
                 BypassGovernanceRetention=True,
             )
-        except ClientError:
-            # Not found
-            pass
+        except ClientError as e:
+            self.log_object.write_log(
+                "MESHFETCH0002c",
+                None,
+                {
+                    "client_error": e,
+                    "number_of_chunks": self.number_of_chunks,
+                    "aws_upload_id": self.aws_upload_id,
+                },
+            )
 
-        if not last_chunk:  # not on last chunk
-            if len(buffer) < 5 * self.MEBIBYTE:
-                # write to s3 if buffer is less than 5 MebiBytes and last part of chunk
-                self.s3_client.put_object(
-                    Bucket=self.s3_bucket,
-                    Key=s3_tempfile_key,
-                    Body=buffer,
-                )
-                self.log_object.write_log(
-                    "MESHFETCH0002a",
-                    None,
-                    {
-                        "aws_part_size": len(buffer),
-                        "aws_upload_id": self.aws_upload_id,
-                    },
-                )
-                return None
         try:
             response = self.s3_client.upload_part(
                 Body=buffer,
                 Bucket=self.s3_bucket,
                 Key=self.s3_key,
                 PartNumber=self.aws_current_part_id,
                 ContentLength=len(buffer),
@@ -168,26 +248,52 @@
             }
         )
         self.aws_current_part_id += 1
         self.log_object.write_log(
             "MESHFETCH0002",
             None,
             {
+                "number_of_chunks": self.number_of_chunks,
                 "aws_part_id": self.aws_current_part_id,
                 "aws_part_size": len(buffer),
                 "aws_upload_id": self.aws_upload_id,
                 "etag": etag,
             },
         )
         return etag
 
+    def _upload_to_s3(self, buffer, s3_key):
+        self.s3_client.put_object(
+            Bucket=self.s3_bucket,
+            Key=s3_key,
+            Body=buffer,
+        )
+        self.log_object.write_log(
+            "MESHFETCH0002a",
+            None,
+            {
+                "HEADERS": self.http_response.headers,
+                "RESPONSE": self.http_response,
+                "aws_part_size": len(buffer),
+                "aws_upload_id": self.aws_upload_id,
+            },
+        )
+
     def _create_multipart_upload(self):
         """Create an S3 multipart upload"""
-
         try:
+            self.log_object.write_log(
+                "MESHFETCH0009",
+                None,
+                {
+                    "CHUNKS": self.number_of_chunks,
+                    "key": self.s3_key,
+                    "bucket": self.s3_bucket,
+                },
+            )
             multipart_upload = self.s3_client.create_multipart_upload(
                 Bucket=self.s3_bucket,
                 Key=self.s3_key,
             )
             self.aws_upload_id = multipart_upload["UploadId"]
         except ClientError as e:
             self.response.update({"statusCode": HTTPStatus.INTERNAL_SERVER_ERROR.value})
@@ -201,131 +307,79 @@
                 },
             )
             raise e
 
     def _finish_multipart_upload(self):
         """Complete the s3 multipart upload"""
         try:
+            self.log_object.write_log(
+                "MESHFETCH0008",
+                None,
+                {
+                    "mesh_msg_id": self.message_id,
+                    "key": self.s3_key,
+                    "bucket": self.s3_bucket,
+                    "aws_upload_id": self.aws_upload_id,
+                    "PARTS": {"Parts": self.aws_part_etags},
+                },
+            )
+
             self.s3_client.complete_multipart_upload(
                 Bucket=self.s3_bucket,
                 Key=self.s3_key,
                 UploadId=self.aws_upload_id,
                 MultipartUpload={"Parts": self.aws_part_etags},
             )
 
         except ClientError as e:
             self.response.update({"statusCode": HTTPStatus.INTERNAL_SERVER_ERROR.value})
             self.log_object.write_log(
                 "MESHFETCH0007",
                 None,
                 {
+                    "number_of_chunks": self.number_of_chunks,
                     "mesh_msg_id": self.message_id,
                     "key": self.s3_key,
                     "bucket": self.s3_bucket,
                     "aws_upload_id": self.aws_upload_id,
                     "error": e,
                 },
             )
             raise e
 
-    def start(self):
-        """
-        Main body of lambda function
-        """
-        self.s3_client = boto3.client("s3", region_name=self.region)
-
-        self.log_object.internal_id = self.internal_id
-        self._setup_mailbox()
-
-        self.log_object.write_log(
-            "MESHFETCH0001",
-            None,
-            {
-                "message_id": self.message_id,
-            },
-        )
-
-        # get stream for this chunk
-        self.http_response = self.mailbox.get_chunk(
-            self.message_id, chunk_num=self.current_chunk
-        )
-        self.http_response.raise_for_status()
-        self.chunked = (
-            self.http_response.status_code == HTTPStatus.PARTIAL_CONTENT.value
-        )
-
-        # get s3 bucket and key
-        self._get_aws_bucket_and_key()
-
-        if self.current_chunk == 1:
-            # create multipart upload even if only one chunk
-            self._create_multipart_upload()
-
-        parts_read = 0
-        part_buffer = b""
-        self.http_headers_bytes_read = 0
-
-        is_report = self.http_response.headers.get("Mex-Messagetype") == "REPORT"
-        if is_report:
-            buffer = json.dumps(dict(self.http_response.headers))
-            self._upload_part_to_s3(buffer, True)
-            self.http_headers_bytes_read = len(buffer)
-        else:
-            # read bytes into buffer
-            for buffer in self.http_response.iter_content(
-                chunk_size=self.DEFAULT_BUFFER_SIZE
-            ):
-                parts_read += 1
-                last_chunk = self._is_last_chunk(self.current_chunk)
-                etag = self._upload_part_to_s3(part_buffer + buffer, last_chunk)
-                if etag:
-                    part_buffer = b""
-                else:
-                    part_buffer = buffer
-                    self.http_headers_bytes_read += len(buffer)
-
-        self.log_object.write_log(
-            "MESHFETCH0001a",
-            None,
-            {
-                "length": self.http_headers_bytes_read,
-                "message_id": self.message_id,
-            },
-        )
-
-        is_finished = not self.chunked
-        if is_finished:
-            self._finish_multipart_upload()
-            self.log_object.write_log(
-                "MESHFETCH0004", None, {"message_id": self.message_id}
-            )
-            self.mailbox.acknowledge_message(self.message_id)
-        else:
-            self.log_object.write_log(
-                "MESHFETCH0003",
-                None,
-                {"chunk": self.current_chunk, "message_id": self.message_id},
-            )
-            self.current_chunk += 1
-
-        # update event to send as response
+    def _update_response_and_mailbox_cleanup(self, complete: bool):
         self.response.update({"statusCode": self.http_response.status_code})
         self.response["body"].update(
             {
-                "complete": is_finished,
+                "complete": complete,
                 "chunk_num": self.current_chunk,
                 "aws_upload_id": self.aws_upload_id,
                 "aws_current_part_id": self.aws_current_part_id,
                 "aws_part_etags": self.aws_part_etags,
                 "internal_id": self.internal_id,
                 "file_name": self._get_filename(),
             }
         )
         self.mailbox.clean_up()
 
+    def _read_bytes_into_buffer(self):
+        part_buffer = b""
+        for buffer in self.http_response.iter_content(
+            chunk_size=self.DEFAULT_BUFFER_SIZE
+        ):
+            self.log_object.write_log(
+                "MESHFETCH0003a", None, {"buffer_len": len(buffer)}
+            )
+            # Condition here to account for odd sized chunks
+            if len(buffer) < 5 * self.MEBIBYTE:
+                self._upload_to_s3(buffer, self.s3_tempfile_key)
+            else:
+                self._upload_part_to_s3(part_buffer + buffer)
+                self.http_headers_bytes_read += len(buffer)
+
 
 # create instance of class in global space
 # this ensures initial setup of logging/config is only done on cold start
 app = MeshFetchMessageChunkApplication()
 
 
 def lambda_handler(event, context):
```

### Comparing `spine_aws_common-0.2.8/mesh_aws_client/mesh_mailbox.py` & `spine_aws_common-0.2.9/mesh_aws_client/mesh_mailbox.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/mesh_aws_client/mesh_poll_mailbox_application.py` & `spine_aws_common-0.2.9/mesh_aws_client/mesh_poll_mailbox_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/mesh_aws_client/mesh_send_message_chunk_application.py` & `spine_aws_common-0.2.9/mesh_aws_client/mesh_send_message_chunk_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/__init__.py` & `spine_aws_common-0.2.9/spine_aws_common/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/api_gateway_application.py` & `spine_aws_common-0.2.9/spine_aws_common/api_gateway_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/api_gateway_v2_application.py` & `spine_aws_common-0.2.9/spine_aws_common/api_gateway_v2_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/batch_application.py` & `spine_aws_common-0.2.9/spine_aws_common/batch_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/cloudlogbase.cfg` & `spine_aws_common-0.2.9/spine_aws_common/cloudlogbase.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -116,36 +116,68 @@
 
 [MESHFETCH0001a]
 Log Level = INFO
 Log Text = Downloaded length='{length}' bytes for messageId='{message_id}'
 
 [MESHFETCH0002]
 Log Level = INFO
-Log Text = Persisted aws_part_id='{aws_part_id}' size='{aws_part_size}' for aws_upload_id='{aws_upload_id}' to S3
+Log Text = Persisted aws_part_id='{aws_part_id}' size='{aws_part_size}' for aws_upload_id='{aws_upload_id}' to S3 - Number of chunks='{number_of_chunks}'
 
 [MESHFETCH0002a]
 Log Level = INFO
-Log Text = Part too small to persist size='{aws_part_size}' for aws_upload_id='{aws_upload_id}' to S3
+Log Text = Part too small to persist size='{aws_part_size}' for aws_upload_id='{aws_upload_id}' - uploading to S3 via PutObject
 
 [MESHFETCH0002b]
 Log Level = INFO
-Log Text = Found part file size='{aws_part_size}' for aws_upload_id='{aws_upload_id}' to S3
+Log Text = Found overflow file with size='{aws_part_size}' for aws_upload_id='{aws_upload_id}' to S3 - Number of chunks='{number_of_chunks}'
+
+[MESHFETCH0002c]
+Log Level = INFO
+Log Text = No overflow file found, passing ClientError for aws_upload_id='{aws_upload_id}' number_of_chunks='{number_of_chunks}'
 
 [MESHFETCH0003]
 Log Level = INFO
 Log Text = Downloaded chunk='{chunk}' for messageId='{message_id}'
 
+[MESHFETCH0003a]
+Log Level = INFO
+Log Text = Preparing to upload part to S3 with size='{buffer_len}'
+
 [MESHFETCH0004]
 Log Level = INFO
-Log Text = Download completed and acknowledged for message_id='{message_id}'
+Log Text = Last chunk downloaded, finished multipart upload and message acknowledged for message_id='{message_id}'
 
 [MESHFETCH0005]
 Log Level = CRITICAL
 Log Text = Failed to create multipart upload for key='{key}' to bucket='{bucket}' due to error='{error}'
 
 [MESHFETCH0006]
 Log Level = CRITICAL
 Log Text = Failed to save file from MESH to S3 when upload part with content_length='{content_length}' for key='{key}' to bucket='{bucket}' with aws_upload_id='{aws_upload_id}' due to error='{error}'
 
 [MESHFETCH0007]
 Log Level = CRITICAL
-Log Text = Failed to save file from MESH id='{mesh_msg_id}' to S3 when completing the multipart upload for key='{key}' to bucket='{bucket}' with aws_upload_id='{aws_upload_id}' due to error='{error}'
+Log Text = Failed to save file from MESH id='{mesh_msg_id}' to S3 when completing the multipart upload for key='{key}' to bucket='{bucket}' with aws_upload_id='{aws_upload_id}' due to error='{error}' - NUMBER OF CHUNKS='{number_of_chunks}'
+
+[MESHFETCH0008]
+Log Level = INFO
+Log Text = attempting to save file from MESH id='{mesh_msg_id}' to S3 when completing the multipart upload for key='{key}' to bucket='{bucket}' with aws_upload_id='{aws_upload_id}' with parts='{PARTS}'
+
+[MESHFETCH0009]
+Log Level = INFO
+Log Text = Attempting to create multipart upload for key='{key}' to bucket='{bucket}' - NUMBER OF CHUNKS='{CHUNKS}'
+
+[MESHFETCH0010]
+Log Level = INFO
+Log Text = Report file received message_id='{message_id}'
+
+[MESHFETCH0011]
+Log Level = INFO
+Log Text = File with single chunk received message_id='{message_id}'
+
+[MESHFETCH0012]
+Log Level = INFO
+Log Text = Message with message_id='{message_id}' acknowledged and successfully uploaded to S3
+
+[MESHFETCH0013]
+Log Level = INFO
+Log Text = File with multiple chunks received message_id='{message_id}'
```

### Comparing `spine_aws_common-0.2.8/spine_aws_common/dynamodb_streams_application.py` & `spine_aws_common-0.2.9/spine_aws_common/dynamodb_streams_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/lambda_application.py` & `spine_aws_common-0.2.9/spine_aws_common/lambda_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/constants.py` & `spine_aws_common-0.2.9/spine_aws_common/log/constants.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/details.py` & `spine_aws_common-0.2.9/spine_aws_common/log/details.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/formatting.py` & `spine_aws_common-0.2.9/spine_aws_common/log/formatting.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/log_helper.py` & `spine_aws_common-0.2.9/spine_aws_common/log/log_helper.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/loglineprocessor.py` & `spine_aws_common-0.2.9/spine_aws_common/log/loglineprocessor.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/logutil.py` & `spine_aws_common-0.2.9/spine_aws_common/log/logutil.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/masking.py` & `spine_aws_common-0.2.9/spine_aws_common/log/masking.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/spinelogging.py` & `spine_aws_common-0.2.9/spine_aws_common/log/spinelogging.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/thirdpartylogging.py` & `spine_aws_common-0.2.9/spine_aws_common/log/thirdpartylogging.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/log/writer.py` & `spine_aws_common-0.2.9/spine_aws_common/log/writer.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/logger.py` & `spine_aws_common-0.2.9/spine_aws_common/logger.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/s3_object_event_application.py` & `spine_aws_common-0.2.9/spine_aws_common/s3_object_event_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/sns_application.py` & `spine_aws_common-0.2.9/spine_aws_common/sns_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/sqs_application.py` & `spine_aws_common-0.2.9/spine_aws_common/sqs_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/utilities.py` & `spine_aws_common-0.2.9/spine_aws_common/utilities.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common/web_application.py` & `spine_aws_common-0.2.9/spine_aws_common/web_application.py`

 * *Files identical despite different names*

### Comparing `spine_aws_common-0.2.8/spine_aws_common.egg-info/PKG-INFO` & `spine_aws_common-0.2.9/spine_aws_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spine-aws-common
-Version: 0.2.8
+Version: 0.2.9
 Summary: NHS Digital Spine Core common AWS code
 Home-page: https://github.com/NHSDigital/spine-core-aws-common
 Author: NHS Digital
 Author-email: devops.core@nhs.net
 Project-URL: Bug Tracker, https://github.com/NHSDigital/spine-core-aws-common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spine_aws_common-0.2.8/spine_aws_common.egg-info/SOURCES.txt` & `spine_aws_common-0.2.9/spine_aws_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

