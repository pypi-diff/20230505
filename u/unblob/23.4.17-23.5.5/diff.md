# Comparing `tmp/unblob-23.4.17.tar.gz` & `tmp/unblob-23.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unblob-23.4.17.tar", max compression
+gzip compressed data, was "unblob-23.5.5.tar", max compression
```

## Comparing `unblob-23.4.17.tar` & `unblob-23.5.5.tar`

### file list

```diff
@@ -1,86 +1,79 @@
--rw-r--r--   0        0        0     2255 2023-04-17 21:01:21.439076 unblob-23.4.17/LICENSE
--rw-r--r--   0        0        0     1246 2023-04-17 21:01:21.439076 unblob-23.4.17/build.py
--rw-r--r--   0        0        0     4470 2023-04-17 21:01:21.443076 unblob-23.4.17/pyproject.toml
--rw-r--r--   0        0        0      329 2023-04-17 21:01:21.443076 unblob-23.4.17/rust/Cargo.toml
--rw-r--r--   0        0        0      947 2023-04-17 21:01:21.443076 unblob-23.4.17/rust/benches/benches_main.rs
--rw-r--r--   0        0        0      398 2023-04-17 21:01:21.443076 unblob-23.4.17/rust/src/lib.rs
--rw-r--r--   0        0        0      626 2023-04-17 21:01:21.443076 unblob-23.4.17/rust/src/math.rs
--rw-r--r--   0        0        0        0 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/__init__.py
--rw-r--r--   0        0        0      136 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/_py/__init__.py
--rw-r--r--   0        0        0      275 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/_py/math.py
--rwxr-xr-x   0        0        0     6954 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/cli.py
--rw-r--r--   0        0        0      344 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/cli_options.py
--rw-r--r--   0        0        0     1044 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/dependencies.py
--rw-r--r--   0        0        0     3473 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/extractor.py
--rw-r--r--   0        0        0      196 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/extractors/README.md
--rw-r--r--   0        0        0       40 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/extractors/__init__.py
--rw-r--r--   0        0        0     3013 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/extractors/command.py
--rw-r--r--   0        0        0    10439 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/file_utils.py
--rw-r--r--   0        0        0     5259 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/finder.py
--rw-r--r--   0        0        0     2329 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/handlers/archive/__init__.py
--rw-r--r--   0        0        0      924 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/handlers/archive/_safe_tarfile.py
--rw-r--r--   0        0        0     1694 2023-04-17 21:01:21.843075 unblob-23.4.17/unblob/handlers/archive/ar.py
--rw-r--r--   0        0        0     2775 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/arc.py
--rw-r--r--   0        0        0     5683 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/arj.py
--rw-r--r--   0        0        0     2505 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/cab.py
--rw-r--r--   0        0        0     7632 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/cpio.py
--rw-r--r--   0        0        0     2250 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/dlink/encrpted_img.py
--rw-r--r--   0        0        0     3589 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/dlink/shrs.py
--rw-r--r--   0        0        0     3700 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/dmg.py
--rw-r--r--   0        0        0     3018 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/engeniustech/engenius.py
--rw-r--r--   0        0        0     3282 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/hp/bdl.py
--rw-r--r--   0        0        0     3689 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/hp/ipkg.py
--rw-r--r--   0        0        0     2946 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/instar/bneg.py
--rw-r--r--   0        0        0     2553 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/netgear/chk.py
--rw-r--r--   0        0        0     3895 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/netgear/trx.py
--rw-r--r--   0        0        0     5527 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/qnap/qnap_nas.py
--rw-r--r--   0        0        0     1158 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/rar.py
--rw-r--r--   0        0        0     2591 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/sevenzip.py
--rw-r--r--   0        0        0     2332 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/stuffit.py
--rw-r--r--   0        0        0     4298 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/tar.py
--rw-r--r--   0        0        0     6107 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/xiaomi/hdr.py
--rw-r--r--   0        0        0     6354 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/archive/zip.py
--rw-r--r--   0        0        0        0 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/__init__.py
--rw-r--r--   0        0        0     1074 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/_gzip_reader.py
--rw-r--r--   0        0        0     4693 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/bzip2.py
--rw-r--r--   0        0        0     8898 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/compress.py
--rw-r--r--   0        0        0     3800 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/gzip.py
--rw-r--r--   0        0        0     5675 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/lz4.py
--rw-r--r--   0        0        0     2876 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/lzh.py
--rw-r--r--   0        0        0     1423 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/lzip.py
--rw-r--r--   0        0        0     3508 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/lzma.py
--rw-r--r--   0        0        0     4147 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/lzo.py
--rw-r--r--   0        0        0     6073 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/xz.py
--rw-r--r--   0        0        0     1935 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/zlib.py
--rw-r--r--   0        0        0     2662 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/compression/zstd.py
--rw-r--r--   0        0        0        0 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/executable/__init__.py
--rw-r--r--   0        0        0    15477 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/executable/elf.py
--rw-r--r--   0        0        0        0 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/android/__init__.py
--rw-r--r--   0        0        0     2889 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/android/sparse.py
--rw-r--r--   0        0        0     2320 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/cramfs.py
--rw-r--r--   0        0        0     4841 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/extfs.py
--rw-r--r--   0        0        0     6278 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/fat.py
--rw-r--r--   0        0        0     4604 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/iso9660.py
--rw-r--r--   0        0        0     5213 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/jffs2.py
--rw-r--r--   0        0        0     2246 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/ntfs.py
--rw-r--r--   0        0        0    13617 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/romfs.py
--rw-r--r--   0        0        0     9619 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/squashfs.py
--rw-r--r--   0        0        0     5738 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/ubi.py
--rw-r--r--   0        0        0    28094 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/handlers/filesystem/yaffs.py
--rw-r--r--   0        0        0      315 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/hookspecs.py
--rw-r--r--   0        0        0      515 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/identifiers.py
--rw-r--r--   0        0        0      587 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/iter_utils.py
--rw-r--r--   0        0        0     3739 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/logging.py
--rw-r--r--   0        0        0      136 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/math.py
--rw-r--r--   0        0        0     9886 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/models.py
--rw-r--r--   0        0        0     2252 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/parser.py
--rw-r--r--   0        0        0     3408 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/plugins.py
--rw-r--r--   0        0        0     4090 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/pool.py
--rw-r--r--   0        0        0    18736 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/processing.py
--rw-r--r--   0        0        0        0 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/py.typed
--rw-r--r--   0        0        0     4811 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/report.py
--rw-r--r--   0        0        0     1538 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/signals.py
--rw-r--r--   0        0        0     3272 2023-04-17 21:01:21.847075 unblob-23.4.17/unblob/testing.py
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 unblob-23.4.17/PKG-INFO
+-rw-r--r--   0        0        0     2255 2023-05-05 14:46:44.706125 unblob-23.5.5/LICENSE
+-rw-r--r--   0        0        0     4348 2023-05-05 14:46:44.710125 unblob-23.5.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/__init__.py
+-rwxr-xr-x   0        0        0     6954 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/cli.py
+-rw-r--r--   0        0        0      344 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/cli_options.py
+-rw-r--r--   0        0        0     1044 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/dependencies.py
+-rw-r--r--   0        0        0     4100 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/extractor.py
+-rw-r--r--   0        0        0      196 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/extractors/README.md
+-rw-r--r--   0        0        0       40 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/extractors/__init__.py
+-rw-r--r--   0        0        0     3013 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/extractors/command.py
+-rw-r--r--   0        0        0    10384 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/file_utils.py
+-rw-r--r--   0        0        0     5715 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/finder.py
+-rw-r--r--   0        0        0     2371 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/__init__.py
+-rw-r--r--   0        0        0     1218 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/_safe_tarfile.py
+-rw-r--r--   0        0        0     1694 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/ar.py
+-rw-r--r--   0        0        0     2775 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/arc.py
+-rw-r--r--   0        0        0     5683 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/arj.py
+-rw-r--r--   0        0        0     2505 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/cab.py
+-rw-r--r--   0        0        0     7632 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/cpio.py
+-rw-r--r--   0        0        0     2250 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/dlink/encrpted_img.py
+-rw-r--r--   0        0        0     3589 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/dlink/shrs.py
+-rw-r--r--   0        0        0     3700 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/dmg.py
+-rw-r--r--   0        0        0     3018 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/engeniustech/engenius.py
+-rw-r--r--   0        0        0     3282 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/hp/bdl.py
+-rw-r--r--   0        0        0     3689 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/hp/ipkg.py
+-rw-r--r--   0        0        0     2946 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/instar/bneg.py
+-rw-r--r--   0        0        0     1416 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/instar/instar_hd.py
+-rw-r--r--   0        0        0     2553 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/netgear/chk.py
+-rw-r--r--   0        0        0     3895 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/netgear/trx.py
+-rw-r--r--   0        0        0     5527 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/qnap/qnap_nas.py
+-rw-r--r--   0        0        0     1158 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/rar.py
+-rw-r--r--   0        0        0     2591 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/sevenzip.py
+-rw-r--r--   0        0        0     2332 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/stuffit.py
+-rw-r--r--   0        0        0     4298 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/tar.py
+-rw-r--r--   0        0        0     6107 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/xiaomi/hdr.py
+-rw-r--r--   0        0        0     6412 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/zip.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/_gzip_reader.py
+-rw-r--r--   0        0        0     4693 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/bzip2.py
+-rw-r--r--   0        0        0     8898 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/compress.py
+-rw-r--r--   0        0        0     3800 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/gzip.py
+-rw-r--r--   0        0        0     5675 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/lz4.py
+-rw-r--r--   0        0        0     2876 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/lzh.py
+-rw-r--r--   0        0        0     1423 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/lzip.py
+-rw-r--r--   0        0        0     3508 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/lzma.py
+-rw-r--r--   0        0        0     4147 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/lzo.py
+-rw-r--r--   0        0        0     6073 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/xz.py
+-rw-r--r--   0        0        0     1935 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/zlib.py
+-rw-r--r--   0        0        0     2662 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/zstd.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/executable/__init__.py
+-rw-r--r--   0        0        0    15477 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/executable/elf.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/android/__init__.py
+-rw-r--r--   0        0        0     2889 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/android/sparse.py
+-rw-r--r--   0        0        0     2320 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/cramfs.py
+-rw-r--r--   0        0        0     4841 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/extfs.py
+-rw-r--r--   0        0        0     6278 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/fat.py
+-rw-r--r--   0        0        0     4604 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/iso9660.py
+-rw-r--r--   0        0        0     5213 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/jffs2.py
+-rw-r--r--   0        0        0     2246 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/ntfs.py
+-rw-r--r--   0        0        0    13617 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/romfs.py
+-rw-r--r--   0        0        0     9619 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/squashfs.py
+-rw-r--r--   0        0        0     5738 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/ubi.py
+-rw-r--r--   0        0        0    28094 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/yaffs.py
+-rw-r--r--   0        0        0      315 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/hookspecs.py
+-rw-r--r--   0        0        0      515 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/identifiers.py
+-rw-r--r--   0        0        0      587 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/iter_utils.py
+-rw-r--r--   0        0        0     3739 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/logging.py
+-rw-r--r--   0        0        0     9964 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/models.py
+-rw-r--r--   0        0        0     2252 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/parser.py
+-rw-r--r--   0        0        0     3408 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/plugins.py
+-rw-r--r--   0        0        0     4090 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/pool.py
+-rw-r--r--   0        0        0    19578 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/processing.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/py.typed
+-rw-r--r--   0        0        0     5120 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/report.py
+-rw-r--r--   0        0        0     1538 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/signals.py
+-rw-r--r--   0        0        0     3336 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/testing.py
+-rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 unblob-23.5.5/PKG-INFO
```

### Comparing `unblob-23.4.17/LICENSE` & `unblob-23.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/pyproject.toml` & `unblob-23.5.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 [tool.poetry]
 name = "unblob"
