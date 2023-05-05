# Comparing `tmp/compose_chart_export-0.0.15rc1-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.15rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 12828 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 14:47 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 23-May-03 14:47 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    12399 b- defN 23-May-03 14:47 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4967 b- defN 23-May-03 14:47 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-03 14:47 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9145 b- defN 23-May-03 14:47 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2359 b- defN 23-May-03 14:47 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-03 14:47 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      586 b- defN 23-May-03 14:47 compose_chart_export-0.0.15rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 14:47 compose_chart_export-0.0.15rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-03 14:47 compose_chart_export-0.0.15rc1.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-03 14:47 compose_chart_export-0.0.15rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1214 b- defN 23-May-03 14:47 compose_chart_export-0.0.15rc1.dist-info/RECORD
-13 files, 35644 bytes uncompressed, 10742 bytes compressed:  69.9%
+Zip file size: 13069 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 08:44 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 23-May-05 08:44 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    13414 b- defN 23-May-05 08:44 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4967 b- defN 23-May-05 08:44 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-May-05 08:44 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9380 b- defN 23-May-05 08:44 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2359 b- defN 23-May-05 08:44 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-May-05 08:44 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      586 b- defN 23-May-05 08:44 compose_chart_export-0.0.15rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 08:44 compose_chart_export-0.0.15rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 08:44 compose_chart_export-0.0.15rc2.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-05 08:44 compose_chart_export-0.0.15rc2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1214 b- defN 23-May-05 08:44 compose_chart_export-0.0.15rc2.dist-info/RECORD
+13 files, 36970 bytes uncompressed, 10983 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc1.dist-info/METADATA
+Filename: compose_chart_export-0.0.15rc2.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc1.dist-info/WHEEL
+Filename: compose_chart_export-0.0.15rc2.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc1.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.15rc2.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc1.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.15rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc1.dist-info/RECORD
+Filename: compose_chart_export-0.0.15rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compose_chart_export/chart_export.py

```diff
@@ -7,14 +7,15 @@
     chart_yaml,
     daemonset_yaml,
     deployment_yaml,
     helm_ignore,
     helpers_tpl,
     notes_txt,
     persistence_volume_claims,
+    service_account,
     service_yaml,
     values_yaml,
 )
 from zero_3rdparty.file_utils import clean_dir, ensure_parents_write_text
 
 logger = logging.getLogger(__name__)
 
@@ -28,14 +29,15 @@
     "values.yaml": values_yaml,
     "templates/_helpers.tpl": helpers_tpl,
     deployment_path: deployment_yaml,
     service_path: service_yaml,
     "templates/NOTES.txt": notes_txt,
     daemonset_path: daemonset_yaml,
     "templates/persistent-volume-claims.yaml": persistence_volume_claims,
+    "templates/service_account.yaml": service_account,
 }
 SERVICE_DEPLOYMENT = "service_deployment"
 DEPLOYMENT_ONLY = "deployment_only"
 DAEMONSET = "daemonset"
 
 
 def _export_chart(
```

## compose_chart_export/chart_file_templates.py

```diff
@@ -117,17 +117,22 @@
     replacements: TemplateReplacements
     containers: List[str]
     container_host_path_volumes: Dict[str, List[HostPathContainerPath]] = Field(
         default_factory=dict
     )
     persistence_volumes: list[PersistentVolume] = Field(default_factory=list)
     use_resource_limits: bool = True
+    service_account_name: str = ""
     extra_labels: dict[str, kubernetes_label_regex] = Field(default_factory=dict)
 
     @property
+    def use_service_account(self) -> bool:
+        return bool(self.service_account_name)
+
+    @property
     def containers_values_names(self) -> List[str]:
         return [name.replace("-", "_") for name in self.containers]
 
     @property
     def container_name_value_name(self) -> List[Tuple[str, str]]:
         return list(zip(self.containers, self.containers_values_names))
 
@@ -143,20 +148,32 @@
 
 _RESOURCES_YAML = """\
 resources:
   limits:
     cpu: 500m
     memory: 512Mi"""
 
+_SERVICE_ACCOUNT_VALUES = """\
+serviceAccount:
+  name: SERVICE_ACCOUNT_NAME
+  annotations: {}
+  create: true
+"""
+
 
 def values_yaml(spec: ChartTemplateSpec) -> str:
     values_base = _VALUES_YAML
     if spec.use_resource_limits:
         values_base += f"\n{_RESOURCES_YAML}"
-    return _VALUES_YAML + "".join(
+    if service_account_name := spec.service_account_name:
+        service_account_values = _SERVICE_ACCOUNT_VALUES.replace(
+            "SERVICE_ACCOUNT_NAME", service_account_name
+        )
+        values_base += f"\n{service_account_values}"
+    return values_base + "".join(
         f"\n{name}: \n  image: override_me" for name in spec.containers_values_names
     )
 
 
 _helm_ignore = """# Patterns to ignore when building packages.
 # This supports shell glob matching, relative path matching, and
 # negation (prefixed with !). Only one pattern per line.
@@ -403,7 +420,30 @@
 def persistence_volume_claims(spec: ChartTemplateSpec) -> str:
     return "---".join(
         _PVC_YAML.replace("PVC_NAME", pv.name_var).replace(
             "PVC_SIZE", str(pv.storage_gb)
         )
         for pv in spec.persistence_volumes
     )
+
+
+_SERVICE_ACCOUNT = """\
+{{- if .Values.serviceAccount.create }}
+apiVersion: v1
+kind: ServiceAccount
+metadata:
+  name: {{ .Values.serviceAccount.name }}
+  namespace: {{ .Release.Namespace }}
+  labels:
+    {{- include "common.labels.standard" . | nindent 4 }}
+  {{- with .Values.serviceAccount.annotations }}
+  annotations:
+    {{- toYaml . | nindent 4 }}
+  {{- end }}
+{{- end }}
+"""
+
+
+def service_account(spec: ChartTemplateSpec) -> str:
+    if spec.use_service_account:
+        return _SERVICE_ACCOUNT
+    return ""
```

