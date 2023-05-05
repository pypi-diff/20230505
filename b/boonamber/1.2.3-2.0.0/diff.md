# Comparing `tmp/boonamber-1.2.3.tar.gz` & `tmp/boonamber-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boonamber-1.2.3.tar", last modified: Tue Jan 24 16:21:02 2023, max compression
+gzip compressed data, was "boonamber-2.0.0.tar", last modified: Fri May  5 14:55:54 2023, max compression
```

## Comparing `boonamber-1.2.3.tar` & `boonamber-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,90 @@
-drwxr-xr-x   0 ieshalatty   (501) staff       (20)        0 2023-01-24 16:21:02.819454 boonamber-1.2.3/
--rw-r--r--   0 ieshalatty   (501) staff       (20)     1072 2022-12-12 18:47:41.000000 boonamber-1.2.3/LICENSE
--rw-r--r--   0 ieshalatty   (501) staff       (20)     3891 2023-01-24 16:21:02.819589 boonamber-1.2.3/PKG-INFO
--rw-r--r--   0 ieshalatty   (501) staff       (20)     3380 2022-12-12 18:47:41.000000 boonamber-1.2.3/README.md
-drwxr-xr-x   0 ieshalatty   (501) staff       (20)        0 2023-01-24 16:21:02.812766 boonamber-1.2.3/boonamber/
--rw-r--r--   0 ieshalatty   (501) staff       (20)    49497 2023-01-20 21:02:24.000000 boonamber-1.2.3/boonamber/__init__.py
-drwxr-xr-x   0 ieshalatty   (501) staff       (20)        0 2023-01-24 16:21:02.817366 boonamber-1.2.3/boonamber.egg-info/
--rw-r--r--   0 ieshalatty   (501) staff       (20)     3891 2023-01-24 16:21:02.000000 boonamber-1.2.3/boonamber.egg-info/PKG-INFO
--rw-r--r--   0 ieshalatty   (501) staff       (20)      280 2023-01-24 16:21:02.000000 boonamber-1.2.3/boonamber.egg-info/SOURCES.txt
--rw-r--r--   0 ieshalatty   (501) staff       (20)        1 2023-01-24 16:21:02.000000 boonamber-1.2.3/boonamber.egg-info/dependency_links.txt
--rw-r--r--   0 ieshalatty   (501) staff       (20)       15 2023-01-24 16:21:02.000000 boonamber-1.2.3/boonamber.egg-info/requires.txt
--rw-r--r--   0 ieshalatty   (501) staff       (20)       10 2023-01-24 16:21:02.000000 boonamber-1.2.3/boonamber.egg-info/top_level.txt
--rw-r--r--   0 ieshalatty   (501) staff       (20)      683 2023-01-24 16:20:39.000000 boonamber-1.2.3/pyproject.toml
--rw-r--r--   0 ieshalatty   (501) staff       (20)       89 2023-01-24 16:21:02.820741 boonamber-1.2.3/setup.cfg
--rw-r--r--   0 ieshalatty   (501) staff       (20)      685 2023-01-23 15:23:24.000000 boonamber-1.2.3/setup.py
-drwxr-xr-x   0 ieshalatty   (501) staff       (20)        0 2023-01-24 16:21:02.818920 boonamber-1.2.3/test/
--rw-r--r--   0 ieshalatty   (501) staff       (20)    29640 2023-01-18 21:04:36.000000 boonamber-1.2.3/test/test_client.py
--rw-r--r--   0 ieshalatty   (501) staff       (20)     4427 2022-12-12 18:47:41.000000 boonamber-1.2.3/test/test_streaming.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-05 14:55:54.623480 boonamber-2.0.0/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     1072 2023-05-05 14:50:26.000000 boonamber-2.0.0/LICENSE
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      903 2023-05-05 14:55:54.623320 boonamber-2.0.0/PKG-INFO
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      449 2023-05-05 14:50:26.000000 boonamber-2.0.0/README.md
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-05 14:55:54.609876 boonamber-2.0.0/boonamber/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2124 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/__init__.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-05 14:55:54.610827 boonamber-2.0.0/boonamber/util/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      402 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/util/ambererror.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-05 14:55:54.610982 boonamber-2.0.0/boonamber/v1/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    48321 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v1/__init__.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-05 14:55:54.613231 boonamber-2.0.0/boonamber/v2/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4450 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    23030 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/amber_client.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-05 14:55:54.613657 boonamber-2.0.0/boonamber/v2/api/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      139 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/api/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    92075 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/api/default_api.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    24975 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/api_client.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8168 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/configuration.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-05 14:55:54.623138 boonamber-2.0.0/boonamber/v2/models/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4250 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2477 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/amber_state.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    11774 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/analytic_results.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3659 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/autotuning.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6030 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2663 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/delete_model_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3480 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/error.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8715 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/feature_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3880 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/feature_config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3986 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/feature_root_cause.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3681 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/fusion_feature.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3046 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/get_models_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2712 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/get_nano_status_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2736 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/get_pretrain_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3220 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/get_root_cause_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2704 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/get_status_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    31255 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/get_summary_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8967 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/get_version_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9710 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_amber_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9591 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_autotune.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6488 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_buffer_stats.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6625 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_nano.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7210 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_nano_backend.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7188 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_nano_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3108 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_pattern_memory.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_recent_ams.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3852 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_recent_analytics.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3816 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_recent_floats.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_recent_ids.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3846 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_recent_samples.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3804 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_recent_times.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9886 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_streaming_parameters.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6575 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/m_training.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2326 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/magic_number.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7172 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/map.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6827 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/mncp.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4792 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/model.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9003 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/model_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    10035 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/nano_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2346 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/percent_variation.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6232 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_config_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2732 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4149 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_data_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3646 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_data_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3032 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_learning_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3671 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_learning_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3147 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_model_copy_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3131 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_model_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2655 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_model_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4048 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_oauth2_access_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     5888 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_oauth2_access_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3326 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_oauth2_refresh_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     5908 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_oauth2_refresh_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4959 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_pretrain_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4189 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/post_pretrain_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4077 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/pretrain_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4525 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/put_data_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4330 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/put_data_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3045 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/put_model_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2342 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/streaming_window.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8682 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/training_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2334 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/models/version_number.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    12835 2023-05-05 14:50:26.000000 boonamber-2.0.0/boonamber/v2/rest.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-05 14:55:54.610698 boonamber-2.0.0/boonamber.egg-info/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      903 2023-05-05 14:55:54.000000 boonamber-2.0.0/boonamber.egg-info/PKG-INFO
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2962 2023-05-05 14:55:54.000000 boonamber-2.0.0/boonamber.egg-info/SOURCES.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)        1 2023-05-05 14:55:54.000000 boonamber-2.0.0/boonamber.egg-info/dependency_links.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       15 2023-05-05 14:55:54.000000 boonamber-2.0.0/boonamber.egg-info/requires.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       10 2023-05-05 14:55:54.000000 boonamber-2.0.0/boonamber.egg-info/top_level.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      835 2023-05-05 14:54:16.000000 boonamber-2.0.0/pyproject.toml
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       38 2023-05-05 14:55:54.623525 boonamber-2.0.0/setup.cfg
```

### Comparing `boonamber-1.2.3/LICENSE` & `boonamber-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boonamber-1.2.3/boonamber/__init__.py` & `boonamber-2.0.0/boonamber/v1/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,37 @@
 import base64
 import itertools
 import numpy as np
 import json
 import gzip
 import os
