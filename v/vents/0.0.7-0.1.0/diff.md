# Comparing `tmp/vents-0.0.7.tar.gz` & `tmp/vents-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.0.7.tar", last modified: Sun Apr 30 19:00:56 2023, max compression
+gzip compressed data, was "vents-0.1.0.tar", last modified: Fri May  5 08:50:41 2023, max compression
```

## Comparing `vents-0.0.7.tar` & `vents-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.075938 vents-0.0.7/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-04-30 19:00:23.000000 vents-0.0.7/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-30 19:00:56.076033 vents-0.0.7/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-04-30 19:00:56.076443 vents-0.0.7/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-04-30 19:00:23.000000 vents-0.0.7/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.071166 vents-0.0.7/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:23.000000 vents-0.0.7/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4857 2023-04-30 19:00:23.000000 vents-0.0.7/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.072844 vents-0.0.7/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      321 2023-04-30 19:00:23.000000 vents-0.0.7/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2381 2023-04-30 19:00:23.000000 vents-0.0.7/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     2888 2023-04-30 19:00:23.000000 vents-0.0.7/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-04-30 19:00:23.000000 vents-0.0.7/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)      438 2023-04-30 19:00:23.000000 vents-0.0.7/vents/connections/k8s_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-04-30 19:00:23.000000 vents-0.0.7/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.074039 vents-0.0.7/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-04-30 19:00:23.000000 vents-0.0.7/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      233 2023-04-30 19:00:23.000000 vents-0.0.7/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.074401 vents-0.0.7/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.074874 vents-0.0.7/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/aws/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.075346 vents-0.0.7/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/azure/blob_storage.py
--rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.075823 vents-0.0.7/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)      995 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/gcp/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-04-30 19:00:23.000000 vents-0.0.7/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:23.000000 vents-0.0.7/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-30 19:00:23.000000 vents-0.0.7/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 19:00:56.072123 vents-0.0.7/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-30 19:00:56.000000 vents-0.0.7/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1209 2023-04-30 19:00:56.000000 vents-0.0.7/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-30 19:00:56.000000 vents-0.0.7/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       66 2023-04-30 19:00:56.000000 vents-0.0.7/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-04-30 19:00:56.000000 vents-0.0.7/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.985060 vents-0.1.0/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-05-05 08:48:57.000000 vents-0.1.0/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-05-05 08:50:41.985153 vents-0.1.0/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-05-05 08:50:41.985680 vents-0.1.0/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-05-05 08:48:57.000000 vents-0.1.0/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.978065 vents-0.1.0/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4857 2023-05-05 08:48:57.000000 vents-0.1.0/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.980359 vents-0.1.0/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      335 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2485 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2916 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)      513 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/connection_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-05-05 08:48:57.000000 vents-0.1.0/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.982107 vents-0.1.0/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-05-05 08:48:57.000000 vents-0.1.0/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.982685 vents-0.1.0/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.983410 vents-0.1.0/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.984146 vents-0.1.0/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.984877 vents-0.1.0/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-05-05 08:48:57.000000 vents-0.1.0/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.979106 vents-0.1.0/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       66 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/top_level.txt
```

### Comparing `vents-0.0.7/PKG-INFO` & `vents-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.0.7
+Version: 0.1.0
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.0.7/setup.cfg` & `vents-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/setup.py` & `vents-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/config.py` & `vents-0.1.0/vents/config.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/connections/catalog.py` & `vents-0.1.0/vents/connections/catalog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Dict, List, Optional
 
 from clipped.config.schema import BaseSchemaModel
 from pydantic import PrivateAttr
 
 from vents.connections.connection import Connection
-from vents.connections.k8s_resource import K8sResource
+from vents.connections.connection_resource import ConnectionResource
 
 
 class ConnectionCatalog(BaseSchemaModel):
     connections: Optional[List[Connection]]
     _all_connections: List[Connection] = PrivateAttr()
-    _secrets: Optional[List[K8sResource]] = PrivateAttr()
-    _config_maps: Optional[List[K8sResource]] = PrivateAttr()
+    _secrets: Optional[List[ConnectionResource]] = PrivateAttr()
+    _config_maps: Optional[List[ConnectionResource]] = PrivateAttr()
     _connections_by_names: Dict[str, Connection] = PrivateAttr()
 
     def __init__(
         self,
         **data,
     ):
         super().__init__(**data)
@@ -25,34 +25,36 @@
         self._secrets = None
         self._config_maps = None
         self.set_all_connections()
 
     def set_all_connections(self) -> None:
         self._all_connections = self.connections[:] if self.connections else []
         self._connections_by_names = {}
