# Comparing `tmp/ml-infer-0.0.1.tar.gz` & `tmp/ml_infer-0.0.3-cp310-cp310-macosx_11_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-infer-0.0.1.tar", last modified: Thu Apr 27 04:57:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

