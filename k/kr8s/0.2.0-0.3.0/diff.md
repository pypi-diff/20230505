# Comparing `tmp/kr8s-0.2.0.tar.gz` & `tmp/kr8s-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.2.0.tar", max compression
+gzip compressed data, was "kr8s-0.3.0.tar", max compression
```

## Comparing `kr8s-0.2.0.tar` & `kr8s-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
--rw-r--r--   0        0        0     1549 2023-03-23 14:43:10.894081 kr8s-0.2.0/LICENSE
--rw-r--r--   0        0        0     1723 2023-04-06 10:31:33.883067 kr8s-0.2.0/README.md
--rw-r--r--   0        0        0      253 2023-04-06 13:16:03.716834 kr8s-0.2.0/kr8s/__init__.py
--rw-r--r--   0        0        0     5981 2023-04-06 13:15:55.624937 kr8s-0.2.0/kr8s/_api.py
--rw-r--r--   0        0        0     5141 2023-04-05 14:28:29.381766 kr8s-0.2.0/kr8s/_auth.py
--rw-r--r--   0        0        0      361 2023-04-04 19:30:47.872877 kr8s-0.2.0/kr8s/_data_utils.py
--rw-r--r--   0        0        0       81 2023-04-03 16:55:51.155586 kr8s-0.2.0/kr8s/_exceptions.py
--rw-r--r--   0        0        0      672 2023-04-03 16:55:51.155586 kr8s-0.2.0/kr8s/_testutils.py
--rw-r--r--   0        0        0     3543 2023-04-05 14:28:29.381766 kr8s-0.2.0/kr8s/conftest.py
--rw-r--r--   0        0        0    18941 2023-04-06 13:15:55.624937 kr8s-0.2.0/kr8s/objects.py
--rw-r--r--   0        0        0       61 2023-03-31 20:28:17.436142 kr8s-0.2.0/kr8s/tests/resources/serviceaccount.yaml
--rwxr-xr-x   0        0        0      614 2023-04-03 16:55:51.155586 kr8s-0.2.0/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     1500 2023-04-06 11:27:48.029578 kr8s-0.2.0/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     2346 2023-04-03 16:55:51.155586 kr8s-0.2.0/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      300 2023-04-04 19:30:47.872877 kr8s-0.2.0/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0     7333 2023-04-06 13:15:55.624937 kr8s-0.2.0/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-04-03 16:55:51.155586 kr8s-0.2.0/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2149 2023-04-06 13:16:03.716834 kr8s-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 kr8s-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-03-23 14:43:10.894081 kr8s-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2113 2023-04-24 13:00:16.267776 kr8s-0.3.0/README.md
+-rw-r--r--   0        0        0      488 2023-05-05 14:21:46.010648 kr8s-0.3.0/kr8s/__init__.py
+-rw-r--r--   0        0        0    10163 2023-05-05 12:16:31.343064 kr8s-0.3.0/kr8s/_api.py
+-rw-r--r--   0        0        0     4650 2023-05-05 14:21:31.262579 kr8s-0.3.0/kr8s/_asyncio.py
+-rw-r--r--   0        0        0     5260 2023-04-27 16:24:20.588740 kr8s-0.3.0/kr8s/_auth.py
+-rw-r--r--   0        0        0      361 2023-04-04 19:30:47.872877 kr8s-0.3.0/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-04-27 12:49:41.923098 kr8s-0.3.0/kr8s/_exceptions.py
+-rw-r--r--   0        0        0    23828 2023-05-05 12:16:31.343064 kr8s-0.3.0/kr8s/_objects.py
+-rw-r--r--   0        0        0     7500 2023-04-30 18:57:48.474523 kr8s-0.3.0/kr8s/_portforward.py
+-rw-r--r--   0        0        0      672 2023-04-03 16:55:51.155586 kr8s-0.3.0/kr8s/_testutils.py
+-rw-r--r--   0        0        0      886 2023-04-30 18:57:48.474523 kr8s-0.3.0/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0      658 2023-05-05 12:16:31.343064 kr8s-0.3.0/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0       50 2023-04-30 18:57:48.474523 kr8s-0.3.0/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5575 2023-04-30 18:57:48.474523 kr8s-0.3.0/kr8s/conftest.py
+-rw-r--r--   0        0        0     5739 2023-05-05 12:16:31.343064 kr8s-0.3.0/kr8s/objects.py
+-rw-r--r--   0        0        0      157 2023-04-30 18:57:48.478523 kr8s-0.3.0/kr8s/portforward.py
+-rw-r--r--   0        0        0       61 2023-03-31 20:28:17.436142 kr8s-0.3.0/kr8s/tests/resources/serviceaccount.yaml
+-rwxr-xr-x   0        0        0      614 2023-04-03 16:55:51.155586 kr8s-0.3.0/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     3963 2023-05-05 14:21:31.262579 kr8s-0.3.0/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3130 2023-04-30 18:57:48.478523 kr8s-0.3.0/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      300 2023-04-04 19:30:47.872877 kr8s-0.3.0/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0    11641 2023-04-30 18:57:48.478523 kr8s-0.3.0/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-04-03 16:55:51.155586 kr8s-0.3.0/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2504 2023-05-05 14:21:46.010648 kr8s-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 kr8s-0.3.0/PKG-INFO
```

### Comparing `kr8s-0.2.0/LICENSE` & `kr8s-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.2.0/README.md` & `kr8s-0.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-# kr8s
+<div style="text-align: center; width: 100%;"><img src="branding/logo-wide.png" style="max-height: 200px;" /></div>
 
 [![Test](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml/badge.svg)](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml)