-version = "23.4.17"
+version = "23.5.5"
 description = "Extract files from any kind of container formats"
 authors = ["ONEKEY <support@onekey.com>"]
 license = "MIT"
 packages = [
     { include = "unblob" },
 ]
-include = ["rust/*", "rust/src/*"]
-build = "build.py"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
 "dissect.cstruct" = "^2.0"
 attrs = "^22.2.0"
 structlog = "^21.2.0"
 arpy = "^2.2.0"
 rarfile = "^4.0"
 ubi-reader = "^0.8.5"
 python-lzo = "^1.14"
 plotext = ">=4.2.0,<6.0"
 pluggy = "^1.0.0"
 python-magic = "^0.4.27"
-pyperscan = "^0.2.0"
+pyperscan = "^0.2.2"
 lark = "^1.1.2"
 lz4 = "^4.0.0"
 lief = "^0.12.3"
 jefferson = "^0.4.2"
-cryptography = ">=37.0.1,<40.0"
+cryptography = ">=39.0,<41.0"
 treelib = "^1.6.1"
+unblob-native = "^0.1.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.4"
 pyright = "^0.0.12"
 pre-commit = "^2.15.0"
 pytest-cov = "^3.0.0"
 ruff = "^0.0.259"
-setuptools-rust = "^1.1.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "8.5.10"
 mkdocstrings = "^0.19.1"
