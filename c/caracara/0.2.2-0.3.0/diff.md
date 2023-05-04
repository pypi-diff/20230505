# Comparing `tmp/caracara-0.2.2.tar.gz` & `tmp/caracara-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caracara-0.2.2.tar", max compression
+gzip compressed data, was "caracara-0.3.0.tar", max compression
```

## Comparing `caracara-0.2.2.tar` & `caracara-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
--rw-r--r--   0        0        0     1068 2023-02-13 15:35:32.171089 caracara-0.2.2/LICENSE
--rw-r--r--   0        0        0     8994 2023-02-13 15:35:32.171089 caracara-0.2.2/README.md
--rw-r--r--   0        0        0     2314 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/__init__.py
--rw-r--r--   0        0        0     7566 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/client.py
--rw-r--r--   0        0        0      655 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/__init__.py
--rw-r--r--   0        0        0     4032 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/batching.py
--rw-r--r--   0        0        0      603 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/common_filters.py
--rw-r--r--   0        0        0      645 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/constants.py
--rw-r--r--   0        0        0     2061 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/decorators.py
--rw-r--r--   0        0        0     3617 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/exceptions.py
--rw-r--r--   0        0        0     3402 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/interpolation.py
--rw-r--r--   0        0        0      560 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/meta.py
--rw-r--r--   0        0        0     1088 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/module.py
--rw-r--r--   0        0        0     9693 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/pagination.py
--rw-r--r--   0        0        0    15355 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/policy_wrapper.py
--rw-r--r--   0        0        0      152 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/common/sorting.py
--rw-r--r--   0        0        0      293 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/filters/__init__.py
--rw-r--r--   0        0        0     2353 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/filters/decorators.py
--rw-r--r--   0        0        0     5713 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/filters/falcon_filter.py
--rw-r--r--   0        0        0     6948 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/filters/fql.py
--rw-r--r--   0        0        0     3410 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/filters/utils.py
--rw-r--r--   0        0        0     1063 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/__init__.py
--rw-r--r--   0        0        0      282 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/custom_ioa/__init__.py
--rw-r--r--   0        0        0    11857 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/custom_ioa/custom_ioa.py
--rw-r--r--   0        0        0     6044 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/custom_ioa/rule_types.py
--rw-r--r--   0        0        0    25024 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/custom_ioa/rules.py
--rw-r--r--   0        0        0      166 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/flight_control/__init__.py
--rw-r--r--   0        0        0     3811 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/flight_control/flight_control.py
--rw-r--r--   0        0        0      216 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/hosts/__init__.py
--rw-r--r--   0        0        0     1840 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/hosts/_containment.py
--rw-r--r--   0        0        0     2797 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/hosts/_data_history.py
--rw-r--r--   0        0        0    16077 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/hosts/_groups.py
--rw-r--r--   0        0        0     3567 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/hosts/_hiding.py
--rw-r--r--   0        0        0     2776 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/hosts/_tagging.py
--rw-r--r--   0        0        0     5986 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/hosts/hosts.py
--rw-r--r--   0        0        0     9432 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/hosts/hosts_filters.py
--rw-r--r--   0        0        0      191 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/prevention_policies/__init__.py
--rw-r--r--   0        0        0     3440 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/prevention_policies/prevention_policies.py
--rw-r--r--   0        0        0    25781 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/prevention_policies/template.py
--rw-r--r--   0        0        0      173 2023-02-13 15:35:32.171089 caracara-0.2.2/caracara/modules/response_policies/__init__.py
--rw-r--r--   0        0        0     5520 2023-02-13 15:35:32.175089 caracara-0.2.2/caracara/modules/response_policies/response_policies.py
--rw-r--r--   0        0        0     4816 2023-02-13 15:35:32.175089 caracara-0.2.2/caracara/modules/response_policies/template.py
--rw-r--r--   0        0        0      485 2023-02-13 15:35:32.175089 caracara-0.2.2/caracara/modules/rtr/__init__.py
--rw-r--r--   0        0        0    18701 2023-02-13 15:35:32.175089 caracara-0.2.2/caracara/modules/rtr/batch_session.py
--rw-r--r--   0        0        0     1792 2023-02-13 15:35:32.175089 caracara-0.2.2/caracara/modules/rtr/constants.py
--rw-r--r--   0        0        0     3413 2023-02-13 15:35:32.175089 caracara-0.2.2/caracara/modules/rtr/get_file.py
--rw-r--r--   0        0        0     9140 2023-02-13 15:35:32.175089 caracara-0.2.2/caracara/modules/rtr/rtr.py
--rw-r--r--   0        0        0      450 2023-02-13 15:35:32.175089 caracara-0.2.2/caracara/modules/rtr/rtr_filters.py
--rw-r--r--   0        0        0     3862 2023-02-13 15:35:32.175089 caracara-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    12962 1970-01-01 00:00:00.000000 caracara-0.2.2/setup.py
--rw-r--r--   0        0        0     9614 1970-01-01 00:00:00.000000 caracara-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-04 23:01:54.544295 caracara-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8994 2023-05-04 23:01:54.544295 caracara-0.3.0/README.md
+-rw-r--r--   0        0        0     2314 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/__init__.py
+-rw-r--r--   0        0        0     7704 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/client.py
+-rw-r--r--   0        0        0      655 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/__init__.py
+-rw-r--r--   0        0        0     4121 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/batching.py
+-rw-r--r--   0        0        0      603 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/common_filters.py
+-rw-r--r--   0        0        0     1654 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/constants.py
+-rw-r--r--   0        0        0     2061 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/decorators.py
+-rw-r--r--   0        0        0     4111 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/exceptions.py
+-rw-r--r--   0        0        0     3402 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/interpolation.py
+-rw-r--r--   0        0        0      560 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/meta.py
+-rw-r--r--   0        0        0     1110 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/module.py
+-rw-r--r--   0        0        0    12581 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/pagination.py
+-rw-r--r--   0        0        0    15355 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/policy_wrapper.py
+-rw-r--r--   0        0        0      152 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/common/sorting.py
+-rw-r--r--   0        0        0      293 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/filters/__init__.py
+-rw-r--r--   0        0        0     2353 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/filters/decorators.py
+-rw-r--r--   0        0        0     5713 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/filters/falcon_filter.py
+-rw-r--r--   0        0        0     6948 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/filters/fql.py
+-rw-r--r--   0        0        0     3410 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/filters/utils.py
+-rw-r--r--   0        0        0     1268 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/custom_ioa/__init__.py
+-rw-r--r--   0        0        0    11857 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/custom_ioa/custom_ioa.py
+-rw-r--r--   0        0        0     6044 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/custom_ioa/rule_types.py
+-rw-r--r--   0        0        0    25024 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/custom_ioa/rules.py
+-rw-r--r--   0        0        0      166 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/flight_control/__init__.py
+-rw-r--r--   0        0        0     3811 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/flight_control/flight_control.py
+-rw-r--r--   0        0        0      216 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/__init__.py
+-rw-r--r--   0        0        0     1840 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/_containment.py
+-rw-r--r--   0        0        0     2877 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/_data_history.py
+-rw-r--r--   0        0        0    16077 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/_groups.py
+-rw-r--r--   0        0        0     3567 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/_hiding.py
+-rw-r--r--   0        0        0     2846 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/_online_state.py
+-rw-r--r--   0        0        0     2776 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/_tagging.py
+-rw-r--r--   0        0        0     7582 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/hosts.py
+-rw-r--r--   0        0        0     8728 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/hosts/hosts_filters.py
+-rw-r--r--   0        0        0      191 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/prevention_policies/__init__.py
+-rw-r--r--   0        0        0     3440 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/prevention_policies/prevention_policies.py
+-rw-r--r--   0        0        0    25781 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/prevention_policies/template.py
+-rw-r--r--   0        0        0      173 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/response_policies/__init__.py
+-rw-r--r--   0        0        0     5520 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/response_policies/response_policies.py
+-rw-r--r--   0        0        0     4816 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/response_policies/template.py
+-rw-r--r--   0        0        0      485 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/rtr/__init__.py
+-rw-r--r--   0        0        0    18701 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/rtr/batch_session.py
+-rw-r--r--   0        0        0     1792 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/rtr/constants.py
+-rw-r--r--   0        0        0     3413 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/rtr/get_file.py
+-rw-r--r--   0        0        0     9143 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/rtr/rtr.py
+-rw-r--r--   0        0        0      450 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/rtr/rtr_filters.py
+-rw-r--r--   0        0        0      223 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/users/__init__.py
+-rw-r--r--   0        0        0     4921 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/users/users.py
+-rw-r--r--   0        0        0     1838 2023-05-04 23:01:54.548295 caracara-0.3.0/caracara/modules/users/users_filters.py
+-rw-r--r--   0        0        0     3999 2023-05-04 23:01:54.552296 caracara-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9615 1970-01-01 00:00:00.000000 caracara-0.3.0/PKG-INFO
```

### Comparing `caracara-0.2.2/LICENSE` & `caracara-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/README.md` & `caracara-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/__init__.py` & `caracara-0.3.0/caracara/__init__.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/client.py` & `caracara-0.3.0/caracara/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from caracara.modules import (
     CustomIoaApiModule,
     FlightControlApiModule,
     HostsApiModule,
     PreventionPoliciesApiModule,
     ResponsePoliciesApiModule,
     RTRApiModule,
+    UsersApiModule,
     MODULE_FILTER_ATTRIBUTES,
 )
 
 
 class Client:
     """Falcon API client.
 
@@ -157,14 +158,16 @@
         self.hosts = HostsApiModule(self.api_authentication)
         self.logger.debug("Setting up the Prevention Policies module")
         self.prevention_policies = PreventionPoliciesApiModule(self.api_authentication)
         self.logger.debug("Setting up the Response Policies module")
         self.response_policies = ResponsePoliciesApiModule(self.api_authentication)
         self.logger.debug("Setting up the RTR module")
         self.rtr = RTRApiModule(self.api_authentication)
+        self.logger.debug("Setting up the Users module")
+        self.users = UsersApiModule(self.api_authentication)
 
         self.logger.debug("Configuring FQL filters")
         # Pre-configure the FQL modules for faster instantiation later
         filter_attribute_classes = [
             *common_filter_attributes,
             *MODULE_FILTER_ATTRIBUTES,
         ]
```

### Comparing `caracara-0.2.2/caracara/common/__init__.py` & `caracara-0.3.0/caracara/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/common/batching.py` & `caracara-0.3.0/caracara/common/batching.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,14 +101,16 @@
     for resource in resources:
         if 'id' in resource:
             resources_dict[resource['id']] = resource
         elif 'device_id' in resource:
             resources_dict[resource['device_id']] = resource
         elif 'child_cid' in resource:
             resources_dict[resource['child_cid']] = resource
+        elif 'uuid' in resource:
+            resources_dict[resource['uuid']] = resource
         else:
             raise Exception("No ID field to build the dictionary from")
 
     BATCH_LOGGER.debug("Returned resources")
     BATCH_LOGGER.debug(resources_dict)
 
     if errors:
```

### Comparing `caracara-0.2.2/caracara/common/common_filters.py` & `caracara-0.3.0/caracara/common/common_filters.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/common/decorators.py` & `caracara-0.3.0/caracara/common/decorators.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/common/exceptions.py` & `caracara-0.3.0/caracara/common/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Caracara exceptions."""
 from typing import Dict, List
 
