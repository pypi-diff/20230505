# Comparing `tmp/cloud_resource_matcher-0.1.0.tar.gz` & `tmp/cloud_resource_matcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_resource_matcher-0.1.0.tar", max compression
+gzip compressed data, was "cloud_resource_matcher-0.2.0.tar", max compression
```

## Comparing `cloud_resource_matcher-0.1.0.tar` & `cloud_resource_matcher-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1069 2023-04-28 17:26:42.035219 cloud_resource_matcher-0.1.0/LICENSE
--rw-r--r--   0        0        0     6035 2023-04-29 09:54:45.911393 cloud_resource_matcher-0.1.0/README.md
--rw-r--r--   0        0        0       74 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/__init__.py
--rw-r--r--   0        0        0      260 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/__init__.py
--rw-r--r--   0        0        0      738 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/__init__.py
--rw-r--r--   0        0        0     2428 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/build_mip.py
--rw-r--r--   0        0        0     1412 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/data.py
--rw-r--r--   0        0        0     2422 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/extract_solution.py
--rw-r--r--   0        0        0     1968 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/validate.py
--rw-r--r--   0        0        0      623 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/multi_cloud/__init__.py
--rw-r--r--   0        0        0     3424 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/multi_cloud/build_mip.py
--rw-r--r--   0        0        0     1325 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/multi_cloud/data.py
--rw-r--r--   0        0        0     2324 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/multi_cloud/validate.py
--rw-r--r--   0        0        0      608 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/__init__.py
--rw-r--r--   0        0        0     4987 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/build_mip.py
--rw-r--r--   0        0        0     2102 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/data.py
--rw-r--r--   0        0        0     1514 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/pre_processing.py
--rw-r--r--   0        0        0     4201 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/validate.py
--rw-r--r--   0        0        0      595 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/__init__.py
--rw-r--r--   0        0        0     1791 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/build_mip.py
--rw-r--r--   0        0        0     1339 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/data.py
--rw-r--r--   0        0        0     1352 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/pre_processing.py
--rw-r--r--   0        0        0     2333 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/validate.py
--rw-r--r--   0        0        0      565 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/service_limits/__init__.py
--rw-r--r--   0        0        0     1880 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/service_limits/build_mip.py
--rw-r--r--   0        0        0      656 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/service_limits/data.py
--rw-r--r--   0        0        0     2080 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/service_limits/validate.py
--rw-r--r--   0        0        0        0 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/py.typed
--rw-r--r--   0        0        0     1736 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.1.0/cloud_resource_matcher/solver.py
--rw-r--r--   0        0        0     1275 2023-04-29 10:08:15.570599 cloud_resource_matcher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7481 1970-01-01 00:00:00.000000 cloud_resource_matcher-0.1.0/setup.py
--rw-r--r--   0        0        0     6707 1970-01-01 00:00:00.000000 cloud_resource_matcher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-28 17:26:42.035219 cloud_resource_matcher-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6035 2023-04-29 09:54:45.911393 cloud_resource_matcher-0.2.0/README.md
+-rw-r--r--   0        0        0       74 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.2.0/cloud_resource_matcher/__init__.py
+-rw-r--r--   0        0        0      260 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/__init__.py
+-rw-r--r--   0        0        0      786 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/__init__.py
+-rw-r--r--   0        0        0     1411 2023-05-02 10:29:28.817566 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/data.py
+-rw-r--r--   0        0        0     2446 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/mip_construction.py
+-rw-r--r--   0        0        0     2431 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/solution_extraction.py
+-rw-r--r--   0        0        0     1959 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/validation.py
+-rw-r--r--   0        0        0      650 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/multi_cloud/__init__.py
+-rw-r--r--   0        0        0     1324 2023-05-02 10:29:28.817566 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/multi_cloud/data.py
+-rw-r--r--   0        0        0     3436 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/multi_cloud/mip_construction.py
+-rw-r--r--   0        0        0     2316 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/multi_cloud/validation.py
+-rw-r--r--   0        0        0      631 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/__init__.py
+-rw-r--r--   0        0        0     2102 2023-05-02 10:29:28.817566 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/data.py
+-rw-r--r--   0        0        0     5028 2023-05-05 18:46:52.542377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/mip_construction.py
+-rw-r--r--   0        0        0     1502 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/pre_processing.py
+-rw-r--r--   0        0        0     4191 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/validation.py
+-rw-r--r--   0        0        0      618 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/__init__.py
+-rw-r--r--   0        0        0     1339 2023-05-02 10:29:28.817566 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/data.py
+-rw-r--r--   0        0        0     1766 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/mip_construction.py
+-rw-r--r--   0        0        0     1304 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/pre_processing.py
+-rw-r--r--   0        0        0     2323 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/validation.py
+-rw-r--r--   0        0        0      592 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/service_limits/__init__.py
+-rw-r--r--   0        0        0      656 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/service_limits/data.py
+-rw-r--r--   0        0        0     1899 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/service_limits/mip_construction.py
+-rw-r--r--   0        0        0     2072 2023-05-05 18:46:52.546377 cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/service_limits/validation.py
+-rw-r--r--   0        0        0        0 2023-04-28 19:37:18.608437 cloud_resource_matcher-0.2.0/cloud_resource_matcher/py.typed
+-rw-r--r--   0        0        0     1736 2023-05-02 10:29:28.817566 cloud_resource_matcher-0.2.0/cloud_resource_matcher/solver.py
+-rw-r--r--   0        0        0     1280 2023-05-05 19:04:45.687994 cloud_resource_matcher-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7481 1970-01-01 00:00:00.000000 cloud_resource_matcher-0.2.0/setup.py
+-rw-r--r--   0        0        0     6707 1970-01-01 00:00:00.000000 cloud_resource_matcher-0.2.0/PKG-INFO
```

### Comparing `cloud_resource_matcher-0.1.0/LICENSE` & `cloud_resource_matcher-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud_resource_matcher-0.1.0/README.md` & `cloud_resource_matcher-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/__init__.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 This module implements the core of the cloud resource matching problem.
 It allows you to specify which cloud resources need to be deployed
 and which cloud services are available.
 
 This module isn't very useful on its own, but provides the basis for all other modules.
 """
+from optiframe import OptimizationModule
+
 from .data import BaseData
-from .validate import ValidateBaseTask
-from .build_mip import BuildMipBaseTask, BaseMipData
-from .extract_solution import ExtractSolutionBaseTask, BaseSolution
-from optiframe.framework import OptimizationModule
+from .mip_construction import BaseMipData, MipConstructionBaseTask
+from .solution_extraction import BaseSolution, SolutionExtractionBaseTask
+from .validation import ValidationBaseTask
 
 base_module = OptimizationModule(
-    validate=ValidateBaseTask, build_mip=BuildMipBaseTask, extract_solution=ExtractSolutionBaseTask
+    validation=ValidationBaseTask,
+    mip_construction=MipConstructionBaseTask,
+    solution_extraction=SolutionExtractionBaseTask,
 )
 
 __all__ = ["BaseData", "BaseMipData", "BaseSolution", "base_module"]
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/build_mip.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/mip_construction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""Implementation of the build MIP step for the base module."""
+"""Implementation of the MIP construction step for the base module."""
 from dataclasses import dataclass
 