@@ -145,15 +143,15 @@
   build
   target
   tests/integration
 """
 
 [tool.vulture]
 paths = ["unblob/", "vulture_whitelist.py" ]
-exclude = ["unblob/_py/", "unblob/testing.py"]
+exclude = ["unblob/testing.py"]
 
 [tool.pyright]
 exclude = ["build"]
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools>=60.9.3", "setuptools-rust==1.5.1"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `unblob-23.4.17/unblob/cli.py` & `unblob-23.5.5/unblob/cli.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/dependencies.py` & `unblob-23.5.5/unblob/dependencies.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/extractor.py` & `unblob-23.5.5/unblob/extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """File extraction related functions."""
+import errno
 import os
 from pathlib import Path
 
 from structlog import get_logger
 
 from .file_utils import iterate_file
 from .models import Chunk, File, TaskResult, UnknownChunk, ValidChunk
@@ -57,15 +58,21 @@
         error_report = MaliciousSymlinkRemoved(
             link=path.as_posix(), target=os.readlink(path)
         )
         task_result.add_report(error_report)
         path.unlink()
         return path
 
-    target = Path(os.readlink(path))
+    raw_target = os.readlink(path)
+    if not raw_target:
+        logger.error("Symlink with empty target, removing.")
+        path.unlink()
+        return path
+
+    target = Path(raw_target)
 
     if target.is_absolute():
         target = Path(target.as_posix().lstrip("/"))
     else:
         target = path.resolve()
 
     safe = is_safe_path(outdir, target)
@@ -81,20 +88,32 @@
         relative_target = os.path.relpath(outdir.joinpath(target), start=path.parent)
         path.unlink()
         path.symlink_to(relative_target)
     return path
 
 
 def fix_extracted_directory(outdir: Path, task_result: TaskResult):
+    def _fix_extracted_directory(directory: Path):
+        if not directory.exists():
+            return
+        for path in (directory / p for p in os.listdir(directory)):
+            try:
+                fix_permission(path)
+                if path.is_symlink():
+                    fix_symlink(path, outdir, task_result)
+                    continue
+                if path.is_dir():
+                    _fix_extracted_directory(path)
+            except OSError as e:
+                if e.errno == errno.ENAMETOOLONG:
+                    continue
+                raise e from None
+
     fix_permission(outdir)
-    for path in outdir.rglob("*"):
-        if path.is_symlink():
-            fix_symlink(path, outdir, task_result)
-        else:
-            fix_permission(path)
+    _fix_extracted_directory(outdir)
 
 
 def carve_unknown_chunk(extract_dir: Path, file: File, chunk: UnknownChunk) -> Path:
     filename = f"{chunk.start_offset}-{chunk.end_offset}.unknown"
     carve_path = extract_dir / filename
     logger.info("Extracting unknown chunk", path=carve_path, chunk=chunk)
     carve_chunk_to_file(carve_path, file, chunk)
```

### Comparing `unblob-23.4.17/unblob/extractors/command.py` & `unblob-23.5.5/unblob/extractors/command.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/file_utils.py` & `unblob-23.5.5/unblob/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 import shutil
 import struct
 from pathlib import Path
 from typing import Iterator, List, Tuple, Union
 
 from dissect.cstruct import cstruct
-from pyperscan import Scan
 
 from .logging import format_hex
 
 DEFAULT_BUFSIZE = shutil.COPY_BUFSIZE  # type: ignore
 
 
 class SeekError(ValueError):
@@ -25,17 +24,18 @@
     def from_bytes(cls, content: bytes):
         m = cls(-1, len(content))
         m.write(content)
         m.seek(0)
         return m
 
     @classmethod
-    def from_path(cls, path: Path):
-        with path.open("rb") as base_file:
-            return cls(base_file.fileno(), 0, access=mmap.ACCESS_READ)
+    def from_path(cls, path: Path, access=mmap.ACCESS_READ):
+        mode = "r+b" if access == mmap.ACCESS_WRITE else "rb"
+        with path.open(mode) as base_file:
+            return cls(base_file.fileno(), 0, access=access)
 
     def seek(self, pos: int, whence: int = os.SEEK_SET) -> int:
         try:
             super().seek(pos, whence)
         except ValueError as e:
             raise SeekError from e
         return self.tell()
@@ -250,17 +250,15 @@
             break
 
         yield data
 
 
 def stream_scan(scanner, file: File):
     """Scan the whole file by increment of DEFAULT_BUFSIZE using Hyperscan's streaming mode."""
