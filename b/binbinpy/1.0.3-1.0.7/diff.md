# Comparing `tmp/binbinpy-1.0.3.tar.gz` & `tmp/binbinpy-1.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sher/Desktop/Sher/python/demopackage/dist/.tmp-muytr0ab/binbinpy-1.0.3.tar", last modified: Fri May  5 10:11:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

