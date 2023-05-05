# Comparing `tmp/Qcover-2.4.0.tar.gz` & `tmp/Qcover-2.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qcover-2.4.0.tar", last modified: Sun Apr 23 09:13:05 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

