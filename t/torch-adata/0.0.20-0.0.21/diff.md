# Comparing `tmp/torch-adata-0.0.20.tar.gz` & `tmp/torch_adata-0.0.21-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-adata-0.0.20.tar", last modified: Tue Feb  7 20:23:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