+from caracara.common.constants import OnlineState
+
 
 class BaseCaracaraError(Exception):
     """Base exception class from which all other exceptions inherit."""
 
 
 class GenericAPIError(BaseCaracaraError):
     """A generic error from the API."""
@@ -110,7 +112,20 @@
         arg_str = f"{arg_names} were not provided"
 
         self.errors = [{
             "code": 500,
             "message": arg_str
         }]
         super().__init__(self.errors)
+
+
+class InvalidOnlineState(GenericAPIError):
+    """The provided online state is invalid."""
+
+    def __init__(self, online_state_string):
+        """Construct an instance of the InvalidOnlineState class."""
+        self.errors = [{
+            "code": 500,
+            "message": f"Invalid online state '{online_state_string}'. \
+                        Expected one of {OnlineState.VALUES}."
+        }]
+        super().__init__(self.errors)
```

### Comparing `caracara-0.2.2/caracara/common/interpolation.py` & `caracara-0.3.0/caracara/common/interpolation.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/common/meta.py` & `caracara-0.3.0/caracara/common/meta.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/common/module.py` & `caracara-0.3.0/caracara/common/module.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     @abstractmethod
     def help(self) -> str:
         """Store the help string to be made available for each API module."""
 
     def __init__(self, api_authentication: OAuth2):
         """Configure a Caracara API module with a FalconPy OAuth2 module."""
         class_name = self.__class__.__name__
