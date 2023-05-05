# Comparing `tmp/appmesh-0.4.2-py3-none-any.whl.zip` & `tmp/appmesh-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14683 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-21 08:50 appmesh/__init__.py
--rw-r--r--  2.0 unx    53245 b- defN 23-Apr-21 08:50 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10620 b- defN 23-Apr-21 08:51 appmesh-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 08:51 appmesh-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-21 08:51 appmesh-0.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 23-Apr-21 08:51 appmesh-0.4.2.dist-info/RECORD
-6 files, 64431 bytes uncompressed, 13861 bytes compressed:  78.5%
+Zip file size: 14659 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 23-May-05 12:46 appmesh/__init__.py
+-rw-r--r--  2.0 unx    52878 b- defN 23-May-05 12:46 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10699 b- defN 23-May-05 12:46 appmesh-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 12:46 appmesh-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-05 12:46 appmesh-0.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 23-May-05 12:46 appmesh-0.4.3.dist-info/RECORD
+6 files, 64143 bytes uncompressed, 13837 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.4.2.dist-info/METADATA
+Filename: appmesh-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.4.2.dist-info/WHEEL
+Filename: appmesh-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.4.2.dist-info/top_level.txt
+Filename: appmesh-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.4.2.dist-info/RECORD
+Filename: appmesh-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -832,27 +832,15 @@
         return (resp.status_code == HTTPStatus.OK), resp.json()
 
     def role_update(self, role_name: str, role_permission_json: dict) -> bool:
         """Update (or add) a role with defined permissions, the permission ID can be App Mesh pre-defined or other permission ID.
 
         Args:
             role_name (str): the role name.
-            role_permission_json (dict): role permission definition array, e.g
-                    [
-                        "app-control",
-                        "app-delete",
-                        "cloud-app-reg",
-                        "cloud-app-delete",
-                        "app-reg",
-                        "config-set",
-                        "file-download",
-                        "file-upload",
-                        "label-delete",
-                        "label-set"
-                    ]
+            role_permission_json (dict): role permission definition array, e.g: ["app-control", "app-delete", "cloud-app-reg", "cloud-app-delete"]
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(method=AppMeshClient.Method.POST, path=f"/appmesh/role/{role_name}", body=role_permission_json)
         return resp.status_code == HTTPStatus.OK
```

## Comparing `appmesh-0.4.2.dist-info/METADATA` & `appmesh-0.4.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.4.2
+Version: 0.4.3
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,15 @@
 
 ## Features
 
 Feature | Description
 ---|---
 Application management | 1. Manage independent applications and guard the process running, similar with systemd but more flexible (long/short running, periodic long running, cron schedule, customized day time and error handling control) and comprehensive monitoring (number of starts, return code, error message, health-check) for both native and docker application. <br> 2. Use SDK/CLI run application on a remote host with sync/async mode and fetch result to client. <br> 3. Full control of application lifecycle (cgroup for resource limitation, specific OS user for execution user). <br> 4. Interactive application start support specify input data by pipe and environment variables.<br> 5. All functionality provides by [CLI](https://app-mesh.readthedocs.io/en/latest/CLI.html), [REST](https://app-mesh.readthedocs.io/en/latest/Development.html#rest-apis), [SDK](https://github.com/laoshanxi/app-mesh/tree/main/src/sdk) and [WebGUI](https://github.com/laoshanxi/app-mesh-ui) interface.<br>
 Security |  ⚡️ [JWT authentication](https://app-mesh.readthedocs.io/en/latest/JWT.html) for CLI and REST interface <br> ⚡️ [LDAP support](https://app-mesh.readthedocs.io/en/latest/LDAP.html) <br> ⚡️ [Role based permission control](https://app-mesh.readthedocs.io/en/latest/USER_ROLE.html) <br> ⚡️ [Multi-factor authentication](https://app-mesh.readthedocs.io/en/latest/MFA.html)<br> SSL support (ECDH and secure ciphers) for REST http connection  <br> Multi-tenant support
-Cloud native | Schedule cloud level applications for running on multile hosts with resource size request.<br> ⚡️ [Prometheus Exporter (build-in)](https://app-mesh.readthedocs.io/en/latest/PROMETHEUS.html) <br> ⚡️ [Grafana SimpleJson datasource](https://app-mesh.readthedocs.io/en/latest/GrafanaDataSource.html) <br> ⚡️ [Grafana Loki](https://app-mesh.readthedocs.io/en/latest/Loki.html) <br>
+Cloud native | Schedule cloud level applications for running on multile hosts with resource size request.<br> ⚡️ [Prometheus Exporter (build-in)](https://app-mesh.readthedocs.io/en/latest/PROMETHEUS.html) <br> ⚡️ [Grafana SimpleJson datasource](https://app-mesh.readthedocs.io/en/latest/GrafanaDataSource.html) <br> ⚡️ [Grafana Loki](https://app-mesh.readthedocs.io/en/latest/Loki.html) <br>⚡️ [Dockerfile](https://github.com/laoshanxi/app-mesh/blob/main/Dockerfile)
 Micro service application | ⚡️ [Consul micro-service cluster management](https://app-mesh.readthedocs.io/en/latest/CONSUL.html)
 Extra Features | Collect host/app resource usage <br> Remote run shell commands <br> Download/Upload files interface <br> Hot-update support `systemctl reload appmesh` <br> Bash completion <br> Reverse proxy <br> [Web GUI](https://github.com/laoshanxi/app-mesh-ui)
 Platform support | X86_64 <br> ARM32 <br> ARM64
 SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/appmesh_client.html) <br> [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/appmesh_client.go)
 
 ## Getting started
 The [Installation doc](https://app-mesh.readthedocs.io/en/latest/Install.html) introduces how
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.4.2 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.4.3 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
@@ -52,14 +52,15 @@
 Multi-tenant support Cloud native | Schedule cloud level applications for
 running on multile hosts with resource size request.
 â¡ï¸ [Prometheus Exporter (build-in)](https://app-mesh.readthedocs.io/en/
 latest/PROMETHEUS.html)
 â¡ï¸ [Grafana SimpleJson datasource](https://app-mesh.readthedocs.io/en/
 latest/GrafanaDataSource.html)
 â¡ï¸ [Grafana Loki](https://app-mesh.readthedocs.io/en/latest/Loki.html)
+â¡ï¸ [Dockerfile](https://github.com/laoshanxi/app-mesh/blob/main/Dockerfile)
 Micro service application | â¡ï¸ [Consul micro-service cluster management]
 (https://app-mesh.readthedocs.io/en/latest/CONSUL.html) Extra Features |
 Collect host/app resource usage
 Remote run shell commands
 Download/Upload files interface
 Hot-update support `systemctl reload appmesh`
 Bash completion
```