-    for i in range(0, file.size(), DEFAULT_BUFSIZE):
-        if scanner.scan(file[i : i + DEFAULT_BUFSIZE]) == Scan.Terminate:
-            break
+    scanner.scan(file, DEFAULT_BUFSIZE)
 
 
 class StructParser:
     """Wrapper for dissect.cstruct to handle different endianness parsing dynamically."""
 
     def __init__(self, definitions: str):
         self._definitions = definitions
```

### Comparing `unblob-23.4.17/unblob/finder.py` & `unblob-23.5.5/unblob/finder.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 from functools import lru_cache
 from typing import List, Optional
 
 import attr
 from pyperscan import Flag, Pattern, Scan, StreamDatabase
 from structlog import get_logger
 
-from .file_utils import InvalidInputFormat, SeekError, stream_scan
+from .file_utils import DEFAULT_BUFSIZE, InvalidInputFormat, SeekError
 from .handlers import Handlers
 from .models import File, Handler, TaskResult, ValidChunk
 from .parser import InvalidHexString
 from .report import CalculateChunkExceptionReport
 
 logger = get_logger()
 
 
 @attr.define
 class HyperscanMatchContext:
     file: File
     file_size: int
     all_chunks: List
     task_result: TaskResult
+    start_offset: int
 
 
 def _calculate_chunk(
     handler: Handler, file: File, real_offset, task_result: TaskResult
 ) -> Optional[ValidChunk]:
     file.seek(real_offset)
     try:
@@ -65,14 +66,15 @@
         )
 
 
 def _hyperscan_match(
     context: HyperscanMatchContext, handler: Handler, offset: int, end: int
 ) -> Scan:
     del end  # unused argument
+    offset += context.start_offset
     real_offset = offset + handler.PATTERN_MATCH_OFFSET
 
     if real_offset < 0:
         return Scan.Continue
 
     # Skip chunk calculation if this would start inside another one,
     # similar to remove_inner_chunks, but before we even begin calculating.
@@ -86,36 +88,45 @@
         return Scan.Continue
 
     logger.debug(
         "Calculating chunk for pattern match",
         start_offset=offset,
         real_offset=real_offset,
         _verbosity=2,
+        handler=handler.NAME,
     )
 
     chunk = _calculate_chunk(handler, context.file, real_offset, context.task_result)
 
     # We found some random bytes this handler couldn't parse
     if chunk is None:
         return Scan.Continue
 
     if chunk.end_offset > context.file_size:
         logger.debug("Chunk overflows file", chunk=chunk, _verbosity=2)
         return Scan.Continue
 
     chunk.handler = handler
-    logger.debug("Found valid chunk", chunk=chunk, handler=handler.NAME, _verbosity=2)
+    logger.debug("Found valid chunk", chunk=chunk, handler=handler.NAME, _verbosity=1)
     context.all_chunks.append(chunk)
+    context.start_offset = chunk.end_offset
 
-    # Terminate scan if we match till the end of the file
-    if chunk.end_offset == context.file_size:
-        logger.debug("Chunk covers till end of the file", chunk=chunk)
-        return Scan.Terminate
+    return Scan.Terminate
 
