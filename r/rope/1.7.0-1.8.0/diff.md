# Comparing `tmp/rope-1.7.0.tar.gz` & `tmp/rope-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rope-1.7.0.tar", last modified: Tue Jan 17 02:36:06 2023, max compression
+gzip compressed data, was "rope-1.8.0.tar", last modified: Fri May  5 05:06:22 2023, max compression
```

## Comparing `rope-1.7.0.tar` & `rope-1.8.0.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.582532 rope-1.7.0/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14368 2023-01-17 01:59:16.000000 rope-1.7.0/.all-contributorsrc
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      125 2022-07-29 12:45:37.000000 rope-1.7.0/.git-blame-ignore-revs
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.538530 rope-1.7.0/.github/
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.538530 rope-1.7.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      916 2022-07-29 12:45:37.000000 rope-1.7.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      595 2022-07-29 12:45:37.000000 rope-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      411 2023-01-17 01:59:16.000000 rope-1.7.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.538530 rope-1.7.0/.github/workflows/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      160 2022-07-29 12:45:37.000000 rope-1.7.0/.github/workflows/black.yml
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      670 2023-01-17 01:59:16.000000 rope-1.7.0/.github/workflows/main.yml
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      274 2023-01-17 01:59:16.000000 rope-1.7.0/.github/workflows/task-completed-checker-action.yml
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1864 2022-07-29 12:46:52.000000 rope-1.7.0/.gitignore
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      120 2022-07-29 12:45:37.000000 rope-1.7.0/.readthedocs.yaml
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9416 2023-01-17 02:31:57.000000 rope-1.7.0/CHANGELOG.md
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    21134 2023-01-17 01:59:16.000000 rope-1.7.0/CONTRIBUTORS.md
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7652 2022-07-29 12:45:37.000000 rope-1.7.0/COPYING
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      150 2022-07-29 12:45:37.000000 rope-1.7.0/MANIFEST.in
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5084 2023-01-17 02:36:06.582532 rope-1.7.0/PKG-INFO
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3911 2023-01-17 01:59:16.000000 rope-1.7.0/README.rst
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.538530 rope-1.7.0/bin/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1607 2023-01-17 01:59:16.000000 rope-1.7.0/bin/tag-release.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.542530 rope-1.7.0/docs/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      634 2022-07-29 12:45:37.000000 rope-1.7.0/docs/Makefile
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2247 2022-09-19 07:11:34.000000 rope-1.7.0/docs/conf.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1719 2023-01-17 01:59:16.000000 rope-1.7.0/docs/configuration.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4062 2023-01-17 01:59:16.000000 rope-1.7.0/docs/contributing.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5165 2022-12-16 04:43:54.000000 rope-1.7.0/docs/default_config.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.542530 rope-1.7.0/docs/dev/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3906 2023-01-17 01:59:16.000000 rope-1.7.0/docs/dev/issues.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      526 2023-01-17 01:59:16.000000 rope-1.7.0/docs/index.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    28522 2023-01-17 01:59:16.000000 rope-1.7.0/docs/library.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      765 2022-07-29 12:45:37.000000 rope-1.7.0/docs/make.bat
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    31016 2023-01-17 01:59:16.000000 rope-1.7.0/docs/overview.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      439 2023-01-17 01:59:16.000000 rope-1.7.0/docs/release-process.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1459 2022-09-19 07:41:21.000000 rope-1.7.0/docs/rope.rst
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2211 2023-01-17 02:32:38.000000 rope-1.7.0/pyproject.toml
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.542530 rope-1.7.0/rope/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1431 2023-01-17 01:59:16.000000 rope-1.7.0/rope/__init__.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.550531 rope-1.7.0/rope/base/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      161 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3283 2022-12-15 11:40:37.000000 rope-1.7.0/rope/base/arguments.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2416 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/ast.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    26263 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/builtins.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13675 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/change.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11774 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/codeanalyze.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13587 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/evaluate.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1370 2022-12-15 11:40:37.000000 rope-1.7.0/rope/base/exceptions.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8421 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/fscommands.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8342 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/history.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3841 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/libutils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1656 2022-12-15 11:40:37.000000 rope-1.7.0/rope/base/nameanalyze.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.554531 rope-1.7.0/rope/base/oi/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1682 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7369 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/doa.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3440 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/memorydb.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4547 2022-12-16 03:37:02.000000 rope-1.7.0/rope/base/oi/objectdb.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8624 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/objectinfo.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8519 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/runmod.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5862 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/soa.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7800 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/soi.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9829 2022-12-15 11:40:37.000000 rope-1.7.0/rope/base/oi/transform.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.554531 rope-1.7.0/rope/base/oi/type_hinting/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8867 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/type_hinting/evaluate.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2728 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/type_hinting/factory.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      715 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/interfaces.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.558531 rope-1.7.0/rope/base/oi/type_hinting/providers/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/providers/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1856 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/providers/composite.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6167 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/providers/docstrings.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2116 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/providers/inheritance.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1055 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/providers/interfaces.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1389 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/type_hinting/providers/numpydocstrings.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1525 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/type_hinting/providers/pep0484_type_comments.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.558531 rope-1.7.0/rope/base/oi/type_hinting/resolvers/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/resolvers/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      778 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/resolvers/composite.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      405 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/resolvers/interfaces.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      611 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/oi/type_hinting/resolvers/types.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5162 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/oi/type_hinting/utils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    10158 2023-01-17 01:59:43.000000 rope-1.7.0/rope/base/prefs.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14976 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/project.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12805 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/pycore.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6390 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/pynames.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2098 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/pynamesdef.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9179 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/pyobjects.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22735 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/pyobjectsdef.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11468 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/pyscopes.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    10291 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/resourceobserver.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7892 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/resources.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5590 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/serializer.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1905 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/simplify.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1607 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/stdmods.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4990 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/taskhandle.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.558531 rope-1.7.0/rope/base/utils/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3949 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/utils/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1824 2022-12-15 11:40:37.000000 rope-1.7.0/rope/base/utils/datastructures.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1405 2023-01-17 01:59:16.000000 rope-1.7.0/rope/base/versioning.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22416 2022-07-29 12:45:37.000000 rope-1.7.0/rope/base/worder.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.562531 rope-1.7.0/rope/contrib/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      169 2022-07-29 12:45:37.000000 rope-1.7.0/rope/contrib/__init__.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.562531 rope-1.7.0/rope/contrib/autoimport/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      196 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/autoimport/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2444 2022-07-29 12:45:37.000000 rope-1.7.0/rope/contrib/autoimport/defs.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3273 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/autoimport/models.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5276 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/autoimport/parse.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8394 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/autoimport/pickle.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    19713 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/autoimport/sqlite.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4823 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/autoimport/utils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1350 2022-07-29 12:45:37.000000 rope-1.7.0/rope/contrib/changestack.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    26473 2022-12-15 11:40:37.000000 rope-1.7.0/rope/contrib/codeassist.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2935 2022-12-15 11:40:37.000000 rope-1.7.0/rope/contrib/finderrors.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4483 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/findit.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2194 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/fixmodnames.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6777 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/fixsyntax.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14846 2023-01-17 01:59:16.000000 rope-1.7.0/rope/contrib/generate.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.570531 rope-1.7.0/rope/refactor/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2126 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13432 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/change_signature.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8459 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/encapsulate_field.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    39148 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/extract.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8316 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/functionutils.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.570531 rope-1.7.0/rope/refactor/importutils/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13354 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/importutils/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14255 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/importutils/actions.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5735 2022-07-29 12:45:37.000000 rope-1.7.0/rope/refactor/importutils/importinfo.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    21673 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/importutils/module_imports.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    25111 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/inline.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5913 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/introduce_factory.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3717 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/introduce_parameter.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2076 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/localtofield.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3829 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/method_object.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    33953 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/move.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2544 2022-12-15 11:40:37.000000 rope-1.7.0/rope/refactor/multiproject.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13040 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/occurrences.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    31196 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/patchedast.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9348 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/rename.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11441 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/restructure.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12719 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/similarfinder.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3001 2022-12-15 11:40:37.000000 rope-1.7.0/rope/refactor/sourceutils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5152 2022-12-15 11:40:37.000000 rope-1.7.0/rope/refactor/suites.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1226 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/topackage.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6651 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/usefunction.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5740 2023-01-17 01:59:16.000000 rope-1.7.0/rope/refactor/wildcards.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.542530 rope-1.7.0/rope.egg-info/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5084 2023-01-17 02:36:06.000000 rope-1.7.0/rope.egg-info/PKG-INFO
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5070 2023-01-17 02:36:06.000000 rope-1.7.0/rope.egg-info/SOURCES.txt
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        1 2023-01-17 02:36:06.000000 rope-1.7.0/rope.egg-info/dependency_links.txt
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      199 2023-01-17 02:36:06.000000 rope-1.7.0/rope.egg-info/requires.txt
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        5 2023-01-17 02:36:06.000000 rope-1.7.0/rope.egg-info/top_level.txt
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.574531 rope-1.7.0/ropetest/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-12-15 11:40:37.000000 rope-1.7.0/ropetest/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    37493 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/advanced_oi_test.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    23217 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/builtinstest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    35910 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/codeanalyzetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      787 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/conftest.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.578532 rope-1.7.0/ropetest/contrib/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-12-15 11:40:37.000000 rope-1.7.0/ropetest/contrib/__init__.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.578532 rope-1.7.0/ropetest/contrib/autoimport/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      795 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/autoimport/autoimporttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      703 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/autoimport/conftest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2128 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/autoimport/modeltest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      647 2022-07-29 12:45:37.000000 rope-1.7.0/ropetest/contrib/autoimport/parsetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1884 2022-12-15 11:40:37.000000 rope-1.7.0/ropetest/contrib/autoimport/utilstest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7286 2022-11-22 15:02:03.000000 rope-1.7.0/ropetest/contrib/autoimporttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      955 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/changestacktest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    56041 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/codeassisttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1629 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/finderrorstest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5475 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/findittest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2066 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/fixmodnamestest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15157 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/contrib/generatetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2894 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/doatest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15912 2022-12-15 11:40:37.000000 rope-1.7.0/ropetest/historytest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6879 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/objectdbtest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15681 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/objectinfertest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    48095 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/projecttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    52145 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/pycoretest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    19385 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/pyscopestest.py
-drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-01-17 02:36:06.582532 rope-1.7.0/ropetest/refactor/
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    38589 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/__init__.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    27113 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/change_signature_test.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)   101254 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/extracttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    69500 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/importutilstest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    42803 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/inlinetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    41603 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/movetest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3434 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/multiprojecttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    59540 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/patchedasttest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    50303 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/renametest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9672 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/restructuretest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12065 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/similarfindertest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6766 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/suitestest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6400 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/refactor/usefunctiontest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5653 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/reprtest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6404 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/runmodtest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4801 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/serializer_test.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2203 2022-11-22 15:02:03.000000 rope-1.7.0/ropetest/simplifytest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3166 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/testutils.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    16326 2022-12-15 11:40:37.000000 rope-1.7.0/ropetest/type_hinting_test.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1448 2023-01-17 01:59:16.000000 rope-1.7.0/ropetest/versioningtest.py
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      154 2023-01-17 02:36:06.582532 rope-1.7.0/setup.cfg
--rw-rw-r--   0 lieryan   (1000) lieryan   (1000)       38 2022-12-15 11:40:37.000000 rope-1.7.0/setup.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.501347 rope-1.8.0/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14368 2023-01-17 01:59:16.000000 rope-1.8.0/.all-contributorsrc
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      125 2022-07-29 12:45:37.000000 rope-1.8.0/.git-blame-ignore-revs
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.417344 rope-1.8.0/.github/
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.421344 rope-1.8.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      916 2022-07-29 12:45:37.000000 rope-1.8.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      595 2022-07-29 12:45:37.000000 rope-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      411 2023-01-17 01:59:16.000000 rope-1.8.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.421344 rope-1.8.0/.github/workflows/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      160 2022-07-29 12:45:37.000000 rope-1.8.0/.github/workflows/black.yml
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      742 2023-05-05 04:53:06.000000 rope-1.8.0/.github/workflows/main.yml
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      274 2023-01-17 01:59:16.000000 rope-1.8.0/.github/workflows/task-completed-checker-action.yml
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1864 2022-07-29 12:46:52.000000 rope-1.8.0/.gitignore
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      120 2022-07-29 12:45:37.000000 rope-1.8.0/.readthedocs.yaml
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9838 2023-05-05 04:58:59.000000 rope-1.8.0/CHANGELOG.md
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    21134 2023-01-17 01:59:16.000000 rope-1.8.0/CONTRIBUTORS.md
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7652 2022-07-29 12:45:37.000000 rope-1.8.0/COPYING
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      150 2022-07-29 12:45:37.000000 rope-1.8.0/MANIFEST.in
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5673 2023-05-05 05:06:22.501347 rope-1.8.0/PKG-INFO
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4478 2023-05-05 04:53:06.000000 rope-1.8.0/README.rst
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.421344 rope-1.8.0/bin/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1607 2023-01-17 01:59:16.000000 rope-1.8.0/bin/tag-release.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.425345 rope-1.8.0/docs/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      634 2022-07-29 12:45:37.000000 rope-1.8.0/docs/Makefile
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2247 2022-09-19 07:11:34.000000 rope-1.8.0/docs/conf.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1719 2023-01-17 01:59:16.000000 rope-1.8.0/docs/configuration.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4518 2023-05-05 04:53:06.000000 rope-1.8.0/docs/contributing.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5165 2022-12-16 04:43:54.000000 rope-1.8.0/docs/default_config.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.425345 rope-1.8.0/docs/dev/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3906 2023-01-17 01:59:16.000000 rope-1.8.0/docs/dev/issues.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      526 2023-01-17 01:59:16.000000 rope-1.8.0/docs/index.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    28522 2023-01-17 01:59:16.000000 rope-1.8.0/docs/library.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      765 2022-07-29 12:45:37.000000 rope-1.8.0/docs/make.bat
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    31016 2023-01-17 01:59:16.000000 rope-1.8.0/docs/overview.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      976 2023-05-05 05:01:06.000000 rope-1.8.0/docs/release-process.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1459 2022-09-19 07:41:21.000000 rope-1.8.0/docs/rope.rst
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2256 2023-05-05 05:05:09.000000 rope-1.8.0/pyproject.toml
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.429345 rope-1.8.0/rope/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1431 2023-01-17 01:59:16.000000 rope-1.8.0/rope/__init__.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.441345 rope-1.8.0/rope/base/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      161 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3283 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/arguments.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2521 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/ast.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    26263 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/builtins.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13675 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/change.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11774 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/codeanalyze.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13587 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/evaluate.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1370 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/exceptions.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8481 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/fscommands.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8342 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/history.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3841 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/libutils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1656 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/nameanalyze.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.445345 rope-1.8.0/rope/base/oi/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1682 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7397 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/doa.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3440 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/memorydb.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4547 2022-12-16 03:37:02.000000 rope-1.8.0/rope/base/oi/objectdb.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8624 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/objectinfo.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8532 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/runmod.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5862 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/soa.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7719 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/soi.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9829 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/oi/transform.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.449345 rope-1.8.0/rope/base/oi/type_hinting/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9057 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/evaluate.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2728 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/type_hinting/factory.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      715 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/interfaces.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.453345 rope-1.8.0/rope/base/oi/type_hinting/providers/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1856 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/composite.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6164 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/docstrings.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2116 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/inheritance.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1055 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/interfaces.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1419 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/numpydocstrings.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1525 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/oi/type_hinting/providers/pep0484_type_comments.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.453345 rope-1.8.0/rope/base/oi/type_hinting/resolvers/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/resolvers/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      778 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/resolvers/composite.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      405 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/oi/type_hinting/resolvers/interfaces.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      609 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/resolvers/types.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5394 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/oi/type_hinting/utils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    10203 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/prefs.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15177 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/project.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12804 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/pycore.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6390 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/pynames.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2098 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/pynamesdef.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9271 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/pyobjects.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22557 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/pyobjectsdef.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11468 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/pyscopes.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    10291 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/resourceobserver.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7812 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/resources.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5590 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/serializer.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1905 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/simplify.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1606 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/stdmods.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4907 2023-05-05 04:53:06.000000 rope-1.8.0/rope/base/taskhandle.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.457346 rope-1.8.0/rope/base/utils/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3949 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/utils/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1824 2022-12-15 11:40:37.000000 rope-1.8.0/rope/base/utils/datastructures.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1405 2023-01-17 01:59:16.000000 rope-1.8.0/rope/base/versioning.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    22416 2022-07-29 12:45:37.000000 rope-1.8.0/rope/base/worder.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.457346 rope-1.8.0/rope/contrib/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      169 2022-07-29 12:45:37.000000 rope-1.8.0/rope/contrib/__init__.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.461346 rope-1.8.0/rope/contrib/autoimport/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      196 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/autoimport/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2444 2022-07-29 12:45:37.000000 rope-1.8.0/rope/contrib/autoimport/defs.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3273 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/autoimport/models.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5276 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/autoimport/parse.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8394 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/autoimport/pickle.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    19728 2023-05-05 04:53:06.000000 rope-1.8.0/rope/contrib/autoimport/sqlite.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4826 2023-05-05 04:53:06.000000 rope-1.8.0/rope/contrib/autoimport/utils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1350 2022-07-29 12:45:37.000000 rope-1.8.0/rope/contrib/changestack.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    26473 2022-12-15 11:40:37.000000 rope-1.8.0/rope/contrib/codeassist.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2935 2022-12-15 11:40:37.000000 rope-1.8.0/rope/contrib/finderrors.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4483 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/findit.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2194 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/fixmodnames.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6777 2023-01-17 01:59:16.000000 rope-1.8.0/rope/contrib/fixsyntax.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14845 2023-05-05 04:53:06.000000 rope-1.8.0/rope/contrib/generate.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.473346 rope-1.8.0/rope/refactor/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2126 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13432 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/change_signature.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8459 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/encapsulate_field.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    39187 2023-05-05 04:53:06.000000 rope-1.8.0/rope/refactor/extract.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     8316 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/functionutils.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.477346 rope-1.8.0/rope/refactor/importutils/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13354 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/importutils/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    14255 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/importutils/actions.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5790 2023-05-05 04:53:06.000000 rope-1.8.0/rope/refactor/importutils/importinfo.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    21673 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/importutils/module_imports.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    25109 2023-05-05 04:53:06.000000 rope-1.8.0/rope/refactor/inline.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5913 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/introduce_factory.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3717 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/introduce_parameter.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2076 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/localtofield.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3829 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/method_object.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    34458 2023-05-05 04:53:06.000000 rope-1.8.0/rope/refactor/move.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2544 2022-12-15 11:40:37.000000 rope-1.8.0/rope/refactor/multiproject.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    13040 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/occurrences.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    31196 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/patchedast.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9348 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/rename.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    11441 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/restructure.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12719 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/similarfinder.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3001 2022-12-15 11:40:37.000000 rope-1.8.0/rope/refactor/sourceutils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5152 2022-12-15 11:40:37.000000 rope-1.8.0/rope/refactor/suites.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1226 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/topackage.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6651 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/usefunction.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5740 2023-01-17 01:59:16.000000 rope-1.8.0/rope/refactor/wildcards.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.429345 rope-1.8.0/rope.egg-info/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5673 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/PKG-INFO
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5070 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/SOURCES.txt
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        1 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/dependency_links.txt
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      230 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/requires.txt
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        5 2023-05-05 05:06:22.000000 rope-1.8.0/rope.egg-info/top_level.txt
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.489347 rope-1.8.0/ropetest/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-12-15 11:40:37.000000 rope-1.8.0/ropetest/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    37493 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/advanced_oi_test.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    23217 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/builtinstest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    35910 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/codeanalyzetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      787 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/conftest.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.493347 rope-1.8.0/ropetest/contrib/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)        0 2022-12-15 11:40:37.000000 rope-1.8.0/ropetest/contrib/__init__.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.493347 rope-1.8.0/ropetest/contrib/autoimport/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      795 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/autoimport/autoimporttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      703 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/autoimport/conftest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2128 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/autoimport/modeltest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      647 2022-07-29 12:45:37.000000 rope-1.8.0/ropetest/contrib/autoimport/parsetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2237 2023-05-05 04:53:06.000000 rope-1.8.0/ropetest/contrib/autoimport/utilstest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     7286 2022-11-22 15:02:03.000000 rope-1.8.0/ropetest/contrib/autoimporttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      955 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/changestacktest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    56041 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/codeassisttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1629 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/finderrorstest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5475 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/findittest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2066 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/fixmodnamestest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15157 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/contrib/generatetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2894 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/doatest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15912 2022-12-15 11:40:37.000000 rope-1.8.0/ropetest/historytest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6879 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/objectdbtest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    15681 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/objectinfertest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    48095 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/projecttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    52145 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/pycoretest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    19385 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/pyscopestest.py
+drwxrwxr-x   0 lieryan   (1000) lieryan   (1000)        0 2023-05-05 05:06:22.501347 rope-1.8.0/ropetest/refactor/
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    38589 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/__init__.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    27113 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/change_signature_test.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)   101254 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/extracttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    69500 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/importutilstest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    42803 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/inlinetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    41603 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/movetest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3434 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/multiprojecttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    59540 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/patchedasttest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    50303 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/renametest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     9672 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/restructuretest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    12065 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/similarfindertest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6766 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/suitestest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6400 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/refactor/usefunctiontest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     5653 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/reprtest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     6404 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/runmodtest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     4801 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/serializer_test.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     2203 2022-11-22 15:02:03.000000 rope-1.8.0/ropetest/simplifytest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     3166 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/testutils.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)    16326 2022-12-15 11:40:37.000000 rope-1.8.0/ropetest/type_hinting_test.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)     1448 2023-01-17 01:59:16.000000 rope-1.8.0/ropetest/versioningtest.py
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)      154 2023-05-05 05:06:22.501347 rope-1.8.0/setup.cfg
+-rw-rw-r--   0 lieryan   (1000) lieryan   (1000)       38 2022-12-15 11:40:37.000000 rope-1.8.0/setup.py
```

### Comparing `rope-1.7.0/.all-contributorsrc` & `rope-1.8.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/.github/ISSUE_TEMPLATE/bug-report.md` & `rope-1.8.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `rope-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/.github/workflows/main.yml` & `rope-1.8.0/.github/workflows/main.yml`

 * *Files 13% similar despite different names*

