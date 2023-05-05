# Comparing `tmp/transcribe-anything-2.1.2.tar.gz` & `tmp/transcribe_anything-2.2.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe-anything-2.1.2.tar", last modified: Mon Mar 20 23:50:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