-        self.logger = logging.getLogger(class_name)
+        self.logger = logging.getLogger(f"caracara.modules.{class_name}")
         self.logger.debug("Initialising API module: %s", class_name)
 
         self.api_authentication = api_authentication
```

### Comparing `caracara-0.2.2/caracara/common/pagination.py` & `caracara-0.3.0/caracara/common/pagination.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 The endpoints handled here typically return a list of IDs based on some
 kind of filter operation. If you are looking for parallised batching
 of data dictionaries returned in response to a list of IDs, the batching
 code file contains the required code to pull this data down as quickly
 as possible.
 
-Four types of paginator are in use:
+Five types of paginator are in use:
 
 Style 1 (Numerical Offset)
 Implementation function: all_pages_numbered_offset()
 
 We paginate by providing a limit (default: 100), and grabbing pages with
 that number of items per page. Keep going until len(list of items) == total
 
@@ -70,14 +70,26 @@
 Some APIs (such as those associated with our Intel service) divide data up by
 times, rather than by pages of data. In these cases, an FQL filter named
 _marker is used to indicate the position within the result set.
 Once a Caracara wrapper to such an API is implemented, a function to handle
 this will be built.
 See the "Deep Pagination Leveraging Markers (Timestamp)" section here:
     https://falconpy.io/Usage/Response-Handling.html