```diff
@@ -14,13 +14,15 @@
       fail-fast: false
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        cache: 'pip'
+        cache-dependency-path: 'gha-cache-key.txt'
     - name: Install dependencies
       run: |
         python -m pip install -e .[dev]
     - name: Test with pytest
       run: |
         python -m pytest -v
```

### Comparing `rope-1.7.0/.gitignore` & `rope-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/CHANGELOG.md` & `rope-1.8.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # **Upcoming release**
 
-...
+# Release 1.8.0
 
+- #650 Install pre-commit hooks on rope repository (@lieryan)
+- #655 Remove unused __init__() methods (@edreamleo, @lieryan)
+- #656 Reformat using black 23.1.0 (@edreamleo)
+- #674 Fix/supress all mypy complaints (@edreamleo)
+- #680 Remove a do-nothing statement in soi._handle_first_parameter (@edreamleo)
+- #687, #688 Fix autoimport not scanning packages recursively (@lieryan)
 
 # Release 1.7.0
 
 ## Feature
 
 - #548 Implement MoveGlobal using string as destination module names (@lieryan)
 
@@ -45,20 +51,20 @@
 - #620 Remove unused import in occurrences.py (@edreamleo)
 - #625 Remove support for deprecated ast nodes (@lieryan)
 
 
 ## Tests/Dev
 
 - #626 Install pre-commit hooks on rope repository (@lieryan)