-    return Scan.Continue
+
+def stream_scan_chunks(scanner, file: File, context: HyperscanMatchContext):
+    """Scan the whole file by increment of DEFAULT_BUFSIZE using Hyperscan's streaming mode."""
+    i = context.start_offset
+    with memoryview(file) as data:
+        while i < file.size():
+            if scanner.scan(data[i : i + DEFAULT_BUFSIZE]) == Scan.Terminate:
+                scanner.reset()
+                i = context.start_offset
+            else:
+                i += DEFAULT_BUFSIZE
 
 
 def search_chunks(
     file: File,
     file_size: int,
     handlers: Handlers,
     task_result: TaskResult,
@@ -132,20 +143,21 @@
     hyperscan_db = build_hyperscan_database(handlers)
 
     hyperscan_context = HyperscanMatchContext(
         file=file,
         file_size=file_size,
         all_chunks=all_chunks,
         task_result=task_result,
+        start_offset=0,
     )
 
     scanner = hyperscan_db.build(hyperscan_context, _hyperscan_match)
 
     try:
-        stream_scan(scanner, file)
+        stream_scan_chunks(scanner, file, hyperscan_context)
     except Exception as e:
         logger.error(
             "Error scanning for patterns",
             error=e,
         )
 
     logger.debug(
```

### Comparing `unblob-23.4.17/unblob/handlers/__init__.py` & `unblob-23.5.5/unblob/handlers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ..models import Handlers
 from .archive import ar, arc, arj, cab, cpio, dmg, rar, sevenzip, stuffit, tar, zip
 from .archive.dlink import encrpted_img, shrs
 from .archive.engeniustech import engenius
 from .archive.hp import bdl, ipkg
-from .archive.instar import bneg
+from .archive.instar import bneg, instar_hd
 from .archive.netgear import chk, trx
 from .archive.qnap import qnap_nas
 from .archive.xiaomi import hdr
 from .compression import (
     bzip2,
     compress,
     gzip,
@@ -59,14 +59,15 @@
     encrpted_img.EncrptedHandler,
     shrs.SHRSHandler,
     hdr.HDR1Handler,
     hdr.HDR2Handler,
     qnap_nas.QnapHandler,
     bneg.BNEGHandler,
     bdl.HPBDLHandler,
+    instar_hd.InstarHDHandler,
     ipkg.HPIPKGHandler,
     sparse.SparseHandler,
     ar.ARHandler,
     arc.ARCHandler,
     arj.ARJHandler,
     cab.CABHandler,
     tar.TarHandler,
```

### Comparing `unblob-23.4.17/unblob/handlers/archive/_safe_tarfile.py` & `unblob-23.5.5/unblob/handlers/archive/_safe_tarfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,32 @@
 from structlog import get_logger
 
 from unblob.extractor import is_safe_path
 
 logger = get_logger()
 
 RUNNING_AS_ROOT = os.getuid() == 0
+MAX_PATH_LEN = 255
 
 
 class SafeTarFile(TarFile):
     def extract(
         self, member, path="", set_attrs=True, *, numeric_owner=False  # noqa: FBT002
     ):
         path_as_path = Path(str(path))
         member_name_path = Path(str(member.name))
 
+        if not member.name:
+            logger.warning("File with empty filename in tar archive. Skipping")
+            return
+
+        if len(member.name) > MAX_PATH_LEN:
+            logger.warning("File with filename too long in tar archive. Skipping")
+            return
+
         if not RUNNING_AS_ROOT and (member.ischr() or member.isblk()):
             logger.warning(
                 "missing elevated permissions, skipping block and character device creation",
                 path=member_name_path,
             )
             return
         if not is_safe_path(path_as_path, member_name_path):
```

### Comparing `unblob-23.4.17/unblob/handlers/archive/ar.py` & `unblob-23.5.5/unblob/handlers/archive/ar.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/arc.py` & `unblob-23.5.5/unblob/handlers/archive/arc.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/arj.py` & `unblob-23.5.5/unblob/handlers/archive/arj.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/cab.py` & `unblob-23.5.5/unblob/handlers/archive/cab.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/cpio.py` & `unblob-23.5.5/unblob/handlers/archive/cpio.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/dlink/encrpted_img.py` & `unblob-23.5.5/unblob/handlers/archive/dlink/encrpted_img.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/dlink/shrs.py` & `unblob-23.5.5/unblob/handlers/archive/dlink/shrs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/dmg.py` & `unblob-23.5.5/unblob/handlers/archive/dmg.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/engeniustech/engenius.py` & `unblob-23.5.5/unblob/handlers/archive/engeniustech/engenius.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/hp/bdl.py` & `unblob-23.5.5/unblob/handlers/archive/hp/bdl.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/hp/ipkg.py` & `unblob-23.5.5/unblob/handlers/archive/hp/ipkg.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/instar/bneg.py` & `unblob-23.5.5/unblob/handlers/archive/instar/bneg.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/netgear/chk.py` & `unblob-23.5.5/unblob/handlers/archive/netgear/chk.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/netgear/trx.py` & `unblob-23.5.5/unblob/handlers/archive/netgear/trx.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/qnap/qnap_nas.py` & `unblob-23.5.5/unblob/handlers/archive/qnap/qnap_nas.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/rar.py` & `unblob-23.5.5/unblob/handlers/archive/rar.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/sevenzip.py` & `unblob-23.5.5/unblob/handlers/archive/sevenzip.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/stuffit.py` & `unblob-23.5.5/unblob/handlers/archive/stuffit.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/tar.py` & `unblob-23.5.5/unblob/handlers/archive/tar.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/xiaomi/hdr.py` & `unblob-23.5.5/unblob/handlers/archive/xiaomi/hdr.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/archive/zip.py` & `unblob-23.5.5/unblob/handlers/archive/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 
 from ...extractors import Command
 from ...file_utils import InvalidInputFormat, iterate_patterns
 from ...models import File, HexString, StructHandler, ValidChunk
 
 logger = get_logger()
 
-ENCRYPTED_FLAG = 0b0001
-EOCD_RECORD_HEADER = 0x6054B50
-ZIP64_EOCD_SIGNATURE = 0x06064B50
-ZIP64_EOCD_LOCATOR_HEADER = 0x07064B50
-
 
 class ZIPHandler(StructHandler):
     NAME = "zip"
 
     PATTERNS = [HexString("50 4B 03 04 // Local file header only")]
     C_DEFINITIONS = r"""
 
@@ -82,24 +77,29 @@
 
     """
     HEADER_STRUCT = "end_of_central_directory_t"
 
     # empty password with -p will make sure the command will not hang
     EXTRACTOR = Command("7z", "x", "-p", "-y", "{inpath}", "-o{outdir}")
 
+    ENCRYPTED_FLAG = 0b0001
+    EOCD_RECORD_HEADER = 0x6054B50
+    ZIP64_EOCD_SIGNATURE = 0x06064B50
+    ZIP64_EOCD_LOCATOR_HEADER = 0x07064B50
+
     def has_encrypted_files(
         self,
         file: File,
         start_offset: int,
         end_of_central_directory: Instance,
     ) -> bool:
         file.seek(start_offset + end_of_central_directory.offset_of_cd, io.SEEK_SET)
         for _ in range(0, end_of_central_directory.total_entries):
             cd_header = self.cparser_le.cd_file_header_t(file)
-            if cd_header.flags & ENCRYPTED_FLAG:
+            if cd_header.flags & self.ENCRYPTED_FLAG:
                 return True
         return False
 
     @staticmethod
     def is_zip64_eocd(end_of_central_directory: Instance):
         # see https://pkware.cachefly.net/webdocs/APPNOTE/APPNOTE-6.3.1.TXT section J
         return (
@@ -110,42 +110,44 @@
             or end_of_central_directory.central_directory_size == 0xFFFFFFFF
             or end_of_central_directory.offset_of_cd == 0xFFFFFFFF
         )
 
     def _parse_zip64(self, file: File, start_offset: int, offset: int) -> int:
         file.seek(start_offset, io.SEEK_SET)
         for eocd_locator_offset in iterate_patterns(
-            file, struct.pack("<I", ZIP64_EOCD_LOCATOR_HEADER)
+            file, struct.pack("<I", self.ZIP64_EOCD_LOCATOR_HEADER)
         ):
             file.seek(eocd_locator_offset, io.SEEK_SET)
             eocd_locator = self.cparser_le.zip64_end_of_central_directory_locator_t(
                 file
             )
             logger.debug("eocd_locator", eocd_locator=eocd_locator, _verbosity=3)
 
             # ZIP64 EOCD locator is right before the EOCD record
             if eocd_locator_offset + len(eocd_locator) == offset:
                 file.seek(start_offset + eocd_locator.offset_of_cd)
                 zip64_eocd = self.cparser_le.zip64_end_of_central_directory_t(file)
                 logger.debug("zip64_eocd", zip64_eocd=zip64_eocd, _verbosity=3)
 
-                if zip64_eocd.signature != ZIP64_EOCD_SIGNATURE:
+                if zip64_eocd.signature != self.ZIP64_EOCD_SIGNATURE:
                     raise InvalidInputFormat(
                         "Missing ZIP64 EOCD header record header in ZIP chunk."
                     )
                 return zip64_eocd
         raise InvalidInputFormat(
             "Missing ZIP64 EOCD locator record header in ZIP chunk."
         )
 
     def calculate_chunk(self, file: File, start_offset: int) -> Optional[ValidChunk]:
         has_encrypted_files = False
         file.seek(start_offset, io.SEEK_SET)
 
-        for offset in iterate_patterns(file, struct.pack("<I", EOCD_RECORD_HEADER)):
+        for offset in iterate_patterns(
+            file, struct.pack("<I", self.EOCD_RECORD_HEADER)
+        ):
             file.seek(offset, io.SEEK_SET)
             end_of_central_directory = self.parse_header(file)
 
             if self.is_zip64_eocd(end_of_central_directory):
                 end_of_central_directory = self._parse_zip64(file, start_offset, offset)
                 break
```

### Comparing `unblob-23.4.17/unblob/handlers/compression/_gzip_reader.py` & `unblob-23.5.5/unblob/handlers/compression/_gzip_reader.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/bzip2.py` & `unblob-23.5.5/unblob/handlers/compression/bzip2.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/compress.py` & `unblob-23.5.5/unblob/handlers/compression/compress.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/gzip.py` & `unblob-23.5.5/unblob/handlers/compression/gzip.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/lz4.py` & `unblob-23.5.5/unblob/handlers/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/lzh.py` & `unblob-23.5.5/unblob/handlers/compression/lzh.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/lzip.py` & `unblob-23.5.5/unblob/handlers/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/lzma.py` & `unblob-23.5.5/unblob/handlers/compression/lzma.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/lzo.py` & `unblob-23.5.5/unblob/handlers/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/xz.py` & `unblob-23.5.5/unblob/handlers/compression/xz.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/zlib.py` & `unblob-23.5.5/unblob/handlers/compression/zlib.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/compression/zstd.py` & `unblob-23.5.5/unblob/handlers/compression/zstd.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/executable/elf.py` & `unblob-23.5.5/unblob/handlers/executable/elf.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/android/sparse.py` & `unblob-23.5.5/unblob/handlers/filesystem/android/sparse.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/cramfs.py` & `unblob-23.5.5/unblob/handlers/filesystem/cramfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/extfs.py` & `unblob-23.5.5/unblob/handlers/filesystem/extfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/fat.py` & `unblob-23.5.5/unblob/handlers/filesystem/fat.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/iso9660.py` & `unblob-23.5.5/unblob/handlers/filesystem/iso9660.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/jffs2.py` & `unblob-23.5.5/unblob/handlers/filesystem/jffs2.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/ntfs.py` & `unblob-23.5.5/unblob/handlers/filesystem/ntfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/romfs.py` & `unblob-23.5.5/unblob/handlers/filesystem/romfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/squashfs.py` & `unblob-23.5.5/unblob/handlers/filesystem/squashfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/ubi.py` & `unblob-23.5.5/unblob/handlers/filesystem/ubi.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/handlers/filesystem/yaffs.py` & `unblob-23.5.5/unblob/handlers/filesystem/yaffs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/identifiers.py` & `unblob-23.5.5/unblob/identifiers.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/iter_utils.py` & `unblob-23.5.5/unblob/iter_utils.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/logging.py` & `unblob-23.5.5/unblob/logging.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/models.py` & `unblob-23.5.5/unblob/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import attr
 from structlog import get_logger
 
 from .file_utils import Endian, File, InvalidInputFormat, StructParser
 from .identifiers import new_id
 from .parser import hexstring2regex
-from .report import ChunkReport, ErrorReport, Report, UnknownChunkReport
+from .report import ChunkReport, EntropyReport, ErrorReport, Report, UnknownChunkReport
 
 logger = get_logger()
 
 # The state transitions are:
 #
 # file ──► pattern match ──► ValidChunk
 #
@@ -119,20 +119,21 @@
     Important for manual analysis, and analytical certanity: for example
     entropy, other chunks inside it, metadata, etc.
 
     These are not extracted, just logged for information purposes and further analysis,
     like most common bytes (like \x00 and \xFF), ASCII strings, high entropy, etc.
     """
 
-    def as_report(self) -> UnknownChunkReport:
+    def as_report(self, entropy: Optional[EntropyReport]) -> UnknownChunkReport:
         return UnknownChunkReport(
             chunk_id=self.chunk_id,
             start_offset=self.start_offset,
             end_offset=self.end_offset,
             size=self.size,
+            entropy=entropy,
         )
 
 
 @attr.define
 class TaskResult:
     task: Task
     reports: List[Report] = attr.field(factory=list)
```

### Comparing `unblob-23.4.17/unblob/parser.py` & `unblob-23.5.5/unblob/parser.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/plugins.py` & `unblob-23.5.5/unblob/plugins.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/pool.py` & `unblob-23.5.5/unblob/pool.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/processing.py` & `unblob-23.5.5/unblob/processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import multiprocessing
 import shutil
-import statistics
 from operator import attrgetter
 from pathlib import Path
 from typing import Iterable, List, Optional, Sequence
 
 import attr
 import magic
 import plotext as plt
 from structlog import get_logger
+from unblob_native import math_tools as mt
 
 from unblob.handlers import BUILTIN_HANDLERS, Handlers
 
 from .extractor import carve_unknown_chunk, carve_valid_chunk, fix_extracted_directory
 from .file_utils import iterate_file
 from .finder import search_chunks
 from .iter_utils import pairwise
 from .logging import noformat
-from .math import shannon_entropy
 from .models import (
     Chunk,
     ExtractError,
     File,
     ProcessResult,
     Task,
     TaskResult,
     UnknownChunk,
     ValidChunk,
 )
 from .pool import make_pool
 from .report import (
+    EntropyReport,
     ExtractDirectoryExistsReport,
     FileMagicReport,
     HashReport,
     StatReport,
     UnknownError,
 )
 from .signals import terminate_gracefully
@@ -328,36 +328,49 @@
             assign_file_to_chunks(unknown_chunks, file=file)
 
             if outer_chunks or unknown_chunks:
                 self._process_chunks(file, outer_chunks, unknown_chunks)
             else:
                 # we don't consider whole files as unknown chunks, but we still want to
                 # calculate entropy for whole files which produced no valid chunks
-                self._calculate_entropy(self.task.path)
+                entropy = self._calculate_entropy(self.task.path)
+                if entropy:
+                    self.result.add_report(entropy)
 
     def _process_chunks(
         self,
         file: File,
         outer_chunks: List[ValidChunk],
         unknown_chunks: List[UnknownChunk],
     ):
         if unknown_chunks:
             logger.warning("Found unknown Chunks", chunks=unknown_chunks)
 
         for chunk in unknown_chunks:
             carved_unknown_path = carve_unknown_chunk(self.carve_dir, file, chunk)
-            self._calculate_entropy(carved_unknown_path)
-            self.result.add_report(chunk.as_report())
+            entropy = self._calculate_entropy(carved_unknown_path)
+            self.result.add_report(chunk.as_report(entropy=entropy))
 
         for chunk in outer_chunks:
             self._extract_chunk(file, chunk)
 
-    def _calculate_entropy(self, path: Path):
+    def _calculate_entropy(self, path: Path) -> Optional[EntropyReport]:
         if self.task.depth < self.config.entropy_depth:
-            calculate_entropy(path, draw_plot=self.config.entropy_plot)
+            report = calculate_entropy(path)
+            if self.config.entropy_plot:
+                logger.debug(
+                    "Entropy chart",
+                    # New line so that chart title will be aligned correctly in the next line
+                    chart="\n"
+                    + format_entropy_plot(report.percentages, report.block_size),
+                    path=path,
+                    _verbosity=3,
+                )
+            return report
+        return None
 
     def _extract_chunk(self, file, chunk: ValidChunk):
         skip_carving = chunk.is_whole_file
         if skip_carving:
             inpath = self.task.path
             extract_dir = self.carve_dir
             carved_path = None
@@ -480,74 +493,89 @@
             end_offset=file_size,
         )
         unknown_chunks.append(unknown_chunk)
 
     return unknown_chunks
 
 
-def calculate_entropy(path: Path, *, draw_plot: bool):
-    """Calculate and log shannon entropy divided by 8 for the file in 1mB chunks.
+def calculate_entropy(path: Path) -> EntropyReport:
+    """Calculate and log shannon entropy divided by 8 for the file in chunks.
 
     Shannon entropy returns the amount of information (in bits) of some numeric
     sequence. We calculate the average entropy of byte chunks, which in theory
     can contain 0-8 bits of entropy. We normalize it for visualization to a
     0-100% scale, to make it easier to interpret the graph.
     """
     percentages = []
 
     # We could use the chunk size instead of another syscall,
     # but we rely on the actual file size written to the disk
     file_size = path.stat().st_size
     logger.debug("Calculating entropy for file", path=path, size=file_size)
 
-    # Smaller chuk size would be very slow to calculate.
+    # Smaller chunk size would be very slow to calculate.
     # 1Mb chunk size takes ~ 3sec for a 4,5 GB file.
-    buffer_size = calculate_buffer_size(
-        file_size, chunk_count=80, min_limit=1024, max_limit=1024 * 1024
+    block_size = calculate_block_size(
+        file_size,
+        chunk_count=80,
+        min_limit=1024,
+        max_limit=1024 * 1024,
     )
 
+    entropy_sum = 0.0
     with File.from_path(path) as file:
-        for chunk in iterate_file(file, 0, file_size, buffer_size=buffer_size):
-            entropy = shannon_entropy(chunk)
+        for chunk in iterate_file(file, 0, file_size, buffer_size=block_size):
+            entropy = mt.shannon_entropy(chunk)
             entropy_percentage = round(entropy / 8 * 100, 2)
             percentages.append(entropy_percentage)
+            entropy_sum += entropy * len(chunk)
+
+    report = EntropyReport(
+        percentages=percentages,
+        block_size=block_size,
+        mean=entropy_sum / file_size / 8 * 100,
+    )
 
     logger.debug(
         "Entropy calculated",
-        mean=round(statistics.mean(percentages), 2),
-        highest=max(percentages),
-        lowest=min(percentages),
+        path=path,
+        size=file_size,
+        block_size=report.block_size,
+        mean=round(report.mean, 2),
+        highest=round(report.highest, 2),
+        lowest=round(report.lowest, 2),
     )
 
-    if draw_plot:
-        draw_entropy_plot(percentages)
+    return report
 
 
-def calculate_buffer_size(
+def calculate_block_size(
     file_size, *, chunk_count: int, min_limit: int, max_limit: int
 ) -> int:
     """Split the file into even sized chunks, limited by lower and upper values."""
     # We don't care about floating point precision here
-    buffer_size = file_size // chunk_count
-    buffer_size = max(min_limit, buffer_size)
-    buffer_size = min(buffer_size, max_limit)
-    return buffer_size
+    block_size = file_size // chunk_count
+    block_size = max(min_limit, block_size)
+    block_size = min(block_size, max_limit)
+    return block_size
 
 
-def draw_entropy_plot(percentages: List[float]):
-    plt.clear_data()
+def format_entropy_plot(percentages: List[float], block_size: int):
+    # start from scratch
+    plt.clear_figure()
+    # go colorless
     plt.clear_color()
     plt.title("Entropy distribution")
-    plt.xlabel("mB")
+    # plt.xlabel(humanize.naturalsize(block_size))
+    plt.xlabel(f"{block_size} bytes")
     plt.ylabel("entropy %")
 
     plt.scatter(percentages, marker="dot")
     # 16 height leaves no gaps between the lines
     plt.plot_size(100, 16)
     plt.ylim(0, 100)
     # Draw ticks every 1Mb on the x axis.
     plt.xticks(range(len(percentages) + 1))
     # Always show 0% and 100%
     plt.yticks(range(0, 101, 10))
 
-    # New line so that chart title will be aligned correctly in the next line
-    logger.debug("Entropy chart", chart="\n" + plt.build(), _verbosity=3)
+    return plt.build()
```

### Comparing `unblob-23.4.17/unblob/report.py` & `unblob-23.5.5/unblob/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -168,14 +168,29 @@
 
 @attr.define(kw_only=True)
 class FileMagicReport(Report):
     magic: str
     mime_type: str
 
 
+@attr.define(kw_only=True)
+class EntropyReport(Report):
+    percentages: List[float]
+    block_size: int
+    mean: float
+
+    @property
+    def highest(self):
+        return max(self.percentages)
+
+    @property
+    def lowest(self):
+        return min(self.percentages)
+
+
 @final
 @attr.define(kw_only=True)
 class ChunkReport(Report):
     chunk_id: str
     handler_name: str
     start_offset: int
     end_offset: int
@@ -187,7 +202,8 @@
 @final
 @attr.define(kw_only=True)
 class UnknownChunkReport(Report):
     chunk_id: str
     start_offset: int
     end_offset: int
     size: int
+    entropy: Optional[EntropyReport]
```

### Comparing `unblob-23.4.17/unblob/signals.py` & `unblob-23.5.5/unblob/signals.py`

 * *Files identical despite different names*

### Comparing `unblob-23.4.17/unblob/testing.py` & `unblob-23.5.5/unblob/testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import shlex
 import subprocess
 from pathlib import Path
 
 import pytest
 from pytest_cov.embed import cleanup_on_sigterm
 
@@ -17,15 +18,17 @@
     configure_logger(verbosity_level=3, extract_root=Path(""))
 
     # https://pytest-cov.readthedocs.io/en/latest/subprocess-support.html#if-you-use-multiprocessing-process
     cleanup_on_sigterm()
 
 
 def gather_integration_tests(test_data_path: Path):
-    test_input_dirs = list(test_data_path.glob("**/__input__"))
+    test_input_dirs = [
+        Path(p) for p in glob.iglob(f"{test_data_path}/**/__input__", recursive=True)
+    ]
     test_case_dirs = [p.parent for p in test_input_dirs]
     test_output_dirs = [p / "__output__" for p in test_case_dirs]
     test_ids = [
         f"{str(p.relative_to(test_data_path)).replace('/', '.')}"
         for p in test_case_dirs
     ]
```

### Comparing `unblob-23.4.17/PKG-INFO` & `unblob-23.5.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: unblob
-Version: 23.4.17
+Version: 23.5.5
 Summary: Extract files from any kind of container formats
 License: MIT
 Author: ONEKEY
 Author-email: support@onekey.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arpy (>=2.2.0,<3.0.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: cryptography (>=37.0.1,<40.0)
+Requires-Dist: cryptography (>=39.0,<41.0)
 Requires-Dist: dissect.cstruct (>=2.0,<3.0)
 Requires-Dist: jefferson (>=0.4.2,<0.5.0)
 Requires-Dist: lark (>=1.1.2,<2.0.0)
 Requires-Dist: lief (>=0.12.3,<0.13.0)
 Requires-Dist: lz4 (>=4.0.0,<5.0.0)
 Requires-Dist: plotext (>=4.2.0,<6.0)
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
-Requires-Dist: pyperscan (>=0.2.0,<0.3.0)
+Requires-Dist: pyperscan (>=0.2.2,<0.3.0)
 Requires-Dist: python-lzo (>=1.14,<2.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: structlog (>=21.2.0,<22.0.0)
 Requires-Dist: treelib (>=1.6.1,<2.0.0)
 Requires-Dist: ubi-reader (>=0.8.5,<0.9.0)
+Requires-Dist: unblob-native (>=0.1.0,<0.2.0)
```