-import sys
 import time
 import requests
 import urllib3
 from collections.abc import Iterable
 from numbers import Number, Integral
+from ..util.ambererror import AmberCloudError, AmberUserError
 
 from urllib3.exceptions import InsecureRequestWarning
 
 
 ############################
 # Boon Amber Python SDK v1 #
 ############################
 
 
-class AmberUserError(Exception):
-    """Raised to indicate an error in SDK usage"""
-
-    def __init__(self, message):
-        self.message = message
-
-
-class AmberCloudError(Exception):
-    """Raised upon any non-200 response from the Amber cloud"""
-
-    def __init__(self, code, message):
-        self.code = code
-        self.message = message
-        super().__init__("{}: {}".format(code, message))
-
-
 class AmberClient:
-
-    def __init__(self, license_id='default', license_file="~/.Amber.license", verify=True, cert=None, timeout=300):
+    def __init__(
+        self,
+        license_id="default",
+        license_file="~/.Amber.license",
+        verify=True,
+        cert=None,
+        timeout=300,
+    ):
         """Main client which interfaces with the Amber cloud. Amber account
         credentials are discovered within a .Amber.license file located in the
         home directory, or optionally overridden using environment variables.
 
         Args:
             license_id (str): license identifier label found within .Amber.license file
             license_file (str): path to .Amber.license file
@@ -68,235 +58,232 @@
 
         Raises:
             AmberUserError: if error supplying authentication credentials
         """
 
         self.token = None
         self.reauth_time = 0
-        self.user_agent = 'Boon Logic / amber-python-sdk / requests'
+        self.user_agent = "Boon Logic / amber-python-sdk / requests"
         self.timeout = timeout
 
         # first load from license file, override from environment if specified
         self.license_file = license_file
-        self.license_file = os.environ.get('AMBER_LICENSE_FILE', self.license_file)
+        self.license_file = os.environ.get("AMBER_LICENSE_FILE", self.license_file)
 
         # determine which license_id to use, override from environment if specified
-        self.license_id = os.environ.get('AMBER_LICENSE_ID', license_id)
+        self.license_id = os.environ.get("AMBER_LICENSE_ID", license_id)
 
+        # TODO allow non existant license file and license id only if username/password/server are set in environ
         # create license profile
         if self.license_file is not None:
             license_path = os.path.expanduser(self.license_file)
             if not os.path.exists(license_path):
                 self.license_profile = json.loads('{"username": "", "password": "", "server": "", "oauth-server": ""}')
             else:
                 try:
-                    with open(license_path, 'r') as f:
+                    with open(license_path, "r") as f:
                         file_data = json.load(f)
                 except json.JSONDecodeError as e:
-                    raise AmberUserError(
-                        "JSON formatting error in license file: {}, line: {}, col: {}".format(e.msg, e.lineno, e.colno))
+                    raise AmberUserError("JSON formatting error in license file: {}, line: {}, col: {}".format(e.msg, e.lineno, e.colno))
                 try:
                     self.license_profile = file_data[self.license_id]
                 except KeyError:
-                    raise AmberUserError("license_id \"{}\" not found in license file".format(self.license_id))
+                    raise AmberUserError('license_id "{}" not found in license file'.format(self.license_id))
         else:
             # no license file found, create a stub profile to be filled in from environment
             self.license_profile = json.loads('{"username": "", "password": "", "server": "", "oauth-server": ""}')
 
         # override from environment if specified
         try:
-            self.license_profile['username'] = os.environ.get('AMBER_USERNAME', self.license_profile['username'])
-            self.license_profile['password'] = os.environ.get('AMBER_PASSWORD', self.license_profile['password'])
-            self.license_profile['server'] = os.environ.get('AMBER_SERVER', self.license_profile['server'])
-            if 'oauth-server' not in self.license_profile or not self.license_profile:
-                self.license_profile['oauth-server'] = self.license_profile['server']
-            self.license_profile['oauth-server'] = os.environ.get('AMBER_OAUTH_SERVER',
-                                                                  self.license_profile['oauth-server'])
-            if self.license_profile['oauth-server'] == "":
-                self.license_profile['oauth-server'] = self.license_profile['server']
-            self.license_profile['cert'] = os.environ.get('AMBER_SSL_CERT', cert)
-            verify_str = os.environ.get('AMBER_SSL_VERIFY', "true").lower()
-            self.license_profile['verify'] = True  # Default
+            self.license_profile["username"] = os.environ.get("AMBER_USERNAME", self.license_profile["username"])
+            self.license_profile["password"] = os.environ.get("AMBER_PASSWORD", self.license_profile["password"])
+            self.license_profile["server"] = os.environ.get("AMBER_SERVER", self.license_profile["server"])
+            if "oauth-server" not in self.license_profile or not self.license_profile:
+                self.license_profile["oauth-server"] = self.license_profile["server"]
+            self.license_profile["oauth-server"] = os.environ.get("AMBER_OAUTH_SERVER", self.license_profile["oauth-server"])
+            if self.license_profile["oauth-server"] == "":
+                self.license_profile["oauth-server"] = self.license_profile["server"]
+            self.license_profile["cert"] = os.environ.get("AMBER_SSL_CERT", cert)
+            verify_str = os.environ.get("AMBER_SSL_VERIFY", "true").lower()
+            self.license_profile["verify"] = True  # Default
             if not verify or verify_str == "false":
-                self.license_profile['verify'] = False
+                self.license_profile["verify"] = False
         except KeyError as e:
             raise AmberUserError("missing field")
 
-        if self.license_profile['verify'] is False:
+        if self.license_profile["verify"] is False:
             urllib3.disable_warnings(category=InsecureRequestWarning)
 
         # verify required profile elements have been created