-from optiframe.framework.tasks import BuildMipTask
-from pulp import LpVariable, LpProblem, LpBinary, lpSum
+from optiframe import MipConstructionTask
+from pulp import LpBinary, LpProblem, LpVariable, lpSum
 
-from .data import BaseData, CloudService, CloudResource
+from .data import BaseData, CloudResource, CloudService
 
 VarCrToCsMatching = dict[tuple[CloudResource, CloudService], LpVariable]
 CsToCrList = dict[CloudService, set[CloudResource]]
 
 
 @dataclass
 class BaseMipData:
@@ -17,25 +17,25 @@
     Includes the variables that have been added to the MIP.
     """
 
     # Which cloud resource should be deployed on which cloud service?
     var_cr_to_cs_matching: VarCrToCsMatching
 
 
-class BuildMipBaseTask(BuildMipTask[BaseMipData]):
+class MipConstructionBaseTask(MipConstructionTask[BaseMipData]):
     """A task to modify the MIP to implement the base module."""
 
     base_data: BaseData
     problem: LpProblem
 
     def __init__(self, base_data: BaseData, problem: LpProblem):
         self.base_data = base_data
         self.problem = problem
 
-    def execute(self) -> BaseMipData:
+    def construct_mip(self) -> BaseMipData:
         """Modify the MIP to implement the base module.
 
         Adds the central variables to determine which CR to deploy on which CS.
         """
         # Assign cloud resource cr to cloud service cs at time t?
         # ASSUMPTION: Each cloud service instance can only be used by one cloud resource instance
         # ASSUMPTION: All instances of one cloud resource have to be deployed
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/data.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """The data for the base module."""
 from dataclasses import dataclass
 
-
 # Any resource that needs to be deployed to the cloud (e.g. virtual machines).
 # Often abbreviated as 'CR'.
 CloudResource = str
 
 # A service offered by the cloud service provider that can host cloud resources.
 # Often abbreviated as 'CS'.
 CloudService = str
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/extract_solution.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/solution_extraction.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Implementation of the extract solution step for the base module."""
 from dataclasses import dataclass
 
