# Comparing `tmp/pants_py_deploy-0.0.15rc2-py3-none-any.whl.zip` & `tmp/pants_py_deploy-0.0.15rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10732 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 14:48 pants_py_deploy/__init__.py
--rw-r--r--  2.0 unx     4618 b- defN 23-May-03 14:48 pants_py_deploy/compose_file.py
--rw-r--r--  2.0 unx     7083 b- defN 23-May-03 14:48 pants_py_deploy/export_env.py
--rw-r--r--  2.0 unx      606 b- defN 23-May-03 14:48 pants_py_deploy/fields.py
--rw-r--r--  2.0 unx     3534 b- defN 23-May-03 14:48 pants_py_deploy/models.py
--rw-r--r--  2.0 unx     9260 b- defN 23-May-03 14:48 pants_py_deploy/plugin.py
--rw-r--r--  2.0 unx      482 b- defN 23-May-03 14:48 pants_py_deploy/register.py
--rw-r--r--  2.0 unx     2256 b- defN 23-May-03 14:48 pants_py_deploy-0.0.15rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 14:48 pants_py_deploy-0.0.15rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-03 14:48 pants_py_deploy-0.0.15rc2.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-03 14:48 pants_py_deploy-0.0.15rc2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1041 b- defN 23-May-03 14:48 pants_py_deploy-0.0.15rc2.dist-info/RECORD
-12 files, 28989 bytes uncompressed, 8952 bytes compressed:  69.1%
+Zip file size: 10808 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 06:58 pants_py_deploy/__init__.py
+-rw-r--r--  2.0 unx     4618 b- defN 23-May-05 06:58 pants_py_deploy/compose_file.py
+-rw-r--r--  2.0 unx     7083 b- defN 23-May-05 06:58 pants_py_deploy/export_env.py
+-rw-r--r--  2.0 unx      606 b- defN 23-May-05 06:58 pants_py_deploy/fields.py
+-rw-r--r--  2.0 unx     3534 b- defN 23-May-05 06:58 pants_py_deploy/models.py
+-rw-r--r--  2.0 unx     9499 b- defN 23-May-05 06:58 pants_py_deploy/plugin.py
+-rw-r--r--  2.0 unx      482 b- defN 23-May-05 06:58 pants_py_deploy/register.py
+-rw-r--r--  2.0 unx     2256 b- defN 23-May-05 06:58 pants_py_deploy-0.0.15rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 06:58 pants_py_deploy-0.0.15rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 06:58 pants_py_deploy-0.0.15rc3.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-05 06:58 pants_py_deploy-0.0.15rc3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1041 b- defN 23-May-05 06:58 pants_py_deploy-0.0.15rc3.dist-info/RECORD
+12 files, 29228 bytes uncompressed, 9028 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pants_py_deploy/plugin.py
 Comment: 
 
 Filename: pants_py_deploy/register.py
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc2.dist-info/METADATA
+Filename: pants_py_deploy-0.0.15rc3.dist-info/METADATA
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc2.dist-info/WHEEL
+Filename: pants_py_deploy-0.0.15rc3.dist-info/WHEEL
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc2.dist-info/namespace_packages.txt
+Filename: pants_py_deploy-0.0.15rc3.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc2.dist-info/top_level.txt
+Filename: pants_py_deploy-0.0.15rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc2.dist-info/RECORD
+Filename: pants_py_deploy-0.0.15rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pants_py_deploy/plugin.py

```diff
@@ -81,14 +81,22 @@
             Get(ComposeExportChart, ComposeExportChartRequest(service, chart_path))
         )
     exports = await MultiGet(requests)
     charts = {export.chart_path: export.files for export in exports}
     return HelmChartsExported(charts)
 
 
+def as_chart_version(image_tag: str) -> str:
+    """
+    >>> as_chart_version('0.0.1-latest-amd')
+    '0.0.1-latest-chart'
+    """
+    return ensure_suffix(image_tag.removesuffix("-amd").removesuffix("-arm"), "-chart")
+
+
 @rule
 async def export_helm_chart(request: ComposeExportChartRequest) -> ComposeExportChart:
     chart_yaml_path = request.chart_path
     chart_path = PurePath(chart_yaml_path).parent
     chart_digest: Optional[DigestContents] = None
 
     def store_digest(exported_chart_path: Path):
@@ -113,15 +121,15 @@
             compose_yaml = as_compose_yaml([service], digest[0])
         else:
             compose_yaml = as_new_compose_yaml([service])
         docker_compose_path = Path(tmpdir) / "docker-compose.yaml"
         docker_compose_path.write_text(compose_yaml)
         export_from_compose(
             compose_path=docker_compose_path,
-            chart_version=service.image_tag,
+            chart_version=as_chart_version(service.image_tag),
             chart_name=service.chart_inferred_name,
             image_url=service.image_url,
             on_exported=store_digest,
         )
     assert chart_digest
     return ComposeExportChart(chart_path=chart_yaml_path, files=chart_digest)
```

## Comparing `pants_py_deploy-0.0.15rc2.dist-info/METADATA` & `pants_py_deploy-0.0.15rc3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pants-py-deploy
-Version: 0.0.15rc2
+Version: 0.0.15rc3
 Summary: Make it easy to maintain docker-compose files and helm-charts across projects with pants-py-deploy
 Home-page: https://github.com/EspenAlbert/py-libs
 Author: Espen Albert
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: <3.10,>=3.9
 Description-Content-Type: text/markdown
```

## Comparing `pants_py_deploy-0.0.15rc2.dist-info/RECORD` & `pants_py_deploy-0.0.15rc3.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pants_py_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pants_py_deploy/compose_file.py,sha256=kl6m34S_tdU1SxirGM5FEasPeqqjb_jUndwA2AQBO4c,4618
 pants_py_deploy/export_env.py,sha256=z0a7Sa2Lc4_7cFf9oH7rdoHjUqHgU-e6oshAQ9bm1Yg,7083
 pants_py_deploy/fields.py,sha256=entMoIWLwKiEwOBBr54Mi9CDX6HdqLDdo8RZ-aDIJP4,606
 pants_py_deploy/models.py,sha256=96cqQqW1w3z-tZhthlOyGozL4YwR93H_FVEkipH0qsA,3534
-pants_py_deploy/plugin.py,sha256=-OMXkbL3J-yeassGXoMsDbO9ih-Lx6Z_ijE55ZG55TA,9260
+pants_py_deploy/plugin.py,sha256=28pNAMjmmJv8ETQN7uCeZc_MGFYvzeDBETeurDag3Sw,9499
 pants_py_deploy/register.py,sha256=DdsyxfuCEzkruWOItCsoYMpTN75iBkQ1df25Si46KZk,482
-pants_py_deploy-0.0.15rc2.dist-info/METADATA,sha256=L1VVwIczyq_yi3Ib06R6HfgE_uKVSNbUVDsdPNOauFo,2256
-pants_py_deploy-0.0.15rc2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pants_py_deploy-0.0.15rc2.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pants_py_deploy-0.0.15rc2.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
-pants_py_deploy-0.0.15rc2.dist-info/RECORD,,
+pants_py_deploy-0.0.15rc3.dist-info/METADATA,sha256=thJKhGWmJkLrem1IifpR8fdKRhM9JEkEKoycHdgm3Qw,2256
+pants_py_deploy-0.0.15rc3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pants_py_deploy-0.0.15rc3.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pants_py_deploy-0.0.15rc3.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
+pants_py_deploy-0.0.15rc3.dist-info/RECORD,,
```

