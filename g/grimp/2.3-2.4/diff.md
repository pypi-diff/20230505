# Comparing `tmp/grimp-2.3.tar.gz` & `tmp/grimp-2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimp-2.3.tar", last modified: Fri Mar  3 11:21:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