-        if self.license_profile['username'] == "":
-            raise AmberUserError("username \"{}\" not specified".format(self.license_profile['username']))
-        if self.license_profile['password'] == "":
-            raise AmberUserError("password \"{}\" not specified".format(self.license_profile['password']))
-        if self.license_profile['server'] == "":
-            raise AmberUserError("server \"{}\" not specified".format(self.license_profile['server']))
+        if self.license_profile["username"] == "":
+            raise AmberUserError('username "{}" not specified'.format(self.license_profile["username"]))
+        if self.license_profile["password"] == "":
+            raise AmberUserError('password "{}" not specified'.format(self.license_profile["password"]))
+        if self.license_profile["server"] == "":
+            raise AmberUserError('server "{}" not specified'.format(self.license_profile["server"]))
 
     def _authenticate(self):
         """Authenticate client for the next hour using the credentials given at
         initialization. This acquires and stores an oauth2 token which remains
         valid for one hour and is used to authenticate all other API requests.
 
         Raises:
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['oauth-server'] + '/oauth2'
-        headers = {
-            'Content-Type': 'application/json',
-            'User-Agent': self.user_agent
-        }
+        url = self.license_profile["oauth-server"] + "/oauth2"
+        headers = {"Content-Type": "application/json", "User-Agent": self.user_agent}
         body = {
-            'username': self.license_profile['username'],
-            'password': self.license_profile['password']
+            "username": self.license_profile["username"],
+            "password": self.license_profile["password"],
         }
 
         try:
-            response = requests.request(method='POST', url=url, headers=headers, json=body,
-                                        verify=self.license_profile['verify'],
-                                        cert=self.license_profile['cert'],
-                                        timeout=self.timeout)
+            response = requests.request(
+                method="POST",
+                url=url,
+                headers=headers,
+                json=body,
+                verify=self.license_profile["verify"],
+                cert=self.license_profile["cert"],
+                timeout=self.timeout,
+            )
 
             if response.status_code != 200:
-                message = "authentication failed: {}".format(response.json().get('message', 'no message'))
+                message = "authentication failed: {}".format(response.json().get("message", "no message"))
                 raise AmberCloudError(response.status_code, message)
 
             # invalid credentials return a 200 where token is an empty string
-            self.token = response.json().get('idToken')
+            self.token = response.json().get("idToken")
             if self.token is None:
                 raise AmberCloudError(401, "authentication failed: invalid credentials")
 
-            expire_secs = int(response.json().get('expiresIn'))
+            expire_secs = int(response.json().get("expiresIn"))
             if expire_secs is None:
                 raise AmberCloudError(401, "authentication failed: missing expiration")
             self.reauth_time = time.time() + expire_secs - 60
 
         except requests.exceptions.Timeout:
             raise AmberCloudError(500, "request timed out")
         except Exception:
-            raise AmberCloudError(401, 'invalid server connection')
+            raise AmberCloudError(401, "invalid server connection")
 
     def _api_call(self, method, url, headers, body=None):
         """Make a REST call to the Amber server and handle the response"""
 
         if time.time() > self.reauth_time:
             self._authenticate()
 
-        headers['Authorization'] = 'Bearer {}'.format(self.token)
-        headers['User-Agent'] = self.user_agent
-        headers['Content-Type'] = 'application/json'
-
-        impersonate = os.environ.get('AMBER_IMPERSONATE', '')
-        if impersonate != '':
-            headers['impersonate'] = impersonate
+        headers["Authorization"] = "Bearer {}".format(self.token)
+        headers["User-Agent"] = self.user_agent
+        headers["Content-Type"] = "application/json"
+
+        impersonate = os.environ.get("AMBER_IMPERSONATE", "")
+        if impersonate != "":
+            headers["impersonate"] = impersonate
 
         body = json.dumps(body)
 
-        if method == 'POST' and len(body) > 10000:
-            headers['content-encoding'] = 'gzip'
-            body = gzip.compress(body.encode('utf-8'))
+        if method == "POST" and len(body) > 10000:
+            headers["content-encoding"] = "gzip"
+            body = gzip.compress(body.encode("utf-8"))
 
         try:
-            response = requests.request(method=method, url=url, headers=headers, data=body,
-                                        verify=self.license_profile['verify'],
-                                        cert=self.license_profile['cert'],
-                                        timeout=self.timeout)
+            response = requests.request(
+                method=method,
+                url=url,
+                headers=headers,
+                data=body,
+                verify=self.license_profile["verify"],
+                cert=self.license_profile["cert"],
+                timeout=self.timeout,
+            )
         except requests.exceptions.Timeout:
             # request timed out
             raise AmberCloudError(500, "request timed out")
         except requests.exceptions.ConnectionError:
             raise AmberCloudError(500, "server does not exist")
 
         if response.status_code > 299:
             try:
                 msg = response.json()
                 try:
-                    msg = msg.get('message', 'no message')
+                    msg = msg.get("message", "no message")
                 except AttributeError:
                     pass
             except json.JSONDecodeError:
                 msg = response.text
             raise AmberCloudError(response.status_code, msg)
 
         try:
             respbody = response.json()
         except json.JSONDecodeError:
             msg = response.text
             raise AmberCloudError(response.status_code, f"could not decode response as JSON: '{msg}'")
 
         # if code is returned in the message, it should agree with the header
-        if 'code' in respbody and respbody['code'] != response.status_code:
-            raise AmberCloudError(respbody['code'], respbody.get('message', 'no message'))
+        if "code" in respbody and respbody["code"] != response.status_code:
+            raise AmberCloudError(respbody["code"], respbody.get("message", "no message"))
 
-        if 'errorMessage' in respbody:
-            raise AmberCloudError(500, respbody['errorMessage'])
+        if "errorMessage" in respbody:
+            raise AmberCloudError(500, respbody["errorMessage"])
 
         return response
 
     def get_summary(self, sensor_id):
         """Get summary information for a sensor
 
         Returns:
             json summary information
 
         Raises:
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/__summary'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        response = self._api_call('GET', url, headers)
+        url = self.license_profile["server"] + "/__summary"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        response = self._api_call("GET", url, headers)
 
         return response.json()
 
     def get_version(self):
         """Get version information for Amber
 
         Returns:
             json version information
 
         Raises:
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/version'
-        headers = {
-            'Content-Type': 'application/json'
-        }
-        response = self._api_call('GET', url, headers)
+        url = self.license_profile["server"] + "/version"
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
 
         return response.json()
 
-    def create_sensor(self, label=''):
+    def create_sensor(self, label=""):
         """Create a new sensor instance
 
         Args:
             label (str): label to assign to created sensor
 
         Returns:
             A string containing the `sensor_id` that was created
 
         Raises:
             AmberUserError: if client is not authenticated
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/sensor'
-        headers = {
-            'Content-Type': 'application/json'
-        }
-        body = {
-            'label': label
-        }
-        response = self._api_call('POST', url, headers, body=body)
-        sensor_id = response.json()['sensorId']
+        url = self.license_profile["server"] + "/sensor"
+        headers = {"Content-Type": "application/json"}
+        body = {"label": label}
+        response = self._api_call("POST", url, headers, body=body)
+        sensor_id = response.json()["sensorId"]
 
         return sensor_id
 
     def update_label(self, sensor_id, label):
         """Update the label of a sensor instance
 
         Args:
@@ -307,85 +294,76 @@
             A string containing the new label assigned to sensor
 
         Raises:
             AmberUserError: if client is not authenticated
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/sensor'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        body = {
-            'label': label
-        }
-        response = self._api_call('PUT', url, headers, body=body)
-        label = response.json()['label']
+        url = self.license_profile["server"] + "/sensor"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        body = {"label": label}
+        response = self._api_call("PUT", url, headers, body=body)
+        label = response.json()["label"]
 
         return label
 
     def delete_sensor(self, sensor_id):
         """Delete an amber sensor instance
 
         Args:
             sensor_id (str): sensor identifier
 
         Raises:
             AmberUserError: if client is not authenticated
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/sensor'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        response = self._api_call('DELETE', url, headers)
+        url = self.license_profile["server"] + "/sensor"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        response = self._api_call("DELETE", url, headers)
         return response.json()
 
     def list_sensors(self):
         """List all sensor instances currently associated with Amber account
 
         Returns:
             A dictionary mapping sensor IDs to corresponding labels
 
         Raises:
             AmberUserError: if client is not authenticated
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/sensors'
-        headers = {
-            'Content-Type': 'application/json'
-        }
-        response = self._api_call('GET', url, headers)
-        sensors = {s['sensorId']: s.get('label', None) for s in response.json()}
+        url = self.license_profile["server"] + "/sensors"
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
+        sensors = {s["sensorId"]: s.get("label", None) for s in response.json()}
 
         return sensors
 
     def post_outage(self, sensor_id):
-
-        url = self.license_profile['server'] + '/outage'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        response = self._api_call('POST', url, headers)
+        url = self.license_profile["server"] + "/outage"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        response = self._api_call("POST", url, headers)
         return response.json()
 
-    def configure_sensor(self, sensor_id, feature_count=1, streaming_window_size=25,
-                         samples_to_buffer=10000,
-                         anomaly_history_window=10000,
-                         learning_rate_numerator=10,
-                         learning_rate_denominator=10000,
-                         learning_max_clusters=1000,
-                         learning_max_samples=1000000,
-                         features=None,
-                         override_pv=None):
+    def configure_sensor(
+        self,
+        sensor_id,
+        feature_count=1,
+        streaming_window_size=25,
+        samples_to_buffer=10000,
+        anomaly_history_window=10000,
+        learning_rate_numerator=10,
+        learning_rate_denominator=10000,
+        learning_max_clusters=1000,
+        learning_max_samples=1000000,
+        features=None,
+        override_pv=None,
+    ):
         """Configure an amber sensor instance
 
         Args:
             sensor_id (str): sensor identifier
             feature_count (int): number of features (dimensionality of each data sample)
             streaming_window_size (int): streaming window size (number of samples)
             samples_to_buffer (int): number of samples to load before autotuning
