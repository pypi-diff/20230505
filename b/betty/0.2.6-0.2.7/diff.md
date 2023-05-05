# Comparing `tmp/betty-0.2.6.tar.gz` & `tmp/betty-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/betty-0.2.6.tar", last modified: Sat Jan 23 11:55:42 2021, max compression
+gzip compressed data, was "betty-0.2.7.tar", last modified: Fri May  5 19:36:21 2023, max compression
```

## Comparing `betty-0.2.6.tar` & `betty-0.2.7.tar`

### file list

```diff
@@ -1,160 +1,198 @@
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.498793 betty-0.2.6/
--rw-rw-r--   0 bart      (1000) bart      (1000)    32453 2020-07-10 23:06:36.000000 betty-0.2.6/LICENSE.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)    16786 2021-01-23 11:55:42.498793 betty-0.2.6/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)    13465 2021-01-23 11:55:26.000000 betty-0.2.6/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        6 2021-01-23 11:55:42.000000 betty-0.2.6/VERSION
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.482792 betty-0.2.6/betty/
--rw-rw-r--   0 bart      (1000) bart      (1000)       87 2020-12-20 18:39:39.000000 betty-0.2.6/betty/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      258 2021-01-21 21:55:51.000000 betty-0.2.6/betty/about.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    25523 2021-01-23 11:38:14.000000 betty-0.2.6/betty/ancestry.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      768 2021-01-23 11:38:14.000000 betty-0.2.6/betty/asyncio.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5181 2021-01-23 11:55:26.000000 betty-0.2.6/betty/cli.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      594 2021-01-21 21:55:51.000000 betty-0.2.6/betty/concurrent.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7489 2021-01-23 11:38:14.000000 betty-0.2.6/betty/config.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1837 2021-01-23 11:55:26.000000 betty-0.2.6/betty/demo.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      756 2021-01-23 11:38:14.000000 betty-0.2.6/betty/dispatch.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      946 2021-01-21 21:55:51.000000 betty-0.2.6/betty/error.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2684 2021-01-06 00:32:54.000000 betty-0.2.6/betty/fs.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      534 2020-12-21 21:26:04.000000 betty-0.2.6/betty/functools.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7483 2021-01-23 11:38:14.000000 betty-0.2.6/betty/generate.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1481 2021-01-23 11:38:14.000000 betty-0.2.6/betty/graph.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      203 2020-12-02 23:11:33.000000 betty-0.2.6/betty/html.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      379 2020-12-21 21:26:04.000000 betty-0.2.6/betty/importlib.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    18303 2021-01-23 11:38:14.000000 betty-0.2.6/betty/jinja2.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    13393 2021-01-23 11:38:14.000000 betty-0.2.6/betty/json.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    15776 2021-01-21 21:55:51.000000 betty-0.2.6/betty/locale.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      552 2021-01-06 00:32:54.000000 betty-0.2.6/betty/lock.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      708 2020-12-21 21:26:04.000000 betty-0.2.6/betty/logging.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1379 2021-01-06 00:32:54.000000 betty-0.2.6/betty/media_type.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8742 2021-01-23 11:38:14.000000 betty-0.2.6/betty/openapi.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      677 2020-12-21 21:26:04.000000 betty-0.2.6/betty/os.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      363 2021-01-23 11:38:14.000000 betty-0.2.6/betty/parse.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      414 2020-12-02 23:11:33.000000 betty-0.2.6/betty/path.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/
--rw-rw-r--   0 bart      (1000) bart      (1000)     1167 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/anonymizer/
--rw-rw-r--   0 bart      (1000) bart      (1000)     3296 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/anonymizer/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/cleaner/
--rw-rw-r--   0 bart      (1000) bart      (1000)     3876 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/cleaner/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/demo/
--rw-rw-r--   0 bart      (1000) bart      (1000)    10337 2021-01-23 11:55:26.000000 betty-0.2.6/betty/plugin/demo/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/deriver/
--rw-rw-r--   0 bart      (1000) bart      (1000)     8972 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/deriver/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/gramps/
--rw-rw-r--   0 bart      (1000) bart      (1000)    21692 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/gramps/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/maps/
--rw-rw-r--   0 bart      (1000) bart      (1000)     2834 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/maps/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/nginx/
--rw-rw-r--   0 bart      (1000) bart      (1000)     3012 2021-01-23 11:55:26.000000 betty-0.2.6/betty/plugin/nginx/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      998 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/nginx/artifact.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1706 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/nginx/docker.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1976 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/nginx/serve.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/privatizer/
--rw-rw-r--   0 bart      (1000) bart      (1000)     4966 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/privatizer/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/trees/
--rw-rw-r--   0 bart      (1000) bart      (1000)     2704 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/trees/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty/plugin/wikipedia/
--rw-rw-r--   0 bart      (1000) bart      (1000)     9574 2021-01-23 11:38:14.000000 betty-0.2.6/betty/plugin/wikipedia/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      648 2020-12-21 21:26:04.000000 betty-0.2.6/betty/render.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1219 2021-01-23 11:38:14.000000 betty-0.2.6/betty/sass.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1864 2021-01-23 11:38:14.000000 betty-0.2.6/betty/search.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3119 2021-01-23 11:38:14.000000 betty-0.2.6/betty/serve.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7821 2021-01-23 11:55:26.000000 betty-0.2.6/betty/site.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      418 2021-01-11 01:12:21.000000 betty-0.2.6/betty/subprocess.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/
--rw-rw-r--   0 bart      (1000) bart      (1000)     3626 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/assets/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2020-09-26 11:34:36.000000 betty-0.2.6/betty/tests/assets/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/assets/templates/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2020-09-26 11:34:36.000000 betty-0.2.6/betty/tests/assets/templates/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/assets/templates/label/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2020-09-26 11:34:36.000000 betty-0.2.6/betty/tests/assets/templates/label/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4282 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/assets/templates/label/test_event_html_j2.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2626 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/assets/templates/label/test_person_html_j2.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1673 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/assets/templates/label/test_place_html_j2.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/assets/templates/macro/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2020-09-26 11:34:36.000000 betty-0.2.6/betty/tests/assets/templates/macro/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2490 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/assets/templates/macro/test_person_html_j2.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/assets/templates/meta/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2020-09-26 11:34:36.000000 betty-0.2.6/betty/tests/assets/templates/meta/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3982 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/assets/templates/meta/test_person_html_j2.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2860 2021-01-06 00:32:54.000000 betty-0.2.6/betty/tests/assets/templates/meta/test_place_html_j2.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/assets/templates/page/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-01 17:34:35.000000 betty-0.2.6/betty/tests/assets/templates/page/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1118 2021-01-06 00:32:54.000000 betty-0.2.6/betty/tests/assets/templates/page/test_person_html_j2.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2792 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/assets/templates/test_event_dimensions_html_j2.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/plugin/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/plugin/anonymizer/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/anonymizer/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    12473 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/anonymizer/test__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/plugin/cleaner/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/cleaner/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    11415 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/cleaner/test__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.494793 betty-0.2.6/betty/tests/plugin/demo/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:26.000000 betty-0.2.6/betty/tests/plugin/demo/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      901 2021-01-23 11:55:26.000000 betty-0.2.6/betty/tests/plugin/demo/test__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.498793 betty-0.2.6/betty/tests/plugin/deriver/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/deriver/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    18960 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/deriver/test__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.498793 betty-0.2.6/betty/tests/plugin/gramps/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/gramps/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    19553 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/gramps/test__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.498793 betty-0.2.6/betty/tests/plugin/maps/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/maps/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1109 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/maps/test__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.498793 betty-0.2.6/betty/tests/plugin/nginx/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/nginx/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    11595 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/nginx/test__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8057 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/nginx/test_integration.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1387 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/nginx/test_serve.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.498793 betty-0.2.6/betty/tests/plugin/privatizer/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/privatizer/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    15168 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/privatizer/test__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      381 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/test__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.498793 betty-0.2.6/betty/tests/plugin/trees/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/trees/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1118 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/trees/test__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.498793 betty-0.2.6/betty/tests/plugin/wikipedia/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/wikipedia/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    26010 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/plugin/wikipedia/test__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      160 2021-01-21 21:55:51.000000 betty-0.2.6/betty/tests/test_about.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    41057 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_ancestry.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2291 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/test_asyncio.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    10022 2021-01-23 11:55:26.000000 betty-0.2.6/betty/tests/test_cli.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      659 2020-12-02 23:11:33.000000 betty-0.2.6/betty/tests/test_concurrent.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    13119 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_config.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      420 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/test_error.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8000 2021-01-06 00:32:54.000000 betty-0.2.6/betty/tests/test_fs.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1791 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/test_functools.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8650 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_generate.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1498 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_graph.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      491 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/test_html.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      849 2021-01-06 00:32:54.000000 betty-0.2.6/betty/tests/test_importlib.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    19581 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_jinja2.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    22691 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_json.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    17810 2021-01-06 00:32:54.000000 betty-0.2.6/betty/tests/test_locale.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      517 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/test_lock.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1056 2020-11-05 12:04:28.000000 betty-0.2.6/betty/tests/test_logging.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1778 2021-01-06 00:32:54.000000 betty-0.2.6/betty/tests/test_media_type.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1022 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_openapi.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1304 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/test_os.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      807 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_readme.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2214 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_sass.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8068 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_search.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      833 2020-12-21 21:26:04.000000 betty-0.2.6/betty/tests/test_serve.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8603 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_site.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      408 2020-12-02 23:11:33.000000 betty-0.2.6/betty/tests/test_subprocess.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4509 2021-01-23 11:38:14.000000 betty-0.2.6/betty/tests/test_url.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1763 2021-01-06 00:32:54.000000 betty-0.2.6/betty/tests/test_voluptuous.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4303 2021-01-23 11:38:14.000000 betty-0.2.6/betty/url.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      443 2021-01-06 00:51:22.000000 betty-0.2.6/betty/voluptuous.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2021-01-23 11:55:42.486792 betty-0.2.6/betty.egg-info/
--rw-rw-r--   0 bart      (1000) bart      (1000)    16786 2021-01-23 11:55:42.000000 betty-0.2.6/betty.egg-info/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)     3690 2021-01-23 11:55:42.000000 betty-0.2.6/betty.egg-info/SOURCES.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2021-01-23 11:55:42.000000 betty-0.2.6/betty.egg-info/dependency_links.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       42 2021-01-23 11:55:42.000000 betty-0.2.6/betty.egg-info/entry_points.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      490 2021-01-23 11:55:42.000000 betty-0.2.6/betty.egg-info/requires.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        6 2021-01-23 11:55:42.000000 betty-0.2.6/betty.egg-info/top_level.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       38 2021-01-23 11:55:42.498793 betty-0.2.6/setup.cfg
--rw-rw-r--   0 bart      (1000) bart      (1000)     3381 2021-01-23 11:38:14.000000 betty-0.2.6/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/
+-rw-r--r--   0 bart      (1000) bart      (1000)    16818 2023-05-05 19:36:21.533118 betty-0.2.7/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)    13470 2023-05-05 19:35:34.000000 betty-0.2.7/README.md
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty/
+-rw-r--r--   0 bart      (1000) bart      (1000)       87 2023-05-05 19:35:34.000000 betty-0.2.7/betty/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      254 2023-05-05 19:35:48.000000 betty-0.2.7/betty/about.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    25523 2023-05-05 19:35:34.000000 betty-0.2.7/betty/ancestry.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty/assets/
+-rw-r--r--   0 bart      (1000) bart      (1000)        6 2023-05-05 19:36:21.000000 betty-0.2.7/betty/assets/VERSION
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.503118 betty-0.2.7/betty/assets/locale/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.493118 betty-0.2.7/betty/assets/locale/fr_FR/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty/assets/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 bart      (1000) bart      (1000)    20871 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/locale/fr_FR/LC_MESSAGES/betty.po
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.503118 betty-0.2.7/betty/assets/locale/nl_NL/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty/assets/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 bart      (1000) bart      (1000)    19336 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/locale/nl_NL/LC_MESSAGES/betty.po
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.503118 betty-0.2.7/betty/assets/locale/uk/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty/assets/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 bart      (1000) bart      (1000)    20038 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/locale/uk/LC_MESSAGES/betty.po
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.503118 betty-0.2.7/betty/assets/public/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty/assets/public/localized/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty/assets/public/localized/api/
+-rw-r--r--   0 bart      (1000) bart      (1000)      620 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/localized/api/index.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     2776 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/localized/index.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      355 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/localized/search-index.json.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty/assets/public/static/
+-rw-r--r--   0 bart      (1000) bart      (1000)      524 2023-05-05 10:41:10.000000 betty-0.2.7/betty/assets/public/static/betty-16x16.png
+-rw-r--r--   0 bart      (1000) bart      (1000)     8229 2023-05-05 10:41:10.000000 betty-0.2.7/betty/assets/public/static/betty-192x192.png
+-rw-r--r--   0 bart      (1000) bart      (1000)     1101 2023-05-05 10:41:10.000000 betty-0.2.7/betty/assets/public/static/betty-32x32.png
+-rw-r--r--   0 bart      (1000) bart      (1000)    19708 2023-05-05 10:41:10.000000 betty-0.2.7/betty/assets/public/static/betty-512x512.png
+-rw-r--r--   0 bart      (1000) bart      (1000)    15406 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/betty.ico
+-rw-r--r--   0 bart      (1000) bart      (1000)      553 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/betty.webmanifest
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.523118 betty-0.2.7/betty/assets/public/static/css/
+-rw-r--r--   0 bart      (1000) bart      (1000)      333 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/accessibility.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      279 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/betty.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      506 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/citation.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      173 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/entity.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)     1491 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/file.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      300 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/meta.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      756 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/overlay.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)     3792 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/page.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      235 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/permalink.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      934 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/person.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)     2911 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/search.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      497 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/show.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      523 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/text.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)     2134 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/css/variables.scss.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     1813 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/file.js
+-rw-r--r--   0 bart      (1000) bart      (1000)      186 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/index.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       43 2023-05-05 10:41:10.000000 betty-0.2.7/betty/assets/public/static/robots.txt.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)    14924 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/schema.json
+-rw-r--r--   0 bart      (1000) bart      (1000)     6066 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/search.js
+-rw-r--r--   0 bart      (1000) bart      (1000)      626 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/show.js
+-rw-r--r--   0 bart      (1000) bart      (1000)     1075 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/public/static/sitemap.xml.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.523118 betty-0.2.7/betty/assets/templates/
+-rw-r--r--   0 bart      (1000) bart      (1000)     9824 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/base.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     1096 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/event-dimensions.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      397 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/file-extended--application--pdf.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      323 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/file-extended--image.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       49 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/file-extended.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       44 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/file-summary--application--pdf.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      263 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/file-summary--image.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       95 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/file-summary.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     2541 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/file.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      401 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/footer.html.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.523118 betty-0.2.7/betty/assets/templates/label/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1177 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/label/citation.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     1634 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/label/event.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      852 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/label/person.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      672 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/label/place.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       68 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/label/resource.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      282 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/label/source.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      505 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/list-event.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      409 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/list-file.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      677 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/list-person.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      798 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/list-place.html.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.523118 betty-0.2.7/betty/assets/templates/macro/
+-rw-r--r--   0 bart      (1000) bart      (1000)      433 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/macro/citation.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     1574 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/macro/person.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       88 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/macro/personname.html.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.523118 betty-0.2.7/betty/assets/templates/meta/
+-rw-r--r--   0 bart      (1000) bart      (1000)        0 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/meta/citation.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      115 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/meta/event.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     1741 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/meta/person.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      819 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/meta/place.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       67 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/meta/resource.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      218 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/meta/source.html.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/assets/templates/page/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1442 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/citation.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     1882 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/event.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     2496 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/file.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      365 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/list-event.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      361 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/list-file.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      430 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/list-person.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      380 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/list-place.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      538 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/list-source.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)    12829 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/person.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     2013 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/place.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     1217 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/page/source.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      166 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/permalink.html.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/assets/templates/search/
+-rw-r--r--   0 bart      (1000) bart      (1000)      552 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/search/result-file.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      667 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/search/result-person.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      250 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/search/result-place.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       66 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/search/result.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)       87 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/search/results.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      271 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/show-countable.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      442 2023-05-05 19:35:34.000000 betty-0.2.7/betty/assets/templates/show.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      768 2023-05-05 19:35:34.000000 betty-0.2.7/betty/asyncio.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5181 2023-05-05 19:35:34.000000 betty-0.2.7/betty/cli.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      594 2023-05-05 19:35:34.000000 betty-0.2.7/betty/concurrent.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7489 2023-05-05 19:35:34.000000 betty-0.2.7/betty/config.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1837 2023-05-05 19:35:34.000000 betty-0.2.7/betty/demo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      756 2023-05-05 19:35:34.000000 betty-0.2.7/betty/dispatch.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      946 2023-05-05 19:35:34.000000 betty-0.2.7/betty/error.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2684 2023-05-05 19:35:34.000000 betty-0.2.7/betty/fs.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      534 2023-05-05 19:35:34.000000 betty-0.2.7/betty/functools.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7483 2023-05-05 19:35:34.000000 betty-0.2.7/betty/generate.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1481 2023-05-05 19:35:34.000000 betty-0.2.7/betty/graph.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      203 2023-05-05 19:35:34.000000 betty-0.2.7/betty/html.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      379 2023-05-05 10:41:10.000000 betty-0.2.7/betty/importlib.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    18303 2023-05-05 19:35:34.000000 betty-0.2.7/betty/jinja2.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    13393 2023-05-05 19:35:34.000000 betty-0.2.7/betty/json.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    15776 2023-05-05 19:35:34.000000 betty-0.2.7/betty/locale.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      552 2023-05-05 10:41:10.000000 betty-0.2.7/betty/lock.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      708 2023-05-05 19:35:34.000000 betty-0.2.7/betty/logging.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1379 2023-05-05 19:35:34.000000 betty-0.2.7/betty/media_type.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     8742 2023-05-05 19:35:34.000000 betty-0.2.7/betty/openapi.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      677 2023-05-05 19:35:34.000000 betty-0.2.7/betty/os.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      363 2023-05-05 19:35:34.000000 betty-0.2.7/betty/parse.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      414 2023-05-05 19:35:34.000000 betty-0.2.7/betty/path.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1167 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/anonymizer/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3296 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/anonymizer/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/cleaner/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3876 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/cleaner/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/demo/
+-rw-r--r--   0 bart      (1000) bart      (1000)    10337 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/demo/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/deriver/
+-rw-r--r--   0 bart      (1000) bart      (1000)     8972 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/deriver/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/gramps/
+-rw-r--r--   0 bart      (1000) bart      (1000)    21692 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/gramps/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/maps/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2834 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/maps/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.503118 betty-0.2.7/betty/plugin/maps/assets/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/maps/assets/js/
+-rw-r--r--   0 bart      (1000) bart      (1000)       63 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/maps/assets/js/configuration.json.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     2395 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/maps/assets/js/maps.js
+-rw-r--r--   0 bart      (1000) bart      (1000)      109 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/maps/assets/js/maps.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)      543 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/maps/assets/js/package.json
+-rw-r--r--   0 bart      (1000) bart      (1000)     1870 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/maps/assets/js/webpack.config.js
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      278 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/maps/assets/js/webpack.config.json.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/nginx/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3012 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/nginx/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      998 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/nginx/artifact.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/nginx/assets/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/nginx/assets/docker/
+-rw-r--r--   0 bart      (1000) bart      (1000)      222 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/nginx/assets/docker/Dockerfile
+-rw-r--r--   0 bart      (1000) bart      (1000)     3048 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/nginx/assets/nginx.conf.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)     1706 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/nginx/docker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1976 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/nginx/serve.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/privatizer/
+-rw-r--r--   0 bart      (1000) bart      (1000)     4966 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/privatizer/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/trees/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2704 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/trees/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.503118 betty-0.2.7/betty/plugin/trees/assets/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/trees/assets/js/
+-rw-r--r--   0 bart      (1000) bart      (1000)      509 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/trees/assets/js/package.json
+-rw-r--r--   0 bart      (1000) bart      (1000)     3407 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/trees/assets/js/trees.js
+-rw-r--r--   0 bart      (1000) bart      (1000)      111 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/trees/assets/js/trees.scss
+-rw-r--r--   0 bart      (1000) bart      (1000)     1604 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/trees/assets/js/webpack.config.js
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      278 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/trees/assets/js/webpack.config.json.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.503118 betty-0.2.7/betty/plugin/trees/assets/public/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/trees/assets/public/localized/
+-rw-r--r--   0 bart      (1000) bart      (1000)      589 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/trees/assets/public/localized/people.json.j2
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/wikipedia/
+-rw-r--r--   0 bart      (1000) bart      (1000)     9574 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/wikipedia/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.503118 betty-0.2.7/betty/plugin/wikipedia/assets/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.533118 betty-0.2.7/betty/plugin/wikipedia/assets/templates/
+-rw-r--r--   0 bart      (1000) bart      (1000)      439 2023-05-05 19:35:34.000000 betty-0.2.7/betty/plugin/wikipedia/assets/templates/wikipedia.html.j2
+-rw-r--r--   0 bart      (1000) bart      (1000)      648 2023-05-05 19:35:34.000000 betty-0.2.7/betty/render.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1219 2023-05-05 19:35:34.000000 betty-0.2.7/betty/sass.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1864 2023-05-05 19:35:34.000000 betty-0.2.7/betty/search.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3119 2023-05-05 19:35:34.000000 betty-0.2.7/betty/serve.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7744 2023-05-05 19:35:34.000000 betty-0.2.7/betty/site.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      418 2023-05-05 19:35:34.000000 betty-0.2.7/betty/subprocess.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4303 2023-05-05 19:35:34.000000 betty-0.2.7/betty/url.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      443 2023-05-05 19:35:34.000000 betty-0.2.7/betty/voluptuous.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-05 19:36:21.513118 betty-0.2.7/betty.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)    16818 2023-05-05 19:36:21.000000 betty-0.2.7/betty.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     5465 2023-05-05 19:36:21.000000 betty-0.2.7/betty.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-05-05 19:36:21.000000 betty-0.2.7/betty.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       42 2023-05-05 19:36:21.000000 betty-0.2.7/betty.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      445 2023-05-05 19:36:21.000000 betty-0.2.7/betty.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        6 2023-05-05 19:36:21.000000 betty-0.2.7/betty.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-05-05 19:36:21.533118 betty-0.2.7/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)     2947 2023-05-05 19:35:48.000000 betty-0.2.7/setup.py
```

### Comparing `betty-0.2.6/PKG-INFO` & `betty-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: betty
-Version: 0.2.6
+Version: 0.2.7
 Summary: Betty is a static ancestry site generator.
 Home-page: https://github.com/bartfeenstra/betty
 Author: Bart Feenstra & contributors
 Author-email: bart@mynameisbart.com
 License: GPLv3
 Description: # Betty 👵
         
