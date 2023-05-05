# Comparing `tmp/static-frame-1.4.0.tar.gz` & `tmp/static-frame-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-1.4.0.tar", last modified: Thu May  4 19:41:21 2023, max compression
+gzip compressed data, was "static-frame-1.4.1.tar", last modified: Fri May  5 16:02:33 2023, max compression
```

## Comparing `static-frame-1.4.0.tar` & `static-frame-1.4.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.711680 static-frame-1.4.0/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.4.0/LICENSE.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.4.0/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-04 19:41:21.711680 static-frame-1.4.0/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23553 2023-05-04 17:09:05.000000 static-frame-1.4.0/README.rst
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.4.0/requirements-extras.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-04 17:09:05.000000 static-frame-1.4.0/requirements-test.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-04 17:09:05.000000 static-frame-1.4.0/requirements.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-04 19:41:21.711680 static-frame-1.4.0/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.4.0/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.683680 static-frame-1.4.0/static_frame/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7660 2023-05-04 17:34:51.000000 static-frame-1.4.0/static_frame/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/__main__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.695680 static-frame-1.4.0/static_frame/core/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/core/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/assign.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/core/display_html_datatables.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/display_visidata.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/doc_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/exception.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   379744 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    56830 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   107720 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/interface_meta.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/node_dt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_hashlib.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-04-24 22:32:18.000000 static-frame-1.4.0/static_frame/core/node_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/node_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_selector.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_transpose.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_values.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/protocol_dfi_abc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_client_mixin.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14787 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   185868 2023-05-03 15:14:12.000000 static-frame-1.4.0/static_frame/core/type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   128804 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/yarn.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/py.typed
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.695680 static-frame-1.4.0/static_frame/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/test/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/test_case.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.707680 static-frame-1.4.0/static_frame/test/unit/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/test/unit/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_doc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   641142 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_via_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_via_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/test/unit/test_interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23361 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.4.0/static_frame/test/unit/test_platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   242465 2023-04-24 22:32:18.000000 static-frame-1.4.0/static_frame/test/unit/test_series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_series_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14218 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/test/unit/test_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10382 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_yarn.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.683680 static-frame-1.4.0/static_frame.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/requires.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.925144 static-frame-1.4.1/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.4.1/LICENSE.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.4.1/MANIFEST.in
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-05 16:02:33.925144 static-frame-1.4.1/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23553 2023-05-04 17:09:05.000000 static-frame-1.4.1/README.rst
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.4.1/requirements-extras.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-04 17:09:05.000000 static-frame-1.4.1/requirements-test.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-04 17:09:05.000000 static-frame-1.4.1/requirements.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-05 16:02:33.925144 static-frame-1.4.1/setup.cfg
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.4.1/setup.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.909144 static-frame-1.4.1/static_frame/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7660 2023-05-05 03:07:47.000000 static-frame-1.4.1/static_frame/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/__main__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.917144 static-frame-1.4.1/static_frame/core/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/core/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/assign.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/core/display_html_datatables.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/display_visidata.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/doc_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/exception.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   379744 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    56830 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   107720 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/interface_meta.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/node_dt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_hashlib.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-04-24 22:32:18.000000 static-frame-1.4.1/static_frame/core/node_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/node_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_selector.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_transpose.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_values.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/protocol_dfi_abc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_client_mixin.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14787 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   185709 2023-05-05 03:05:19.000000 static-frame-1.4.1/static_frame/core/type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   128804 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/yarn.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/py.typed
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.917144 static-frame-1.4.1/static_frame/test/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/test/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/test_case.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.925144 static-frame-1.4.1/static_frame/test/unit/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/test/unit/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_doc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   641142 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_via_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/test/unit/test_interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23164 2023-05-05 03:05:19.000000 static-frame-1.4.1/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.4.1/static_frame/test/unit/test_platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   242465 2023-04-24 22:32:18.000000 static-frame-1.4.1/static_frame/test/unit/test_series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_series_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14218 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/test/unit/test_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10382 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_yarn.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.909144 static-frame-1.4.1/static_frame.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/requires.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-1.4.0/LICENSE.txt` & `static-frame-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/PKG-INFO` & `static-frame-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.0
+Version: 1.4.1
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
```

### Comparing `static-frame-1.4.0/README.rst` & `static-frame-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/setup.py` & `static-frame-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/__init__.py` & `static-frame-1.4.1/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,8 @@
 from static_frame.core.util import IndexSpecifier as IndexSpecifier
 from static_frame.core.util import KeyOrKeys as KeyOrKeys
 from static_frame.core.util import PathSpecifierOrFileLike as PathSpecifierOrFileLike
 from static_frame.core.util import SeriesInitializer as SeriesInitializer
 from static_frame.core.www import WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '1.4.0'