@@ -432,33 +410,30 @@
 
         if not feature_count > 0 or not isinstance(feature_count, Integral):
             raise AmberUserError("invalid 'feature_count': must be positive integer")
 
         if not streaming_window_size > 0 or not isinstance(streaming_window_size, Integral):
             raise AmberUserError("invalid 'streaming_window_size': must be positive integer")
 
-        url = self.license_profile['server'] + '/config'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
+        url = self.license_profile["server"] + "/config"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
         body = {
-            'featureCount': feature_count,
-            'streamingWindowSize': streaming_window_size,
-            'samplesToBuffer': samples_to_buffer,
-            'anomalyHistoryWindow': anomaly_history_window,
-            'learningRateNumerator': learning_rate_numerator,
-            'learningRateDenominator': learning_rate_denominator,
-            'learningMaxClusters': learning_max_clusters,
-            'learningMaxSamples': learning_max_samples,
-            'features': features
+            "featureCount": feature_count,
+            "streamingWindowSize": streaming_window_size,
+            "samplesToBuffer": samples_to_buffer,
+            "anomalyHistoryWindow": anomaly_history_window,
+            "learningRateNumerator": learning_rate_numerator,
+            "learningRateDenominator": learning_rate_denominator,
+            "learningMaxClusters": learning_max_clusters,
+            "learningMaxSamples": learning_max_samples,
+            "features": features,
         }
         if override_pv is not None:
-            body['percentVariationOverride'] = override_pv
-        config = self._api_call('POST', url, headers, body=body)
+            body["percentVariationOverride"] = override_pv
+        config = self._api_call("POST", url, headers, body=body)
 
         return config.json()
 
     def configure_fusion(self, sensor_id, feature_count=5, features=None):
         """Configure an Amber instance for sensor fusion
 
         Args:
@@ -481,32 +456,35 @@
             AmberUserError: if client is not authenticated or supplies invalid data
             AmberCloudError: if Amber cloud gives non-200 response.
         """
         if not features:
             if not feature_count > 0 or not isinstance(feature_count, Integral):
                 raise AmberUserError("invalid 'feature_count': must be positive integer")
             for i in range(feature_count):
-                features.append({
-                    "label": "",  # allow server to fill in default values
-                    "submitRule": ""
-                })
-
-        url = self.license_profile['server'] + '/config'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        body = {'features': features}
-        response = self._api_call('PUT', url, headers, body=body)
-        return response.json()['features']
-
-    def enable_learning(self, sensor_id, learning_rate_numerator=None,
-                        learning_rate_denominator=None,
-                        learning_max_clusters=None,
-                        learning_max_samples=None):
+                features.append(
+                    {
+                        "label": "",  # allow server to fill in default values
+                        "submitRule": "",
+                    }
+                )
+
+        url = self.license_profile["server"] + "/config"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        body = {"features": features}
+        response = self._api_call("PUT", url, headers, body=body)
+        return response.json()["features"]
+
+    def enable_learning(
+        self,
+        sensor_id,
+        learning_rate_numerator=None,
+        learning_rate_denominator=None,
+        learning_max_clusters=None,
+        learning_max_samples=None,
+    ):
         """Enable learning for a sensor thats in monitoring state
 
 
         Args:
             sensor_id (str): sensor identifier
             learning_rate_numerator (int): number of new clusters created as a max before turning off learning
             learning_rate_denominator (int): number of recent inferences to count the number of new clusters over
@@ -527,30 +505,27 @@
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
         # Server expects data as a plaintext string of comma-separated values.
 
         streaming = {}
         if learning_rate_numerator:
-            streaming['learningRateNumerator'] = learning_rate_numerator
+            streaming["learningRateNumerator"] = learning_rate_numerator
         if learning_rate_denominator:
-            streaming['learningRateDenominator'] = learning_rate_denominator
+            streaming["learningRateDenominator"] = learning_rate_denominator
         if learning_max_samples:
-            streaming['learningMaxSamples'] = learning_max_samples
+            streaming["learningMaxSamples"] = learning_max_samples
         if learning_max_clusters:
-            streaming['learningMaxClusters'] = learning_max_clusters
+            streaming["learningMaxClusters"] = learning_max_clusters
 
-        url = self.license_profile['server'] + '/config'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        body = {'streaming': streaming}
-        response = self._api_call('PUT', url, headers, body=body)
-        return response.json()['streaming']
+        url = self.license_profile["server"] + "/config"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        body = {"streaming": streaming}
+        response = self._api_call("PUT", url, headers, body=body)
+        return response.json()["streaming"]
 
     def pretrain_sensor(self, sensor_id, data, autotune_config=True, block=True):
         """Pretrain a sensor with historical data
 
         Args:
             sensor_id (str): sensor identifier
             data (array-like): data to be inferenced. Must be non-empty,
@@ -581,32 +556,26 @@
 
         # Server expects data as a plaintext string of comma-separated values.
         try:
             data_csv = float_list_to_csv_string(data)
         except ValueError as e:
             raise AmberUserError("invalid data: {}".format(e))
 
-        url = self.license_profile['server'] + '/pretrain'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        body = {
-            'data': data_csv,
-            'autotuneConfig': autotune_config
-        }
+        url = self.license_profile["server"] + "/pretrain"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        body = {"data": data_csv, "autotuneConfig": autotune_config}
 
-        results = self._api_call('POST', url, headers, body=body)
+        results = self._api_call("POST", url, headers, body=body)
 
         if not block:
             return results.json()
 
         while True:
             results = self.get_pretrain_state(sensor_id)