-        ![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/master/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project) 
+        ![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg?branch=0.2.x) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/0.2.x/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project)
         
         Betty is a static site generator for [Gramps](https://gramps-project.org/) and
         [GEDCOM](https://en.wikipedia.org/wiki/GEDCOM) family trees.
         
         ## Table of Contents
         
         - [Features](#features)
@@ -39,17 +39,17 @@
         - [Responsive](https://en.wikipedia.org/wiki/Responsive_web_design), and mobile- and touch-friendly interface.
         - Privacy and anonymization filters for living people.
         - [View an example](https://ancestry.bartfeenstra.com/).
         
         ## Installation
         
         ### Requirements
-        - **Python 3.6+**
+        - **Python 3.7+**
         - Node.js 10+ (optional)
-        - Linux, Mac OS, or Windows. On Windows you are encouraged to use Python 3.6, 3.7, or 3.8, because one of Betty's
+        - Linux, Mac OS, or Windows. On Windows you are encouraged to use Python 3.7 or 3.8, because one of Betty's
           dependencies (libsass) cannot be installed automatically when using Python 3.9.
         
         ### Instructions
         Run `pip install betty` to install the latest stable release.
         
         To install the latest development version, run `pip install git+https://github.com/bartfeenstra/betty.git`. If you want
         the latest source code, read the [development](#development) documentation.
@@ -280,24 +280,25 @@
         Betty is copyright [Bart Feenstra](https://twitter.com/BartFeenstra/) and contributors, and released under the
         [GNU General Public License, Version 3](./LICENSE.txt). In short, that means **you are free to use Betty**, but **if you
         distribute Betty yourself, you must do so under the exact same license**, provide that license, and make your source
         code available. 
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: JavaScript
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology :: Genealogy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Natural Language :: Dutch
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Ukrainian
-Requires-Python: ~= 3.6
+Requires-Python: ~= 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: development
```

### Comparing `betty-0.2.6/README.md` & `betty-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Betty 👵
 
-![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/master/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project) 
+![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg?branch=0.2.x) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/0.2.x/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project)
 
 Betty is a static site generator for [Gramps](https://gramps-project.org/) and
 [GEDCOM](https://en.wikipedia.org/wiki/GEDCOM) family trees.
 
 ## Table of Contents
 
 - [Features](#features)
@@ -31,17 +31,17 @@
 - [Responsive](https://en.wikipedia.org/wiki/Responsive_web_design), and mobile- and touch-friendly interface.
 - Privacy and anonymization filters for living people.
 - [View an example](https://ancestry.bartfeenstra.com/).
 
 ## Installation
 
 ### Requirements
-- **Python 3.6+**
+- **Python 3.7+**
 - Node.js 10+ (optional)
-- Linux, Mac OS, or Windows. On Windows you are encouraged to use Python 3.6, 3.7, or 3.8, because one of Betty's
+- Linux, Mac OS, or Windows. On Windows you are encouraged to use Python 3.7 or 3.8, because one of Betty's
   dependencies (libsass) cannot be installed automatically when using Python 3.9.
 
 ### Instructions
 Run `pip install betty` to install the latest stable release.
 
 To install the latest development version, run `pip install git+https://github.com/bartfeenstra/betty.git`. If you want
 the latest source code, read the [development](#development) documentation.
```

### Comparing `betty-0.2.6/betty/ancestry.py` & `betty-0.2.7/betty/ancestry.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/asyncio.py` & `betty-0.2.7/betty/asyncio.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/cli.py` & `betty-0.2.7/betty/cli.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/concurrent.py` & `betty-0.2.7/betty/concurrent.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/config.py` & `betty-0.2.7/betty/config.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/demo.py` & `betty-0.2.7/betty/demo.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/dispatch.py` & `betty-0.2.7/betty/dispatch.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/error.py` & `betty-0.2.7/betty/error.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/fs.py` & `betty-0.2.7/betty/fs.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/functools.py` & `betty-0.2.7/betty/functools.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/generate.py` & `betty-0.2.7/betty/generate.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/graph.py` & `betty-0.2.7/betty/graph.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/jinja2.py` & `betty-0.2.7/betty/jinja2.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/json.py` & `betty-0.2.7/betty/json.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/locale.py` & `betty-0.2.7/betty/locale.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/lock.py` & `betty-0.2.7/betty/lock.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/logging.py` & `betty-0.2.7/betty/logging.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/media_type.py` & `betty-0.2.7/betty/media_type.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/openapi.py` & `betty-0.2.7/betty/openapi.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/os.py` & `betty-0.2.7/betty/os.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/__init__.py` & `betty-0.2.7/betty/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/anonymizer/__init__.py` & `betty-0.2.7/betty/plugin/anonymizer/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/cleaner/__init__.py` & `betty-0.2.7/betty/plugin/cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/demo/__init__.py` & `betty-0.2.7/betty/plugin/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/deriver/__init__.py` & `betty-0.2.7/betty/plugin/deriver/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/gramps/__init__.py` & `betty-0.2.7/betty/plugin/gramps/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/maps/__init__.py` & `betty-0.2.7/betty/plugin/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/nginx/__init__.py` & `betty-0.2.7/betty/plugin/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/nginx/artifact.py` & `betty-0.2.7/betty/plugin/nginx/artifact.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/nginx/docker.py` & `betty-0.2.7/betty/plugin/nginx/docker.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/nginx/serve.py` & `betty-0.2.7/betty/plugin/nginx/serve.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/privatizer/__init__.py` & `betty-0.2.7/betty/plugin/privatizer/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/trees/__init__.py` & `betty-0.2.7/betty/plugin/trees/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/plugin/wikipedia/__init__.py` & `betty-0.2.7/betty/plugin/wikipedia/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/render.py` & `betty-0.2.7/betty/render.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/sass.py` & `betty-0.2.7/betty/sass.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/search.py` & `betty-0.2.7/betty/search.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/serve.py` & `betty-0.2.7/betty/serve.py`

 * *Files identical despite different names*

### Comparing `betty-0.2.6/betty/site.py` & `betty-0.2.7/betty/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 
 from betty.concurrent import ExceptionRaisingExecutor
 from betty.dispatch import Dispatcher
 from betty.lock import Locks
 from betty.render import Renderer, SequentialRenderer
 from betty.sass import SassRenderer
 
-try:
-    from contextlib import AsyncExitStack
-except ImportError:
-    from async_exit_stack import AsyncExitStack
+from contextlib import AsyncExitStack
 from copy import copy
 from os.path import abspath, dirname, join
 from typing import Type, Dict
 
 from betty.ancestry import Ancestry
 from betty.config import Configuration
 from betty.fs import FileSystem
```

### Comparing `betty-0.2.6/betty/tests/test_url.py` & `betty-0.2.7/betty/url.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,98 @@
-from typing import Any
+from contextlib import suppress
+from typing import Any, Type, Optional
 
-from parameterized import parameterized
-
-from betty.ancestry import Person, Place, File, Source, Identifiable, PlaceName, IdentifiableEvent, \
-    IdentifiableSource, IdentifiableCitation, Death
-from betty.config import Configuration, LocaleConfiguration
-from betty.tests import TestCase
-from betty.url import LocalizedPathUrlGenerator, IdentifiableResourceUrlGenerator, SiteUrlGenerator
-
-
-class LocalizedPathUrlGeneratorTest(TestCase):
-    @parameterized.expand([
-        ('/', '/'),
-        ('/index.html', '/index.html'),
-        ('/example', 'example'),
-        ('/example', '/example'),
-        ('/example/', 'example/'),
-        ('/example/', '/example/'),
-        ('/example/index.html', 'example/index.html'),
-        ('/example/index.html', '/example/index.html'),
-    ])
-    def test_generate(self, expected: str, resource: str):
-        configuration = Configuration('/tmp', 'https://example.com')
-        sut = LocalizedPathUrlGenerator(configuration)
-        self.assertEquals(expected, sut.generate(resource, 'text/html'))
-
-    @parameterized.expand([
-        ('/', 'index.html'),
-        ('/', '/index.html'),
-        ('/example/', 'example/index.html'),
-        ('/example/', '/example/index.html'),
-    ])
-    def test_generate_with_clean_urls(self, expected: str, resource: str):
-        configuration = Configuration('/tmp', 'https://example.com')
-        configuration.clean_urls = True
-        sut = LocalizedPathUrlGenerator(configuration)
-        self.assertEquals(expected, sut.generate(resource, 'text/html'))
-
-    @parameterized.expand([
-        ('https://example.com/', '/'),
-        ('https://example.com/example', 'example'),
-    ])
-    def test_generate_absolute(self, expected: str, resource: str):
-        configuration = Configuration('/tmp', 'https://example.com')
-        sut = LocalizedPathUrlGenerator(configuration)
-        self.assertEquals(expected, sut.generate(
-            resource, 'text/html', absolute=True))
-
-    def test_generate_with_invalid_value(self):
-        configuration = Configuration('/tmp', 'https://example.com')
-        sut = LocalizedPathUrlGenerator(configuration)
-        with self.assertRaises(ValueError):
-            sut.generate(9, 'text/html')
-
-    def test_generate_multilingual(self):
-        configuration = Configuration('/tmp', 'https://example.com')
-        configuration.locales.clear()
-        configuration.locales['nl'] = LocaleConfiguration('nl')
-        configuration.locales['en'] = LocaleConfiguration('en')
-        sut = LocalizedPathUrlGenerator(configuration)
-        self.assertEquals('/nl/index.html',
-                          sut.generate('/index.html', 'text/html'))
-        self.assertEquals(
-            '/en/index.html', sut.generate('/index.html', 'text/html', locale='en'))
-
-
-class IdentifiableResourceUrlGeneratorTest(TestCase):
-    def test_generate(self):
-        configuration = Configuration('/tmp', 'https://example.com')
-        sut = IdentifiableResourceUrlGenerator(
-            configuration, Identifiable, 'prefix/%s/index.%s')
-        self.assertEquals('/prefix/I1/index.html',
-                          sut.generate(Identifiable('I1'), 'text/html'))
-
-    def test_generate_with_invalid_value(self):
-        configuration = Configuration('/tmp', 'https://example.com')
-        sut = IdentifiableResourceUrlGenerator(
-            configuration, Identifiable, 'prefix/%s/index.html')
-        with self.assertRaises(ValueError):
-            sut.generate(9, 'text/html')
-
-
-class SiteUrlGeneratorTest(TestCase):
-    @parameterized.expand([
-        ('/index.html', '/index.html'),
-        ('/person/P1/index.html', Person('P1')),
-        ('/event/E1/index.html', IdentifiableEvent('E1', Death())),
-        ('/place/P1/index.html', Place('P1', [PlaceName('Place 1')])),
-        ('/file/F1/index.html', File('F1', '/tmp')),
-        ('/source/S1/index.html', IdentifiableSource('S1', 'Source 1')),
-        ('/citation/C1/index.html', IdentifiableCitation('C1', Source('Source 1'))),
-    ])
-    def test_generate(self, expected: str, resource: Any):
-        configuration = Configuration('/tmp', 'https://example.com')
-        sut = SiteUrlGenerator(configuration)
-        self.assertEquals(expected, sut.generate(resource, 'text/html'))
-
-    def test_generate_with_invalid_value(self):
-        configuration = Configuration('/tmp', 'https://example.com')
-        sut = SiteUrlGenerator(configuration)
-        with self.assertRaises(ValueError):
-            sut.generate(9, 'text/html')
+from betty.ancestry import Person, File, Place, Identifiable, PersonName, IdentifiableSource, IdentifiableEvent, \
+    IdentifiableCitation
+from betty.config import Configuration
+from betty.media_type import EXTENSIONS
+
+
+class LocalizedUrlGenerator:
+    def generate(self, resource: Any, media_type: str, absolute: bool = False, locale: Optional[str] = None) -> str:
+        raise NotImplementedError
+
+
+class StaticUrlGenerator:
+    def generate(self, resource: Any, absolute: bool = False, ) -> str:
+        raise NotImplementedError
+
+
+class LocalizedPathUrlGenerator(LocalizedUrlGenerator):
+    def __init__(self, configuration: Configuration):
+        self._configuration = configuration
+
+    def generate(self, resource, media_type, **kwargs) -> str:
+        return _generate_from_path(self._configuration, resource, localize=True, **kwargs)
+
+
+class StaticPathUrlGenerator(StaticUrlGenerator):
+    def __init__(self, configuration: Configuration):
+        self._configuration = configuration
+
+    def generate(self, resource, **kwargs) -> str:
+        return _generate_from_path(self._configuration, resource, localize=False, **kwargs)
+
+
+class IdentifiableResourceUrlGenerator(LocalizedUrlGenerator):
+    def __init__(self, configuration: Configuration, identifiable_type: Type[Identifiable], pattern: str):
+        self._configuration = configuration
+        self._type = identifiable_type
+        self._pattern = pattern
+
+    def generate(self, resource: Identifiable, media_type, **kwargs) -> str:
+        if not isinstance(resource, self._type):
+            raise ValueError('%s is not a %s' % (type(resource), self._type))
+        kwargs['localize'] = True
+        return _generate_from_path(self._configuration, self._pattern % (resource.id, EXTENSIONS[media_type]), **kwargs)
+
+
+class PersonNameUrlGenerator(LocalizedUrlGenerator):
+    def __init__(self, person_url_generator: LocalizedUrlGenerator):
+        self._person_url_generator = person_url_generator
+
+    def generate(self, name: PersonName, *args, **kwargs) -> str:
+        if not isinstance(name, PersonName):
+            raise ValueError('%s is not a %s' % (type(name), PersonName))
+        return self._person_url_generator.generate(name.person, *args, **kwargs)
+
+
+class SiteUrlGenerator(LocalizedUrlGenerator):
+    def __init__(self, configuration: Configuration):
+        person_url_generator = IdentifiableResourceUrlGenerator(configuration, Person, 'person/%s/index.%s')
+        self._generators = [
+            person_url_generator,
+            PersonNameUrlGenerator(person_url_generator),
+            IdentifiableResourceUrlGenerator(
+                configuration, IdentifiableEvent, 'event/%s/index.%s'),
+            IdentifiableResourceUrlGenerator(
+                configuration, Place, 'place/%s/index.%s'),
+            IdentifiableResourceUrlGenerator(
+                configuration, File, 'file/%s/index.%s'),
+            IdentifiableResourceUrlGenerator(
+                configuration, IdentifiableSource, 'source/%s/index.%s'),
+            IdentifiableResourceUrlGenerator(
+                configuration, IdentifiableCitation, 'citation/%s/index.%s'),
+            LocalizedPathUrlGenerator(configuration),
+        ]
+
+    def generate(self, resource: Any, *args, **kwargs) -> str:
+        for generator in self._generators:
+            with suppress(ValueError):
+                return generator.generate(resource, *args, **kwargs)
+        raise ValueError('No URL generator found for %s.' % (
+            resource if isinstance(resource, str) else type(resource)))
+
+
+def _generate_from_path(configuration: Configuration, path: str, localize: bool = False, absolute: bool = False, locale: Optional[str] = None) -> str:
+    if not isinstance(path, str):
+        raise ValueError('%s is not a string.' % type(path))
+    url = configuration.base_url if absolute else ''
+    url += configuration.root_path
+    if localize and configuration.multilingual:
+        if locale is None:
+            locale = configuration.default_locale
+        url += configuration.locales[locale].alias + '/'
+    url += path.lstrip('/')
+    if configuration.clean_urls and (path.endswith('/index.html') or path == 'index.html'):
+        url = url[:-10]
+    return url
```

### Comparing `betty-0.2.6/betty.egg-info/PKG-INFO` & `betty-0.2.7/betty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: betty
-Version: 0.2.6
+Version: 0.2.7
 Summary: Betty is a static ancestry site generator.
 Home-page: https://github.com/bartfeenstra/betty
 Author: Bart Feenstra & contributors
 Author-email: bart@mynameisbart.com
 License: GPLv3
 Description: # Betty 👵
         
-        ![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/master/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project) 
+        ![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg?branch=0.2.x) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/0.2.x/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project)
         
         Betty is a static site generator for [Gramps](https://gramps-project.org/) and
         [GEDCOM](https://en.wikipedia.org/wiki/GEDCOM) family trees.
         
         ## Table of Contents
         
         - [Features](#features)
@@ -39,17 +39,17 @@
         - [Responsive](https://en.wikipedia.org/wiki/Responsive_web_design), and mobile- and touch-friendly interface.
         - Privacy and anonymization filters for living people.
         - [View an example](https://ancestry.bartfeenstra.com/).
         
         ## Installation
         
         ### Requirements
-        - **Python 3.6+**
+        - **Python 3.7+**
         - Node.js 10+ (optional)
-        - Linux, Mac OS, or Windows. On Windows you are encouraged to use Python 3.6, 3.7, or 3.8, because one of Betty's
+        - Linux, Mac OS, or Windows. On Windows you are encouraged to use Python 3.7 or 3.8, because one of Betty's
           dependencies (libsass) cannot be installed automatically when using Python 3.9.
         
         ### Instructions
         Run `pip install betty` to install the latest stable release.
         
         To install the latest development version, run `pip install git+https://github.com/bartfeenstra/betty.git`. If you want
         the latest source code, read the [development](#development) documentation.
@@ -280,24 +280,25 @@
         Betty is copyright [Bart Feenstra](https://twitter.com/BartFeenstra/) and contributors, and released under the
         [GNU General Public License, Version 3](./LICENSE.txt). In short, that means **you are free to use Betty**, but **if you
         distribute Betty yourself, you must do so under the exact same license**, provide that license, and make your source
         code available. 
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: JavaScript
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology :: Genealogy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Natural Language :: Dutch
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Ukrainian
-Requires-Python: ~= 3.6
+Requires-Python: ~= 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: development
```

### Comparing `betty-0.2.6/setup.py` & `betty-0.2.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 """Integrates Betty with Python's setuptools."""
+from os import path
 
-import os
-from glob import glob
-from os.path import abspath, dirname, join
+from setuptools import setup
 
-from setuptools import setup, find_packages
+from betty._package import find_packages, get_data_paths
 
-ROOT_PATH = os.path.dirname(os.path.abspath(__file__))
+ROOT_PATH = path.dirname(path.abspath(__file__))
 
-with open('/'.join((ROOT_PATH, 'VERSION'))) as f:
+with open(path.join(ROOT_PATH, 'betty', 'assets', 'VERSION')) as f:
     VERSION = f.read()
 
-with open('/'.join((ROOT_PATH, 'README.md'))) as f:
+with open(path.join(ROOT_PATH, 'README.md')) as f:
     long_description = f.read()
 
 SETUP = {
     'name': 'betty',
     'description': 'Betty is a static ancestry site generator.',
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
     'version': VERSION,
     'license': 'GPLv3',
     'author': 'Bart Feenstra & contributors',
     'author_email': 'bart@mynameisbart.com',
     'url': 'https://github.com/bartfeenstra/betty',
     'classifiers': [
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: JavaScript',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: JavaScript',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
+        'Topic :: Internet',
         'Topic :: Scientific/Engineering :: Visualization',
         'Topic :: Sociology :: Genealogy',
         'Topic :: Software Development :: Code Generators',
         'Natural Language :: Dutch',
         'Natural Language :: English',
         'Natural Language :: Ukrainian',
     ],
-    'python_requires': '~= 3.6',
+    'python_requires': '~= 3.7',
     'install_requires': [
         'aiohttp ~= 3.7',
-        'async-exit-stack ~= 1.0; python_version <= "3.6"',
-        'async_generator ~= 1.10; python_version <= "3.6"',
         'babel ~= 2.9',
         'click ~= 7.1',
         'docker ~= 4.4',
+        # Work around https://github.com/docker/docker-py/issues/3113 by pinning urllib3 to a compatible version.
+        'urllib3 < 2',
         'geopy ~= 2.0',
         'jinja2 ~= 2.11',
         'jsonschema ~= 3.2',
         'libsass ~= 0.20',
         'markupsafe ~= 1.1',
         'pdf2image ~= 1.14 ',
         'python-resize-image ~= 1.1',
@@ -69,38 +69,22 @@
             'flake8 ~= 3.7.0',
             'html5lib ~= 1.1',
             'mock ~= 4.0; python_version <= "3.7"',
             'lxml ~= 4.6',
             'nose2 ~= 0.9',
             'parameterized ~= 0.7',
             'setuptools ~= 50.3',
-            'twine ~= 3.2',
-            'wheel ~= 0.36',
+            'twine ~= 4.0, >= 4.0.0',
+            'wheel ~= 0.40, >= 0.40.0',
         ],
     },
     'entry_points': {
         'console_scripts': [
             'betty=betty.cli:main',
         ],
     },
     'packages': find_packages(),
-    'data_files': [
-        ('', [
-            'LICENSE.txt',
-            'README.md',
-            'VERSION',
-        ])
-    ],
-    'include_package_data': True,
-    'package_data': {
-        'betty': [
-                     join(dirname(__file__), 'VERSION'),
-                 ]
-                 +
-                 glob(join(dirname(abspath(__file__)), 'betty', 'assets', '**'), recursive=True)
-                 +
-                 glob(join(dirname(abspath(__file__)), 'betty', 'plugin', '*', 'assets', '**'), recursive=True),
-    },
+    'package_data': get_data_paths(),
 }
 
 if __name__ == '__main__':
     setup(**SETUP)
```