+__version__ = '1.4.1'
```

### Comparing `static-frame-1.4.0/static_frame/__main__.py` & `static-frame-1.4.1/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/archive_npy.py` & `static-frame-1.4.1/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/axis_map.py` & `static-frame-1.4.1/static_frame/core/axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/batch.py` & `static-frame-1.4.1/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/bus.py` & `static-frame-1.4.1/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/container.py` & `static-frame-1.4.1/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/container_util.py` & `static-frame-1.4.1/static_frame/core/container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/display.py` & `static-frame-1.4.1/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/display_color.py` & `static-frame-1.4.1/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/display_config.py` & `static-frame-1.4.1/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/display_html_datatables.py` & `static-frame-1.4.1/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/display_visidata.py` & `static-frame-1.4.1/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/doc_str.py` & `static-frame-1.4.1/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/exception.py` & `static-frame-1.4.1/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/fill_value_auto.py` & `static-frame-1.4.1/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/frame.py` & `static-frame-1.4.1/static_frame/core/frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/hloc.py` & `static-frame-1.4.1/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/index.py` & `static-frame-1.4.1/static_frame/core/index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/index_auto.py` & `static-frame-1.4.1/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/index_base.py` & `static-frame-1.4.1/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/index_correspondence.py` & `static-frame-1.4.1/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/index_datetime.py` & `static-frame-1.4.1/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/index_hierarchy.py` & `static-frame-1.4.1/static_frame/core/index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-1.4.1/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/interface.py` & `static-frame-1.4.1/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/interface_meta.py` & `static-frame-1.4.1/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/join.py` & `static-frame-1.4.1/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/loc_map.py` & `static-frame-1.4.1/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/memory_measure.py` & `static-frame-1.4.1/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_dt.py` & `static-frame-1.4.1/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_fill_value.py` & `static-frame-1.4.1/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_hashlib.py` & `static-frame-1.4.1/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_iter.py` & `static-frame-1.4.1/static_frame/core/node_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_re.py` & `static-frame-1.4.1/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_selector.py` & `static-frame-1.4.1/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_str.py` & `static-frame-1.4.1/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_transpose.py` & `static-frame-1.4.1/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/node_values.py` & `static-frame-1.4.1/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/pivot.py` & `static-frame-1.4.1/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/platform.py` & `static-frame-1.4.1/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/protocol_dfi.py` & `static-frame-1.4.1/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/protocol_dfi_abc.py` & `static-frame-1.4.1/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/quilt.py` & `static-frame-1.4.1/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/rank.py` & `static-frame-1.4.1/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/series.py` & `static-frame-1.4.1/static_frame/core/series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/store.py` & `static-frame-1.4.1/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/store_client_mixin.py` & `static-frame-1.4.1/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/store_config.py` & `static-frame-1.4.1/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/store_filter.py` & `static-frame-1.4.1/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/store_hdf5.py` & `static-frame-1.4.1/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/store_sqlite.py` & `static-frame-1.4.1/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/store_xlsx.py` & `static-frame-1.4.1/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/store_zip.py` & `static-frame-1.4.1/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/style_config.py` & `static-frame-1.4.1/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/type_blocks.py` & `static-frame-1.4.1/static_frame/core/type_blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing as tp
 from copy import deepcopy
 from functools import partial
 from itertools import chain
+from itertools import repeat
 from itertools import zip_longest
 
 import numpy as np
 from arraykit import array_deepcopy
 from arraykit import column_1d_filter
 from arraykit import column_2d_filter
 from arraykit import first_true_1d
@@ -415,15 +416,14 @@
     '''An ordered collection of type-heterogenous, immutable NumPy arrays, providing an external array-like interface of a single, 2D array. Used by :obj:`Frame` for core, unindexed array management.
 
     A TypeBlocks instance can have a zero size shape (where the length of one axis is zero). Internally, when axis 0 (rows) is of size 0, we store similarly sized arrays. When axis 1 (columns) is of size 0, we do not store arrays, as such arrays do not define a type (as types are defined by columns).
     '''
 
     __slots__ = (
             '_blocks',
-            '_dtypes',
             '_index',
             '_shape',
             '_row_dtype',
             )
 
     STATIC = False
 