## compose_chart_export/compose_export.py

```diff
@@ -68,14 +68,18 @@
     return labels.get("chart_repo_owner", "")
 
 
 def parse_existing_chart(labels: dict[str, str]):
     return labels.get("chart_path", "")
 
 
+def parse_service_account_name(labels: dict[str, str]):
+    return labels.get("chart_service_account_name", "")
+
+
 class ExtraContainer(BaseModel):
     name: kubernetes_label_regex
     env: dict[str, str]
     command: list[str]
 
 
 def parse_service_name_extra_containers(
@@ -240,20 +244,22 @@
         logger.info(f"no ports for {service_name}")
         template_name = template_name or ChartTemplate.DEPLOYMENT_ONLY
     target_volumes = parse_target_volumes(compose_labels)
     persistent_volumes = parse_persistent_volumes(compose_labels)
     use_resource_limits = parse_use_resource_limits(compose_labels)
     repo_name = parse_repo_name(compose_labels) or container_name
     repo_owner = parse_repo_owner(compose_labels) or "unknown"
+    service_account_name = parse_service_account_name(compose_labels)
     return template_name, ChartTemplateSpec(
         replacements=TemplateReplacements(
             APP_VERSION=chart_version,
             CHART_VERSION=chart_version,
             REPO_NAME=repo_name,
             REPO_OWNER=repo_owner,
             APP_NAME=chart_name,
         ),
         containers=[container_name],
         container_host_path_volumes={container_name: target_volumes},
         persistence_volumes=persistent_volumes,
         use_resource_limits=use_resource_limits,
+        service_account_name=service_account_name,
     )
```

## Comparing `compose_chart_export-0.0.15rc1.dist-info/METADATA` & `compose_chart_export-0.0.15rc2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.15rc1
+Version: 0.0.15rc2
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Requires-Dist: docker-compose-parser (==0.0.15)
 Requires-Dist: model-lib (==0.0.15)
```

## Comparing `compose_chart_export-0.0.15rc1.dist-info/RECORD` & `compose_chart_export-0.0.15rc2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 compose_chart_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-compose_chart_export/chart_export.py,sha256=PKwJCJ6RG67L91pu0OTd7Fr4Ok3uSppkvnopd4P1eVA,2458
-compose_chart_export/chart_file_templates.py,sha256=DzCmYQVyanVrjI8WcQLKxoGLCjorpMSWvMlVt_yAVbI,12399
+compose_chart_export/chart_export.py,sha256=oDgolV_QNeF12D2xh2D9xhn45IQSbKDMmj2WRZ2UTaI,2534
+compose_chart_export/chart_file_templates.py,sha256=dXw9DzRJqKJK9c2cTYOJb5vyaFmX-EgIn6eYEW08gbM,13414
 compose_chart_export/chart_mods.py,sha256=Zn-NSYhv7jJfUtGs6V--fquIolVqFT3bwL8mSWrwgOI,4967
 compose_chart_export/chart_read.py,sha256=chwkPcucA6dLWStADbP2kpAGNbhYVMms9zmPjNIQrLs,2211
-compose_chart_export/compose_export.py,sha256=7QhbW8XPk1WKzwRePl0gd83psxkWkSaEYS5Y7ZjzIUA,9145
+compose_chart_export/compose_export.py,sha256=w0ionkwWLTGOz9Lf2MIZVTRrUAjj7_pzmhJOxU80ZZw,9380
 compose_chart_export/ports.py,sha256=06WBSFYTUEPUYh9x4U5BjjUeE-EPNCs1Pot6MO7zxD4,2359
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.15rc1.dist-info/METADATA,sha256=V498IVr98Bab0SF5UkUffRYgDEuJYIj9cL94KCLJcUU,586
-compose_chart_export-0.0.15rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.15rc1.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.15rc1.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.15rc1.dist-info/RECORD,,
+compose_chart_export-0.0.15rc2.dist-info/METADATA,sha256=ZrAxW3u3b6iGZ1q5VlA5YHQ3IMF5lQifspKpF_Cc1xE,586
+compose_chart_export-0.0.15rc2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.15rc2.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.15rc2.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.15rc2.dist-info/RECORD,,
```