-- #628 Add isort to pre-commit
-- #638 Add a function to identify ast Constant nodes more granularly 
+- #628 Add isort to pre-commit (@lieryan)
+- #638 Add a function to identify ast Constant nodes more granularly (@lieryan)
 
 ## Docs
 
-- #636 Update readme to reflect 1.0 has been released.
+- #636 Update readme to reflect 1.0 has been released. (@maxnoe)
 
 
 # Release 1.6.0
 
 ## New features & Enhancements
 
 - #559, #560 Improve handling of whitespace in import and from-import statements (@lieryan)
```

### Comparing `rope-1.7.0/CONTRIBUTORS.md` & `rope-1.8.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/COPYING` & `rope-1.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/PKG-INFO` & `rope-1.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rope
-Version: 1.7.0
+Version: 1.8.0
 Summary: a python refactoring library...
 Author-email: Ali Gholami Rudi <aligrudi@users.sourceforge.net>
 Maintainer-email: Lie Ryan <lieryan.24@proton.me>
 License: LGPL-3.0-or-later
 Project-URL: Source, https://github.com/python-rope/rope
 Project-URL: Documentation, https://rope.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: dev
+License-File: COPYING
 
 
 .. _GitHub python-rope / rope: https://github.com/python-rope/rope
 
 
 =========================================================================
  rope -- the world's most advanced open source Python refactoring library
@@ -85,14 +86,15 @@
 - Rope aims to provide powerful and safe refactoring
 - Rope is light on dependency, Rope only depends on Python itself
 - Unlike PyRight or PyLance, Rope does not depend on Node.js
 - Unlike PyLance or PyCharm, Rope is open source.
 - Unlike PyRight and PyLance, Rope is written in Python itself, so if you experience problems, you would be able to debug and hack it yourself in a language that you are already familiar with
 - In comparison to Jedi, Rope is focused on refactoring. While Jedi provides some basic refactoring capabilities, Rope supports many more advanced refactoring operations and options that Jedi does not.
 
+
 Bug Reports
 ===========
 
 Send your bug reports and feature requests at `python-rope's issue tracker`_ in GitHub.
 
 .. _`python-rope's issue tracker`: https://github.com/python-rope/rope/issues
 
@@ -107,21 +109,34 @@
 
 Many thanks the following people:
 
 - Ali Gholami Rudi (`@aligrudi`_) for initially creating the initial Rope project and most of Rope's code
 - Matej Cepl (`@mcepl`_) as former long-time Rope maintainer
 - Nick Smith <nicks@fastmail.fm> (`@soupytwist`_) as former Rope maintainer
 - `all of our current and former contributors`_
-- authors of editor integrations
+- `all authors of editor integrations`_
+- all maintainers of distro/package managers
 
 .. _`@aligrudi`: https://github.com/aligrudi
 .. _`@soupytwist`: https://github.com/soupytwist
 .. _`@lieryan`: https://github.com/lieryan
 .. _`@mcepl`: https://github.com/mcepl
 .. _`all of our current and former contributors`: https://github.com/python-rope/rope/blob/master/CONTRIBUTORS.md
+.. _`all authors of editor integrations`: https://github.com/python-rope/rope/wiki/How-to-use-Rope-in-my-IDE-or-Text-editor%3F
+
+Packaging Status
+================
+
+.. image:: https://repology.org/badge/vertical-allrepos/python:rope.svg?exclude_unsupported=1
+   :target: https://repology.org/project/python:rope/versions
+   :alt: Packaging status
+
+.. image:: https://repology.org/badge/vertical-allrepos/rope.svg?exclude_unsupported=1
+   :target: https://repology.org/project/rope/versions
+   :alt: Packaging status
 
 License
 =======
 
 This program is under the terms of LGPL v3+ (GNU Lesser General Public License).
 Have a look at `COPYING`_ for more information.
