# Comparing `tmp/remodnav-1.1.1.tar.gz` & `tmp/remodnav-1.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remodnav-1.1.1.tar", last modified: Wed Dec  1 11:05:12 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