-            if results['state'] == "Pretraining":
+            if results["state"] == "Pretraining":
                 time.sleep(5)
                 continue
             else:
                 return results
 
     def pretrain_sensor_xl(self, sensor_id, data, autotune_config=True, block=True, chunk_size=4000000):
         """Pretrain a sensor with extra large sets of historical data.
@@ -641,59 +610,52 @@
 
         # Server expects data as a plaintext string of comma-separated values.
         try:
             data = packed_floats(data)
         except ValueError as e:
             raise AmberUserError("invalid data: {}".format(e))
 
-        url = self.license_profile['server'] + '/pretrain'
-        headers = {
-            'content-type': 'application/octet-stream',
-            'sensorId': sensor_id
-        }
-        body = {
-            'data': '',
-            'format': "packed-float",
-            'autotuneConfig': autotune_config
-        }
+        url = self.license_profile["server"] + "/pretrain"
+        headers = {"content-type": "application/octet-stream", "sensorId": sensor_id}
+        body = {"data": "", "format": "packed-float", "autotuneConfig": autotune_config}
 
         # chunk size is set at 4MB (1 million floats * 4 bytes)
         if chunk_size > 4000000:
             raise AmberCloudError(400, "chunk_size must be <= 4000000")
 
         # compute number of chunks to send
         num_chunks = int(len(data) / chunk_size)
         if len(data) % chunk_size != 0:
             num_chunks += 1
 
         amber_transaction = None
         response = None
         for chunk_num in range(0, num_chunks):
             # include amberChunk header designation, .ie 1:3, 2:3, 3:3
-            headers['amberchunk'] = '{}:{}'.format(chunk_num + 1, num_chunks)
+            headers["amberchunk"] = "{}:{}".format(chunk_num + 1, num_chunks)
             if amber_transaction is not None:
-                headers['ambertransaction'] = amber_transaction
+                headers["ambertransaction"] = amber_transaction
 
             # compute start and end range of next chunk
             start = chunk_num * chunk_size
             end = start + chunk_size
             if end > len(data):
                 end = len(data)
 
-            body['data'] = base64.b64encode(data[start:end]).decode('ascii')
-            response = self._api_call('POST', url, headers, body=body)
-            if 'ambertransaction' in response.headers:
-                amber_transaction = response.headers['ambertransaction']
+            body["data"] = base64.b64encode(data[start:end]).decode("ascii")
+            response = self._api_call("POST", url, headers, body=body)
+            if "ambertransaction" in response.headers:
+                amber_transaction = response.headers["ambertransaction"]
 
         if not block:
             return response.json()
 
         while True:
             results = self.get_pretrain_state(sensor_id)
-            if results['state'] == "Pretraining":
+            if results["state"] == "Pretraining":
                 time.sleep(5)
                 continue
             else:
                 return results
 
     def get_pretrain_state(self, sensor_id):
         """Gets the state of sensor that is being pretrained
@@ -712,21 +674,18 @@
                 "Pretrained": pretraining has completed
                 "Error": error has occurred
         Raises:
             AmberUserError: if client is not authenticated or supplies invalid data
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/pretrain'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
+        url = self.license_profile["server"] + "/pretrain"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
 
-        response = self._api_call('GET', url, headers)
+        response = self._api_call("GET", url, headers)
         return response.json()
 
     def stream_fusion(self, sensor_id, vector, submit=None):
         """Stream data to a fusion-configured sensor
 
         Args:
             sensor_id (str): sensor identifier
@@ -774,30 +733,24 @@
                 }
             }
 
         Raises:
             AmberUserError: if client is not authenticated or supplies invalid data
             AmberCloudError: if Amber cloud gives non-200 response.
         """
-        sopts = ['submit', 'nosubmit', 'default']
+        sopts = ["submit", "nosubmit", "default"]
         if submit is None:
-            submit = 'default'
+            submit = "default"
         if submit not in sopts:
             raise ValueError("'submit' must be one of {}, got {}".format(sopts, submit))
 
-        url = self.license_profile['server'] + '/stream'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        body = {
-            'vector': vector,
-            'submitRule': submit
-        }
-        response = self._api_call('PUT', url, headers, body=body)
+        url = self.license_profile["server"] + "/stream"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        body = {"vector": vector, "submitRule": submit}
+        response = self._api_call("PUT", url, headers, body=body)
         return response.json()
 
     def stream_sensor(self, sensor_id, data, save_image=True):
         """Stream data to an amber sensor and return the inference result
 
         Args:
             sensor_id (str): sensor identifier
@@ -895,24 +848,18 @@
 
         # Server expects data as a plaintext string of comma-separated values.
         try:
             data_csv = float_list_to_csv_string(data)
         except ValueError as e:
             raise AmberUserError("invalid data: {}".format(e))
 
-        url = self.license_profile['server'] + '/stream'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        body = {
-            'saveImage': save_image,
-            'data': data_csv
-        }
-        response = self._api_call('POST', url, headers, body=body)
+        url = self.license_profile["server"] + "/stream"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        body = {"saveImage": save_image, "data": data_csv}
+        response = self._api_call("POST", url, headers, body=body)
         return response.json()
 
     def get_sensor(self, sensor_id):
         """Get info about a sensor
 
         Args:
             sensor_id (str): sensor identifier
