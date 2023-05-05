# Comparing `tmp/VikyTest-2.0.tar.gz` & `tmp/VikyTest-3.0-py38-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VikyTest-2.0.tar", last modified: Fri May  5 06:06:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