```

### Comparing `rope-1.7.0/README.rst` & `rope-1.8.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 - Rope aims to provide powerful and safe refactoring
 - Rope is light on dependency, Rope only depends on Python itself
 - Unlike PyRight or PyLance, Rope does not depend on Node.js
 - Unlike PyLance or PyCharm, Rope is open source.
 - Unlike PyRight and PyLance, Rope is written in Python itself, so if you experience problems, you would be able to debug and hack it yourself in a language that you are already familiar with
 - In comparison to Jedi, Rope is focused on refactoring. While Jedi provides some basic refactoring capabilities, Rope supports many more advanced refactoring operations and options that Jedi does not.
 
+
 Bug Reports
 ===========
 
 Send your bug reports and feature requests at `python-rope's issue tracker`_ in GitHub.
 
 .. _`python-rope's issue tracker`: https://github.com/python-rope/rope/issues
 
@@ -78,21 +79,34 @@
 
 Many thanks the following people:
 
 - Ali Gholami Rudi (`@aligrudi`_) for initially creating the initial Rope project and most of Rope's code
 - Matej Cepl (`@mcepl`_) as former long-time Rope maintainer
 - Nick Smith <nicks@fastmail.fm> (`@soupytwist`_) as former Rope maintainer
 - `all of our current and former contributors`_
-- authors of editor integrations
+- `all authors of editor integrations`_
+- all maintainers of distro/package managers
 
 .. _`@aligrudi`: https://github.com/aligrudi
 .. _`@soupytwist`: https://github.com/soupytwist
 .. _`@lieryan`: https://github.com/lieryan
 .. _`@mcepl`: https://github.com/mcepl
 .. _`all of our current and former contributors`: https://github.com/python-rope/rope/blob/master/CONTRIBUTORS.md
+.. _`all authors of editor integrations`: https://github.com/python-rope/rope/wiki/How-to-use-Rope-in-my-IDE-or-Text-editor%3F
+
+Packaging Status
+================
+
+.. image:: https://repology.org/badge/vertical-allrepos/python:rope.svg?exclude_unsupported=1
+   :target: https://repology.org/project/python:rope/versions
+   :alt: Packaging status
+
+.. image:: https://repology.org/badge/vertical-allrepos/rope.svg?exclude_unsupported=1
+   :target: https://repology.org/project/rope/versions
+   :alt: Packaging status
 
 License
 =======
 
 This program is under the terms of LGPL v3+ (GNU Lesser General Public License).
 Have a look at `COPYING`_ for more information.
```

### Comparing `rope-1.7.0/bin/tag-release.py` & `rope-1.8.0/bin/tag-release.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/Makefile` & `rope-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/conf.py` & `rope-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/configuration.rst` & `rope-1.8.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/contributing.rst` & `rope-1.8.0/docs/contributing.rst`

 * *Files 14% similar despite different names*

```diff
@@ -136,7 +136,26 @@
 
     pip install -e .[dev]
 
 .. _GitHub: http://github.com/
 .. _`python-rope/rope`: https://github.com/python-rope/rope
 .. _`pull request`: https://help.github.com/articles/using-pull-requests
 .. _`pytest`: https://pytest.org/
+
+
+.. _gha-cache-key:
+
+Updating gha-cache-key.txt
+--------------------------
+
+``gha-cache-key.txt`` file is used as cache-key for Github Action to cache pip
+packages. Refer to `PR #650`_ to see how it works.
+
+.. _`PR #650`: https://github.com/python-rope/rope/pull/650
+
+To re-generate the cache key, run this command:
+
+.. code-block:: sh
+
+    $ pip-compile --extra dev --generate-hashes -o gha-cache-key.txt
+    $ git add gha-cache-key.txt
+    $ git commit
```

### Comparing `rope-1.7.0/docs/default_config.py` & `rope-1.8.0/docs/default_config.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/dev/issues.rst` & `rope-1.8.0/docs/dev/issues.rst`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/index.rst` & `rope-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/library.rst` & `rope-1.8.0/docs/library.rst`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/make.bat` & `rope-1.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/overview.rst` & `rope-1.8.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/docs/rope.rst` & `rope-1.8.0/docs/rope.rst`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/pyproject.toml` & `rope-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Topic :: Software Development',
 ]
-version = '1.7.0'
+version = '1.8.0'
 dependencies = ['pytoolconfig[global] >= 1.2.2']
 
 [[project.authors]]
 name = 'Ali Gholami Rudi'
 email = 'aligrudi@users.sourceforge.net'
 
 [[project.maintainers]]
@@ -46,14 +46,16 @@
     "sphinx-rtd-theme>=1.0.0",
 ]
 dev = [
     'pytest>=7.0.1',
     'pytest-timeout>=2.1.0',
     'build>=0.7.0',
     'pre-commit>=2.20.0',
+    'pip-tools>=6.12.1',
+    'toml>=0.10.2',
 ]
 [tool.setuptools]
 packages = [
     'rope',
     'rope.base',
     'rope.base.oi',
     'rope.base.oi.type_hinting',
```

### Comparing `rope-1.7.0/rope/__init__.py` & `rope-1.8.0/rope/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/arguments.py` & `rope-1.8.0/rope/base/arguments.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/builtins.py` & `rope-1.8.0/rope/base/builtins.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/change.py` & `rope-1.8.0/rope/base/change.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/codeanalyze.py` & `rope-1.8.0/rope/base/codeanalyze.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/evaluate.py` & `rope-1.8.0/rope/base/evaluate.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/exceptions.py` & `rope-1.8.0/rope/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/fscommands.py` & `rope-1.8.0/rope/base/fscommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         with open(path, "rb") as handle:
             return handle.read()
 
 
 class SubversionCommands:
     def __init__(self, *args):
         self.normal_actions = FileSystemCommands()
-        import pysvn
+        import pysvn  # type:ignore
 
         self.client = pysvn.Client()
 
     def create_file(self, path):
         self.normal_actions.create_file(path)
         self.client.add(path, force=True)
 
@@ -110,17 +110,17 @@
             self.ui.setconfig("ui", "verbose", "no")
             self.ui.setconfig("ui", "report_untrusted", "no")
             self.ui.setconfig("ui", "quiet", "yes")
 
         self.repo = self.hg.hg.repository(self.ui, root)
 
     def _import_mercurial(self):
-        import mercurial.commands
-        import mercurial.hg
-        import mercurial.ui
+        import mercurial.commands  # type:ignore
+        import mercurial.hg  # type:ignore
+        import mercurial.ui  # type:ignore
 
         return mercurial
 
     def create_file(self, path):
         self.normal_actions.create_file(path)
         self.hg.commands.add(self.ui, self.repo, path)
```

### Comparing `rope-1.7.0/rope/base/history.py` & `rope-1.8.0/rope/base/history.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/libutils.py` & `rope-1.8.0/rope/base/libutils.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/nameanalyze.py` & `rope-1.8.0/rope/base/nameanalyze.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/__init__.py` & `rope-1.8.0/rope/base/oi/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/doa.py` & `rope-1.8.0/rope/base/oi/doa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import base64
 import contextlib
 import hashlib
 import hmac
 
 try:
-    import cPickle as pickle
+    import cPickle as pickle  # type:ignore
 except ImportError:
-    import pickle
+    import pickle  # type:ignore
 import marshal
 import os
 import socket
 import subprocess
 import sys
 import tempfile
 import threading
