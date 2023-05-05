# Comparing `tmp/CSV to JSON Python-260.tar.gz` & `tmp/CSV_to_JSON_Python-413-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CSV to JSON Python-260.tar", last modified: Fri May  5 21:00:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