+
+
+Style 5 (Generic Parallelised One-by-One Call)
+Some APIs, such as the User Management ones, include functions that accept
+only one parameter at a time (e.g., a single ID rather than a list of IDs).
+These APIs could be parallelised within individual Caracara modules / functions,
+but instead a generic implementation is provided here.
+
+Given that there are different types of IDs within the API (CIDs, AIDs, UUIDs, etc.),
+this function takes a parameter name / parameter value list pair.
+Param Name = the name of the kwarg that should be swapped out in each call
+Value List = a list of strings to be iterated over
 """
 import concurrent.futures
 import logging
 
 from functools import partial
 from threading import current_thread
 from typing import Callable, Dict, List
@@ -276,7 +288,75 @@
         else:
             complete = True
 
     logger.debug("Returned IDs:")
     logger.debug(item_ids)
 
     return item_ids
+
+
+def _generic_parallel_list_execution_worker(
+    func: Callable[[Dict[str, Dict]], List[Dict] or List[str]] or partial,
+    logger: logging.Logger,
+    param_name: str,
+    param_value: str,
+):
+    thread_name = current_thread().name
+    if isinstance(func, partial):
+        logger.info(
+            "%s | Batch worker started with partial function: %s",
+            thread_name, func.func.__name__,
+        )
+    else:
+        logger.info(
+            "%s | Batch worker started with function: %s",
+            thread_name, func.__name__,
+        )
+
+    response = func(**{param_name: param_value})['body']
+    logger.debug("%s | %s", thread_name, response)
+    resources = response.get('resources', [])
+    logger.info("%s | Retrieved %d resources", thread_name, len(resources))
+
+    return resources
+
+
+def generic_parallel_list_execution(
+        func: Callable[[Dict[str, Dict]], List[Dict] or List[str]] or partial,
+        logger: logging.Logger,
+        param_name: str,
+        value_list: List[str],
+):
+    """Call a function many times in a thread pool based on a list of kwarg values.
+
+    This is what is described above as Pagination Style 5. A function (or partial)
+    should be provided, along with a param_name (e.g., id, cid, uuid, etc.) and
+    a list of strings to be iterated over, each of which will be assigned in turn to
+    the param named in the previous parameter.
+    """
+    logger = logger.getChild(__name__)
+    if isinstance(func, partial):
+        logger.info(
+            "Pagination Style 5: Repeatedly executing the partial function %s",
+            func.func.__name__,
+        )
+    else:
+        logger.info(
+            "Pagination Style 2: Grabbing all pages from the function %s",
+            func.__name__,
+        )
+
+    all_resources = []
+    threads = batch_data_pull_threads()
+
+    with concurrent.futures.ThreadPoolExecutor(max_workers=threads) as executor:
+        partial_worker = partial(_generic_parallel_list_execution_worker, func, logger, param_name)
+        completed = executor.map(
+            partial_worker,
+            value_list,
+        )
+
+    for complete in completed:
+        logger.debug("Completed a function execution against one item")
+        all_resources.extend(complete)
+
+    return all_resources
```

### Comparing `caracara-0.2.2/caracara/common/policy_wrapper.py` & `caracara-0.3.0/caracara/common/policy_wrapper.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/filters/decorators.py` & `caracara-0.3.0/caracara/filters/decorators.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/filters/falcon_filter.py` & `caracara-0.3.0/caracara/filters/falcon_filter.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/filters/fql.py` & `caracara-0.3.0/caracara/filters/fql.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/filters/utils.py` & `caracara-0.3.0/caracara/filters/utils.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/__init__.py` & `caracara-0.3.0/caracara/modules/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
-Falcon Host module.
+Caracara Modules Package Initialisation.
 
-Exposes functions to get host data and perform actions on hosts, such as network containment.
+Proides pipework to link together the various modules within Caracara and expose them to
+the Client object at setup.
 """
 __all__ = [
     'CustomIoaApiModule',
     'FlightControlApiModule',
     'HostsApiModule',
     'PreventionPoliciesApiModule',
     'ResponsePoliciesApiModule',
     'RTRApiModule',
+    'UsersApiModule',
     'MODULE_FILTER_ATTRIBUTES',
 ]
 
 from caracara.modules.custom_ioa import CustomIoaApiModule
 from caracara.modules.flight_control import FlightControlApiModule
 from caracara.modules.hosts import (
     FILTER_ATTRIBUTES as hosts_filter_attributes,
@@ -21,14 +23,19 @@
 )
 from caracara.modules.prevention_policies import PreventionPoliciesApiModule
 from caracara.modules.response_policies import ResponsePoliciesApiModule
 from caracara.modules.rtr import (
     FILTER_ATTRIBUTES as rtr_filter_attributes,
     RTRApiModule,
 )
