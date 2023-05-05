# Comparing `tmp/compose_chart_export-0.0.15rc3-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.15rc4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13081 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 09:54 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 23-May-05 09:54 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    13551 b- defN 23-May-05 09:54 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4967 b- defN 23-May-05 09:54 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-05 09:54 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9380 b- defN 23-May-05 09:54 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2359 b- defN 23-May-05 09:54 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-05 09:54 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      586 b- defN 23-May-05 09:54 compose_chart_export-0.0.15rc3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 09:54 compose_chart_export-0.0.15rc3.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-05 09:54 compose_chart_export-0.0.15rc3.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-05 09:54 compose_chart_export-0.0.15rc3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1214 b- defN 23-May-05 09:54 compose_chart_export-0.0.15rc3.dist-info/RECORD
-13 files, 37107 bytes uncompressed, 10995 bytes compressed:  70.4%
+Zip file size: 13232 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 10:09 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 23-May-05 10:09 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14200 b- defN 23-May-05 10:09 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4967 b- defN 23-May-05 10:09 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-May-05 10:09 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9380 b- defN 23-May-05 10:09 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2359 b- defN 23-May-05 10:09 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-May-05 10:09 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      586 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1214 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/RECORD
+13 files, 37756 bytes uncompressed, 11146 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc3.dist-info/METADATA
+Filename: compose_chart_export-0.0.15rc4.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc3.dist-info/WHEEL
+Filename: compose_chart_export-0.0.15rc4.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc3.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.15rc4.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc3.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.15rc4.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc3.dist-info/RECORD
+Filename: compose_chart_export-0.0.15rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compose_chart_export/chart_file_templates.py

```diff
@@ -223,23 +223,38 @@
 {{- end -}}
 
 {{- define "common.labels.matchLabels" -}}
 app.kubernetes.io/name: {{ .Chart.Name }}
 app.kubernetes.io/instance: {{ .Release.Name }}
 {{- end -}}
 """
+_service_account_tpl = """
+# Template from
+# https://github.com/influxdata/helm-charts/blob/master/charts/telegraf-ds/templates/_helpers.tpl#L400
+{{- define "APP_NAME.serviceAccountName" -}}
+{{- if .Values.serviceAccount.create -}}
+    {{ .Values.serviceAccount.name }}
+{{- else -}}
+    {{ default "default" .Values.serviceAccount.name }}
+{{- end -}}
+{{- end -}}
+"""
 
 
 def helpers_tpl(spec: ChartTemplateSpec) -> str:
     helpers_tpl_content = spec.replacements.replace(_HELPERS_TPL)
     extra_labels_str = "\n"
     if extra_labels := spec.extra_labels:
         extra_labels_str = "\n".join(
             f"{key}: {value}" for key, value in extra_labels.items()
         )
+    if spec.use_service_account:
+        helpers_tpl_content += _service_account_tpl.replace(
+            "APP_NAME", spec.replacements.APP_NAME
+        )
     helpers_tpl_content = helpers_tpl_content.replace("EXTRA_LABELS", extra_labels_str)
     return helpers_tpl_content
 
 
 _DEPLOYMENT_YAML = """\
 apiVersion: apps/v1
 kind: Deployment
@@ -287,16 +302,20 @@
 def _add_template_spec(template: str, spec: ChartTemplateSpec):
     with TemporaryDirectory() as path:
         deploy_file = Path(path) / "template.yaml"
         deploy_file.write_text(template)
         with edit_helm_template(
             deploy_file, yaml_path="spec.template.spec"
         ) as file_spec:  # type: dict
-            if service_account_name := spec.service_account_name:
-                file_spec["serviceAccountName"] = service_account_name
+            if spec.use_service_account:
+                file_spec[
+                    "serviceAccountName"
+                ] = '{{ template "APP_NAME.serviceAccountName" . }}'.replace(
+                    "APP_NAME", spec.replacements.APP_NAME
+                )
             containers: list = file_spec["containers"]
             for name, value_name in spec.container_name_value_name:
                 container_spec = dict(
                     name=name,
                     image="{{ .Values.%s.image | quote }}" % value_name,
                     imagePullPolicy="IfNotPresent",
                     resources="{{- toYaml .Values.resources | nindent 10 }}"
```

## Comparing `compose_chart_export-0.0.15rc3.dist-info/METADATA` & `compose_chart_export-0.0.15rc4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.15rc3
+Version: 0.0.15rc4
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Requires-Dist: docker-compose-parser (==0.0.15)
 Requires-Dist: model-lib (==0.0.15)
```

## Comparing `compose_chart_export-0.0.15rc3.dist-info/RECORD` & `compose_chart_export-0.0.15rc4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 compose_chart_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 compose_chart_export/chart_export.py,sha256=oDgolV_QNeF12D2xh2D9xhn45IQSbKDMmj2WRZ2UTaI,2534
-compose_chart_export/chart_file_templates.py,sha256=eHEMRh0YJP1hbYxWu2S8tmEDFZ97uMmLvE0OIvIAZhQ,13551
+compose_chart_export/chart_file_templates.py,sha256=bG35ma5Un9_18GpPiB5MYdKtvbZOQ-4zzEn7oCv0rSs,14200
 compose_chart_export/chart_mods.py,sha256=Zn-NSYhv7jJfUtGs6V--fquIolVqFT3bwL8mSWrwgOI,4967
 compose_chart_export/chart_read.py,sha256=chwkPcucA6dLWStADbP2kpAGNbhYVMms9zmPjNIQrLs,2211
 compose_chart_export/compose_export.py,sha256=w0ionkwWLTGOz9Lf2MIZVTRrUAjj7_pzmhJOxU80ZZw,9380
 compose_chart_export/ports.py,sha256=06WBSFYTUEPUYh9x4U5BjjUeE-EPNCs1Pot6MO7zxD4,2359
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.15rc3.dist-info/METADATA,sha256=9HYY7nCgFzWkcO7JXpmN-bSisH6cnU1Tioh1txRwbJE,586
-compose_chart_export-0.0.15rc3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.15rc3.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.15rc3.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.15rc3.dist-info/RECORD,,
+compose_chart_export-0.0.15rc4.dist-info/METADATA,sha256=2sFIxXvY3vSrO3mmYAoniFD49LzOIawzFpn3M7lTULk,586
+compose_chart_export-0.0.15rc4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.15rc4.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.15rc4.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.15rc4.dist-info/RECORD,,
```

