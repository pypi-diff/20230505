# Comparing `tmp/packagebinbin-0.0.5.tar.gz` & `tmp/packagebinbin-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/packagebinbin-0.0.5.tar", last modified: Fri May  5 08:47:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