@@ -24,15 +24,15 @@
     for cryptography.
     """
     if len(a) != len(b):
         return False
     # Computes the bitwise difference of all characters in the two strings
     # before returning whether or not they are equal.
     difference = 0
-    for (a_char, b_char) in zip(a, b):
+    for a_char, b_char in zip(a, b):
         difference |= ord(a_char) ^ ord(b_char)
     return difference == 0
 
 
 try:
     from hmac import compare_digest
 except ImportError:
```

### Comparing `rope-1.7.0/rope/base/oi/memorydb.py` & `rope-1.8.0/rope/base/oi/memorydb.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/objectdb.py` & `rope-1.8.0/rope/base/oi/objectdb.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/objectinfo.py` & `rope-1.8.0/rope/base/oi/objectinfo.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/runmod.py` & `rope-1.8.0/rope/base/oi/runmod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 def __rope_start_everything():
     import os
     import socket
     import sys
 
     try:
-        import cPickle as pickle
+        import cPickle as pickle  # type:ignore
     except ImportError:
         import pickle
     import base64
     import hashlib
     import hmac
     import inspect
     import marshal
@@ -97,15 +97,15 @@
             try:
                 data = (
                     self._object_to_persisted_form(frame.f_code),
                     tuple(args),
                     returned,
                 )
                 self.sender.send_data(data)
-            except (TypeError):
+            except TypeError:
                 pass
             return self.on_function_call
 
         def _is_an_interesting_call(self, frame):
             # if frame.f_code.co_name in ['?', '<module>']:
             #    return False
             # return not frame.f_back or
```

### Comparing `rope-1.7.0/rope/base/oi/soa.py` & `rope-1.8.0/rope/base/oi/soa.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/soi.py` & `rope-1.8.0/rope/base/oi/soi.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,14 @@
         result = _parameter_objects(pyfunction)
     _handle_first_parameter(pyfunction, result)
     return result
 
 
 def _handle_first_parameter(pyobject, parameters):
     kind = pyobject.get_kind()
-    if parameters is None or kind not in ["method", "classmethod"]:
-        pass
     if not parameters:
         if not pyobject.get_param_names(special_args=False):
             return
         parameters.append(pyobjects.get_unknown())
     if kind == "method":
         parameters[0] = pyobjects.PyObject(pyobject.parent)
     if kind == "classmethod":
```

### Comparing `rope-1.7.0/rope/base/oi/transform.py` & `rope-1.8.0/rope/base/oi/transform.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/evaluate.py` & `rope-1.8.0/rope/base/oi/type_hinting/evaluate.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 
 from rope.base import utils as base_utils
 from rope.base.oi.type_hinting import utils
 
 
 class SymbolBase:
-
     name = None  # node/token type name
 
     def __init__(self):
         self.value = None  # used by name and literals
         self.first = None
         self.second = None
         self.third = None  # used by tree nodes
@@ -66,25 +65,25 @@
             s.name = name
             s.lbp = bp
             self.symbol_table[name] = s
         else:
             s.lbp = max(bp, s.lbp)
         return s
 
-    @multi
+    @multi  # type:ignore
     def infix(self, name, bp):
         symbol = self.symbol(name, bp)
 
         @method(symbol)
         def led(self, left, parser):
             self.first = left
             self.second = parser.expression(bp)
             return self
 
-    @multi
+    @multi  # type:ignore
     def infix_r(self, name, bp):
         symbol = self.symbol(name, bp)
 
         @method(symbol)
         def led(self, left, parser):
             self.first = left
             self.second = parser.expression(bp - 0.1)
@@ -98,24 +97,24 @@
         def led(self, left, parser):
             self.first = left
             self.second = parser.expression(symbol2.lbp)
             parser.advance(symbol2.name)
             self.third = parser.expression(symbol2.lbp + 0.1)
             return self
 
-    @multi
-    def prefix(self, name, bp):
+    @multi  # type:ignore
+    def prefix(self, name, bp):  # type:ignore
         symbol = self.symbol(name, bp)
 
         @method(symbol)
         def nud(self, parser):
             self.first = parser.expression(bp)
             return self
 
-    @multi
+    @multi  # type:ignore
     def postfix(self, name, bp):
         symbol = self.symbol(name, bp)
 
         @method(symbol)
         def led(self, left, parser):
             self.first = left
             return self
@@ -123,15 +122,14 @@
     multi = staticmethod(multi)  # Just for code checker
 
 
 symbol_table = SymbolTable()
 
 
 class Lexer:
-
     _token_pattern = re.compile(
         r"""
         \s*
         (?:
               (
                     [,()\[\]|]
                   | ->
@@ -175,15 +173,14 @@
                 yield "(name)", name
             else:
                 raise SyntaxError
         yield "(end)", "(end)"
 
 
 class Parser:
-
     token = None
     next = None
 
     def __init__(self, lexer):
         self.lexer = lexer
 
     def parse(self, program):
@@ -236,26 +233,26 @@
 infix("or", 170)
 symbol(",")
 
 symbol("(name)")
 symbol("(end)")
 
 
-@method(symbol("(name)"))
+@method(symbol("(name)"))  # type:ignore
 def nud(self, parser):
     return self
 
 
-@method(symbol("(name)"))
+@method(symbol("(name)"))  # type:ignore
 def evaluate(self, pyobject):
     return utils.resolve_type(self.value, pyobject)
 
 
 # Parametrized objects
-@method(symbol("["))
+@method(symbol("["))  # type:ignore
 def led(self, left, parser):
     self.first = left
     self.second = []
     if parser.token.name != "]":
         while 1:
             if parser.token.name == "]":
                 break
@@ -263,23 +260,23 @@
             if parser.token.name != ",":
                 break
             parser.advance(",")
     parser.advance("]")
     return self
 
 
-@method(symbol("["))
+@method(symbol("["))  # type:ignore
 def evaluate(self, pyobject):
     return utils.parametrize_type(
         self.first.evaluate(pyobject), *[i.evaluate(pyobject) for i in self.second]
     )
 
 
 # Anonymous Function Calls
-@method(symbol("("))
+@method(symbol("("))  # type:ignore
 def nud(self, parser):
     self.second = []
     if parser.token.name != ")":
         while 1:
             self.second.append(parser.expression())
             if parser.token.name != ",":
                 break
@@ -287,15 +284,15 @@
     parser.advance(")")
     parser.advance("->")
     self.third = parser.expression(symbol("->").lbp + 0.1)
     return self
 
 
 # Function Calls
-@method(symbol("("))
+@method(symbol("("))  # type:ignore
 def led(self, left, parser):
     self.first = left
     self.second = []
     if parser.token.name != ")":
         while 1:
             self.second.append(parser.expression())
             if parser.token.name != ",":
@@ -303,29 +300,28 @@
             parser.advance(",")
     parser.advance(")")
     parser.advance("->")
     self.third = parser.expression(symbol("->").lbp + 0.1)
     return self
 
 
-@method(symbol("("))
+@method(symbol("("))  # type:ignore
 def evaluate(self, pyobject):
     # TODO: Implement me
     raise NotImplementedError
 
 
-@method(symbol("or"))
+@method(symbol("or"))  # type:ignore
 @method(symbol("|"))
 def evaluate(self, pyobject):
     # TODO: Implement me
     raise NotImplementedError
 
 
 class Compiler:
-
     parser_factory = Parser
     lexer_factory = Lexer
     symbol_table = symbol_table
 
     def _make_parser(self):
         return self.parser_factory(self.lexer_factory(self.symbol_table))
 
@@ -338,15 +334,14 @@
         return self._make_parser().parse(program)
 
 
 compile = Compiler()
 
 
 class Evaluator:
-
     compile = compile
 
     def __call__(self, program, pyobject):
         """Evaluates the program string or AST
 
         :type program: str or rope.base.oi.type_hinting.evaluate.SymbolBase
         :rtype: rope.base.pyobjects.PyDefinedObject | rope.base.pyobjects.PyObject or None
```

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/factory.py` & `rope-1.8.0/rope/base/oi/type_hinting/factory.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/interfaces.py` & `rope-1.8.0/rope/base/oi/type_hinting/interfaces.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/providers/composite.py` & `rope-1.8.0/rope/base/oi/type_hinting/providers/composite.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/providers/docstrings.py` & `rope-1.8.0/rope/base/oi/type_hinting/providers/docstrings.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     def __call__(self, docstring):
         """
         :type docstring: str
         """
 
 
 class DocstringParamParser(IParamParser):
-
     DOCSTRING_PARAM_PATTERNS = [
         r"\s*:type\s+%s:\s*([^\n]+)",  # Sphinx
         r"\s*:param\s+(\w+)\s+%s:[^\n]+",  # Sphinx param with type
         r"\s*@type\s+%s:\s*([^\n]+)",  # Epydoc
     ]
 
     def __init__(self):
@@ -140,15 +139,14 @@
             if match:
                 return [self._strip_rst_role(match.group(1))]
 
         return []
 
 
 class DocstringReturnParser(IReturnParser):
-
     DOCSTRING_RETURN_PATTERNS = [
         re.compile(r"\s*:rtype:\s*([^\n]+)", re.M),  # Sphinx
         re.compile(r"\s*@rtype:\s*([^\n]+)", re.M),  # Epydoc
     ]
 
     def __init__(self):
         self._strip_rst_role = RSTRoleStrip()
@@ -160,15 +158,14 @@
             match = p.search(docstring)
             if match:
                 return [self._strip_rst_role(match.group(1))]
         return []
 
 
 class RSTRoleStrip:
-
     RST_ROLE_PATTERN = re.compile(r":[^`]+:`([^`]+)`")
 
     def __call__(self, type_str):
         """
         Strip off the part looks like a ReST role in `type_str`.
 
         >>> RSTRoleStrip()(':class:`ClassName`')  # strip off :class:
```

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/providers/inheritance.py` & `rope-1.8.0/rope/base/oi/type_hinting/providers/inheritance.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/providers/interfaces.py` & `rope-1.8.0/rope/base/oi/type_hinting/providers/interfaces.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/providers/numpydocstrings.py` & `rope-1.8.0/rope/base/oi/type_hinting/providers/numpydocstrings.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 import re
 
 from rope.base.ast import literal_eval
 from rope.base.oi.type_hinting.providers import docstrings
 
 try:
-    from numpydoc.docscrape import NumpyDocString
+    from numpydoc.docscrape import NumpyDocString  # type:ignore
 except ImportError:
     NumpyDocString = None
 
 
 class NumPyDocstringParamParser(docstrings.IParamParser):
     def __call__(self, docstring, param_name):
         """Search `docstring` (in numpydoc format) for type(-s) of `param_name`."""
@@ -36,8 +36,8 @@
 
 class _DummyParamParser(docstrings.IParamParser):
     def __call__(self, docstring, param_name):
         return []
 
 
 if not NumpyDocString:
-    NumPyDocstringParamParser = _DummyParamParser
+    NumPyDocstringParamParser = _DummyParamParser  # type:ignore
```

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/providers/pep0484_type_comments.py` & `rope-1.8.0/rope/base/oi/type_hinting/providers/pep0484_type_comments.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/resolvers/composite.py` & `rope-1.8.0/rope/base/oi/type_hinting/resolvers/composite.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/resolvers/types.py` & `rope-1.8.0/rope/base/oi/type_hinting/resolvers/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
         :param hint: For example "List[int]" or "(Foo, Bar) -> Baz" or simple "Foo"
         :type hint: str
         :type pyobject: rope.base.pyobjects.PyDefinedObject | rope.base.pyobjects.PyObject
         :rtype: rope.base.pyobjects.PyDefinedObject | rope.base.pyobjects.PyObject or None
         """
         try:
             return evaluate.evaluate(hint, pyobject)
-        except (Exception):
+        except Exception:
             pass
```

### Comparing `rope-1.7.0/rope/base/oi/type_hinting/utils.py` & `rope-1.8.0/rope/base/oi/type_hinting/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from __future__ import annotations
+
 import logging
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import rope.base.utils as base_utils
 from rope.base import evaluate
 from rope.base.exceptions import AttributeNotFoundError
 from rope.base.pyobjects import PyClass, PyDefinedObject, PyFunction, PyObject
 
 
 def get_super_func(pyfunc):
-
     if not isinstance(pyfunc.parent, PyClass):
         return
 
     for cls in get_mro(pyfunc.parent)[1:]:
         try:
             superfunc = cls.get_attribute(pyfunc.get_name()).get_object()
         except AttributeNotFoundError:
@@ -69,24 +70,29 @@
     for cls in class_list:
         for super_cls in cls.get_superclasses():
             if isinstance(super_cls, PyClass) and super_cls not in class_list:
                 class_list.append(super_cls)
     return class_list
 
 
-def resolve_type(type_name, pyobject):
-    # type: (str, Union[PyDefinedObject, PyObject]) -> Optional[PyDefinedObject, PyObject]
+def resolve_type(
+    type_name: str,
+    pyobject: Union[PyDefinedObject, PyObject],
+) -> Optional[Union[PyDefinedObject, PyObject]]:
     """
     Find proper type object from its name.
     """
     deprecated_aliases = {"collections": "collections.abc"}
     ret_type = None
     logging.debug("Looking for %s", type_name)
     if "." not in type_name:
         try:
+            # XXX: this looks incorrect? It doesn't seem like it would work
+            # correctly if you have a type/class not defined in the
+            # module/global scope
             ret_type = (
                 pyobject.get_module().get_scope().get_name(type_name).get_object()
             )
         except AttributeNotFoundError:
             logging.exception("Cannot resolve type %s", type_name)
     else:
         mod_name, attr_name = type_name.rsplit(".", 1)
@@ -109,15 +115,14 @@
                         "Cannot resolve type %s in %s", attr_name, dir(mod)
                     )
     logging.debug("ret_type = %s", ret_type)
     return ret_type
 
 
 class ParametrizeType:
-
     _supported_mapping = {
         "builtins.list": "rope.base.builtins.get_list",
         "builtins.tuple": "rope.base.builtins.get_tuple",
         "builtins.set": "rope.base.builtins.get_set",
         "builtins.dict": "rope.base.builtins.get_dict",
         "_collections_abc.Iterable": "rope.base.builtins.get_iterator",
         "_collections_abc.Iterator": "rope.base.builtins.get_iterator",
```

### Comparing `rope-1.7.0/rope/base/prefs.py` & `rope-1.8.0/rope/base/prefs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# mypy reports many problems.
+# type: ignore
 """Rope preferences."""
 from dataclasses import asdict, dataclass
 from textwrap import dedent
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from packaging.requirements import Requirement
 from pytoolconfig import PyToolConfig, UniversalKey, field
```

### Comparing `rope-1.7.0/rope/base/project.py` & `rope-1.8.0/rope/base/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+from __future__ import annotations
 import contextlib
 import json
 import os
 import sys
 import warnings
 from contextlib import ExitStack
 from typing import Optional
 
 import rope.base.fscommands  # Use full qualification for clarity.
 import rope.base.resourceobserver as resourceobserver
 from rope.base import exceptions, history, pycore, taskhandle, utils
 from rope.base.exceptions import ModuleNotFoundError
-from rope.base.prefs import Prefs, get_config
+
+# At present rope.base.prefs starts with `# type:ignore`.
+# As a result, mypy knows nothing about Prefs and get_config.
+from rope.base.prefs import Prefs, get_config  # type:ignore
 from rope.base.resources import File, Folder, _ResourceMatcher
 
 try:
-    import cPickle as pickle
+    import cPickle as pickle  # type:ignore
 except ImportError:
-    import pickle
+    import pickle  # type:ignore
 
 
 class _Project:
     prefs: Prefs
 
     def __init__(self, fscommands):
         self.observers = []
```

### Comparing `rope-1.7.0/rope/base/pycore.py` & `rope-1.8.0/rope/base/pycore.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,14 @@
         pymodule = self.resource_to_pyobject(resource)
         self.module_cache.forget_all_data()
         rope.base.oi.soa.analyze_module(
             self, pymodule, should_analyze, search_subscopes, followed_calls
         )
 
     def get_classes(self, task_handle=taskhandle.DEFAULT_TASK_HANDLE):
-
         warnings.warn(
             "`PyCore.get_classes()` is deprecated", DeprecationWarning, stacklevel=2
         )
         return []
 
     def __str__(self):
         return str(self.module_cache) + str(self.object_info)
```

### Comparing `rope-1.7.0/rope/base/pynames.py` & `rope-1.8.0/rope/base/pynames.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/pynamesdef.py` & `rope-1.8.0/rope/base/pynamesdef.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/pyobjects.py` & `rope-1.8.0/rope/base/pyobjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
         return self.type.get_attributes()
 
     def get_attribute(self, name):
         if name not in self.get_attributes():
             raise exceptions.AttributeNotFoundError("Attribute %s not found" % name)
         return self.get_attributes()[name]
 
+    def get_module(self):
+        return None
+
     def get_type(self):
         return self.type
 
     def __getitem__(self, key):
         """The same as ``get_attribute(key)``"""
         return self.get_attribute(key)
 
@@ -221,14 +224,17 @@
 
     def get_module(self):
         current_object = self
         while current_object.parent is not None:
             current_object = current_object.parent
         return current_object
 
+    def get_name(self):
+        return None
+
     def get_doc(self) -> Optional[str]:
         if len(self.get_ast().body) > 0:
             expr = self.get_ast().body[0]
             if isinstance(expr, ast.Expr) and isinstance(expr.value, ast.Str):
                 docstring = expr.value.s
                 assert isinstance(docstring, str)
                 return docstring
```

### Comparing `rope-1.7.0/rope/base/pyobjectsdef.py` & `rope-1.8.0/rope/base/pyobjectsdef.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,22 +579,18 @@
             self.names[node.id] = self._get_pyobject(node)
 
     def _get_pyobject(self, node):
         return pynamesdef.AssignedName(lineno=node.lineno, module=self.get_module())
 
 
 class _GlobalVisitor(_ScopeVisitor):
-    def __init__(self, pycore, owner_object):
-        super().__init__(pycore, owner_object)
+    pass
 
 
 class _ClassVisitor(_ScopeVisitor):
-    def __init__(self, pycore, owner_object):
-        super().__init__(pycore, owner_object)
-
     def _FunctionDef(self, node):
         _ScopeVisitor._FunctionDef(self, node)
         if len(node.args.args) > 0:
             first = node.args.args[0]
             new_visitor = None
             if isinstance(first, ast.arg):
                 new_visitor = _ClassInitVisitor(self, first.arg)
```

### Comparing `rope-1.7.0/rope/base/pyscopes.py` & `rope-1.8.0/rope/base/pyscopes.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/resourceobserver.py` & `rope-1.8.0/rope/base/resourceobserver.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/resources.py` & `rope-1.8.0/rope/base/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,17 +155,14 @@
     def create(self):
         self.parent.create_file(self.name)
 
 
 class Folder(Resource):
     """Represents a folder"""
 
-    def __init__(self, project, name):
-        super().__init__(project, name)
-
     def is_folder(self):
         return True
 
     def get_children(self):
         """Return the children of this folder"""
         try:
             children = os.listdir(self.real_path)
```

### Comparing `rope-1.7.0/rope/base/serializer.py` & `rope-1.8.0/rope/base/serializer.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/simplify.py` & `rope-1.8.0/rope/base/simplify.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/stdmods.py` & `rope-1.8.0/rope/base/stdmods.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import sys
 
 from rope.base import utils
 
 
 def _stdlib_path():
-
     return os.path.dirname(inspect.getsourcefile(inspect))
 
 
 @utils.cached(1)
 def standard_modules():
     return python_modules() | dynload_modules()
```

### Comparing `rope-1.7.0/rope/base/taskhandle.py` & `rope-1.8.0/rope/base/taskhandle.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,17 +160,14 @@
         return self.name
 
     def increment(self):
         self.count += 1
 
 
 class NullTaskHandle(BaseTaskHandle):
-    def __init__(self):
-        pass
-
     def is_stopped(self):
         return False
 
     def stop(self):
         pass
 
     def create_jobset(self, *args, **kwds):
@@ -184,17 +181,14 @@
 
     def current_jobset(self) -> None:
         """Return the current `JobSet`"""
         return None
 
 
 class NullJobSet(BaseJobSet):
-    def __init__(self, *args):
-        pass
-
     def started_job(self, name):
         pass
 
     def finished_job(self):
         pass
 
     def check_status(self):
```

### Comparing `rope-1.7.0/rope/base/utils/__init__.py` & `rope-1.8.0/rope/base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/utils/datastructures.py` & `rope-1.8.0/rope/base/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/versioning.py` & `rope-1.8.0/rope/base/versioning.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/base/worder.py` & `rope-1.8.0/rope/base/worder.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/autoimport/defs.py` & `rope-1.8.0/rope/contrib/autoimport/defs.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/autoimport/models.py` & `rope-1.8.0/rope/contrib/autoimport/models.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/autoimport/parse.py` & `rope-1.8.0/rope/contrib/autoimport/parse.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/autoimport/pickle.py` & `rope-1.8.0/rope/contrib/autoimport/pickle.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/autoimport/sqlite.py` & `rope-1.8.0/rope/contrib/autoimport/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
 
     def _get_python_folders(self) -> List[Path]:
         def filter_folders(folder: Path) -> bool:
             return folder.is_dir() and folder.as_posix() != "/usr/bin"
 
         folders = self.project.get_python_path_folders()
         folder_paths = map(lambda folder: Path(folder.real_path), folders)
-        folder_paths = filter(filter_folders, folder_paths)
+        folder_paths = filter(filter_folders, folder_paths)  # type:ignore
         return list(OrderedDict.fromkeys(folder_paths))
 
     def _get_available_packages(self) -> List[Package]:
         packages: List[Package] = [
             Package(module, Source.BUILTIN, None, PackageType.BUILTIN)
             for module in sys.builtin_module_names
         ]
```

### Comparing `rope-1.7.0/rope/contrib/autoimport/utils.py` & `rope-1.8.0/rope/contrib/autoimport/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             yield ModuleCompiled(None, package.name, underlined, True)
     elif package.type == PackageType.SINGLE_FILE:
         assert package.path
         assert package.path.suffix == ".py"
         yield ModuleFile(package.path, package.path.stem, underlined, False)
     else:
         assert package.path
-        for file in package.path.glob("*.py"):
+        for file in package.path.glob("**/*.py"):
             if file.name == "__init__.py":
                 yield ModuleFile(
                     file,
                     get_modname_from_path(file.parent, package.path),
                     underlined,
                     True,
                 )
```

### Comparing `rope-1.7.0/rope/contrib/changestack.py` & `rope-1.8.0/rope/contrib/changestack.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/codeassist.py` & `rope-1.8.0/rope/contrib/codeassist.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/finderrors.py` & `rope-1.8.0/rope/contrib/finderrors.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/findit.py` & `rope-1.8.0/rope/contrib/findit.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/fixmodnames.py` & `rope-1.8.0/rope/contrib/fixmodnames.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/fixsyntax.py` & `rope-1.8.0/rope/contrib/fixsyntax.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/contrib/generate.py` & `rope-1.8.0/rope/contrib/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 def create_generate(
     kind: GenerateKind,
     project: Project,
     resource: Resource,
     offset: int,
     goal_resource: Optional[Resource] = None,
 ):
-
     """A factory for creating `Generate` objects
 
     Used in https://github.com/python-rope/ropemode but not in Rope itself.
     """
     d = {
         "class": GenerateClass,
         "function": GenerateFunction,
```

### Comparing `rope-1.7.0/rope/refactor/__init__.py` & `rope-1.8.0/rope/refactor/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/change_signature.py` & `rope-1.8.0/rope/refactor/change_signature.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/encapsulate_field.py` & `rope-1.8.0/rope/refactor/encapsulate_field.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/extract.py` & `rope-1.8.0/rope/refactor/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Dict
 from contextlib import contextmanager
 from itertools import chain
 
 from rope.base import ast, codeanalyze
 from rope.base.change import ChangeContents, ChangeSet
 from rope.base.exceptions import RefactoringError
 from rope.base.utils.datastructures import OrderedSet
@@ -30,16 +31,15 @@
 #
 # _ExtractPerformer: Uses above classes to collect refactoring
 # changes.
 #
 # There are a few more helper functions and classes used by above
 # classes.
 class _ExtractRefactoring:
-
-    kind_prefixes = {}
+    kind_prefixes: Dict[str, str] = {}
 
     def __init__(self, project, resource, start_offset, end_offset, variable=False):
         self.project = project
         self.resource = resource
         self.start_offset = self._fix_start(resource.read(), start_offset)
         self.end_offset = self._fix_end(resource.read(), end_offset)
```

### Comparing `rope-1.7.0/rope/refactor/functionutils.py` & `rope-1.8.0/rope/refactor/functionutils.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/importutils/__init__.py` & `rope-1.8.0/rope/refactor/importutils/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/importutils/actions.py` & `rope-1.8.0/rope/refactor/importutils/actions.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/importutils/importinfo.py` & `rope-1.8.0/rope/refactor/importutils/importinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import List, Tuple
+
+
 class ImportStatement:
     """Represent an import in a module
 
     `readonly` attribute controls whether this import can be changed
     by import actions or not.
 
     """
@@ -183,16 +186,15 @@
         return len(self.names_and_aliases) == 0
 
     def is_star_import(self):
         return len(self.names_and_aliases) > 0 and self.names_and_aliases[0][0] == "*"
 
 
 class EmptyImport(ImportInfo):
-
-    names_and_aliases = []
+    names_and_aliases: List[Tuple[str, str]] = []
 
     def is_empty(self):
         return True
 
     def get_imported_primaries(self, context):
         return []
```

### Comparing `rope-1.7.0/rope/refactor/importutils/module_imports.py` & `rope-1.8.0/rope/refactor/importutils/module_imports.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/inline.py` & `rope-1.8.0/rope/refactor/inline.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,30 +435,28 @@
         for name, value in paramdict.items():
             if name != value and value is not None:
                 header += name + " = " + value.replace("\n", " ") + "\n"
                 to_be_inlined.append(name)
         return header, to_be_inlined
 
     def _calculate_definition(self, primary, pyname, call, host_vars, returns):
-
         header, to_be_inlined = self._calculate_header(primary, pyname, call)
 
         source = header + self.body
         mod = libutils.get_string_module(self.project, source)
         name_dict = mod.get_scope().get_names()
         all_names = [
             x
             for x in name_dict
             if not isinstance(name_dict[x], rope.base.builtins.BuiltinName)
         ]
 
         # If there is a name conflict, all variable names
         # inside the inlined function are renamed
         if set(all_names).intersection(set(host_vars)):
-
             prefix = next(_DefinitionGenerator.unique_prefix)
             guest = libutils.get_string_module(self.project, source, self.resource)
 
             to_be_inlined = [prefix + item for item in to_be_inlined]
             for item in all_names:
                 pyname = guest[item]
                 occurrence_finder = occurrences.create_finder(
```

### Comparing `rope-1.7.0/rope/refactor/introduce_factory.py` & `rope-1.8.0/rope/refactor/introduce_factory.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/introduce_parameter.py` & `rope-1.8.0/rope/refactor/introduce_parameter.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/localtofield.py` & `rope-1.8.0/rope/refactor/localtofield.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/method_object.py` & `rope-1.8.0/rope/refactor/method_object.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/move.py` & `rope-1.8.0/rope/refactor/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 `create_move()` is a factory for creating move refactoring objects
 based on inputs.
 
 """
 from __future__ import annotations
 
 import typing
-from typing import Union
+from typing import Optional, List, Union
 
 from rope.base import (
     codeanalyze,
     evaluate,
     exceptions,
     libutils,
     pynames,
@@ -306,37 +306,43 @@
         return pyobject.get_scope().parent == pyobject.get_module().get_scope()
 
     def _is_variable(self, pyname):
         return isinstance(pyname, pynames.AssignedName)
 
     def get_changes(
         self,
-        dest: Union[None, str, resources.Resource],
-        resources=None,
+        dest: Optional[Union[str, resources.Resource]],
+        resources: Optional[List[resources.File]] = None,
         task_handle=taskhandle.DEFAULT_TASK_HANDLE,
     ):
         """Return the changes needed for this refactoring
 
         Parameters:
 
         - `dest`: the Resource or dotted moddule name of the move destination
         - `resources` can be a list of `rope.base.resources.File` to
           apply this refactoring on.  If `None`, the restructuring
           will be applied to all python files.
 
         """
+        # To do (in another PR): Create a new var: dest_resource: resource.Reource
+        # Doing so should remove the type:ignore below.
         if isinstance(dest, str):
             dest = self.project.find_module(dest)
         if resources is None:
             resources = self.project.get_python_files()
+        # The previous guards protect against this mypy complaint:
+        # "Resource" has no attribute "has_child"
         if dest is None or not dest.exists():
             raise exceptions.RefactoringError("Move destination does not exist.")
-        if dest.is_folder() and dest.has_child("__init__.py"):
-            dest = dest.get_child("__init__.py")
-        if dest.is_folder():
+        if dest.is_folder() and dest.has_child("__init__.py"):  # type:ignore
+            dest = dest.get_child("__init__.py")  # type:ignore
+        # The previous guards protect against this mypy complaint:
+        # Item "None" of "Union[str, Resource, None]" has no attribute "is_folder"
+        if dest.is_folder():  # type:ignore
             raise exceptions.RefactoringError(
                 "Move destination for non-modules should not be folders."
             )
         if self.source == dest:
             raise exceptions.RefactoringError(
                 "Moving global elements to the same module."
             )
```

### Comparing `rope-1.7.0/rope/refactor/multiproject.py` & `rope-1.8.0/rope/refactor/multiproject.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/occurrences.py` & `rope-1.8.0/rope/refactor/occurrences.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/patchedast.py` & `rope-1.8.0/rope/refactor/patchedast.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/rename.py` & `rope-1.8.0/rope/refactor/rename.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/restructure.py` & `rope-1.8.0/rope/refactor/restructure.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/similarfinder.py` & `rope-1.8.0/rope/refactor/similarfinder.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/sourceutils.py` & `rope-1.8.0/rope/refactor/sourceutils.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/suites.py` & `rope-1.8.0/rope/refactor/suites.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/topackage.py` & `rope-1.8.0/rope/refactor/topackage.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/usefunction.py` & `rope-1.8.0/rope/refactor/usefunction.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope/refactor/wildcards.py` & `rope-1.8.0/rope/refactor/wildcards.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/rope.egg-info/PKG-INFO` & `rope-1.8.0/rope.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rope
-Version: 1.7.0
+Version: 1.8.0
 Summary: a python refactoring library...
 Author-email: Ali Gholami Rudi <aligrudi@users.sourceforge.net>
 Maintainer-email: Lie Ryan <lieryan.24@proton.me>
 License: LGPL-3.0-or-later
 Project-URL: Source, https://github.com/python-rope/rope
 Project-URL: Documentation, https://rope.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: dev
+License-File: COPYING
 
 
 .. _GitHub python-rope / rope: https://github.com/python-rope/rope
 
 
 =========================================================================
  rope -- the world's most advanced open source Python refactoring library
@@ -85,14 +86,15 @@
 - Rope aims to provide powerful and safe refactoring
 - Rope is light on dependency, Rope only depends on Python itself
 - Unlike PyRight or PyLance, Rope does not depend on Node.js
 - Unlike PyLance or PyCharm, Rope is open source.
 - Unlike PyRight and PyLance, Rope is written in Python itself, so if you experience problems, you would be able to debug and hack it yourself in a language that you are already familiar with
 - In comparison to Jedi, Rope is focused on refactoring. While Jedi provides some basic refactoring capabilities, Rope supports many more advanced refactoring operations and options that Jedi does not.
 
+
 Bug Reports
 ===========
 
 Send your bug reports and feature requests at `python-rope's issue tracker`_ in GitHub.
 
 .. _`python-rope's issue tracker`: https://github.com/python-rope/rope/issues
 
@@ -107,21 +109,34 @@
 
 Many thanks the following people:
 
 - Ali Gholami Rudi (`@aligrudi`_) for initially creating the initial Rope project and most of Rope's code
 - Matej Cepl (`@mcepl`_) as former long-time Rope maintainer
 - Nick Smith <nicks@fastmail.fm> (`@soupytwist`_) as former Rope maintainer
 - `all of our current and former contributors`_
-- authors of editor integrations
+- `all authors of editor integrations`_
+- all maintainers of distro/package managers
 
 .. _`@aligrudi`: https://github.com/aligrudi
 .. _`@soupytwist`: https://github.com/soupytwist
 .. _`@lieryan`: https://github.com/lieryan
 .. _`@mcepl`: https://github.com/mcepl
 .. _`all of our current and former contributors`: https://github.com/python-rope/rope/blob/master/CONTRIBUTORS.md
+.. _`all authors of editor integrations`: https://github.com/python-rope/rope/wiki/How-to-use-Rope-in-my-IDE-or-Text-editor%3F
+
+Packaging Status
+================
+
+.. image:: https://repology.org/badge/vertical-allrepos/python:rope.svg?exclude_unsupported=1
+   :target: https://repology.org/project/python:rope/versions
+   :alt: Packaging status
+
+.. image:: https://repology.org/badge/vertical-allrepos/rope.svg?exclude_unsupported=1
+   :target: https://repology.org/project/rope/versions
+   :alt: Packaging status
 
 License
 =======
 
 This program is under the terms of LGPL v3+ (GNU Lesser General Public License).
 Have a look at `COPYING`_ for more information.
```

### Comparing `rope-1.7.0/rope.egg-info/SOURCES.txt` & `rope-1.8.0/rope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/advanced_oi_test.py` & `rope-1.8.0/ropetest/advanced_oi_test.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/builtinstest.py` & `rope-1.8.0/ropetest/builtinstest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/codeanalyzetest.py` & `rope-1.8.0/ropetest/codeanalyzetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/conftest.py` & `rope-1.8.0/ropetest/conftest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/autoimport/autoimporttest.py` & `rope-1.8.0/ropetest/contrib/autoimport/autoimporttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/autoimport/conftest.py` & `rope-1.8.0/ropetest/contrib/autoimport/conftest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/autoimport/modeltest.py` & `rope-1.8.0/ropetest/contrib/autoimport/modeltest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/autoimport/parsetest.py` & `rope-1.8.0/ropetest/contrib/autoimport/parsetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/autoimport/utilstest.py` & `rope-1.8.0/ropetest/contrib/autoimport/utilstest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Tests for autoimport utility functions, written in pytest"""
 
+from pathlib import Path
+
 from rope.contrib.autoimport import utils
 from rope.contrib.autoimport.defs import Package, PackageType, Source
 
 
 def test_get_package_source(mod1_path, project):
     assert utils.get_package_source(mod1_path, project, "") == Source.PROJECT
 
@@ -53,7 +55,17 @@
 
 
 def test_get_package_tuple_compiled(compiled_lib):
     lib_name, lib_path = compiled_lib
     assert Package(
         lib_name, Source.STANDARD, lib_path, PackageType.COMPILED
     ) == utils.get_package_tuple(lib_path)
+
+
+def test_get_files(project, mod1, pkg1, mod2):
+    root: Package = utils.get_package_tuple(project.root.pathlib)
+    paths = [m.filepath.relative_to(project.root.pathlib) for m in utils.get_files(root)]
+    assert set(paths) == {
+        Path("mod1.py"),
+        Path("pkg1/__init__.py"),
+        Path("pkg1/mod2.py"),
+    }
```

### Comparing `rope-1.7.0/ropetest/contrib/autoimporttest.py` & `rope-1.8.0/ropetest/contrib/autoimporttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/changestacktest.py` & `rope-1.8.0/ropetest/contrib/changestacktest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/codeassisttest.py` & `rope-1.8.0/ropetest/contrib/codeassisttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/finderrorstest.py` & `rope-1.8.0/ropetest/contrib/finderrorstest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/findittest.py` & `rope-1.8.0/ropetest/contrib/findittest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/fixmodnamestest.py` & `rope-1.8.0/ropetest/contrib/fixmodnamestest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/contrib/generatetest.py` & `rope-1.8.0/ropetest/contrib/generatetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/doatest.py` & `rope-1.8.0/ropetest/doatest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/historytest.py` & `rope-1.8.0/ropetest/historytest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/objectdbtest.py` & `rope-1.8.0/ropetest/objectdbtest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/objectinfertest.py` & `rope-1.8.0/ropetest/objectinfertest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/projecttest.py` & `rope-1.8.0/ropetest/projecttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/pycoretest.py` & `rope-1.8.0/ropetest/pycoretest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/pyscopestest.py` & `rope-1.8.0/ropetest/pyscopestest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/__init__.py` & `rope-1.8.0/ropetest/refactor/__init__.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/change_signature_test.py` & `rope-1.8.0/ropetest/refactor/change_signature_test.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/extracttest.py` & `rope-1.8.0/ropetest/refactor/extracttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/importutilstest.py` & `rope-1.8.0/ropetest/refactor/importutilstest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/inlinetest.py` & `rope-1.8.0/ropetest/refactor/inlinetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/movetest.py` & `rope-1.8.0/ropetest/refactor/movetest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/multiprojecttest.py` & `rope-1.8.0/ropetest/refactor/multiprojecttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/patchedasttest.py` & `rope-1.8.0/ropetest/refactor/patchedasttest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/renametest.py` & `rope-1.8.0/ropetest/refactor/renametest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/restructuretest.py` & `rope-1.8.0/ropetest/refactor/restructuretest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/similarfindertest.py` & `rope-1.8.0/ropetest/refactor/similarfindertest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/suitestest.py` & `rope-1.8.0/ropetest/refactor/suitestest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/refactor/usefunctiontest.py` & `rope-1.8.0/ropetest/refactor/usefunctiontest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/reprtest.py` & `rope-1.8.0/ropetest/reprtest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/runmodtest.py` & `rope-1.8.0/ropetest/runmodtest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/serializer_test.py` & `rope-1.8.0/ropetest/serializer_test.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/simplifytest.py` & `rope-1.8.0/ropetest/simplifytest.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/testutils.py` & `rope-1.8.0/ropetest/testutils.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/type_hinting_test.py` & `rope-1.8.0/ropetest/type_hinting_test.py`

 * *Files identical despite different names*

### Comparing `rope-1.7.0/ropetest/versioningtest.py` & `rope-1.8.0/ropetest/versioningtest.py`

 * *Files identical despite different names*