-from optiframe.framework.tasks import ExtractSolutionTask
+from optiframe import SolutionExtractionTask
 from pulp import pulp
 
-from .data import BaseData, CloudService, CloudResource
-from .build_mip import BaseMipData
+from .data import BaseData, CloudResource, CloudService
+from .mip_construction import BaseMipData
 
 CrToCsMatching = dict[tuple[CloudResource, CloudService], int]
 ServiceInstanceCount = dict[CloudService, int]
 
 
 @dataclass
 class BaseSolution:
@@ -21,25 +21,25 @@
 
     # Which cloud resource should be deployed on which cloud service?
     cr_to_cs_matching: CrToCsMatching
     # How many instances of each service should be bought?
     cs_instance_count: ServiceInstanceCount
 
 
-class ExtractSolutionBaseTask(ExtractSolutionTask[BaseSolution]):
+class SolutionExtractionBaseTask(SolutionExtractionTask[BaseSolution]):
     """A task to extract the solution for the base module."""
 
     base_data: BaseData
     base_mip_data: BaseMipData
 
     def __init__(self, base_data: BaseData, base_mip_data: BaseMipData):
         self.base_data = base_data
         self.base_mip_data = base_mip_data
 
-    def execute(self) -> BaseSolution:
+    def extract_solution(self) -> BaseSolution:
         """Extract the solution for the base module.
 
         Extracts which CRs are deployed on which CS and
         how many instances have to be bought of each CS.
         """
         cr_to_cs_matching: CrToCsMatching = dict()
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/base/validate.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/base/validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Implementation of the validation step for the base module."""
-from optiframe.framework.tasks import ValidateTask
+from optiframe import ValidationTask
 
 from .data import BaseData
 
 
-class ValidateBaseTask(ValidateTask):
+class ValidationBaseTask(ValidationTask):
     """A task to validate the data of the base module."""
 
     base_data: BaseData
 
     def __init__(self, base_data: BaseData):
         self.base_data = base_data
 
-    def execute(self) -> None:
+    def validate(self) -> None:
         """Validate the data for consistency.
 
         :raises AssertionError: When the data is not valid.
         """
         # Validate cr_to_cs_list
         for cr in self.base_data.cloud_resources:
             assert cr in self.base_data.cr_to_cs_list.keys(), f"Valid CSs for CR {cr} not defined"
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/multi_cloud/build_mip.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/multi_cloud/mip_construction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Implementation of the build MIP step for the multi cloud module."""
 from dataclasses import dataclass
 
-from optiframe.framework.tasks import BuildMipTask
-from pulp import LpProblem, LpBinary, LpVariable, lpSum
+from optiframe import MipConstructionTask
+from pulp import LpBinary, LpProblem, LpVariable, lpSum
 
-from .data import MultiCloudData, CloudServiceProvider
 from cloud_resource_matcher.modules.base import BaseData, BaseMipData
 
+from .data import CloudServiceProvider, MultiCloudData
+
 
 @dataclass
 class MultiCloudMipData:
     """The data generated by the build MIP step for the multi cloud module.
 
     Includes the variables that have been added to the MIP.
     """
 
     var_csp_used: dict[CloudServiceProvider, LpVariable]
 
 
-class BuildMipMultiCloudTask(BuildMipTask[MultiCloudMipData]):
+class MipConstructionMultiCloudTask(MipConstructionTask[MultiCloudMipData]):
     """A task to modify the MIP to implement the multi cloud module."""
 
     base_data: BaseData
     multi_cloud_data: MultiCloudData
     base_mip_data: BaseMipData
     problem: LpProblem
 
@@ -34,15 +35,15 @@
         problem: LpProblem,
     ):
         self.base_data = base_data
         self.multi_cloud_data = multi_cloud_data
         self.base_mip_data = base_mip_data
         self.problem = problem
 