+from caracara.modules.users import (
+    FILTER_ATTRIBUTES as users_filter_attributes,
+    UsersApiModule,
+)
 
 # Build up a list with all filter attributes from the includes modules.
 # This makes makes for much easier importing when setting up Falcon Filters.
 MODULE_FILTER_ATTRIBUTES = [
     *hosts_filter_attributes,
     *rtr_filter_attributes,
+    *users_filter_attributes,
 ]
```

### Comparing `caracara-0.2.2/caracara/modules/custom_ioa/custom_ioa.py` & `caracara-0.3.0/caracara/modules/custom_ioa/custom_ioa.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/custom_ioa/rule_types.py` & `caracara-0.3.0/caracara/modules/custom_ioa/rule_types.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/custom_ioa/rules.py` & `caracara-0.3.0/caracara/modules/custom_ioa/rules.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/flight_control/flight_control.py` & `caracara-0.3.0/caracara/modules/flight_control/flight_control.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/hosts/_containment.py` & `caracara-0.3.0/caracara/modules/hosts/_containment.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/hosts/_data_history.py` & `caracara-0.3.0/caracara/modules/hosts/_data_history.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 @filter_string
 def describe_state(
     self: HostsApiModule,
     filters: FalconFilter or str = None,
 ) -> Dict[str, Dict]:
     """Return a dictionary containing online state for devices matching the provided filter.
 
+    DEPRECATED. The describe_devices function now captures this functionality.
+
     Arguments
     ---------
     filters: FalconFilter or str, optional
         Filters to apply to the device search.
 
     Returns
     -------
```

### Comparing `caracara-0.2.2/caracara/modules/hosts/_groups.py` & `caracara-0.3.0/caracara/modules/hosts/_groups.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/hosts/_hiding.py` & `caracara-0.3.0/caracara/modules/hosts/_hiding.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/hosts/_tagging.py` & `caracara-0.3.0/caracara/modules/hosts/_tagging.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/hosts/hosts.py` & `caracara-0.3.0/caracara/modules/hosts/hosts.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 
 This module handles interactions with the CrowdStrike Falcon Hosts and Host Group APIs.
 """
 from functools import partial
 from typing import (
     Dict,
     List,
+    Union,
+    Optional,
 )
 
 from falconpy import (
     Hosts,
     HostGroup,
     OAuth2,
 )
 
 from caracara.common.batching import batch_get_data