@@ -442,37 +442,34 @@
 
         Args:
             raw_blocks: iterable (generator compatible) of NDArrays, or a single NDArray.
             shape_reference: optional argument to support cases where no blocks are found in the ``raw_blocks`` iterable, but the outer context is one with rows but no columns, or columns and no rows.
 
         '''
         blocks: tp.List[np.ndarray] = [] # ordered blocks
-        dtypes: tp.List[np.dtype] = [] # column position to dtype
         index: tp.List[tp.Tuple[int, int]] = [] # columns position to blocks key
         block_count = 0
 
         row_count: tp.Optional[int]
 
         # if a single block, no need to loop
         if raw_blocks.__class__ is np.ndarray:
             if raw_blocks.ndim > 2: #type: ignore
                 raise ErrorInitTypeBlocks('arrays of dimensionality greater than 2 cannot be used to create TypeBlocks')
 
             row_count, column_count = shape_filter(raw_blocks)
             if column_count == 0:
                 # set shape but do not store array
                 return cls(blocks=blocks,
-                        dtypes=dtypes,
                         index=index,
                         shape=(row_count, column_count) #type: ignore
                         )
             blocks.append(immutable_filter(raw_blocks))
             for i in range(column_count):
                 index.append((block_count, i))
-                dtypes.append(raw_blocks.dtype) #type: ignore
 
         else: # an iterable of blocks
             row_count = None
             column_count = 0
 
             for block in raw_blocks:
                 if not block.__class__ is np.ndarray:
@@ -494,30 +491,28 @@
                     continue
 
                 blocks.append(immutable_filter(block))
 
                 # store position to key of block, block columns
                 for i in range(c):
                     index.append((block_count, i))
-                    dtypes.append(block.dtype)
 
                 column_count += c
                 block_count += 1
 
         # blocks can be empty
         if row_count is None:
             if shape_reference is not None:
                 # if columns have gone to zero, and this was created from a TB that had rows, continue to represent those rows
                 row_count = shape_reference[0]
             else:
                 raise ErrorInitTypeBlocks('cannot derive a row_count from blocks; provide a shape reference')
 
         return cls(
                 blocks=blocks,
-                dtypes=dtypes,
                 index=index,
                 shape=(row_count, column_count),
                 )
 
     @classmethod
     def from_element_items(cls,
             items: tp.Iterable[tp.Tuple[tp.Tuple[int, ...], object]],
@@ -555,15 +550,15 @@
                 blocks = np.empty(shape)
                 blocks.flags.writeable = False
             else:
                 blocks = (np.empty(rows, dtype=get_col_dtype(i)) for i in range(columns))
             return cls.from_blocks(blocks)
 
         # for arrays with no width, favor storing shape alone and not creating an array object; the shape will be binding for future appending
-        return cls(blocks=list(), dtypes=list(), index=list(), shape=shape)
+        return cls(blocks=list(), index=list(), shape=shape)
 
     @staticmethod
     def vstack_blocks_to_blocks(
             type_blocks: tp.Sequence['TypeBlocks'],
             block_compatible: tp.Optional[bool] = None,
             reblock_compatible: tp.Optional[bool] = None,
             ) -> tp.Iterator[np.ndarray]:
@@ -604,29 +599,26 @@
                 yield concat_resolved(block_parts)
 
 
     #---------------------------------------------------------------------------
 
     def __init__(self, *,
             blocks: tp.List[np.ndarray],
-            dtypes: tp.List[np.dtype],
             index: tp.List[tp.Tuple[int, int]],
-            shape: tp.Tuple[int, int]
+            shape: tp.Tuple[int, int],
             ) -> None:
         '''
         Default constructor. We own all lists passed in to this constructor. This instance takes ownership of all lists passed to it.
 
         Args:
             blocks: A list of one or two-dimensional NumPy arrays. The list is owned by this instance.