+        self._secrets = None
+        self._config_maps = None
 
     @property
     def all_connections(self) -> List[Connection]:
         return self._all_connections
 
     @property
-    def secrets(self) -> List[K8sResource]:
+    def secrets(self) -> List[ConnectionResource]:
         if self._secrets or not self._all_connections:
             return self._secrets
         secret_names = set()
         secrets = []
         for c in self._all_connections:
             if c.secret and c.secret.name not in secret_names:
                 secret_names.add(c.secret.name)
                 secrets.append(c.secret)
         self._secrets = secrets
         return self._secrets
 
     @property
-    def config_maps(self) -> List[K8sResource]:
+    def config_maps(self) -> List[ConnectionResource]:
         if self._config_maps or not self._all_connections:
             return self._config_maps
         config_map_names = set()
         config_maps = []
         for c in self._all_connections:
             if c.config_map and c.config_map.name not in config_map_names:
                 config_map_names.add(c.config_map.name)
```

### Comparing `vents-0.0.7/vents/connections/connection.py` & `vents-0.1.0/vents/connections/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Dict, List, Optional, Union
 
 from clipped.config.schema import BaseSchemaModel
 from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr
 
+from vents.connections.connection_resource import ConnectionResource
 from vents.connections.connection_schema import ConnectionSchema
-from vents.connections.k8s_resource import K8sResource
 from vents.providers.kinds import ProviderKind
 
 
 class Connection(BaseSchemaModel):
     _IDENTIFIER = "connection"
 
     name: StrictStr
     kind: ProviderKind
     description: Optional[StrictStr]
     tags: Optional[Union[List[StrictStr], RefField]]
     schema_: Optional[ConnectionSchema] = Field(alias="schema")
-    secret: Optional[Union[K8sResource, RefField]]
-    config_map: Optional[Union[K8sResource, RefField]] = Field(alias="configMap")
+    secret: Optional[Union[ConnectionResource, RefField]]
+    config_map: Optional[Union[ConnectionResource, RefField]] = Field(alias="configMap")
     env: Optional[Union[List[Dict], RefField]]
     annotations: Optional[Union[Dict, RefField]]
 
     @classmethod
     def from_model(cls, model) -> "Connection":
         schema = model.schema_
         secret = model.secret
```

### Comparing `vents-0.0.7/vents/connections/connection_schema.py` & `vents-0.1.0/vents/connections/connection_schema.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/notifiers/__init__.py` & `vents-0.1.0/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/notifiers/base.py` & `vents-0.1.0/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/notifiers/discord_webhook.py` & `vents-0.1.0/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/notifiers/hipchat_webhook.py` & `vents-0.1.0/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/notifiers/mattermost_webhook.py` & `vents-0.1.0/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/notifiers/pagerduty_webhook.py` & `vents-0.1.0/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/notifiers/slack_webhook.py` & `vents-0.1.0/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/notifiers/webhook.py` & `vents-0.1.0/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/aws/base.py` & `vents-0.1.0/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/aws/s3.py` & `vents-0.1.0/vents/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/aws/service.py` & `vents-0.1.0/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/azure/base.py` & `vents-0.1.0/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/azure/blob_storage.py` & `vents-0.1.0/vents/providers/azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/azure/service.py` & `vents-0.1.0/vents/providers/azure/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/base.py` & `vents-0.1.0/vents/providers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/gcp/base.py` & `vents-0.1.0/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/gcp/gcs.py` & `vents-0.1.0/vents/providers/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/gcp/service.py` & `vents-0.1.0/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents/providers/kinds.py` & `vents-0.1.0/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.7/vents.egg-info/PKG-INFO` & `vents-0.1.0/vents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.0.7
+Version: 0.1.0
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.0.7/vents.egg-info/SOURCES.txt` & `vents-0.1.0/vents.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 vents.egg-info/SOURCES.txt
 vents.egg-info/dependency_links.txt
 vents.egg-info/requires.txt
 vents.egg-info/top_level.txt
 vents/connections/__init__.py
 vents/connections/catalog.py
 vents/connections/connection.py
+vents/connections/connection_resource.py
 vents/connections/connection_schema.py
-vents/connections/k8s_resource.py
 vents/notifiers/__init__.py
 vents/notifiers/base.py
 vents/notifiers/discord_webhook.py
 vents/notifiers/hipchat_webhook.py
 vents/notifiers/mattermost_webhook.py
 vents/notifiers/pagerduty_webhook.py
 vents/notifiers/slack_webhook.py
```