+from caracara.common.constants import OnlineState
 from caracara.common.exceptions import (
     GenericAPIError,
 )
 from caracara.common.module import FalconApiModule
 from caracara.common.pagination import (
     all_pages_token_offset,
 )
@@ -89,54 +92,90 @@
     from caracara.modules.hosts._hiding import (
         describe_hidden_devices,
         get_hidden_ids,
         hide,
         unhide,
     )
 
+    # Import functions to filter by device online state
+    from caracara.modules.hosts._online_state import (
+        get_online_state,
+        filter_device_ids_by_online_state,
+        validate_online_state,
+    )
+
     # Import functions to create and modify device tags
     from caracara.modules.hosts._tagging import (
         _create_tag_list,
         _update_device_tags,
         tag,
         untag,
     )
 
     # Static methods have to be set within the class
     _create_tag_list = staticmethod(_create_tag_list)
 
-    def _perform_action(self, action_name: str, device_ids: List[str]) -> Dict:
+    def _perform_action(
+            self,
+            action_name: str,
+            device_ids: List[str],
+    ) -> Dict:
         """Perform the specified action against the list of targets."""
         returned = self.hosts_api.perform_action(ids=device_ids, action_name=action_name)["body"]
 
         if returned["errors"]:
             raise GenericAPIError(returned["errors"])
 
         return returned
 
     @filter_string
-    def describe_devices(self, filters: FalconFilter or str = None) -> Dict[str, Dict]:
+    def describe_devices(
+        self,
+        filters: FalconFilter or str = None,
+        online_state: Optional[Union[OnlineState, str]] = None,
+    ) -> Dict[str, Dict]:
         """Return a dictionary containing details for every device matching the provided filter.
 
         Arguments
         ---------
         filters: FalconFilter or str, optional
             Filters to apply to the device search.
+        online_state: OnlineState or str, optional
+            Device online state to filter devices on. Options are "online", "offline", "unknown"
 
         Returns
         -------
         dict: A dictionary containing details for every device discovered.
         """
         self.logger.info("Describing devices according to the filter string %s", filters)
         device_ids = self.get_device_ids(filters)