-            dtypes: list of dtypes per external column. The list is owned by this instance.
             index: list of pairs, where the first element is the block index, the second elemetns is the intra-block column
             shape: two-element tuple defining row and column count. A (0, 0) shape is permitted for empty TypeBlocks.
         '''
         self._blocks = blocks
-        self._dtypes = dtypes
         self._index = index # list where index, as column, gets block, offset
         self._shape = shape
 
         if self._blocks:
             self._row_dtype = resolve_dtype_iter(b.dtype for b in self._blocks)
         else:
             # NOTE: this violates the type; however, this is desirable when appending such that this value does not force an undesirable type resolution
@@ -644,48 +636,55 @@
 
         for b in self._blocks:
             b.flags.writeable = False
 
     def __deepcopy__(self, memo: tp.Dict[int, tp.Any]) -> 'TypeBlocks':
         obj = self.__class__.__new__(self.__class__)
         obj._blocks = [array_deepcopy(b, memo) for b in self._blocks]
-        obj._dtypes = deepcopy(self._dtypes, memo)
         obj._index = self._index.copy() # list of tuples of ints
         obj._shape = self._shape # immutable, no copy necessary
         obj._row_dtype = deepcopy(self._row_dtype, memo)
         memo[id(self)] = obj
         return obj
 
     def __copy__(self) -> 'TypeBlocks':
         '''
         Return shallow copy of this TypeBlocks. Underlying arrays are not copied.
         '''
         return self.__class__(
                 blocks=[b for b in self._blocks],
-                dtypes=self._dtypes.copy(), # list
                 index=self._index.copy(), # list
                 shape=self._shape,
                 )
 
     def copy(self) -> 'TypeBlocks':
         '''
         Return shallow copy of this TypeBlocks. Underlying arrays are not copied.
         '''
         return self.__copy__()
 
     #---------------------------------------------------------------------------
     # new properties
 
+    def _iter_dtypes(self) -> tp.Iterator[np.dtype]:
+        for b in self._blocks:
+            dt = b.dtype
+            if b.ndim == 1:
+                yield dt
+            else: # PERF: repeat is much faster than a for loop
+                yield from repeat(dt, b.shape[1])
+
     @property
     def dtypes(self) -> np.ndarray:
         '''
         Return an immutable array that, for each realizable column (not each block), the dtype is given.
         '''
         # this creates a new array every time it is called; could cache
-        a = np.array(self._dtypes, dtype=DTYPE_OBJECT)
+        a = np.empty(self._shape[1], dtype=DTYPE_OBJECT)
+        a[NULL_SLICE] = list(self._iter_dtypes())
         a.flags.writeable = False
         return a
 
     @property
     def shapes(self) -> np.ndarray:
         '''
         Return an immutable array that, for each block, reports the shape as a tuple.
@@ -1461,15 +1460,14 @@
         '''
         Return a TypeBlocks rounded to the given decimals. Negative decimals round to the left of the decimal point.
         '''
         func = partial(np.round, decimals=decimals)
         # for now, we do not expose application of rounding on a subset of blocks, but is doable by setting the column_key
         return self.__class__(
                 blocks=list(self._ufunc_blocks(column_key=NULL_SLICE, func=func)),
-                dtypes=self._dtypes.copy(), # list
                 index=self._index.copy(),
                 shape=self._shape
                 )
 
     def __len__(self) -> int:
         '''Length, as with NumPy and Pandas, is the number of rows. Note that A shape of (3, 0) will return a length of 3, even though there is no data.
         '''
@@ -4211,16 +4209,19 @@
         elif not isinstance(other, TypeBlocks):
             return False
 
         # same type from here
         if self._shape != other._shape:
             return False
 