-    def execute(self) -> MultiCloudMipData:
+    def construct_mip(self) -> MultiCloudMipData:
         """Modify the MIP to implement the multi cloud module.
 
         This adds variables  to track which CSPs are used and enforces the corresponding
         requirements and objectives.
         """
         # Is cloud service provider csp used at all?
         var_csp_used: dict[CloudServiceProvider, LpVariable] = {
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/multi_cloud/data.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/multi_cloud/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """The data for the multi cloud module."""
 from dataclasses import dataclass
 
 from cloud_resource_matcher.modules.base.data import CloudService, Cost
 
-
 # The identifier for a cloud service provider such as AWS, Google Cloud or Azure.
 # Commonly abbreviated as 'CSP'.
 CloudServiceProvider = str
 
 
 @dataclass
 class MultiCloudData:
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/multi_cloud/validate.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/multi_cloud/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Implementation of the validation step for the multi cloud module."""
-from optiframe.framework.tasks import ValidateTask
+from optiframe import ValidationTask
 
 from cloud_resource_matcher.modules.base import BaseData
+
 from .data import MultiCloudData
 
 
-class ValidateMultiCloudTask(ValidateTask):
+class ValidationMultiCloudTask(ValidationTask):
     """A task to validate the data for the multi cloud module."""
 
     base_data: BaseData
     multi_cloud_data: MultiCloudData
 
     def __init__(self, base_data: BaseData, multi_cloud_data: MultiCloudData):
         self.base_data = base_data
         self.multi_cloud_data = multi_cloud_data
 
-    def execute(self) -> None:
+    def validate(self) -> None:
         """Validate the data for consistency.
 
         :raises AssertionError: When the data is not valid.
         """
         # Validate csp_to_cs_list
         for csp in self.multi_cloud_data.cloud_service_providers:
             assert (
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/build_mip.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/mip_construction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Implementation of the build MIP step for the network module."""
 from dataclasses import dataclass
 
-from optiframe.framework.tasks import BuildMipTask
-from pulp import LpProblem, LpBinary, LpVariable, lpSum
+from optiframe import MipConstructionTask
+from pulp import LpBinary, LpProblem, LpVariable, lpSum
 
-from .data import NetworkData
-from ..base.data import CloudService, CloudResource
 from cloud_resource_matcher.modules.base import BaseData, BaseMipData
+from cloud_resource_matcher.modules.base.data import CloudResource, CloudService
+
+from .data import NetworkData
 
 
 @dataclass
 class NetworkMipData:
     """The data generated by the build MIP step for the network module.
 
     Includes the variables that have been added to the MIP.
@@ -18,15 +19,15 @@
 
     # Is cr1 deployed to cs1 and cr2 deployed to cs2?
     var_cr_pair_cs_deployment: dict[
         tuple[CloudResource, CloudService, CloudResource, CloudService], LpVariable
     ]
 
 
-class BuildMipNetworkTask(BuildMipTask[NetworkMipData]):
+class MipConstructionNetworkTask(MipConstructionTask[NetworkMipData]):
     """A task to modify the MIP to implement the network module."""
 
     base_data: BaseData
     network_data: NetworkData
     base_mip_data: BaseMipData
     problem: LpProblem
 
@@ -38,15 +39,15 @@
         problem: LpProblem,
     ):
         self.base_data = base_data
         self.network_data = network_data
         self.base_mip_data = base_mip_data
         self.problem = problem
 
-    def execute(self) -> NetworkMipData:
+    def construct_mip(self) -> NetworkMipData:
         """Modify the MIP to implement the network module."""
         connection_deployments = dict()
 
         # Pre-compute the possible deployments for CR pairs respecting the latency
         for (
             cr1,
             cr2,
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/data.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The data for the network module."""
 from dataclasses import dataclass
 
-from cloud_resource_matcher.modules.base.data import CloudService, CloudResource, Cost
+from cloud_resource_matcher.modules.base.data import CloudResource, CloudService, Cost
 
 Location = str
 Latency = int
 NetworkTraffic = int
 
 
 @dataclass
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/pre_processing.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/pre_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Implementation of the pre-processing step for the network module."""
-from optiframe.framework.tasks import PreProcessingTask
+from optiframe import PreProcessingTask
 
 from cloud_resource_matcher.modules.base import BaseData
 from cloud_resource_matcher.modules.network import NetworkData
 
 
 class PreProcessingNetworkTask(PreProcessingTask[BaseData]):
     """A task to apply pre-processing techniques to the network module."""
@@ -11,15 +11,15 @@
     base_data: BaseData
     network_data: NetworkData
 
     def __init__(self, base_data: BaseData, network_data: NetworkData):
         self.base_data = base_data
         self.network_data = network_data
 
-    def execute(self) -> BaseData:
+    def pre_process(self) -> BaseData:
         """Enforce the latency requirements for the network module.
 
         Removes CSs from list of applicable CSs if the corresponding CR cannot support
         the latency of the CS to a given location.
         This only implements the maximum latency requirements for CR -> location connections.
         """
         for (cr, loc), max_latency in self.network_data.cr_and_loc_to_max_latency.items():
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/network/validate.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/network/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Implementation of the validation step for the network module."""
-from optiframe.framework.tasks import ValidateTask
+from optiframe import ValidationTask
 
 from cloud_resource_matcher.modules.base import BaseData
+
 from .data import NetworkData
 
 
-class ValidateNetworkTask(ValidateTask):
+class ValidateNetworkTask(ValidationTask):
     """Validate the data provided for the network module."""
 
     base_data: BaseData
     network_data: NetworkData
 
     def __init__(self, base_data: BaseData, network_data: NetworkData):
         self.base_data = base_data
         self.network_data = network_data
 
-    def execute(self) -> None:
+    def validate(self) -> None:
         """Validate the data for consistency.
 
         :raises AssertionError: When the data is not valid.
         """
         # Validate loc_and_loc_to_latency
         for (loc1, loc2), latency in self.network_data.loc_and_loc_to_latency.items():
             assert (
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/__init__.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """The performance module.
 
 This module can be used to enforce performance requirements
 and to represent usage-based pricing models.
 """
+from optiframe import OptimizationModule
+
 from .data import PerformanceData
+from .mip_construction import MipConstructionPerformanceTask
 from .pre_processing import PreProcessingPerformanceTask
-from .validate import ValidatePerformanceTask
-from .build_mip import BuildMipPerformanceTask
-from optiframe.framework import OptimizationModule
+from .validation import ValidatePerformanceTask
 
 performance_module = OptimizationModule(
-    validate=ValidatePerformanceTask,
+    validation=ValidatePerformanceTask,
     pre_processing=PreProcessingPerformanceTask,
-    build_mip=BuildMipPerformanceTask,
+    mip_construction=MipConstructionPerformanceTask,
 )
 
 __all__ = ["PerformanceData", "performance_module"]
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/build_mip.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/mip_construction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Implementation of the build MIP step for the performance module."""
-from optiframe.framework.tasks import BuildMipTask
+from optiframe import MipConstructionTask
 from pulp import LpProblem, lpSum
 
 from cloud_resource_matcher.modules.base import BaseData, BaseMipData
-from cloud_resource_matcher.modules.performance import PerformanceData
 
+from .data import PerformanceData
 
-class BuildMipPerformanceTask(BuildMipTask[None]):
+
+class MipConstructionPerformanceTask(MipConstructionTask[None]):
     """A task to modify the MIP for the performance module."""
 
     problem: LpProblem
     base_data: BaseData
     performance_data: PerformanceData
     base_mip_data: BaseMipData
 
@@ -22,15 +23,15 @@
         problem: LpProblem,
     ) -> None:
         self.base_data = base_data
         self.performance_data = performance_data
         self.base_mip_data = base_mip_data
         self.problem = problem
 
-    def execute(self) -> None:
+    def construct_mip(self) -> None:
         """Modify the MIP for the performance module.
 
         The constraints are enforced entirely in the pre-processing step.
         The MIP only needs to be adjusted to add the cost to the objective.
         """
         # Pay for the performance used by the cloud resources
         self.problem.objective += lpSum(
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/data.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The data for the performance module."""
 from dataclasses import dataclass
 
-from cloud_resource_matcher.modules.base.data import CloudService, CloudResource, Cost
+from cloud_resource_matcher.modules.base.data import CloudResource, CloudService, Cost
 
 PerformanceCriterion = str
 
 
 @dataclass
 class PerformanceData:
     """The data for the performance module.
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/pre_processing.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/pre_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Implementation of the pre-processing step for the performance module."""
-from optiframe.framework.tasks import PreProcessingTask
+from optiframe import PreProcessingTask
 
 from cloud_resource_matcher.modules.base import BaseData
-from cloud_resource_matcher.modules.performance import PerformanceData
+
+from .data import PerformanceData
 
 
 class PreProcessingPerformanceTask(PreProcessingTask[BaseData]):
     """A task to implement the pre-processing for the performance module."""
 
     base_data: BaseData
     performance_data: PerformanceData
 
     def __init__(self, base_data: BaseData, performance_data: PerformanceData):
         self.base_data = base_data
         self.performance_data = performance_data
 
-    def execute(self) -> BaseData:
+    def pre_process(self) -> BaseData:
         """Enforce the performance requirements as a pre-processing step.
 
         Removes CSs from the list of applicable CS if they do not satisfy the
         performance requirements of a CR.
         """
         for (cr, pc), demand in self.performance_data.performance_demand.items():
             cs_list = self.base_data.cr_to_cs_list[cr]
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/performance/validate.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/performance/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Implementation of the validation step for the performance module."""
-from optiframe.framework.tasks import ValidateTask
+from optiframe import ValidationTask
 
 from cloud_resource_matcher.modules.base import BaseData
+
 from .data import PerformanceData
 
 
-class ValidatePerformanceTask(ValidateTask):
+class ValidatePerformanceTask(ValidationTask):
     """A task to validate the data provided by the performance module."""
 
     base_data: BaseData
     performance_data: PerformanceData
 
     def __init__(self, base_data: BaseData, performance_data: PerformanceData):
         self.base_data = base_data
         self.performance_data = performance_data
 
-    def execute(self) -> None:
+    def validate(self) -> None:
         """Validate the data for consistency.
 
         :raises AssertionError: When the data is not valid.
         """
         # Validate performance_demand
         for (cr, pc) in self.performance_data.performance_demand.keys():
             assert (
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/service_limits/build_mip.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/service_limits/mip_construction.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Implementation of the build MIP step for the service limits module."""
-from optiframe.framework.tasks import BuildMipTask
+from optiframe import MipConstructionTask
 from pulp import LpProblem, lpSum
 
 from cloud_resource_matcher.modules.base import BaseData, BaseMipData
-from cloud_resource_matcher.modules.base.build_mip import CsToCrList
+from cloud_resource_matcher.modules.base.mip_construction import CsToCrList
+
 from .data import ServiceLimitsData
 
 
-class BuildMipServiceLimitsTask(BuildMipTask[None]):
+class MipConstructionServiceLimitsTask(MipConstructionTask[None]):
     """A task to build the MIP for the service limits module."""
 
     base_data: BaseData
     base_mip_data: BaseMipData
     service_limits_data: ServiceLimitsData
     problem: LpProblem
 
@@ -23,15 +24,15 @@
         problem: LpProblem,
     ):
         self.base_data = base_data
         self.service_limits_data = service_limits_data
         self.base_mip_data = base_mip_data
         self.problem = problem
 
-    def execute(self) -> None:
+    def construct_mip(self) -> None:
         """Add the variables and constraints for the service limits module."""
         # Pre-compute which cloud services can host which cloud resources
         cs_to_cr_list: CsToCrList = {
             cs: set(
                 cr
                 for cr in self.base_data.cloud_resources
                 if cs in self.base_data.cr_to_cs_list[cr]
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/service_limits/data.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/service_limits/data.py`

 * *Files identical despite different names*

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/modules/service_limits/validate.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/modules/service_limits/validation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Implementation of the validation step for the service limits module."""
-from optiframe.framework.tasks import ValidateTask
+from optiframe import ValidationTask
 
 from cloud_resource_matcher.modules.base import BaseData
+
 from .data import ServiceLimitsData
 
 
-class ValidateServiceLimitsTask(ValidateTask):
+class ValidationServiceLimitsTask(ValidationTask):
     """A task to validate the data for the service limits module."""
 
     base_data: BaseData
     service_limits_data: ServiceLimitsData
 
     def __init__(self, base_data: BaseData, service_limits_data: ServiceLimitsData):
         self.base_data = base_data
         self.service_limits_data = service_limits_data
 
-    def execute(self) -> None:
+    def validate(self) -> None:
         """Validate the data for consistency.
 
         :raises AssertionError: When the data is not valid.
         """
         # Validate cs_to_instance_limit
         for (cs, instances) in self.service_limits_data.cs_to_instance_limit.items():
             assert (
```

### Comparing `cloud_resource_matcher-0.1.0/cloud_resource_matcher/solver.py` & `cloud_resource_matcher-0.2.0/cloud_resource_matcher/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utilities to easily create a solver object."""
 
 from datetime import timedelta
 from enum import Enum
-from typing import Optional, Any
+from typing import Any, Optional
 
 import pulp
 
 from cloud_resource_matcher.modules.base.data import Cost
 
 
 class Solver(Enum):
```

### Comparing `cloud_resource_matcher-0.1.0/pyproject.toml` & `cloud_resource_matcher-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud_resource_matcher"
-version = "0.1.0"
+version = "0.2.0"
 description = "A framework to optimize costs of cloud computing deployments."
 authors = ["Tim Jentzsch <cloud_resource_matcher.projects@timjen.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/TimJentzsch/cloud_resource_matcher"
 exclude = ["examples", "benches", "test"]
 
@@ -12,30 +12,30 @@
 demo = "examples.demo:main"
 bench_mini = "benches.bench_mini:bench"
 bench_base = "benches.bench_base:bench"
 bench_complete = "benches.bench_complete:bench"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-optiframe = "^0.4.0"
+optiframe = "^0.5.0"
 pulp = "^2.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 ruff = "^0.0.246"
 pytest = "^7.2.0"
 mypy = "^1.1.1"
 matplotlib = "^3.7.1"
 
 [tool.black]
 line-length = 100
 
 [tool.ruff]
 line-length = 100
-select = ["E", "F", "D"]
+select = ["E", "F", "D", "I"]
 ignore = [
     # multi-line-summary-second-line
     # Collides with other lint rule and is non-standard
     "D213",
     # one-blank-line-before-class
     # Collides with other lint rule and is non-standard
     "D203",
```

### Comparing `cloud_resource_matcher-0.1.0/setup.py` & `cloud_resource_matcher-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,25 @@
  'cloud_resource_matcher.modules.performance',
  'cloud_resource_matcher.modules.service_limits']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['optiframe>=0.4.0,<0.5.0', 'pulp>=2.7.0,<3.0.0']
+['optiframe>=0.5.0,<0.6.0', 'pulp>=2.7.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['bench_base = benches.bench_base:bench',
                      'bench_complete = benches.bench_complete:bench',
                      'bench_mini = benches.bench_mini:bench',
                      'demo = examples.demo:main']}
 
 setup_kwargs = {
     'name': 'cloud-resource-matcher',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'A framework to optimize costs of cloud computing deployments.',
     'long_description': '# Cloud Resource Matcher [![PyPI Version](https://img.shields.io/pypi/v/cloud_resource_matcher)](https://pypi.org/project/cloud_resource_matcher/) [![License](https://img.shields.io/github/license/TimJentzsch/cloud_resource_matcher)](./LICENSE)\n\nA framework to optimize cloud computing costs, using [mixed integer programming](https://en.wikipedia.org/wiki/Integer_programming).\n\nThis library should be used together with [`optiframe`](https://github.com/TimJentzsch/optiframe) and [`pulp`](https://github.com/coin-or/pulp).\n`optiframe` is the underlying optimization framework. This library provides modules for cloud computing that you can use with `optiframe`.\n`pulp` is used to implement the mixed integer program. You only need to use it if you want to add additional modules or if you want to configure the solver.\n\n## Prerequisites\n\n- [Python](https://www.python.org/downloads/) >= 3.11\n- [optiframe](https://github.com/TimJentzsch/optiframe)\n\n## Installation\n\n```cli\npip install optiframe\n```\n\n## Usage\n\n### The Modules\n\nThis library provides multiple modules that you can use in `optiframe` for modeling cloud cost optimization problems:\n\n- `base_module`: This module represents the basic decision of which cloud resources should be deployed on which cloud services.\n    It also adds instance demands and flat (upfront) base costs for cloud services.\n    This module must always be added, all other modules depend on it.\n- `performance_module`: A module for performance requirements.\n    It allows you to define performance criteria (such as vCPUs and RAM) and the corresponding demand & supply.\n    Use-based pricing models can also be represented with this module.\n- `network_module`: This module provides the means to encode network connections, maximum latency requirements and network traffic costs.\n- `multi_cloud_module`: If multiple cloud service providers are considered for the decision, this module can be used.\n    It allows you to assign the cloud services to the providers, specify migration cost and enforce a minimum and maximum number of providers to be used.\n- `service_limits_module`: If a cloud service is under very high demand and only a limited number of instances is available for purchase, this module can encode these requirements.\n\n### Code Example\n\nHere is a small example demonstrating how to use this library:\n\n```py\nfrom pulp import LpMinimize\nfrom optiframe import Optimizer, SolutionObjValue\nfrom cloud_resource_matcher.modules.base import BaseData, BaseSolution, base_module\nfrom cloud_resource_matcher.modules.performance import PerformanceData, performance_module\n\n# Specify the data of the problem instance\nbase_data = BaseData(...)\nperformance_data = PerformanceData(...)\n\nsolution = (\n    Optimizer("cloud_cost_optimization", sense=LpMinimize)\n    # Configure which modules you want to use\n    .add_modules(base_module, performance_module)\n    # Add the data of the problem instance\n    .initialize(base_data, performance_data)\n    # Obtain the optimal solution to the problem\n    .solve()\n)\n\n# Extract the total cost of the solution\ncost = solution[SolutionObjValue].objective_value\n# Determine which cloud resource should be matched to which cloud service\nmatching = solution[BaseSolution]\n```\n\nYou can also take a look at the `examples` folder for a more detailed example.\nThe `test/case_studies` folder also contains examples based on the pricing examples from cloud service providers.\n\n### Configuring the Solver\n\nThis library uses `pulp` under the hood and is therefore agnostic to the solver backend that you can use.\nBy default, it uses the CBC solver, which is pre-bundled with `pulp`.\nHowever, it\'s not very fast, so you probably want to change it.\n\nYou can pass any solver object from `pulp` into the `.solve(...)` method.\nTake a look at [this documentation](https://coin-or.github.io/pulp/guides/how_to_configure_solvers.html) for instructions on how to install and configure the solvers.\n\n## Glossary\n\nHere is a small glossary of terms that are used across this project:\n\n- **Cloud resource** (CR): Anything you want to deploy on the cloud, such as virtual machines, serverless functions or databases.\n- **Cloud service** (CS): An offer that you can buy in the cloud, for example Google Cloud C3, Amazon S3 or Azure Functions.\n- **Cloud service provider** (CSP): A company offering cloud services. For example Google Cloud, AWS or Microsoft Azure.\n- **Mixed integer program** (MIP): A mathematical description of optimization problems.\n    Solvers can use this to return an optimal solution to the problem.\n    See also [mixed integer programming](https://en.wikipedia.org/wiki/Integer_programming).\n- **Module**: A component that implements one set of decision criteria for the optimization problem.\n    For example, the network module implements functionality to represent network traffic and latencies.\n    By choosing the modules you want to use, you can configure the functionality of the optimizer.\n    If a decision criteria or pricing model you need to use is not implemented yet, you can define your own modules.\n- **Solver**: A program implementing multiple algorithms to solve mixed integer programs to optimality.\n    Examples include [CBC](https://github.com/coin-or/Cbc) (open source), [SCIP](https://www.scipopt.org/) (open source) and [Gurobi](https://www.gurobi.com/solutions/gurobi-optimizer/) (commercial).\n\n## Development\n\nWe use [Poetry](https://python-poetry.org/docs/#installation) as a package manager, so you have to install it to properly run the project locally.\nThen you can fork and clone the repository and run `poetry install` to install all dependencies.\n\nWe use several tools to ensure a consistent level of code quality:\n\n- Run `poetry run pytest` to run the test suit for the whole project.\n- Run `poetry run mypy .` to check for typing errors.\n- Run `poetry run black .` to format all Python files.\n- Run `poetry run ruff .` to lint all Python files.\n\n## License\n\nThis project is available under the terms of the [MIT license](./LICENSE)\n',
     'author': 'Tim Jentzsch',
     'author_email': 'cloud_resource_matcher.projects@timjen.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TimJentzsch/cloud_resource_matcher',
```

### Comparing `cloud_resource_matcher-0.1.0/PKG-INFO` & `cloud_resource_matcher-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cloud-resource-matcher
-Version: 0.1.0
+Version: 0.2.0
 Summary: A framework to optimize costs of cloud computing deployments.
 Home-page: https://github.com/TimJentzsch/cloud_resource_matcher
 License: MIT
 Author: Tim Jentzsch
 Author-email: cloud_resource_matcher.projects@timjen.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: optiframe (>=0.4.0,<0.5.0)
+Requires-Dist: optiframe (>=0.5.0,<0.6.0)
 Requires-Dist: pulp (>=2.7.0,<3.0.0)
 Project-URL: Repository, https://github.com/TimJentzsch/cloud_resource_matcher
 Description-Content-Type: text/markdown
 
 # Cloud Resource Matcher [![PyPI Version](https://img.shields.io/pypi/v/cloud_resource_matcher)](https://pypi.org/project/cloud_resource_matcher/) [![License](https://img.shields.io/github/license/TimJentzsch/cloud_resource_matcher)](./LICENSE)
 
 A framework to optimize cloud computing costs, using [mixed integer programming](https://en.wikipedia.org/wiki/Integer_programming).
```