+[![Codecov](https://img.shields.io/codecov/c/gh/kr8s-org/kr8s?logo=codecov&logoColor=ffffff)](https://app.codecov.io/gh/kr8s-org/kr8s)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kr8s-org/kr8s/main.svg)](https://results.pre-commit.ci/latest/github/kr8s-org/kr8s/main)
+[![Read the Docs](https://img.shields.io/readthedocs/kr8s?logo=readthedocs&logoColor=white)](https://kr8s.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - License](https://img.shields.io/pypi/l/kr8s)](https://pypi.org/project/kr8s/)
 
 > **Warning**
 > This is beta software and might not be ready for prime time.
```

### Comparing `kr8s-0.2.0/kr8s/_auth.py` & `kr8s-0.3.0/kr8s/_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,21 @@
             Path(serviceaccount) if serviceaccount else serviceaccount
         )
         self._kubeconfig = Path(
             kubeconfig or os.environ.get("KUBECONFIG", "~/.kube/config")
         ).expanduser()
         if url:
             self.server = url
-        if serviceaccount and not self.server:
+        self.reauthenticate()
+
+    def reauthenticate(self):
+        """Reauthenticate with the server."""
+        if self._serviceaccount and not self.server:
             self.load_service_account()
-        if kubeconfig is not False and not self.server:
+        if self._kubeconfig is not False and not self.server:
             self.load_kubeconfig()
         if not self.server:
             raise ValueError("Unable to find valid credentials")
 
     def load_kubeconfig(self):
         """Load kubernetes auth from kubeconfig."""
         if not self._kubeconfig.is_file():
```

### Comparing `kr8s-0.2.0/kr8s/_testutils.py` & `kr8s-0.3.0/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.2.0/kr8s/objects.py` & `kr8s-0.3.0/kr8s/_objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, Yuvi Panda, Anaconda Inc, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 import asyncio
 import json
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional
 
 import aiohttp
 from aiohttp import ClientResponse
 
-from ._api import Kr8sApi
-from ._data_utils import list_dict_unpack
-from ._exceptions import NotFoundError
+import kr8s
+import kr8s.asyncio
+from kr8s._api import Api
+from kr8s._data_utils import list_dict_unpack
+from kr8s._exceptions import NotFoundError
+from kr8s.asyncio.portforward import PortForward as AsyncPortForward
+from kr8s.portforward import PortForward as SyncPortForward
 
 
 class APIObject:
     """Base class for Kubernetes objects."""
 
     namespaced = False
     scalable = False
     scalable_spec = "replicas"
+    _asyncio = True
 
-    def __init__(self, resource: dict, api: Kr8sApi = None) -> None:
+    def __init__(self, resource: dict, api: Api = None) -> None:
         """Initialize an APIObject."""
         # TODO support passing pykube or kubernetes objects in addition to dicts
-        self.raw = resource
-        # TODO discover existing Kr8sApi object if one exists
-        self.api = api or Kr8sApi()
+        self._raw = resource
+        self.api = api or (kr8s.asyncio.api() if self._asyncio else kr8s.api())
 
     def __repr__(self):
         """Return a string representation of the Kubernetes resource."""
         return f"<{self.kind} {self.name}>"
 
     def __str__(self):
         """Return a string representation of the Kubernetes resource."""
         return self.name
 
     @property
+    def raw(self) -> str:
+        """Raw object returned from the Kubernetes API."""
+        return self._raw
+
+    @raw.setter
+    def raw(self, value):
+        self._raw = value
+
+    @property
     def name(self) -> str:
         """Name of the Kubernetes resource."""
         return self.raw["metadata"]["name"]
 
     @property
     def namespace(self) -> str:
         """Namespace of the Kubernetes resource."""
@@ -84,105 +97,134 @@
         """Replicas of the Kubernetes resource."""
         if self.scalable:
             return self.raw["spec"][self.scalable_spec]
         raise NotImplementedError(f"{self.kind} is not scalable")
 
     @classmethod
     async def get(
-        cls, name: str, namespace: str = None, api: Kr8sApi = None, **kwargs
+        cls, name: str, namespace: str = None, api: Api = None, **kwargs
     ) -> "APIObject":
         """Get a Kubernetes resource by name."""
 
-        api = api or Kr8sApi()
+        api = api or (kr8s.asyncio.api() if cls._asyncio else kr8s.api())
         try:
-            resources = await api.get(cls.endpoint, name, namespace=namespace, **kwargs)
+            resources = await api._get(
+                cls.endpoint, name, namespace=namespace, **kwargs
+            )
             [resource] = resources
         except ValueError:
             raise ValueError(
                 f"Expected exactly one {cls.kind} object. Use selectors to narrow down the search."
             )
 
         return resource
 
     async def exists(self, ensure=False) -> bool:
         """Check if this object exists in Kubernetes."""
-        status, _ = await self.api.call_api(
+        return await self._exists(ensure=ensure)
+
+    async def _exists(self, ensure=False) -> bool:
+        """Check if this object exists in Kubernetes."""
+        async with self.api.call_api(
             "GET",
             version=self.version,
             url=f"{self.endpoint}/{self.name}",
             namespace=self.namespace,
             raise_for_status=False,
-        )
+        ) as resp:
+            status = resp.status
         if status == 200:
             return True
         if ensure:
             raise NotFoundError(f"Object {self.name} does not exist")
         return False
 
     async def create(self) -> None:
         """Create this object in Kubernetes."""
-        _, self.raw = await self.api.call_api(
+        async with self.api.call_api(
             "POST",
             version=self.version,
             url=self.endpoint,
             namespace=self.namespace,
             data=json.dumps(self.raw),
-        )
+        ) as resp:
+            self.raw = await resp.json()
 
     async def delete(self, propagation_policy: str = None) -> None:
         """Delete this object from Kubernetes."""
         data = {}
         if propagation_policy:
             data["propagationPolicy"] = propagation_policy
         try:
-            await self.api.call_api(
+            async with self.api.call_api(
                 "DELETE",
                 version=self.version,
                 url=f"{self.endpoint}/{self.name}",
                 namespace=self.namespace,
                 data=json.dumps(data),
-            )
+            ) as resp:
+                self.raw = await resp.json()
         except aiohttp.ClientResponseError as e:
             raise NotFoundError(f"Object {self.name} does not exist") from e
 
     async def refresh(self) -> None:
         """Refresh this object from Kubernetes."""
-        _, self.raw = await self.api.call_api(
+        await self._refresh()
+
+    async def _refresh(self) -> None:
+        """Refresh this object from Kubernetes."""
+        async with self.api.call_api(
             "GET",
             version=self.version,
             url=f"{self.endpoint}/{self.name}",
             namespace=self.namespace,
-        )
+        ) as resp:
+            self.raw = await resp.json()
 
     async def patch(self, patch, *, subresource=None) -> None:
         """Patch this object in Kubernetes."""
+        return await self._patch(patch, subresource=subresource)
+
+    async def _patch(self, patch, *, subresource=None) -> None:
+        """Patch this object in Kubernetes."""
         url = f"{self.endpoint}/{self.name}"
         if subresource:
             url = f"{url}/{subresource}"
-        _, self.raw = await self.api.call_api(
+        async with self.api.call_api(
             "PATCH",
             version=self.version,
             url=url,
             namespace=self.namespace,
             data=json.dumps(patch),
             headers={"Content-Type": "application/merge-patch+json"},
-        )
+        ) as resp:
+            self.raw = await resp.json()
 
     async def scale(self, replicas=None):
         """Scale this object in Kubernetes."""
-        await self.exists(ensure=True)
+        if not self.scalable:
+            raise NotImplementedError(f"{self.kind} is not scalable")
+        await self._exists(ensure=True)
         # TODO support dot notation in self.scalable_spec to support nested fields
-        await self.patch({"spec": {self.scalable_spec: replicas}})
+        await self._patch({"spec": {self.scalable_spec: replicas}})
         while self.replicas != replicas:
-            await self.refresh()
+            await self._refresh()
             await asyncio.sleep(0.1)
 
-    async def watch(self, timeout: int = None):
+    async def watch(self):
         """Watch this object in Kubernetes."""
-        raise NotImplementedError("Watching is not yet implemented")
+        since = self.metadata.get("resourceVersion")
+        async for event, obj in self.api._watch(
+            self.endpoint,
+            namespace=self.namespace,
+            field_selector=f"metadata.name={self.name}",
+            since=since,
+        ):
+            self.raw = obj.raw
+            yield event, self
 
 
 ## v1 objects
 
 
 class Binding(APIObject):
     """A Kubernetes Binding."""
@@ -274,18 +316,18 @@
     @property
     def unschedulable(self):
         if "unschedulable" in self.raw["spec"]:
             return self.raw["spec"]["unschedulable"]
         return False
 
     async def cordon(self):
-        await self.patch({"spec": {"unschedulable": True}})
+        await self._patch({"spec": {"unschedulable": True}})
 
     async def uncordon(self):
-        await self.patch({"spec": {"unschedulable": False}})
+        await self._patch({"spec": {"unschedulable": False}})
 
 
 class PersistentVolumeClaim(APIObject):
     """A Kubernetes PersistentVolumeClaim."""
 
     version = "v1"
     endpoint = "persistentvolumeclaims"
@@ -314,21 +356,26 @@
     kind = "Pod"
     plural = "pods"
     singular = "pod"
     namespaced = True
 
     async def ready(self):
         """Check if the pod is ready."""
-        await self.refresh()
+        await self._refresh()
         conditions = list_dict_unpack(
             self.status.get("conditions", []),
             key="type",
             value="status",
         )
-        return "Ready" in conditions and conditions.get("Ready", "False") == "True"
+        return (
+            "Ready" in conditions
+            and "ContainersReady" in conditions
+            and conditions.get("Ready", "False") == "True"
+            and conditions.get("ContainersReady", "False") == "True"
+        )
 
     async def logs(
         self,
         container=None,
         pretty=None,
         previous=False,
         since_seconds=None,
@@ -351,22 +398,49 @@
         if timestamps:
             params["timestamps"] = "true"
         if tail_lines is not None:
             params["tailLines"] = int(tail_lines)
         if limit_bytes is not None:
             params["limitBytes"] = int(limit_bytes)
 
-        _, resp = await self.api.call_api(
+        async with self.api.call_api(
             "GET",
             version=self.version,
             url=f"{self.endpoint}/{self.name}/log",
             namespace=self.namespace,
             params=params,
-        )
-        return resp
+        ) as resp:
+            return await resp.text()
+
+    def portforward(self, remote_port: int, local_port: int = None) -> int:
+        """Port forward a pod.
+
+        Returns an instance of :class:`kr8s.portforward.PortForward` for this Pod.
+
+        Example:
+            This can be used as a an async context manager or with explicit start/stop methods.
+
+            Context manager:
+
+            >>> async with pod.portforward(8888) as port:
+            ...     print(f"Forwarding to port {port}")
+            ...     # Do something with port 8888
+
+
+            Explict start/stop:
+
+            >>> pf = pod.portforward(8888)
+            >>> await pf.start()
+            >>> print(f"Forwarding to port {pf.local_port}")
+            >>> # Do something with port 8888
+            >>> await pf.stop()
+        """
+        if self._asyncio:
+            return AsyncPortForward(self, remote_port, local_port)
+        return SyncPortForward(self, remote_port, local_port)
 
 
 class PodTemplate(APIObject):
     """A Kubernetes PodTemplate."""
 
     version = "v1"
     endpoint = "podtemplates"
@@ -385,15 +459,15 @@
     plural = "replicationcontrollers"
     singular = "replicationcontroller"
     namespaced = True
     scalable = True
 
     async def ready(self):
         """Check if the deployment is ready."""
-        await self.refresh()
+        await self._refresh()
         return (
             self.raw["status"].get("observedGeneration", 0)
             >= self.raw["metadata"]["generation"]
             and self.raw["status"].get("readyReplicas", 0) == self.replicas
         )
 
 
@@ -448,45 +522,92 @@
         Args:
             method: HTTP method to use.
             path: Path to proxy.
             port: Port to proxy to. If not specified, the first port in the
                 Service's spec will be used.
             **kwargs: Additional keyword arguments to pass to the API call.
         """
+        return await self._proxy_http_request(method, path, port, **kwargs)
+
+    async def _proxy_http_request(
+        self, method: str, path: str, port: Optional[int] = None, **kwargs: Any
+    ) -> ClientResponse:
         if port is None:
             port = self.raw["spec"]["ports"][0]["port"]
-        _, response = await self.api.call_api(
+        async with self.api.call_api(
             method,
             version=self.version,
             url=f"{self.endpoint}/{self.name}:{port}/proxy/{path}",
             namespace=self.namespace,
-            raw=True,
             **kwargs,
-        )
-        return response
+        ) as response:
+            return response
 
     async def proxy_http_get(
         self, path: str, port: Optional[int] = None, **kwargs
     ) -> None:
-        return await self.proxy_http_request("GET", path, port, **kwargs)
+        return await self._proxy_http_request("GET", path, port, **kwargs)
 
     async def proxy_http_post(
         self, path: str, port: Optional[int] = None, **kwargs
     ) -> None:
-        return await self.proxy_http_request("POST", path, port, **kwargs)
+        return await self._proxy_http_request("POST", path, port, **kwargs)
 
     async def proxy_http_put(
         self, path: str, port: Optional[int] = None, **kwargs
     ) -> None:
-        return await self.proxy_http_request("PUT", path, port, **kwargs)
+        return await self._proxy_http_request("PUT", path, port, **kwargs)
 
     async def proxy_http_delete(
         self, path: str, port: Optional[int] = None, **kwargs
     ) -> None:
-        return await self.proxy_http_request("DELETE", path, port, **kwargs)
+        return await self._proxy_http_request("DELETE", path, port, **kwargs)
+
+    async def ready_pods(self) -> List[Pod]:
+        """Return a list of ready pods for this service."""
+        return await self._ready_pods()
+
+    async def _ready_pods(self) -> List[Pod]:
+        """Return a list of ready pods for this service."""
+        pod_selector = ",".join([f"{k}={v}" for k, v in self.labels.items()])
+        pods = await self.api._get("pods", label_selector=pod_selector)
+        return [pod for pod in pods if await pod.ready()]
+
+    async def ready(self) -> bool:
+        """Check if the service is ready."""
+        pods = await self._ready_pods()
+        return len(pods) > 0
+
+    def portforward(self, remote_port: int, local_port: int = None) -> int:
+        """Port forward a service.
+
+        Returns an instance of :class:`kr8s.portforward.PortForward` for this Service.
+
+        Example:
+            This can be used as a an async context manager or with explicit start/stop methods.
+
+            Context manager:
+
+            >>> async with service.portforward(8888) as port:
+            ...     print(f"Forwarding to port {port}")
+            ...     # Do something with port 8888
+
+
+            Explict start/stop:
+
+            >>> pf = service.portforward(8888)
+            >>> await pf.start()
+            >>> print(f"Forwarding to port {pf.local_port}")
+            >>> # Do something with port 8888
+            >>> await pf.stop()
+
+        """
+        if self._asyncio:
+            return AsyncPortForward(self, remote_port, local_port)
+        return SyncPortForward(self, remote_port, local_port)
 
 
 ## apps/v1 objects
 
 
 class ControllerRevision(APIObject):
     """A Kubernetes ControllerRevision."""
@@ -519,15 +640,15 @@
     plural = "deployments"
     singular = "deployment"
     namespaced = True
     scalable = True
 
     async def ready(self):
         """Check if the deployment is ready."""
-        await self.refresh()
+        await self._refresh()
         return (
             self.raw["status"].get("observedGeneration", 0)
             >= self.raw["metadata"]["generation"]
             and self.raw["status"].get("readyReplicas", 0) == self.replicas
         )
 
 
@@ -703,24 +824,51 @@
     endpoint = "customresourcedefinitions"
     kind = "CustomResourceDefinition"
     plural = "customresourcedefinitions"
     singular = "customresourcedefinition"
     namespaced = False
 
 
-def get_class(kind, version=None):
+## meta.k8s.io/v1 objects
+
+
+class Table(APIObject):
+    """A Kubernetes Table."""
+
+    version = "meta.k8s.io/v1"
+    endpoint = "tables"
+    kind = "Table"
+    plural = "tables"
+    singular = "table"
+    namespaced = False
+
+    @property
+    def rows(self) -> List[Dict]:
+        """Table rows."""
+        return self._raw["rows"]
+
+    @property
+    def column_definitions(self) -> List[Dict]:
+        """Table column definitions."""
+        return self._raw["columnDefinitions"]
+
+
+def get_class(kind, version=None, _asyncio=True):
     for cls in APIObject.__subclasses__():
-        if (cls.kind == kind or cls.singular == kind or cls.plural == kind) and (
-            version is None or cls.version == version
+        if (
+            hasattr(cls, "kind")
+            and (cls.kind == kind or cls.singular == kind or cls.plural == kind)
+            and (version is None or cls.version == version)
+            and cls._asyncio == _asyncio
         ):
             return cls
     raise KeyError(f"No object registered for {version}/{kind}")
 
 
-def object_from_spec(spec: dict, api: Kr8sApi = None) -> APIObject:
+def object_from_spec(spec: dict, api: Api = None) -> APIObject:
     """Create an APIObject from a Kubernetes resource spec.
 
     Args:
         spec: A Kubernetes resource spec.
 
     Returns:
         A corresponding APIObject subclass instance.
```

### Comparing `kr8s-0.2.0/kr8s/tests/scripts/envexec.py` & `kr8s-0.3.0/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.2.0/kr8s/tests/test_auth.py` & `kr8s-0.3.0/kr8s/tests/test_auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 import sys
 import tempfile
 from pathlib import Path
 
+import aiohttp
 import pytest
 import yaml
 
-from kr8s import Kr8sApi
+import kr8s
 from kr8s._testutils import set_env
 
 HERE = Path(__file__).parent.resolve()
 
 
 @pytest.fixture
 async def kubeconfig_with_exec(k8s_cluster):
@@ -34,40 +35,65 @@
         with tempfile.NamedTemporaryFile() as f:
             f.write(yaml.safe_dump(kubeconfig).encode())
             f.flush()
             yield f.name
 
 
 async def test_kubeconfig(k8s_cluster):
-    kubernetes = Kr8sApi(kubeconfig=k8s_cluster.kubeconfig_path)
+    kubernetes = kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
     version = await kubernetes.version()
     assert "major" in version
 
 
+async def test_reauthenticate(k8s_cluster):
+    kubernetes = kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
+    kubernetes.auth.reauthenticate()
+    version = await kubernetes.version()
+    assert "major" in version
+
+
+def test_reauthenticate_sync(k8s_cluster):
+    kubernetes = kr8s.api(kubeconfig=k8s_cluster.kubeconfig_path)
+    kubernetes.auth.reauthenticate()
+    version = kubernetes.version()
+    assert "major" in version
+
+
+async def test_bad_auth(serviceaccount):
+    (Path(serviceaccount) / "token").write_text("abc123")
+    kubernetes = kr8s.asyncio.api(
+        serviceaccount=serviceaccount, kubeconfig="/no/file/here"
+    )
+    serviceaccount = Path(serviceaccount)
+    with pytest.raises(aiohttp.ClientResponseError):
+        await kubernetes.version()
+
+
 async def test_url(kubectl_proxy):
-    kubernetes = Kr8sApi(url=kubectl_proxy)
+    kubernetes = kr8s.asyncio.api(url=kubectl_proxy)
     version = await kubernetes.version()
     assert "major" in version
 
 
 async def test_no_config():
     with pytest.raises(ValueError):
-        kubernetes = Kr8sApi(kubeconfig="/no/file/here")
-        await kubernetes.version()
+        kr8s.api(kubeconfig="/no/file/here")
 
 
 async def test_service_account(serviceaccount):
-    kubernetes = Kr8sApi(serviceaccount=serviceaccount, kubeconfig="/no/file/here")
+    kubernetes = kr8s.asyncio.api(
+        serviceaccount=serviceaccount, kubeconfig="/no/file/here"
+    )
     await kubernetes.version()
 
     serviceaccount = Path(serviceaccount)
     assert kubernetes.auth.server
     assert kubernetes.auth.token == (serviceaccount / "token").read_text()
     assert str(serviceaccount) in kubernetes.auth.server_ca_file
     assert "BEGIN CERTIFICATE" in Path(kubernetes.auth.server_ca_file).read_text()
     assert kubernetes.auth.namespace == (serviceaccount / "namespace").read_text()
 
 
 async def test_exec(kubeconfig_with_exec):
-    kubernetes = Kr8sApi(kubeconfig=kubeconfig_with_exec)
+    kubernetes = kr8s.asyncio.api(kubeconfig=kubeconfig_with_exec)
     version = await kubernetes.version()
     assert "major" in version
```

### Comparing `kr8s-0.2.0/kr8s/tests/test_testutils.py` & `kr8s-0.3.0/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.2.0/pyproject.toml` & `kr8s-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.2.0"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.3.0"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = false
@@ -41,19 +41,32 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 pytest-kind = {git = "https://codeberg.org/hjacobs/pytest-kind.git"}
 pytest-timeout = "^2.1.0"
 pytest-rerunfailures = "^11.1.2"
+pytest-cov = "^4.0.0"
+
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^5.3.0"
+sphinx-autobuild = "^2021.3.14"
+myst-parser = "^1.0.0"
+furo = "^2023.3.27"
+sphinx-copybutton = "^0.5.1"
+sphinx-design = "^0.3.0"
+sphinxcontrib-mermaid = "^0.8.1"
+sphinx-autoapi = "^2.1.0"
 
 [tool.pytest.ini_options]
-addopts = "-v --keep-cluster --durations=10"
+addopts = "-v --keep-cluster --durations=10 --cov=kr8s --cov-report term-missing --cov-report xml:coverage.xml"
 timeout = 300
-reruns = 0
+xfail_strict = true
+reruns = 5
 reruns_delay = 1
 asyncio_mode = "auto"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `kr8s-0.2.0/PKG-INFO` & `kr8s-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -13,18 +13,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncio-atexit (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
-# kr8s
+<div style="text-align: center; width: 100%;"><img src="branding/logo-wide.png" style="max-height: 200px;" /></div>
 
 [![Test](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml/badge.svg)](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml)
+[![Codecov](https://img.shields.io/codecov/c/gh/kr8s-org/kr8s?logo=codecov&logoColor=ffffff)](https://app.codecov.io/gh/kr8s-org/kr8s)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kr8s-org/kr8s/main.svg)](https://results.pre-commit.ci/latest/github/kr8s-org/kr8s/main)
+[![Read the Docs](https://img.shields.io/readthedocs/kr8s?logo=readthedocs&logoColor=white)](https://kr8s.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - License](https://img.shields.io/pypi/l/kr8s)](https://pypi.org/project/kr8s/)
 
 > **Warning**
 > This is beta software and might not be ready for prime time.
```

