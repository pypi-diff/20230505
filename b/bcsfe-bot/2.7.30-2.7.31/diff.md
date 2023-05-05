# Comparing `tmp/bcsfe-bot-2.7.30.tar.gz` & `tmp/bcsfe_bot-2.7.31-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcsfe-bot-2.7.30.tar", last modified: Fri May  5 04:21:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