+
+        # Collect state data
+        device_state_data = self.get_online_state(device_ids)
+
+        # Filter by online state, if applicable.
+        if online_state is not None:
+            self.validate_online_state(online_state)
+            device_ids = list(filter(
+                lambda key: device_state_data[key]["state"] == online_state,
+                device_state_data,
+            ))
+
         device_data = self.get_device_data(device_ids)
 
+        # Enrich the results with the online state field
+        for device_id, data in device_data.items():
+            data["state"] = device_state_data[device_id]["state"]
+
         return device_data
 
-    def get_device_data(self, device_ids: List[str]) -> Dict[str, Dict]:
+    def get_device_data(
+            self,
+            device_ids: List[str],
+    ) -> Dict[str, Dict]:
         """Return a dictionary containing details for every device specified by ID.
 
         You should only use this endpoint if you already have a list of Device IDs / AIDs,
         and want to retreive data about them directly. If you need to get device data via a
         filter, and you do not yet have a list of Device IDs, you should consider using the
         describe_devices() function.
 
@@ -150,23 +189,34 @@
         dict: A dictionary containing details for every device listed.
         """
         self.logger.info("Obtaining data for %s devices", len(device_ids))
         device_data = batch_get_data(device_ids, self.hosts_api.get_device_details)
         return device_data
 
     @filter_string
-    def get_device_ids(self, filters: FalconFilter or str = None) -> List[str]:
+    def get_device_ids(
+        self,
+        filters: FalconFilter or str = None,
+        online_state: Optional[Union[OnlineState, str]] = None,
+    ) -> List[str]:
         """Return a list of IDs (string) for every device in your Falcon tenant.
 
         Arguments
         ---------
         filters: FalconFilter or str, optional
             Filters to apply to the device search.
+        online_state: OnlineState or str, optional
+            Device online state to filter devices on. Options are "online", "offline", "unknown"
 
         Returns
         -------
         List[str]: A list of all device IDs discovered.
         """
         self.logger.info("Searching for device IDs using the filter string %s", filters)
         func = partial(self.hosts_api.query_devices_by_filter_scroll, filter=filters)
         id_list: List[str] = all_pages_token_offset(func=func, logger=self.logger)
+
+        # Filter by online state, if applicable.
+        if online_state is not None:
+            id_list = self.filter_device_ids_by_online_state(id_list, online_state=online_state)
+
         return id_list
```

### Comparing `caracara-0.2.2/caracara/modules/hosts/hosts_filters.py` & `caracara-0.3.0/caracara/modules/hosts/hosts_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,35 +18,14 @@
         "Contained": "contained",
         "Containment Pending": "containment_pending",
         "Not Contained": "normal",
     }
     restrict = True
 
 
-class HostConnectionStatusFilterAttribute(FalconFilterAttribute):
-    """
-    Filter by whether a host is connected to the Falcon cloud.
-
-    Current valid options are Online and Offline.
-    """
-
-    name = "ConnectionStatus"
-    fql = "connection_status"
-    options = ["Online", "Offline"]
-    restrict = True
-
-    def example(self) -> str:
-        """Show filter example."""
-        return (
-            "This filter allows you to search for systems based on whether Falcon assesses them "
-            "as being Online or Offline. Theoretically, all 'Online' systems should be available "
-            "to connect to via Real Time Response (RTR)."
-        )
-
-
 class HostDomainFqlFilterAttribute(FalconFilterAttribute):
     """Filter by host AD domain."""
 
     name = "Domain"
     fql = "machine_domain"
 
     def example(self) -> str:
@@ -288,15 +267,14 @@
             "e.g. UKServers,USServers to target hosts within any of those "
             "OUs. Programmatically, you can pass a Python list of OUs."
         )
 
 
 FILTER_ATTRIBUTES = [
     HostContainedFilterAttribute,
-    HostConnectionStatusFilterAttribute,
     HostDomainFqlFilterAttribute,
     HostGroupIdFilterAttribute,
     HostHostnameFilterAttribute,
     HostLastSeenFilterAttrribute,
     HostFirstSeenFilterAttribute,
     HostLocalIPFilterAttribute,
     HostOSFqlFilterAttribute,
```

### Comparing `caracara-0.2.2/caracara/modules/prevention_policies/prevention_policies.py` & `caracara-0.3.0/caracara/modules/prevention_policies/prevention_policies.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/prevention_policies/template.py` & `caracara-0.3.0/caracara/modules/prevention_policies/template.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/response_policies/response_policies.py` & `caracara-0.3.0/caracara/modules/response_policies/response_policies.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/response_policies/template.py` & `caracara-0.3.0/caracara/modules/response_policies/template.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/rtr/batch_session.py` & `caracara-0.3.0/caracara/modules/rtr/batch_session.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/rtr/constants.py` & `caracara-0.3.0/caracara/modules/rtr/constants.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/rtr/get_file.py` & `caracara-0.3.0/caracara/modules/rtr/get_file.py`

 * *Files identical despite different names*

### Comparing `caracara-0.2.2/caracara/modules/rtr/rtr.py` & `caracara-0.3.0/caracara/modules/rtr/rtr.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         Get a list of queued RTR Session IDs.
 
         Returns
         -------
         List[str]: A list of IDs of all queued RTR sessions discovered.
         """
         self.logger.info("Searching for queued RTR sessions")
-        filter_str = "offline_queued: 1+deleted_at: null"
+        filter_str = "offline_queued: true+deleted_at: null"
         session_ids = self._search_sessions(filters=filter_str)
         return session_ids
 
     def describe_queued_sessions(self) -> Dict:
         """
         Show the contents of all queued RTR sessions.
```

### Comparing `caracara-0.2.2/pyproject.toml` & `caracara-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "caracara"
-version = "0.2.2"
+version = "0.3.0"
 description = "The CrowdStrike Falcon Developer Toolkit"
 authors = [ "CrowdStrike <falconpy@crowdstrike.com>" ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 py7zr = "^0.20"
-crowdstrike-falconpy = "^1.2.9"
+crowdstrike-falconpy = "^1.2.15"
 
 [tool.poetry.dev-dependencies]
-bandit = "^1.7.4"
+bandit = "^1.7.5"
 bullet = "^2.2.0"
 coverage = "^7.1.0"
 flake8 = "^5.0.4"
 pydocstyle = "^6.3.0"
 pylint = "^2.12.2"
 pytest = "^7.2.1"
 PyYAML = "^6.0"
@@ -81,7 +81,10 @@
 # RTR
 clear-queued-sessions = "examples.rtr.clear_queued_sessions:clear_queued_sessions"
 describe-put-files = "examples.rtr.describe_put_files:describe_put_files"
 describe-queued-sessions = "examples.rtr.describe_queued_sessions:describe_queued_sessions"
 describe-scripts = "examples.rtr.describe_scripts:describe_scripts"
 download-event-log = "examples.rtr.download_event_log:download_event_log"
 queue-command = "examples.rtr.queue_command:queue_command"
+# Users
+describe-roles = "examples.users.describe_roles:describe_roles"
+describe-users = "examples.users.describe_users:describe_users"
```

### Comparing `caracara-0.2.2/PKG-INFO` & `caracara-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: caracara
-Version: 0.2.2
+Version: 0.3.0
 Summary: The CrowdStrike Falcon Developer Toolkit
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: crowdstrike-falconpy (>=1.2.9,<2.0.0)
+Requires-Dist: crowdstrike-falconpy (>=1.2.15,<2.0.0)
 Requires-Dist: py7zr (>=0.20,<0.21)
 Description-Content-Type: text/markdown
 
 ![CrowdStrike Falcon](https://raw.githubusercontent.com/CrowdStrike/falconpy/main/docs/asset/cs-logo.png) [![Twitter URL](https://img.shields.io/twitter/url?label=Follow%20%40CrowdStrike&style=social&url=https%3A%2F%2Ftwitter.com%2FCrowdStrike)](https://twitter.com/CrowdStrike)<br/>
 
 # Caracara
```