-        if compare_dtype and self._dtypes != other._dtypes: # these are lists
-            return False
+        if compare_dtype:
+            for d_self, d_other in zip(self._iter_dtypes(), other._iter_dtypes()):
+                # have already validated shape
+                if d_self != d_other:
+                    return False
 
         # NOTE: cannot directly compare blocks as we cannot assume the same number of blocks means that the blocks are consolidated in the same way
 
         for i in range(self._shape[1]):
             if not arrays_equal(
                     self._extract_array_column(i),
                     other._extract_array_column(i),
@@ -4255,15 +4256,14 @@
 
         # extend shape, or define it if not yet set
         self._shape = (row_count, self._shape[1] + block_columns)
 
         # add block, dtypes, index
         for i in range(block_columns):
             self._index.append((block_idx, i))
-            self._dtypes.append(block.dtype)
 
         # make immutable copy if necessary before appending
         self._blocks.append(immutable_filter(block))
 
         # if already aligned, nothing to do
         if not self._row_dtype: # if never set as shape is empty
             self._row_dtype = block.dtype
```

### Comparing `static-frame-1.4.0/static_frame/core/util.py` & `static-frame-1.4.1/static_frame/core/util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/www.py` & `static-frame-1.4.1/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/core/yarn.py` & `static-frame-1.4.1/static_frame/core/yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/test_case.py` & `static-frame-1.4.1/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_archive_npy.py` & `static-frame-1.4.1/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_axis_map.py` & `static-frame-1.4.1/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_batch.py` & `static-frame-1.4.1/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_bus.py` & `static-frame-1.4.1/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_container.py` & `static-frame-1.4.1/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_container_util.py` & `static-frame-1.4.1/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_display.py` & `static-frame-1.4.1/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_display_color.py` & `static-frame-1.4.1/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_doc.py` & `static-frame-1.4.1/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-1.4.1/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_frame.py` & `static-frame-1.4.1/static_frame/test/unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_frame_he.py` & `static-frame-1.4.1/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_frame_iter.py` & `static-frame-1.4.1/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_frame_join.py` & `static-frame-1.4.1/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-1.4.1/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_frame_via_re.py` & `static-frame-1.4.1/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_hloc.py` & `static-frame-1.4.1/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_index.py` & `static-frame-1.4.1/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_index_auto.py` & `static-frame-1.4.1/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_index_base.py` & `static-frame-1.4.1/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_index_correspondence.py` & `static-frame-1.4.1/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_index_datetime.py` & `static-frame-1.4.1/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-1.4.1/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-1.4.1/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_interface.py` & `static-frame-1.4.1/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_loc_map.py` & `static-frame-1.4.1/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_memory_measure.py` & `static-frame-1.4.1/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-1.4.1/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,15 +454,14 @@
             tb._blocks, # [np.array([1, 2, 3])],
             0,
             (0, 0),
             tb._index, # [(0, 0)],
             3, 1,
             tb._shape, # (3, 1),
             np.dtype('int64'),
-            tb._dtypes, # [np.dtype('int64')],
             # _row_dtype, # np.dtype('int64') is already included
             tb
         )))
 
     def test_getsizeof_total_type_blocks_list_of_1d_arrays(self) -> None:
         tb = TypeBlocks.from_blocks([
             np.array([1, 2, 3]),
@@ -476,15 +475,14 @@
             (0, 0),
             1,
             (1, 0),
             tb._index, # [(0, 0), (1, 0)],
             3, 2,
             tb._shape, # (3, 2),
             np.dtype('int64'),
-            tb._dtypes, # [np.dtype('int64'), np.dtype('int64')],
             # _row_dtype, # np.dtype('int64') is already included
             tb
         )))
 
     def test_getsizeof_total_type_blocks_2d_array(self) -> None:
         tb = TypeBlocks.from_blocks(np.array([[1, 2, 3], [4, 5, 6]]))
         self.assertEqual(memory_total(tb), sum(getsizeof(e) for e in (
@@ -496,15 +494,14 @@
             (0, 1),
             2,
             (0, 2),
             tb._index, # [(0, 0), (0, 1), (0, 2)],
             3,
             tb._shape, # (2, 3),
             np.dtype('int64'),
-            tb._dtypes, #[np.dtype('int64'), np.dtype('int64'), np.dtype('int64')],
             # _row_dtype, # np.dtype('int64') is already included
             tb
         )))
 
     #---------------------------------------------------------------------------
     # IndexHierarchy
```

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_pivot.py` & `static-frame-1.4.1/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-1.4.1/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_quilt.py` & `static-frame-1.4.1/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_rank.py` & `static-frame-1.4.1/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_series.py` & `static-frame-1.4.1/static_frame/test/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_series_he.py` & `static-frame-1.4.1/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_store.py` & `static-frame-1.4.1/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_store_filter.py` & `static-frame-1.4.1/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_store_hdf5.py` & `static-frame-1.4.1/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_store_sqlite.py` & `static-frame-1.4.1/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_store_xlsx.py` & `static-frame-1.4.1/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_store_zip.py` & `static-frame-1.4.1/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_style_config.py` & `static-frame-1.4.1/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_type_blocks.py` & `static-frame-1.4.1/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_util.py` & `static-frame-1.4.1/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_www.py` & `static-frame-1.4.1/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame/test/unit/test_yarn.py` & `static-frame-1.4.1/static_frame/test/unit/test_yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.0/static_frame.egg-info/PKG-INFO` & `static-frame-1.4.1/static_frame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.0
+Version: 1.4.1
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
```

### Comparing `static-frame-1.4.0/static_frame.egg-info/SOURCES.txt` & `static-frame-1.4.1/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