@@ -965,20 +912,17 @@
                 'samplesThisPeriod': number of samples processed this billing period
 
         Raises:
             AmberUserError: if client is not authenticated
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/sensor'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        response = self._api_call('GET', url, headers)
+        url = self.license_profile["server"] + "/sensor"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        response = self._api_call("GET", url, headers)
         return response.json()
 
     def get_config(self, sensor_id):
         """Get current sensor configuration
 
         Args:
             sensor_id (str): sensor identifier
@@ -1018,20 +962,17 @@
                 'percentVariation': percent variation parameter discovered by autotuning
                 'features': min/max values per feature discovered by autotuning
         Raises:
             AmberUserError: if client is not authenticated
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/config'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        response = self._api_call('GET', url, headers)
+        url = self.license_profile["server"] + "/config"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        response = self._api_call("GET", url, headers)
 
         return response.json()
 
     def get_status(self, sensor_id):
         """Get sensor status
 
         Args:
@@ -1065,20 +1006,17 @@
                 'numClusters': number of clusters created so far (includes zero cluster)
 
         Raises:
             AmberUserError: if client is not authenticated
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
-        url = self.license_profile['server'] + '/status'
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        response = self._api_call('GET', url, headers)
+        url = self.license_profile["server"] + "/status"
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        response = self._api_call("GET", url, headers)
 
         return response.json()
 
     def get_root_cause(self, sensor_id, id_list=None, pattern_list=None):
         """Get root cause
 
         Args:
@@ -1094,52 +1032,49 @@
         Raises:
             AmberUserError: if client is not authenticated
             AmberCloudError: if Amber cloud gives non-200 response
         """
 
         if id_list is None:
             if pattern_list is None:
-                raise AmberUserError('Must specify either id_list or pattern_list for analysis')
+                raise AmberUserError("Must specify either id_list or pattern_list for analysis")
             id_list = []
         else:
             if pattern_list is not None:
-                raise AmberUserError('Cannot specify both patterns and cluster IDs for analysis')
+                raise AmberUserError("Cannot specify both patterns and cluster IDs for analysis")
             pattern_list = []
 
-        url_call = 'rootCause?'
+        url_call = "rootCause?"
         if len(id_list) != 0:
             # IDs
             id_list = [str(element) for element in id_list]
-            url_call = url_call + 'clusterID=[' + ",".join(id_list) + ']'
+            url_call = url_call + "clusterID=[" + ",".join(id_list) + "]"
         elif len(pattern_list) != 0:
             # patterns
             if len(np.array(pattern_list).shape) == 1:  # only 1 pattern provided
                 pattern_list = [pattern_list]
             else:
                 for i, pattern in enumerate(pattern_list):
-                    pattern_list[i] = ','.join([str(element) for element in pattern])
-            url_call = url_call + 'pattern=[[' + "],[".join(pattern_list) + ']]'
+                    pattern_list[i] = ",".join([str(element) for element in pattern])
+            url_call = url_call + "pattern=[[" + "],[".join(pattern_list) + "]]"
         else:
-            raise AmberUserError('Must specify either cluster IDs or patterns to analyze')
+            raise AmberUserError("Must specify either cluster IDs or patterns to analyze")
 
-        url = self.license_profile['server'] + '/' + url_call
-        headers = {
-            'Content-Type': 'application/json',
-            'sensorId': sensor_id
-        }
-        response = self._api_call('GET', url, headers)
+        url = self.license_profile["server"] + "/" + url_call
+        headers = {"Content-Type": "application/json", "sensorId": sensor_id}
+        response = self._api_call("GET", url, headers)
 
         return response.json()
 
 
 def validate_dims(data):
     """Validate that data is non-empty and one of the following:
-       scalar value, list-like or list-of-lists-like where all
-       sublists have equal length. Return 0, 1 or 2 as inferred
-       number of array dimensions
+    scalar value, list-like or list-of-lists-like where all
+    sublists have equal length. Return 0, 1 or 2 as inferred
+    number of array dimensions
     """
 
     # not-iterable data is a single scalar data point
     if not _isiterable(data):
         return 0
 
     # iterable and unnested data is a 1-d array
@@ -1196,29 +1131,30 @@
         data_flat = list(itertools.chain.from_iterable(float_list))
     else:
         raise ValueError("float_list is not in known format")
 
     for d in data_flat:
         if not isinstance(d, Number) or np.isnan(d):
             raise ValueError("contained {} which is not numeric".format(d.__repr__()))
-    return ','.join([str(float(d)) for d in data_flat])
+    return ",".join([str(float(d)) for d in data_flat])
 
 
 def packed_floats(data):
     """Validate data and convert to a packed float buffer"""
 
     if isinstance(data, str):
-        data = data.split(',')
+        data = data.split(",")
 
-    data = np.array(data, dtype='float32')
+    data = np.array(data, dtype="float32")
     data = data.flatten()
     data = data.tobytes()
 
     return data
 
+
 # def create_packed_float_file(input, output):
 #    list_data = []
 #    with open(input, 'r') as f:
 #        csv_reader = csv.reader(f, delimiter=',')
 #        for row in csv_reader:
 #            for d in row:
 #                list_data.append(float(d))
```

