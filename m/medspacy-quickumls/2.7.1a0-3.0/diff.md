# Comparing `tmp/medspacy_quickumls-2.7.1a0.tar.gz` & `tmp/medspacy_quickumls-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspacy_quickumls-2.7.1a0.tar", last modified: Fri Mar 10 21:19:12 2023, max compression
+gzip compressed data, was "medspacy_quickumls-3.0.tar", last modified: Fri May  5 16:49:07 2023, max compression
```

## Comparing `medspacy_quickumls-2.7.1a0.tar` & `medspacy_quickumls-3.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.252118 medspacy_quickumls-2.7.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-03-10 21:19:12.252118 medspacy_quickumls-2.7.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.244118 medspacy_quickumls-2.7.1a0/medspacy_quickumls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-03-10 21:19:12.000000 medspacy_quickumls-2.7.1a0/medspacy_quickumls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-03-10 21:19:12.000000 medspacy_quickumls-2.7.1a0/medspacy_quickumls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 21:19:12.000000 medspacy_quickumls-2.7.1a0/medspacy_quickumls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-10 21:19:12.000000 medspacy_quickumls-2.7.1a0/medspacy_quickumls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-10 21:19:12.000000 medspacy_quickumls-2.7.1a0/medspacy_quickumls.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.244118 medspacy_quickumls-2.7.1a0/quickumls/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/about.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/spacy_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/quickumls/umls_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.240118 medspacy_quickumls-2.7.1a0/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.244118 medspacy_quickumls-2.7.1a0/resources/quickumls/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.244118 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.248118 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.248118 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.248118 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.248118 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.252118 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-10 21:19:12.252118 medspacy_quickumls-2.7.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 21:19:12.252118 medspacy_quickumls-2.7.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/tests/test_quickumls_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-03-10 21:19:00.000000 medspacy_quickumls-2.7.1a0/tests/test_quickumls_spangroup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.619537 medspacy_quickumls-3.0/
+-rw-rw-rw-   0        0        0     1124 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       43 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9491 2023-05-05 16:49:07.619537 medspacy_quickumls-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8628 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.575337 medspacy_quickumls-3.0/medspacy_quickumls.egg-info/
+-rw-rw-rw-   0        0        0     9491 2023-05-05 16:49:07.000000 medspacy_quickumls-3.0/medspacy_quickumls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7980 2023-05-05 16:49:07.000000 medspacy_quickumls-3.0/medspacy_quickumls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 16:49:07.000000 medspacy_quickumls-3.0/medspacy_quickumls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-05-05 16:49:07.000000 medspacy_quickumls-3.0/medspacy_quickumls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 16:49:07.000000 medspacy_quickumls-3.0/medspacy_quickumls.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.581834 medspacy_quickumls-3.0/quickumls/
+-rw-rw-rw-   0        0        0       93 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/quickumls/__init__.py
+-rw-rw-rw-   0        0        0      657 2023-05-05 16:48:11.000000 medspacy_quickumls-3.0/quickumls/about.py
+-rw-rw-rw-   0        0        0      296 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/quickumls/client.py
+-rw-rw-rw-   0        0        0    13804 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/quickumls/constants.py
+-rw-rw-rw-   0        0        0    18659 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/quickumls/core.py
+-rw-rw-rw-   0        0        0     7232 2023-05-05 16:17:09.000000 medspacy_quickumls-3.0/quickumls/install.py
+-rw-rw-rw-   0        0        0     7558 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/quickumls/network.py
+-rw-rw-rw-   0        0        0     2731 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/quickumls/server.py
+-rw-rw-rw-   0        0        0    11134 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/quickumls/spacy_component.py
+-rw-rw-rw-   0        0        0     8565 2023-05-05 16:48:11.000000 medspacy_quickumls-3.0/quickumls/toolbox.py
+-rw-rw-rw-   0        0        0     1185 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/quickumls/umls_match.py
+-rw-rw-rw-   0        0        0      101 2023-05-05 16:48:11.000000 medspacy_quickumls-3.0/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.560652 medspacy_quickumls-3.0/resources/
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.561652 medspacy_quickumls-3.0/resources/quickumls/
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.583839 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
+-rw-rw-rw-   0        0        0      183 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.585024 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
+-rw-rw-rw-   0        0        0    12288 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
+-rw-rw-rw-   0        0        0    12288 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-rw-rw-   0        0        0        7 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
+-rw-rw-rw-   0        0        0        3 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.600013 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
+-rw-rw-rw-   0        0        0     6116 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-rw-rw-   0        0        0     6892 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-rw-rw-   0        0        0     2788 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-rw-rw-   0        0        0     2664 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-rw-rw-   0        0        0     2744 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-rw-rw-   0        0        0     3016 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-rw-rw-   0        0        0     2904 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-rw-rw-   0        0        0     3140 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-rw-rw-   0        0        0     3228 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-rw-rw-   0        0        0     3460 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-rw-rw-   0        0        0     3148 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-rw-rw-   0        0        0     7344 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-rw-rw-   0        0        0     3224 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-rw-rw-   0        0        0     4984 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-rw-rw-   0        0        0     5152 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-rw-rw-   0        0        0     5024 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-rw-rw-   0        0        0     3384 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-rw-rw-   0        0        0     3824 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-rw-rw-   0        0        0     3544 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-rw-rw-   0        0        0     4064 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-rw-rw-   0        0        0     3624 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-rw-rw-   0        0        0     5160 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-rw-rw-   0        0        0     3788 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-rw-rw-   0        0        0     5368 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-rw-rw-   0        0        0     2384 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.603012 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
+-rw-rw-rw-   0        0        0      183 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.604013 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
+-rw-rw-rw-   0        0        0    20480 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
+-rw-rw-rw-   0        0        0    12288 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-rw-rw-   0        0        0        7 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
+-rw-rw-rw-   0        0        0        3 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.618012 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
+-rw-rw-rw-   0        0        0     2912 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-rw-rw-   0        0        0     6162 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-rw-rw-   0        0        0     2540 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-rw-rw-   0        0        0     2574 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-rw-rw-   0        0        0     2642 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-rw-rw-   0        0        0     2884 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-rw-rw-   0        0        0     2778 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-rw-rw-   0        0        0     2990 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-rw-rw-   0        0        0     3066 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-rw-rw-   0        0        0     3262 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-rw-rw-   0        0        0     2984 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-rw-rw-   0        0        0     5574 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-rw-rw-   0        0        0     3050 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-rw-rw-   0        0        0     4526 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-rw-rw-   0        0        0     3546 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-rw-rw-   0        0        0     4616 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-rw-rw-   0        0        0     3186 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-rw-rw-   0        0        0     3576 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-rw-rw-   0        0        0     3322 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-rw-rw-   0        0        0     3780 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-rw-rw-   0        0        0     3390 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-rw-rw-   0        0        0     4696 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-rw-rw-   0        0        0     3528 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-rw-rw-   0        0        0     4828 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-rw-rw-   0        0        0     2336 2022-12-22 17:44:22.000000 medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+-rw-rw-rw-   0        0        0       85 2023-05-05 16:49:07.620545 medspacy_quickumls-3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2395 2023-05-05 16:17:09.000000 medspacy_quickumls-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:49:07.619537 medspacy_quickumls-3.0/tests/
+-rw-rw-rw-   0        0        0     1149 2023-05-05 16:48:11.000000 medspacy_quickumls-3.0/tests/test_basic.py
+-rw-rw-rw-   0        0        0     2808 2023-05-05 16:48:11.000000 medspacy_quickumls-3.0/tests/test_quickumls_component.py
+-rw-rw-rw-   0        0        0     1325 2023-05-05 16:48:11.000000 medspacy_quickumls-3.0/tests/test_quickumls_spangroup.py
```

### Comparing `medspacy_quickumls-2.7.1a0/PKG-INFO` & `medspacy_quickumls-3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-Metadata-Version: 2.1
-Name: medspacy_quickumls
-Version: 2.7.1a0
-Summary: QuickUMLS is a tool for fast, unsupervised biomedical concept extraction from medical text
-Home-page: https://github.com/Georgetown-IR-Lab/QuickUMLS
-Author: Luca Soldaini, modified by Kelly Peterson
-Author-email: luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
-
-[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
-
-# QuickUMLS
-
-QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
-It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
-For more details on how QuickUMLS works, we remand to our paper.
-
-This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
-
-## Installation
-
-1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
-2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>†</sup>.
-3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
-    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
-    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
-    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
-    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
-
-
-## APIs
-
-A QuickUMLS object can be instantiated as follows:
-
-```python
-from quickumls import QuickUMLS
-
-matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
-                    similarity_name, window, accepted_semtypes)
-```
-
-Where:
-
-- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
-- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
-- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
-- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
-- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
-- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
-
-To use the matcher, simply call
-
-```python
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
-
-If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
-
-## spaCy pipeline component
-
-QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
-
-Adding QuickUMLS as a component in a pipeline can be done as follows:
-
-```python
-from quickumls.spacy_component import SpacyQuickUMLS
-
-# common English pipeline
-nlp = spacy.load('en_core_web_sm')
-
-quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
-nlp.add_pipe(quickumls_component)
-
-doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
-
-for ent in doc.ents:
-    print('Entity text : {}'.format(ent.text))
-    print('Label (UMLS CUI) : {}'.format(ent.label_))
-    print('Similarity : {}'.format(ent._.similarity))
-    print('Semtypes : {}'.format(ent._.semtypes))
-```
-
-## Server / Client Support
-
-Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
-
-To start the server, run `python -m quickumls.server`:
-
-```bash
-python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
-```
-
-Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
-
-To load the client, import `get_quickumls_client` from `quickumls`:
-
-```bash
-from quickumls import get_quickumls_client
-matcher = get_quickumls_client()
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-The API of the client is the same of a QuickUMLS object.
-
-
-In case you wish to run the server in the background, you can do so as follows:
-
-```bash
-nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
-
-```
-
-When you are done, don't forget to stop the server by running.
-```bash
-kill -9 `cat nohup.pid`
-rm nohup.pid
-```
-
-## References
-
-- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
-- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
+Metadata-Version: 2.1
+Name: medspacy_quickumls
+Version: 3.0
+Summary: QuickUMLS is a tool for fast, unsupervised biomedical concept extraction from medical text
+Home-page: https://github.com/Georgetown-IR-Lab/QuickUMLS
+Author: Luca Soldaini, modified by Kelly Peterson and Jianlin Shi
+Author-email: luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
+
+[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
+
+# QuickUMLS
+
+QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
+It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
+For more details on how QuickUMLS works, we remand to our paper.
+
+This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
+
+## Installation
+
+1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
+2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>â€ </sup>.
+3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
+    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
+    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
+    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
+    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
+
+
+## APIs
+
+A QuickUMLS object can be instantiated as follows:
+
+```python
+from quickumls import QuickUMLS
+
+matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
+                    similarity_name, window, accepted_semtypes)
+```
+
+Where:
+
+- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
+- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
+- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
+- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
+- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
+- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
+
+To use the matcher, simply call
+
+```python
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
+
+If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
+
+## spaCy pipeline component
+
+QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
+
+Adding QuickUMLS as a component in a pipeline can be done as follows:
+
+```python
+from quickumls.spacy_component import SpacyQuickUMLS
+
+# common English pipeline
+nlp = spacy.load('en_core_web_sm')
+
+quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
+nlp.add_pipe(quickumls_component)
+
+doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
+
+for ent in doc.ents:
+    print('Entity text : {}'.format(ent.text))
+    print('Label (UMLS CUI) : {}'.format(ent.label_))
+    print('Similarity : {}'.format(ent._.similarity))
+    print('Semtypes : {}'.format(ent._.semtypes))
+```
+
+## Server / Client Support
+
+Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
+
+To start the server, run `python -m quickumls.server`:
+
+```bash
+python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
+```
+
+Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
+
+To load the client, import `get_quickumls_client` from `quickumls`:
+
+```bash
+from quickumls import get_quickumls_client
+matcher = get_quickumls_client()
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+The API of the client is the same of a QuickUMLS object.
+
+
+In case you wish to run the server in the background, you can do so as follows:
+
+```bash
+nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
+
+```
+
+When you are done, don't forget to stop the server by running.
+```bash
+kill -9 `cat nohup.pid`
+rm nohup.pid
+```
+
+## References
+
+- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
+- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
```

### Comparing `medspacy_quickumls-2.7.1a0/README.md` & `medspacy_quickumls-3.0/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
-
-[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
-
-# QuickUMLS
-
-QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
-It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
-For more details on how QuickUMLS works, we remand to our paper.
-
-This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
-
-## Installation
-
-1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
-2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>†</sup>.
-3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
-    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
-    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
-    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
-    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
-
-
-## APIs
-
-A QuickUMLS object can be instantiated as follows:
-
-```python
-from quickumls import QuickUMLS
-
-matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
-                    similarity_name, window, accepted_semtypes)
-```
-
-Where:
-
-- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
-- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
-- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
-- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
-- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
-- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
-
-To use the matcher, simply call
-
-```python
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
-
-If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
-
-## spaCy pipeline component
-
-QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
-
-Adding QuickUMLS as a component in a pipeline can be done as follows:
-
-```python
-from quickumls.spacy_component import SpacyQuickUMLS
-
-# common English pipeline
-nlp = spacy.load('en_core_web_sm')
-
-quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
-nlp.add_pipe(quickumls_component)
-
-doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
-
-for ent in doc.ents:
-    print('Entity text : {}'.format(ent.text))
-    print('Label (UMLS CUI) : {}'.format(ent.label_))
-    print('Similarity : {}'.format(ent._.similarity))
-    print('Semtypes : {}'.format(ent._.semtypes))
-```
-
-## Server / Client Support
-
-Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
-
-To start the server, run `python -m quickumls.server`:
-
-```bash
-python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
-```
-
-Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
-
-To load the client, import `get_quickumls_client` from `quickumls`:
-
-```bash
-from quickumls import get_quickumls_client
-matcher = get_quickumls_client()
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-The API of the client is the same of a QuickUMLS object.
-
-
-In case you wish to run the server in the background, you can do so as follows:
-
-```bash
-nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
-
-```
-
-When you are done, don't forget to stop the server by running.
-```bash
-kill -9 `cat nohup.pid`
-rm nohup.pid
-```
-
-## References
-
-- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
-- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
+[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
+
+[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
+
+# QuickUMLS
+
+QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
+It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
+For more details on how QuickUMLS works, we remand to our paper.
+
+This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
+
+## Installation
+
+1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
+2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>†</sup>.
+3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
+    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
+    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
+    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
+    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
+
+
+## APIs
+
+A QuickUMLS object can be instantiated as follows:
+
+```python
+from quickumls import QuickUMLS
+
+matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
+                    similarity_name, window, accepted_semtypes)
+```
+
+Where:
+
+- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
+- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
+- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
+- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
+- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
+- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
+
+To use the matcher, simply call
+
+```python
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
+
+If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
+
+## spaCy pipeline component
+
+QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
+
+Adding QuickUMLS as a component in a pipeline can be done as follows:
+
+```python
+from quickumls.spacy_component import SpacyQuickUMLS
+
+# common English pipeline
+nlp = spacy.load('en_core_web_sm')
+
+quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
+nlp.add_pipe(quickumls_component)
+
+doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
+
+for ent in doc.ents:
+    print('Entity text : {}'.format(ent.text))
+    print('Label (UMLS CUI) : {}'.format(ent.label_))
+    print('Similarity : {}'.format(ent._.similarity))
+    print('Semtypes : {}'.format(ent._.semtypes))
+```
+
+## Server / Client Support
+
+Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
+
+To start the server, run `python -m quickumls.server`:
+
+```bash
+python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
+```
+
+Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
+
+To load the client, import `get_quickumls_client` from `quickumls`:
+
+```bash
+from quickumls import get_quickumls_client
+matcher = get_quickumls_client()
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+The API of the client is the same of a QuickUMLS object.
+
+
+In case you wish to run the server in the background, you can do so as follows:
+
+```bash
+nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
+
+```
+
+When you are done, don't forget to stop the server by running.
+```bash
+kill -9 `cat nohup.pid`
+rm nohup.pid
+```
+
+## References
+
+- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
+- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
```

### Comparing `medspacy_quickumls-2.7.1a0/medspacy_quickumls.egg-info/PKG-INFO` & `medspacy_quickumls-3.0/medspacy_quickumls.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-Metadata-Version: 2.1
-Name: medspacy-quickumls
-Version: 2.7.1a0
-Summary: QuickUMLS is a tool for fast, unsupervised biomedical concept extraction from medical text
-Home-page: https://github.com/Georgetown-IR-Lab/QuickUMLS
-Author: Luca Soldaini, modified by Kelly Peterson
-Author-email: luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
-
-[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
-
-# QuickUMLS
-
-QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
-It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
-For more details on how QuickUMLS works, we remand to our paper.
-
-This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
-
-## Installation
-
-1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
-2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>†</sup>.
-3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
-    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
-    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
-    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
-    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
-
-
-## APIs
-
-A QuickUMLS object can be instantiated as follows:
-
-```python
-from quickumls import QuickUMLS
-
-matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
-                    similarity_name, window, accepted_semtypes)
-```
-
-Where:
-
-- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
-- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
-- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
-- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
-- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
-- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
-
-To use the matcher, simply call
-
-```python
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
-
-If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
-
-## spaCy pipeline component
-
-QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
-
-Adding QuickUMLS as a component in a pipeline can be done as follows:
-
-```python
-from quickumls.spacy_component import SpacyQuickUMLS
-
-# common English pipeline
-nlp = spacy.load('en_core_web_sm')
-
-quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
-nlp.add_pipe(quickumls_component)
-
-doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
-
-for ent in doc.ents:
-    print('Entity text : {}'.format(ent.text))
-    print('Label (UMLS CUI) : {}'.format(ent.label_))
-    print('Similarity : {}'.format(ent._.similarity))
-    print('Semtypes : {}'.format(ent._.semtypes))
-```
-
-## Server / Client Support
-
-Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
-
-To start the server, run `python -m quickumls.server`:
-
-```bash
-python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
-```
-
-Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
-
-To load the client, import `get_quickumls_client` from `quickumls`:
-
-```bash
-from quickumls import get_quickumls_client
-matcher = get_quickumls_client()
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-The API of the client is the same of a QuickUMLS object.
-
-
-In case you wish to run the server in the background, you can do so as follows:
-
-```bash
-nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
-
-```
-
-When you are done, don't forget to stop the server by running.
-```bash
-kill -9 `cat nohup.pid`
-rm nohup.pid
-```
-
-## References
-
-- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
-- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
+Metadata-Version: 2.1
+Name: medspacy-quickumls
+Version: 3.0
+Summary: QuickUMLS is a tool for fast, unsupervised biomedical concept extraction from medical text
+Home-page: https://github.com/Georgetown-IR-Lab/QuickUMLS
+Author: Luca Soldaini, modified by Kelly Peterson and Jianlin Shi
+Author-email: luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
+
+[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
+
+# QuickUMLS
+
+QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
+It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
+For more details on how QuickUMLS works, we remand to our paper.
+
+This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
+
+## Installation
+
+1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
+2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>â€ </sup>.
+3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
+    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
+    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
+    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
+    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
+
+
+## APIs
+
+A QuickUMLS object can be instantiated as follows:
+
+```python
+from quickumls import QuickUMLS
+
+matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
+                    similarity_name, window, accepted_semtypes)
+```
+
+Where:
+
+- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
+- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
+- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
+- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
+- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
+- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
+
+To use the matcher, simply call
+
+```python
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
+
+If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
+
+## spaCy pipeline component
+
+QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
+
+Adding QuickUMLS as a component in a pipeline can be done as follows:
+
+```python
+from quickumls.spacy_component import SpacyQuickUMLS
+
+# common English pipeline
+nlp = spacy.load('en_core_web_sm')
+
+quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
+nlp.add_pipe(quickumls_component)
+
+doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
+
+for ent in doc.ents:
+    print('Entity text : {}'.format(ent.text))
+    print('Label (UMLS CUI) : {}'.format(ent.label_))
+    print('Similarity : {}'.format(ent._.similarity))
+    print('Semtypes : {}'.format(ent._.semtypes))
+```
+
+## Server / Client Support
+
+Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
+
+To start the server, run `python -m quickumls.server`:
+
+```bash
+python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
+```
+
+Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
+
+To load the client, import `get_quickumls_client` from `quickumls`:
+
+```bash
+from quickumls import get_quickumls_client
+matcher = get_quickumls_client()
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+The API of the client is the same of a QuickUMLS object.
+
+
+In case you wish to run the server in the background, you can do so as follows:
+
+```bash
+nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
+
+```
+
+When you are done, don't forget to stop the server by running.
+```bash
+kill -9 `cat nohup.pid`
+rm nohup.pid
+```
+
+## References
+
+- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
+- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
```

### Comparing `medspacy_quickumls-2.7.1a0/medspacy_quickumls.egg-info/SOURCES.txt` & `medspacy_quickumls-3.0/medspacy_quickumls.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,9 +80,10 @@
 quickumls/../resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
 quickumls/../resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
 quickumls/../resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
 quickumls/../resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
 quickumls/../resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
 quickumls/../resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
 quickumls/../resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+tests/test_basic.py
 tests/test_quickumls_component.py
 tests/test_quickumls_spangroup.py
```

### Comparing `medspacy_quickumls-2.7.1a0/quickumls/about.py` & `medspacy_quickumls-3.0/quickumls/about.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# inspired from:
-# https://python-packaging-user-guide.readthedocs.org/en/latest/single_source_version/
-# https://github.com/pypa/warehouse/blob/master/warehouse/__about__.py
-# https://github.com/explosion/spaCy/blob/master/spacy/about.py
-
-__title__ = 'medspacy_quickumls'
-__version__ = '2.7.1a'
-__author__ = 'Luca Soldaini, modified by Kelly Peterson'
-__email__ = 'luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu'
-__license__ = 'MIT'
-__uri__ = "https://github.com/medspacy/quickumls"
-__copyright__ = '2014-2020, Georgetown University Information Retrieval Lab, updated 2020-2023, University of Utah'
+# inspired from:
+# https://python-packaging-user-guide.readthedocs.org/en/latest/single_source_version/
+# https://github.com/pypa/warehouse/blob/master/warehouse/__about__.py
+# https://github.com/explosion/spaCy/blob/master/spacy/about.py
+
+__title__ = 'medspacy_quickumls'
+__version__ = '3.0'
+__author__ = 'Luca Soldaini, modified by Kelly Peterson and Jianlin Shi'
+__email__ = 'luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu'
+__license__ = 'MIT'
+__uri__ = "https://github.com/medspacy/quickumls"
+__copyright__ = '2014-2020, Georgetown University Information Retrieval Lab, updated 2020-2023, University of Utah'
```

### Comparing `medspacy_quickumls-2.7.1a0/quickumls/constants.py` & `medspacy_quickumls-3.0/quickumls/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,851 +1,863 @@
 00000000: 4d45 4453 5041 4359 5f44 4546 4155 4c54  MEDSPACY_DEFAULT
 00000010: 5f53 5041 4e5f 4752 4f55 505f 4e41 4d45  _SPAN_GROUP_NAME
 00000020: 203d 2022 6d65 6473 7061 6379 5f73 7061   = "medspacy_spa
-00000030: 6e73 220a 0a48 4541 4445 5253 5f4d 5243  ns"..HEADERS_MRC
-00000040: 4f4e 534f 203d 205b 0a20 2020 2027 6375  ONSO = [.    'cu
-00000050: 6927 2c20 276c 6174 272c 2027 7473 272c  i', 'lat', 'ts',
-00000060: 2027 6c75 6927 2c20 2773 7474 272c 2027   'lui', 'stt', '
-00000070: 7375 6927 2c20 2769 7370 7265 6627 2c20  sui', 'ispref', 
-00000080: 2761 7569 272c 2027 7361 7569 272c 0a20  'aui', 'saui',. 
-00000090: 2020 2027 7363 7569 272c 2027 7364 7569     'scui', 'sdui
-000000a0: 272c 2027 7361 6227 2c20 2774 7479 272c  ', 'sab', 'tty',
-000000b0: 2027 636f 6465 272c 2027 7374 7227 2c20   'code', 'str', 
-000000c0: 2773 726c 272c 2027 7375 7070 7265 7373  'srl', 'suppress
-000000d0: 272c 2027 6376 6627 0a5d 0a48 4541 4445  ', 'cvf'.].HEADE
-000000e0: 5253 5f4d 5253 5459 203d 205b 0a20 2020  RS_MRSTY = [.   
-000000f0: 2027 6375 6927 2c20 2773 7479 272c 2027   'cui', 'sty', '
-00000100: 6869 6572 2720 2764 6573 6327 2c20 2773  hier' 'desc', 's
-00000110: 6964 272c 2027 6e75 6d27 0a5d 0a0a 4e45  id', 'num'.]..NE
-00000120: 4741 5449 4f4e 5320 3d20 7b27 6e6f 6e65  GATIONS = {'none
-00000130: 272c 2027 6e6f 6e27 2c20 276e 6569 7468  ', 'non', 'neith
-00000140: 6572 272c 2027 6e6f 7227 2c20 276e 6f27  er', 'nor', 'no'
-00000150: 2c20 276e 6f74 277d 0a0a 2320 5468 6520  , 'not'}..# The 
-00000160: 666f 6c6c 6f77 696e 6720 6973 2061 206c  following is a l
-00000170: 6973 7420 6f66 2061 6c6c 2065 7869 7374  ist of all exist
-00000180: 696e 6720 7365 6d74 7970 6573 2061 6c6f  ing semtypes alo
-00000190: 6e67 2077 6974 6820 7468 6569 7220 6e61  ng with their na
-000001a0: 6d65 2061 6e64 2073 6f6d 6520 6578 616d  me and some exam
-000001b0: 706c 6573 2e20 0a23 2059 6f75 2063 616e  ples. .# You can
-000001c0: 2065 6173 696c 7920 7365 6c65 6374 2074   easily select t
-000001d0: 6865 206f 6e65 7320 796f 7520 6e65 6564  he ones you need
-000001e0: 2062 7920 636f 6d6d 656e 7469 6e67 206f   by commenting o
-000001f0: 7574 2074 6865 206c 696e 6573 2074 6861  ut the lines tha
-00000200: 7420 6172 6520 6e6f 7420 7265 6c65 7661  t are not releva
-00000210: 6e74 2066 6f72 2079 6f75 7220 6170 706c  nt for your appl
-00000220: 6963 6174 696f 6e2e 0a0a 4143 4345 5054  ication...ACCEPT
-00000230: 4544 5f53 454d 5459 5045 5320 3d20 7b0a  ED_SEMTYPES = {.
-00000240: 2020 2020 2320 2754 3032 3027 2c20 2320      # 'T020', # 
-00000250: 4163 7175 6972 6564 2041 626e 6f72 6d61  Acquired Abnorma
-00000260: 6c69 7479 2c20 6578 2e3a 2048 656d 6f72  lity, ex.: Hemor
-00000270: 7268 6f69 6473 3b20 4865 726e 6961 2c20  rhoids; Hernia, 
-00000280: 4665 6d6f 7261 6c3b 2043 6175 6c69 666c  Femoral; Caulifl
-00000290: 6f77 6572 2065 6172 0a20 2020 2023 2027  ower ear.    # '
-000002a0: 5430 3532 272c 2023 2041 6374 6976 6974  T052', # Activit
-000002b0: 792c 2065 782e 3a20 4578 7065 6469 7469  y, ex.: Expediti
-000002c0: 6f6e 733b 2049 6e66 6f72 6d61 7469 6f6e  ons; Information
-000002d0: 2044 6973 7472 6962 7574 696f 6e3b 2053   Distribution; S
-000002e0: 6f63 6961 6c20 506c 616e 6e69 6e67 0a20  ocial Planning. 
-000002f0: 2020 2023 2027 5431 3030 272c 2023 2041     # 'T100', # A
-00000300: 6765 2047 726f 7570 2c20 6578 2e3a 2041  ge Group, ex.: A
-00000310: 6475 6c74 3b20 496e 6661 6e74 2c20 5072  dult; Infant, Pr
-00000320: 656d 6174 7572 653b 2041 646f 6c65 7363  emature; Adolesc
-00000330: 656e 7420 2861 6765 2067 726f 7570 290a  ent (age group).
-00000340: 2020 2020 2320 2754 3038 3727 2c20 2320      # 'T087', # 
-00000350: 416d 696e 6f20 4163 6964 2053 6571 7565  Amino Acid Seque
-00000360: 6e63 652c 2065 782e 3a20 5369 676e 616c  nce, ex.: Signal
-00000370: 2050 6570 7469 6465 733b 2048 6f6d 6f6c   Peptides; Homol
-00000380: 6f67 6f75 7320 5365 7175 656e 6365 732c  ogous Sequences,
-00000390: 2041 6d69 6e6f 2041 6369 643b 2041 626e   Amino Acid; Abn
-000003a0: 6f72 6d61 6c20 616d 696e 6f20 6163 6964  ormal amino acid
-000003b0: 0a20 2020 2023 2027 5431 3136 272c 2023  .    # 'T116', #
-000003c0: 2041 6d69 6e6f 2041 6369 642c 2050 6570   Amino Acid, Pep
-000003d0: 7469 6465 2c20 6f72 2050 726f 7465 696e  tide, or Protein
-000003e0: 2c20 6578 2e3a 2041 6d69 6e6f 2041 6369  , ex.: Amino Aci
-000003f0: 6473 2c20 4379 636c 6963 3b20 476c 7963  ds, Cyclic; Glyc
-00000400: 6f70 6570 7469 6465 733b 204b 6572 6174  opeptides; Kerat
-00000410: 696e 0a20 2020 2023 2027 5430 3131 272c  in.    # 'T011',
-00000420: 2023 2041 6d70 6869 6269 616e 2c20 6578   # Amphibian, ex
-00000430: 2e3a 2053 616c 616d 616e 6472 613b 2055  .: Salamandra; U
-00000440: 726f 6465 6c61 3b20 4272 617a 696c 6961  rodela; Brazilia
-00000450: 6e20 686f 726e 6564 2066 726f 670a 2020  n horned frog.  
-00000460: 2020 2320 2754 3139 3027 2c20 2320 416e    # 'T190', # An
-00000470: 6174 6f6d 6963 616c 2041 626e 6f72 6d61  atomical Abnorma
-00000480: 6c69 7479 2c20 6578 2e3a 2042 726f 6e63  lity, ex.: Bronc
-00000490: 6869 616c 2046 6973 7475 6c61 3b20 466f  hial Fistula; Fo
-000004a0: 6f74 2044 6566 6f72 6d69 7469 6573 3b20  ot Deformities; 
-000004b0: 4879 7065 726f 7374 6f73 6973 206f 6620  Hyperostosis of 
-000004c0: 736b 756c 6c0a 2020 2020 2320 2754 3031  skull.    # 'T01
-000004d0: 3727 2c20 2320 416e 6174 6f6d 6963 616c  7', # Anatomical
-000004e0: 2053 7472 7563 7475 7265 2c20 6578 2e3a   Structure, ex.:
-000004f0: 2043 6164 6176 6572 3b20 5068 6172 796e   Cadaver; Pharyn
-00000500: 676f 7374 6f6d 653b 2041 6e61 746f 6d69  gostome; Anatomi
-00000510: 6320 7374 7275 6374 7572 6573 0a20 2020  c structures.   
-00000520: 2023 2027 5430 3038 272c 2023 2041 6e69   # 'T008', # Ani
-00000530: 6d61 6c2c 2065 782e 3a20 416e 696d 616c  mal, ex.: Animal
-00000540: 733b 2041 6e69 6d61 6c73 2c20 4c61 626f  s; Animals, Labo
-00000550: 7261 746f 7279 3b20 4361 726e 6976 6f72  ratory; Carnivor
-00000560: 650a 2020 2020 2754 3139 3527 2c20 2320  e.    'T195', # 
-00000570: 416e 7469 6269 6f74 6963 2c20 6578 2e3a  Antibiotic, ex.:
-00000580: 2041 6e74 6962 696f 7469 6373 3b20 6261   Antibiotics; ba
-00000590: 6374 6572 6963 6964 653b 2054 6869 656e  ctericide; Thien
-000005a0: 616d 7963 696e 730a 2020 2020 2320 2754  amycins.    # 'T
-000005b0: 3139 3427 2c20 2320 4172 6368 6165 6f6e  194', # Archaeon
-000005c0: 2c20 6578 2e3a 2054 6865 726d 6f70 726f  , ex.: Thermopro
-000005d0: 7465 616c 6573 3b20 4861 6c6f 6665 7261  teales; Halofera
-000005e0: 7820 766f 6c63 616e 6969 3b20 4d65 7468  x volcanii; Meth
-000005f0: 616e 6f73 7069 7269 6c6c 756d 0a20 2020  anospirillum.   
-00000600: 2023 2027 5430 3037 272c 2023 2042 6163   # 'T007', # Bac
-00000610: 7465 7269 756d 2c20 6578 2e3a 2041 6365  terium, ex.: Ace
-00000620: 746f 6261 6374 6572 3b20 4261 6369 6c6c  tobacter; Bacill
-00000630: 7573 2063 6572 6575 733b 2043 7974 6f70  us cereus; Cytop
-00000640: 6861 6761 0a20 2020 2023 2027 5430 3533  haga.    # 'T053
-00000650: 272c 2023 2042 6568 6176 696f 722c 2065  ', # Behavior, e
-00000660: 782e 3a20 486f 6d69 6e67 2042 6568 6176  x.: Homing Behav
-00000670: 696f 723b 2053 6578 7561 6c69 7479 3b20  ior; Sexuality; 
-00000680: 4861 6269 7461 7420 5365 6c65 6374 696f  Habitat Selectio
-00000690: 6e0a 2020 2020 2320 2754 3033 3827 2c20  n.    # 'T038', 
-000006a0: 2320 4269 6f6c 6f67 6963 2046 756e 6374  # Biologic Funct
-000006b0: 696f 6e2c 2065 782e 3a20 416e 7469 626f  ion, ex.: Antibo
-000006c0: 6479 2046 6f72 6d61 7469 6f6e 3b20 4472  dy Formation; Dr
-000006d0: 7567 2072 6573 6973 7461 6e63 653b 2048  ug resistance; H
-000006e0: 6f6d 656f 7374 6173 6973 0a20 2020 2023  omeostasis.    #
-000006f0: 2027 5431 3233 272c 2023 2042 696f 6c6f   'T123', # Biolo
-00000700: 6769 6361 6c6c 7920 4163 7469 7665 2053  gically Active S
-00000710: 7562 7374 616e 6365 2c20 6578 2e3a 2043  ubstance, ex.: C
-00000720: 7974 6f6b 696e 696e 733b 2050 6865 726f  ytokinins; Phero
-00000730: 6d6f 6e65 0a20 2020 2023 2027 5430 3931  mone.    # 'T091
-00000740: 272c 2023 2042 696f 6d65 6469 6361 6c20  ', # Biomedical 
-00000750: 4f63 6375 7061 7469 6f6e 206f 7220 4469  Occupation or Di
-00000760: 7363 6970 6c69 6e65 2c20 6578 2e3a 2041  scipline, ex.: A
-00000770: 646f 6c65 7363 656e 7420 4d65 6469 6369  dolescent Medici
-00000780: 6e65 3b20 4365 6c6c 756c 6172 204e 6575  ne; Cellular Neu
-00000790: 726f 6269 6f6c 6f67 793b 2044 656e 7469  robiology; Denti
-000007a0: 7374 7279 0a20 2020 2023 2027 5431 3232  stry.    # 'T122
-000007b0: 272c 2023 2042 696f 6d65 6469 6361 6c20  ', # Biomedical 
-000007c0: 6f72 2044 656e 7461 6c20 4d61 7465 7269  or Dental Materi
-000007d0: 616c 2c20 6578 2e3a 2041 6372 796c 6963  al, ex.: Acrylic
-000007e0: 2052 6573 696e 733b 2042 6f6e 6520 4365   Resins; Bone Ce
-000007f0: 6d65 6e74 733b 2044 656e 7469 6672 6963  ments; Dentifric
-00000800: 6573 0a20 2020 2023 2027 5430 3132 272c  es.    # 'T012',
-00000810: 2023 2042 6972 642c 2065 782e 3a20 5365   # Bird, ex.: Se
-00000820: 7269 6e75 733b 2044 7563 6b73 3b20 5175  rinus; Ducks; Qu
-00000830: 6169 6c0a 2020 2020 2754 3032 3927 2c20  ail.    'T029', 
-00000840: 2320 426f 6479 204c 6f63 6174 696f 6e20  # Body Location 
-00000850: 6f72 2052 6567 696f 6e2c 2065 782e 3a20  or Region, ex.: 
-00000860: 466f 7265 6865 6164 3b20 5375 626c 696e  Forehead; Sublin
-00000870: 6775 616c 2052 6567 696f 6e3b 2042 6173  gual Region; Bas
-00000880: 6520 6f66 2073 6b75 6c6c 2073 7472 7563  e of skull struc
-00000890: 7475 7265 0a20 2020 2027 5430 3233 272c  ture.    'T023',
-000008a0: 2023 2042 6f64 7920 5061 7274 2c20 4f72   # Body Part, Or
-000008b0: 6761 6e2c 206f 7220 4f72 6761 6e20 436f  gan, or Organ Co
-000008c0: 6d70 6f6e 656e 742c 2065 782e 3a20 416f  mponent, ex.: Ao
-000008d0: 7274 613b 2042 7261 696e 2053 7465 6d3b  rta; Brain Stem;
-000008e0: 2053 7472 7563 7475 7265 206f 6620 6e65   Structure of ne
-000008f0: 636b 206f 6620 6665 6d75 720a 2020 2020  ck of femur.    
-00000900: 2320 2754 3033 3027 2c20 2320 426f 6479  # 'T030', # Body
-00000910: 2053 7061 6365 206f 7220 4a75 6e63 7469   Space or Juncti
-00000920: 6f6e 2c20 6578 2e3a 204b 6e65 6520 6a6f  on, ex.: Knee jo
-00000930: 696e 743b 2047 7265 6174 6572 2073 6163  int; Greater sac
-00000940: 206f 6620 7065 7269 746f 6e65 756d 3b20   of peritoneum; 
-00000950: 5379 6e61 7073 6573 0a20 2020 2027 5430  Synapses.    'T0
-00000960: 3331 272c 2023 2042 6f64 7920 5375 6273  31', # Body Subs
-00000970: 7461 6e63 652c 2065 782e 3a20 416d 6e69  tance, ex.: Amni
-00000980: 6f74 6963 2046 6c75 6964 3b20 7361 6c69  otic Fluid; sali
-00000990: 7661 3b20 536d 6567 6d61 0a20 2020 2023  va; Smegma.    #
-000009a0: 2027 5430 3232 272c 2023 2042 6f64 7920   'T022', # Body 
-000009b0: 5379 7374 656d 2c20 6578 2e3a 2045 6e64  System, ex.: End
-000009c0: 6f63 7269 6e65 2073 7973 7465 6d3b 2052  ocrine system; R
-000009d0: 656e 696e 2d61 6e67 696f 7465 6e73 696e  enin-angiotensin
-000009e0: 2073 7973 7465 6d3b 2052 6574 6963 756c   system; Reticul
-000009f0: 6f65 6e64 6f74 6865 6c69 616c 2053 7973  oendothelial Sys
-00000a00: 7465 6d0a 2020 2020 2320 2754 3038 3827  tem.    # 'T088'
-00000a10: 2c20 2320 4361 7262 6f68 7964 7261 7465  , # Carbohydrate
-00000a20: 2053 6571 7565 6e63 652c 2065 782e 3a20   Sequence, ex.: 
-00000a30: 4361 7262 6f68 7964 7261 7465 2053 6571  Carbohydrate Seq
-00000a40: 7565 6e63 653b 2041 626e 6f72 6d61 6c20  uence; Abnormal 
-00000a50: 6361 7262 6f68 7964 7261 7465 2073 6571  carbohydrate seq
-00000a60: 7565 6e63 650a 2020 2020 2320 2754 3032  uence.    # 'T02
-00000a70: 3527 2c20 2320 4365 6c6c 2c20 6578 2e3a  5', # Cell, ex.:
-00000a80: 2042 2d4c 796d 7068 6f63 7974 6573 3b20   B-Lymphocytes; 
-00000a90: 4465 6e64 7269 7469 6320 4365 6c6c 733b  Dendritic Cells;
-00000aa0: 2046 6962 726f 626c 6173 7473 0a20 2020   Fibroblasts.   
-00000ab0: 2023 2027 5430 3236 272c 2023 2043 656c   # 'T026', # Cel
-00000ac0: 6c20 436f 6d70 6f6e 656e 742c 2065 782e  l Component, ex.
-00000ad0: 3a20 4178 6f6e 3b20 476f 6c67 6920 4170  : Axon; Golgi Ap
-00000ae0: 7061 7261 7475 733b 204f 7267 616e 656c  paratus; Organel
-00000af0: 6c65 730a 2020 2020 2320 2754 3034 3327  les.    # 'T043'
-00000b00: 2c20 2320 4365 6c6c 2046 756e 6374 696f  , # Cell Functio
-00000b10: 6e2c 2065 782e 3a20 4365 6c6c 2043 7963  n, ex.: Cell Cyc
-00000b20: 6c65 3b20 4365 6c6c 2064 6976 6973 696f  le; Cell divisio
-00000b30: 6e3b 2050 6861 676f 6379 746f 7369 730a  n; Phagocytosis.
-00000b40: 2020 2020 2320 2754 3034 3927 2c20 2320      # 'T049', # 
-00000b50: 4365 6c6c 206f 7220 4d6f 6c65 6375 6c61  Cell or Molecula
-00000b60: 7220 4479 7366 756e 6374 696f 6e2c 2065  r Dysfunction, e
-00000b70: 782e 3a20 444e 4120 4461 6d61 6765 3b20  x.: DNA Damage; 
-00000b80: 5761 6c6c 6572 6961 6e20 4465 6765 6e65  Wallerian Degene
-00000b90: 7261 7469 6f6e 3b20 4174 7970 6963 616c  ration; Atypical
-00000ba0: 2073 7175 616d 6f75 7320 6d65 7461 706c   squamous metapl
-00000bb0: 6173 6961 0a20 2020 2023 2027 5431 3033  asia.    # 'T103
-00000bc0: 272c 2023 2043 6865 6d69 6361 6c2c 2065  ', # Chemical, e
-00000bd0: 782e 3a20 4163 6964 733b 2043 6865 6d69  x.: Acids; Chemi
-00000be0: 6361 6c73 3b20 496f 6e69 6320 4c69 7175  cals; Ionic Liqu
-00000bf0: 6964 730a 2020 2020 2320 2754 3132 3027  ids.    # 'T120'
-00000c00: 2c20 2320 4368 656d 6963 616c 2056 6965  , # Chemical Vie
-00000c10: 7765 6420 4675 6e63 7469 6f6e 616c 6c79  wed Functionally
-00000c20: 2c20 6578 2e3a 2041 6572 6f73 6f6c 2050  , ex.: Aerosol P
-00000c30: 726f 7065 6c6c 616e 7473 3b20 4465 7465  ropellants; Dete
-00000c40: 7267 656e 7473 3b20 5374 6162 696c 697a  rgents; Stabiliz
-00000c50: 696e 6720 4167 656e 7473 0a20 2020 2023  ing Agents.    #
-00000c60: 2027 5431 3034 272c 2023 2043 6865 6d69   'T104', # Chemi
-00000c70: 6361 6c20 5669 6577 6564 2053 7472 7563  cal Viewed Struc
-00000c80: 7475 7261 6c6c 792c 2065 782e 3a20 416d  turally, ex.: Am
-00000c90: 6d6f 6e69 756d 2043 6f6d 706f 756e 6473  monium Compounds
-00000ca0: 3b20 4361 7469 6f6e 733b 2053 756c 6675  ; Cations; Sulfu
-00000cb0: 7220 436f 6d70 6f75 6e64 730a 2020 2020  r Compounds.    
-00000cc0: 2320 2754 3138 3527 2c20 2320 436c 6173  # 'T185', # Clas
-00000cd0: 7369 6669 6361 7469 6f6e 2c20 6578 2e3a  sification, ex.:
-00000ce0: 2041 6e61 746f 6d79 2028 4d65 5348 2043   Anatomy (MeSH C
-00000cf0: 6174 6567 6f72 7929 3b20 5475 6d6f 7220  ategory); Tumor 
-00000d00: 5374 6167 6520 436c 6173 7369 6669 6361  Stage Classifica
-00000d10: 7469 6f6e 3b20 6178 6973 2069 0a20 2020  tion; axis i.   
-00000d20: 2027 5432 3031 272c 2023 2043 6c69 6e69   'T201', # Clini
-00000d30: 6361 6c20 4174 7472 6962 7574 652c 2065  cal Attribute, e
-00000d40: 782e 3a20 426f 6e65 2044 656e 7369 7479  x.: Bone Density
-00000d50: 3b20 6865 6172 7420 7261 7465 3b20 5261  ; heart rate; Ra
-00000d60: 6e67 6520 6f66 204d 6f74 696f 6e2c 2041  nge of Motion, A
-00000d70: 7274 6963 756c 6172 0a20 2020 2027 5432  rticular.    'T2
-00000d80: 3030 272c 2023 2043 6c69 6e69 6361 6c20  00', # Clinical 
-00000d90: 4472 7567 2c20 6578 2e3a 2052 616e 6974  Drug, ex.: Ranit
-00000da0: 6964 696e 6520 3330 3020 4d47 204f 7261  idine 300 MG Ora
-00000db0: 6c20 5461 626c 6574 205b 5a61 6e74 6163  l Tablet [Zantac
-00000dc0: 5d3b 2041 7370 6972 696e 2033 3030 204d  ]; Aspirin 300 M
-00000dd0: 4720 4465 6c61 7965 6420 5265 6c65 6173  G Delayed Releas
-00000de0: 6520 4f72 616c 0a20 2020 2023 2027 5430  e Oral.    # 'T0
-00000df0: 3737 272c 2023 2043 6f6e 6365 7074 7561  77', # Conceptua
-00000e00: 6c20 456e 7469 7479 2c20 6578 2e3a 2047  l Entity, ex.: G
-00000e10: 656f 6772 6170 6869 6320 4661 6374 6f72  eographic Factor
-00000e20: 733b 2046 7261 6374 616c 733b 2053 6563  s; Fractals; Sec
-00000e30: 756c 6172 6973 6d0a 2020 2020 2320 2754  ularism.    # 'T
-00000e40: 3031 3927 2c20 2320 436f 6e67 656e 6974  019', # Congenit
-00000e50: 616c 2041 626e 6f72 6d61 6c69 7479 2c20  al Abnormality, 
-00000e60: 6578 2e3a 2041 6c62 696e 6973 6d3b 2043  ex.: Albinism; C
-00000e70: 6c65 6674 2070 616c 6174 6520 7769 7468  left palate with
-00000e80: 2063 6c65 6674 206c 6970 3b20 506f 6c79   cleft lip; Poly
-00000e90: 6461 6374 796c 7920 6f66 2074 6f65 730a  dactyly of toes.
-00000ea0: 2020 2020 2320 2754 3035 3627 2c20 2320      # 'T056', # 
-00000eb0: 4461 696c 7920 6f72 2052 6563 7265 6174  Daily or Recreat
-00000ec0: 696f 6e61 6c20 4163 7469 7669 7479 2c20  ional Activity, 
-00000ed0: 6578 2e3a 2042 6164 6d69 6e74 6f6e 3b20  ex.: Badminton; 
-00000ee0: 4461 6e63 696e 673b 2053 7769 6d6d 696e  Dancing; Swimmin
-00000ef0: 670a 2020 2020 2754 3036 3027 2c20 2320  g.    'T060', # 
-00000f00: 4469 6167 6e6f 7374 6963 2050 726f 6365  Diagnostic Proce
-00000f10: 6475 7265 2c20 6578 2e3a 2042 696f 7073  dure, ex.: Biops
-00000f20: 793b 2048 6561 7274 2041 7573 6375 6c74  y; Heart Auscult
-00000f30: 6174 696f 6e3b 204d 6167 6e65 7469 6320  ation; Magnetic 
-00000f40: 5265 736f 6e61 6e63 6520 496d 6167 696e  Resonance Imagin
-00000f50: 670a 2020 2020 2754 3034 3727 2c20 2320  g.    'T047', # 
-00000f60: 4469 7365 6173 6520 6f72 2053 796e 6472  Disease or Syndr
-00000f70: 6f6d 652c 2065 782e 3a20 4469 6162 6574  ome, ex.: Diabet
-00000f80: 6573 204d 656c 6c69 7475 733b 2044 7275  es Mellitus; Dru
-00000f90: 6720 416c 6c65 7267 793b 204d 616c 6162  g Allergy; Malab
-00000fa0: 736f 7270 7469 6f6e 2053 796e 6472 6f6d  sorption Syndrom
-00000fb0: 650a 2020 2020 2754 3230 3327 2c20 2320  e.    'T203', # 
-00000fc0: 4472 7567 2044 656c 6976 6572 7920 4465  Drug Delivery De
-00000fd0: 7669 6365 2c20 6578 2e3a 204e 6f72 6465  vice, ex.: Norde
-00000fe0: 7474 6520 3231 2044 6179 2050 6163 6b3b  tte 21 Day Pack;
-00000ff0: 207b 3720 2854 6572 617a 6f73 696e 2031   {7 (Terazosin 1
-00001000: 204d 4720 4f72 616c 2054 6162 6c65 7429   MG Oral Tablet)
-00001010: 202f 2037 2028 5465 7261 7a6f 7369 6e20   / 7 (Terazosin 
-00001020: 3220 4d47 0a20 2020 2023 2027 5430 3635  2 MG.    # 'T065
-00001030: 272c 2023 2045 6475 6361 7469 6f6e 616c  ', # Educational
-00001040: 2041 6374 6976 6974 792c 2065 782e 3a20   Activity, ex.: 
-00001050: 4163 6164 656d 6963 2054 7261 696e 696e  Academic Trainin
-00001060: 673b 2046 616d 696c 7920 506c 616e 6e69  g; Family Planni
-00001070: 6e67 2054 7261 696e 696e 673b 2050 7265  ng Training; Pre
-00001080: 6365 7074 6f72 7368 6970 0a20 2020 2023  ceptorship.    #
-00001090: 2027 5431 3936 272c 2023 2045 6c65 6d65   'T196', # Eleme
-000010a0: 6e74 2c20 496f 6e2c 206f 7220 4973 6f74  nt, Ion, or Isot
-000010b0: 6f70 652c 2065 782e 3a20 4361 7262 6f6e  ope, ex.: Carbon
-000010c0: 3b20 4368 726f 6d69 756d 2049 736f 746f  ; Chromium Isoto
-000010d0: 7065 733b 2052 6164 696f 6973 6f74 6f70  pes; Radioisotop
-000010e0: 6573 0a20 2020 2023 2027 5430 3138 272c  es.    # 'T018',
-000010f0: 2023 2045 6d62 7279 6f6e 6963 2053 7472   # Embryonic Str
-00001100: 7563 7475 7265 2c20 6578 2e3a 2042 6c61  ucture, ex.: Bla
-00001110: 7374 6f64 6572 6d3b 2046 6574 7573 3b20  stoderm; Fetus; 
-00001120: 4e65 7572 616c 2043 7265 7374 0a20 2020  Neural Crest.   
-00001130: 2023 2027 5430 3731 272c 2023 2045 6e74   # 'T071', # Ent
-00001140: 6974 792c 2065 782e 3a20 4769 6674 732c  ity, ex.: Gifts,
-00001150: 2046 696e 616e 6369 616c 3b20 496d 6167   Financial; Imag
-00001160: 653b 2050 726f 6475 6374 2050 6172 740a  e; Product Part.
-00001170: 2020 2020 2320 2754 3036 3927 2c20 2320      # 'T069', # 
-00001180: 456e 7669 726f 6e6d 656e 7461 6c20 4566  Environmental Ef
-00001190: 6665 6374 206f 6620 4875 6d61 6e73 2c20  fect of Humans, 
-000011a0: 6578 2e3a 2041 6972 2050 6f6c 6c75 7469  ex.: Air Polluti
-000011b0: 6f6e 3b20 4465 7365 7274 6966 6963 6174  on; Desertificat
-000011c0: 696f 6e3b 2042 696f 7265 6d65 6469 6174  ion; Bioremediat
-000011d0: 696f 6e0a 2020 2020 2320 2754 3132 3627  ion.    # 'T126'
-000011e0: 2c20 2320 456e 7a79 6d65 2c20 6578 2e3a  , # Enzyme, ex.:
-000011f0: 2047 5450 2043 7963 6c6f 6879 6472 6f6c   GTP Cyclohydrol
-00001200: 6173 6520 4949 3b20 656e 7a79 6d65 2073  ase II; enzyme s
-00001210: 7562 7374 7261 7465 2063 6f6d 706c 6578  ubstrate complex
-00001220: 3b20 6172 6769 6e69 6e65 2061 6d69 6461  ; arginine amida
-00001230: 7365 0a20 2020 2023 2027 5432 3034 272c  se.    # 'T204',
-00001240: 2023 2045 756b 6172 796f 7465 2c20 6578   # Eukaryote, ex
-00001250: 2e3a 204f 7264 6572 2041 6361 7269 6e61  .: Order Acarina
-00001260: 3b20 4265 6573 3b20 506c 6173 6d6f 6469  ; Bees; Plasmodi
-00001270: 756d 206d 616c 6172 6961 650a 2020 2020  um malariae.    
-00001280: 2320 2754 3035 3127 2c20 2320 4576 656e  # 'T051', # Even
-00001290: 742c 2065 782e 3a20 416e 6e69 7665 7273  t, ex.: Annivers
-000012a0: 6172 6965 733b 2045 7870 6f73 7572 6520  aries; Exposure 
-000012b0: 746f 204d 756d 7073 2076 6972 7573 2028  to Mumps virus (
-000012c0: 6576 656e 7429 3b20 4465 7669 6365 2055  event); Device U
-000012d0: 6e61 7474 656e 6465 640a 2020 2020 2320  nattended.    # 
-000012e0: 2754 3035 3027 2c20 2320 4578 7065 7269  'T050', # Experi
-000012f0: 6d65 6e74 616c 204d 6f64 656c 206f 6620  mental Model of 
-00001300: 4469 7365 6173 652c 2065 782e 3a20 416c  Disease, ex.: Al
-00001310: 6c6f 7861 6e20 4469 6162 6574 6573 3b20  loxan Diabetes; 
-00001320: 4c69 7665 7220 4369 7272 686f 7369 732c  Liver Cirrhosis,
-00001330: 2045 7870 6572 696d 656e 7461 6c3b 2054   Experimental; T
-00001340: 7261 6e73 6965 6e74 2047 656e 6520 4b6e  ransient Gene Kn
-00001350: 6f63 6b2d 4f75 740a 2020 2020 2320 2754  ock-Out.    # 'T
-00001360: 3039 3927 2c20 2320 4661 6d69 6c79 2047  099', # Family G
-00001370: 726f 7570 2c20 6578 2e3a 2044 6175 6768  roup, ex.: Daugh
-00001380: 7465 723b 2049 7320 616e 206f 6e6c 7920  ter; Is an only 
-00001390: 6368 696c 643b 2055 6e6d 6172 7269 6564  child; Unmarried
-000013a0: 2046 6174 6865 7273 0a20 2020 2027 5430   Fathers.    'T0
-000013b0: 3333 272c 2023 2046 696e 6469 6e67 2c20  33', # Finding, 
-000013c0: 6578 2e3a 2042 6972 7468 2048 6973 746f  ex.: Birth Histo
-000013d0: 7279 3b20 446f 776e 7761 7264 2064 6973  ry; Downward dis
-000013e0: 706c 6163 656d 656e 7420 6f66 2064 6961  placement of dia
-000013f0: 7068 7261 676d 3b20 4465 6372 6561 7365  phragm; Decrease
-00001400: 6420 676c 7563 6f73 6520 6c65 7665 6c0a  d glucose level.
-00001410: 2020 2020 2320 2754 3031 3327 2c20 2320      # 'T013', # 
-00001420: 4669 7368 2c20 6578 2e3a 2042 6173 733b  Fish, ex.: Bass;
-00001430: 2053 616c 6d6f 6e69 6461 653b 2057 6869   Salmonidae; Whi
-00001440: 7465 6669 7368 0a20 2020 2023 2027 5431  tefish.    # 'T1
-00001450: 3638 272c 2023 2046 6f6f 642c 2065 782e  68', # Food, ex.
-00001460: 3a20 4265 7665 7261 6765 733b 2045 6767  : Beverages; Egg
-00001470: 2059 6f6c 6b20 2844 6965 7461 7279 293b   Yolk (Dietary);
-00001480: 2049 6365 2043 7265 616d 0a20 2020 2023   Ice Cream.    #
-00001490: 2027 5430 3231 272c 2023 2046 756c 6c79   'T021', # Fully
-000014a0: 2046 6f72 6d65 6420 416e 6174 6f6d 6963   Formed Anatomic
-000014b0: 616c 2053 7472 7563 7475 7265 2c20 6578  al Structure, ex
-000014c0: 2e3a 2045 6e74 6972 6520 626f 6479 2061  .: Entire body a
-000014d0: 7320 6120 7768 6f6c 653b 2046 656d 616c  s a whole; Femal
-000014e0: 6520 6875 6d61 6e20 626f 6479 3b20 5365  e human body; Se
-000014f0: 7420 6f66 2070 6172 7473 206f 6620 6875  t of parts of hu
-00001500: 6d61 6e20 626f 6479 0a20 2020 2023 2027  man body.    # '
-00001510: 5431 3639 272c 2023 2046 756e 6374 696f  T169', # Functio
-00001520: 6e61 6c20 436f 6e63 6570 742c 2065 782e  nal Concept, ex.
-00001530: 3a20 496e 7465 7276 6965 7765 7220 4566  : Interviewer Ef
-00001540: 6665 6374 3b20 5072 6f62 6c65 6d20 466f  fect; Problem Fo
-00001550: 726d 756c 6174 696f 6e3b 2045 6e64 6f67  rmulation; Endog
-00001560: 656e 6f75 730a 2020 2020 2320 2754 3030  enous.    # 'T00
-00001570: 3427 2c20 2320 4675 6e67 7573 2c20 6578  4', # Fungus, ex
-00001580: 2e3a 2041 7370 6572 6769 6c6c 7573 2063  .: Aspergillus c
-00001590: 6c61 7661 7475 733b 2042 6c61 7374 6f6d  lavatus; Blastom
-000015a0: 7963 6573 3b20 4e65 7572 6f73 706f 7261  yces; Neurospora
-000015b0: 0a20 2020 2023 2027 5430 3238 272c 2023  .    # 'T028', #
-000015c0: 2047 656e 6520 6f72 2047 656e 6f6d 652c   Gene or Genome,
-000015d0: 2065 782e 3a20 416c 6c65 6c65 733b 2047   ex.: Alleles; G
-000015e0: 656e 6f6d 652c 2048 756d 616e 3b20 7252  enome, Human; rR
-000015f0: 4e41 204f 7065 726f 6e0a 2020 2020 2320  NA Operon.    # 
-00001600: 2754 3034 3527 2c20 2320 4765 6e65 7469  'T045', # Geneti
-00001610: 6320 4675 6e63 7469 6f6e 2c20 6578 2e3a  c Function, ex.:
-00001620: 2045 6172 6c79 2047 656e 6520 5472 616e   Early Gene Tran
-00001630: 7363 7269 7074 696f 6e3b 2047 656e 6520  scription; Gene 
-00001640: 416d 706c 6966 6963 6174 696f 6e3b 2052  Amplification; R
-00001650: 4e41 2053 706c 6963 696e 670a 2020 2020  NA Splicing.    
-00001660: 2320 2754 3038 3327 2c20 2320 4765 6f67  # 'T083', # Geog
-00001670: 7261 7068 6963 2041 7265 612c 2065 782e  raphic Area, ex.
-00001680: 3a20 4261 6c74 696d 6f72 653b 2043 616e  : Baltimore; Can
-00001690: 6164 613b 2046 6172 2045 6173 740a 2020  ada; Far East.  
-000016a0: 2020 2320 2754 3036 3427 2c20 2320 476f    # 'T064', # Go
-000016b0: 7665 726e 6d65 6e74 616c 206f 7220 5265  vernmental or Re
-000016c0: 6775 6c61 746f 7279 2041 6374 6976 6974  gulatory Activit
-000016d0: 792c 2065 782e 3a20 4365 7274 6966 6963  y, ex.: Certific
-000016e0: 6174 696f 6e3b 2043 7265 6465 6e74 6961  ation; Credentia
-000016f0: 6c69 6e67 3b20 5075 626c 6963 2050 6f6c  ling; Public Pol
-00001700: 6963 790a 2020 2020 2320 2754 3039 3627  icy.    # 'T096'
-00001710: 2c20 2320 4772 6f75 702c 2065 782e 3a20  , # Group, ex.: 
-00001720: 466f 6375 7320 4772 6f75 7073 3b20 6a75  Focus Groups; ju
-00001730: 7279 3b20 7465 616d 730a 2020 2020 2320  ry; teams.    # 
-00001740: 2754 3130 3227 2c20 2320 4772 6f75 7020  'T102', # Group 
-00001750: 4174 7472 6962 7574 652c 2065 782e 3a20  Attribute, ex.: 
-00001760: 4661 6d69 6c79 2053 697a 653b 2047 726f  Family Size; Gro
-00001770: 7570 2053 7472 7563 7475 7265 3b20 4c69  up Structure; Li
-00001780: 6665 2045 7870 6563 7461 6e63 790a 2020  fe Expectancy.  
-00001790: 2020 2320 2754 3133 3127 2c20 2320 4861    # 'T131', # Ha
-000017a0: 7a61 7264 6f75 7320 6f72 2050 6f69 736f  zardous or Poiso
-000017b0: 6e6f 7573 2053 7562 7374 616e 6365 2c20  nous Substance, 
-000017c0: 6578 2e3a 2043 6172 6369 6e6f 6765 6e73  ex.: Carcinogens
-000017d0: 3b20 4675 6d69 6761 6e74 3b20 4d75 7461  ; Fumigant; Muta
-000017e0: 6765 6e73 0a20 2020 2027 5430 3538 272c  gens.    'T058',
-000017f0: 2023 2048 6561 6c74 6820 4361 7265 2041   # Health Care A
-00001800: 6374 6976 6974 792c 2065 782e 3a20 616d  ctivity, ex.: am
-00001810: 6275 6c61 746f 7279 2063 6172 6520 7365  bulatory care se
-00001820: 7276 6963 6573 3b20 436c 696e 6963 2041  rvices; Clinic A
-00001830: 6374 6976 6974 6965 733b 2050 7265 7665  ctivities; Preve
-00001840: 6e74 6976 6520 4865 616c 7468 2053 6572  ntive Health Ser
-00001850: 7669 6365 730a 2020 2020 2320 2754 3039  vices.    # 'T09
-00001860: 3327 2c20 2320 4865 616c 7468 2043 6172  3', # Health Car
-00001870: 6520 5265 6c61 7465 6420 4f72 6761 6e69  e Related Organi
-00001880: 7a61 7469 6f6e 2c20 6578 2e3a 2043 656e  zation, ex.: Cen
-00001890: 7465 7273 2066 6f72 2044 6973 6561 7365  ters for Disease
-000018a0: 2043 6f6e 7472 6f6c 2061 6e64 2050 7265   Control and Pre
-000018b0: 7665 6e74 696f 6e20 2855 2e53 2e29 3b20  vention (U.S.); 
-000018c0: 4861 6c66 7761 7920 486f 7573 6573 3b0a  Halfway Houses;.
-000018d0: 2020 2020 2320 2754 3132 3527 2c20 2320      # 'T125', # 
-000018e0: 486f 726d 6f6e 652c 2065 782e 3a20 456e  Hormone, ex.: En
-000018f0: 7465 7269 6320 486f 726d 6f6e 6573 3b20  teric Hormones; 
-00001900: 7468 796d 6963 2068 756d 6f72 616c 2066  thymic humoral f
-00001910: 6163 746f 723b 2050 726f 686f 726d 6f6e  actor; Prohormon
-00001920: 650a 2020 2020 2320 2754 3031 3627 2c20  e.    # 'T016', 
-00001930: 2320 4875 6d61 6e2c 2065 782e 3a20 486f  # Human, ex.: Ho
-00001940: 6d6f 2073 6170 6965 6e73 3b20 6a65 616e  mo sapiens; jean
-00001950: 2070 6961 6765 743b 204d 656d 6265 7220   piaget; Member 
-00001960: 6f66 2070 7562 6c69 630a 2020 2020 2320  of public.    # 
-00001970: 2754 3036 3827 2c20 2320 4875 6d61 6e2d  'T068', # Human-
-00001980: 6361 7573 6564 2050 6865 6e6f 6d65 6e6f  caused Phenomeno
-00001990: 6e20 6f72 2050 726f 6365 7373 2c20 6578  n or Process, ex
-000019a0: 2e3a 2042 6162 7920 426f 6f6d 3b20 4375  .: Baby Boom; Cu
-000019b0: 6c74 7572 616c 2045 766f 6c75 7469 6f6e  ltural Evolution
-000019c0: 3b20 4d61 7373 204d 6564 6961 0a20 2020  ; Mass Media.   
-000019d0: 2023 2027 5430 3738 272c 2023 2049 6465   # 'T078', # Ide
-000019e0: 6120 6f72 2043 6f6e 6365 7074 2c20 6578  a or Concept, ex
-000019f0: 2e3a 2043 6170 6974 616c 6973 6d3b 2043  .: Capitalism; C
-00001a00: 6976 696c 2052 6967 6874 733b 2045 7468  ivil Rights; Eth
-00001a10: 6963 730a 2020 2020 2320 2754 3132 3927  ics.    # 'T129'
-00001a20: 2c20 2320 496d 6d75 6e6f 6c6f 6769 6320  , # Immunologic 
-00001a30: 4661 6374 6f72 2c20 6578 2e3a 2041 6e74  Factor, ex.: Ant
-00001a40: 6967 656e 733b 2049 6d6d 756e 6f6c 6f67  igens; Immunolog
-00001a50: 6963 2046 6163 746f 7273 3b20 426c 6f6f  ic Factors; Bloo
-00001a60: 6420 6772 6f75 7020 616e 7469 6765 6e20  d group antigen 
-00001a70: 500a 2020 2020 2754 3133 3027 2c20 2320  P.    'T130', # 
-00001a80: 496e 6469 6361 746f 722c 2052 6561 6765  Indicator, Reage
-00001a90: 6e74 2c20 6f72 2044 6961 676e 6f73 7469  nt, or Diagnosti
-00001aa0: 6320 4169 642c 2065 782e 3a20 466c 756f  c Aid, ex.: Fluo
-00001ab0: 7265 7363 656e 7420 4479 6573 3b20 496e  rescent Dyes; In
-00001ac0: 6469 6361 746f 7273 2061 6e64 2052 6561  dicators and Rea
-00001ad0: 6765 6e74 733b 2049 6e64 6961 2069 6e6b  gents; India ink
-00001ae0: 2073 7461 696e 0a20 2020 2023 2027 5430   stain.    # 'T0
-00001af0: 3535 272c 2023 2049 6e64 6976 6964 7561  55', # Individua
-00001b00: 6c20 4265 6861 7669 6f72 2c20 6578 2e3a  l Behavior, ex.:
-00001b10: 2041 7373 6572 7469 7665 6e65 7373 3b20   Assertiveness; 
-00001b20: 4772 6f6f 6d69 6e67 3b20 5269 736b 2d54  Grooming; Risk-T
-00001b30: 616b 696e 670a 2020 2020 2754 3033 3727  aking.    'T037'
-00001b40: 2c20 2320 496e 6a75 7279 206f 7220 506f  , # Injury or Po
-00001b50: 6973 6f6e 696e 672c 2065 782e 3a20 4163  isoning, ex.: Ac
-00001b60: 6369 6465 6e74 616c 2046 616c 6c73 3b20  cidental Falls; 
-00001b70: 4361 7262 6f6e 204d 6f6e 6f78 6964 6520  Carbon Monoxide 
-00001b80: 506f 6973 6f6e 696e 673b 2053 6e61 6b65  Poisoning; Snake
-00001b90: 2042 6974 6573 0a20 2020 2023 2027 5431   Bites.    # 'T1
-00001ba0: 3937 272c 2023 2049 6e6f 7267 616e 6963  97', # Inorganic
-00001bb0: 2043 6865 6d69 6361 6c2c 2065 782e 3a20   Chemical, ex.: 
-00001bc0: 4361 7262 6f6e 6963 2041 6369 643b 2061  Carbonic Acid; a
-00001bd0: 6c75 6d69 6e75 6d20 6e69 7472 6964 653b  luminum nitride;
-00001be0: 2066 6572 7269 6320 6369 7472 6174 650a   ferric citrate.
-00001bf0: 2020 2020 2754 3137 3027 2c20 2320 496e      'T170', # In
-00001c00: 7465 6c6c 6563 7475 616c 2050 726f 6475  tellectual Produ
-00001c10: 6374 2c20 6578 2e3a 2044 6563 6973 696f  ct, ex.: Decisio
-00001c20: 6e20 5375 7070 6f72 7420 5465 6368 6e69  n Support Techni
-00001c30: 7175 6573 3b20 496e 666f 726d 6174 696f  ques; Informatio
-00001c40: 6e20 5379 7374 656d 733b 204c 6974 6572  n Systems; Liter
-00001c50: 6174 7572 650a 2020 2020 2754 3033 3427  ature.    'T034'
-00001c60: 2c20 2320 4c61 626f 7261 746f 7279 206f  , # Laboratory o
-00001c70: 7220 5465 7374 2052 6573 756c 742c 2065  r Test Result, e
-00001c80: 782e 3a20 426c 6f6f 6420 466c 6f77 2056  x.: Blood Flow V
-00001c90: 656c 6f63 6974 793b 2053 6572 756d 2043  elocity; Serum C
-00001ca0: 616c 6369 756d 204c 6576 656c 3b20 5370  alcium Level; Sp
-00001cb0: 696e 616c 2046 6c75 6964 2050 7265 7373  inal Fluid Press
-00001cc0: 7572 650a 2020 2020 2754 3035 3927 2c20  ure.    'T059', 
-00001cd0: 2320 4c61 626f 7261 746f 7279 2050 726f  # Laboratory Pro
-00001ce0: 6365 6475 7265 2c20 6578 2e3a 2042 6c6f  cedure, ex.: Blo
-00001cf0: 6f64 2050 726f 7465 696e 2045 6c65 6374  od Protein Elect
-00001d00: 726f 7068 6f72 6573 6973 3b20 4372 7973  rophoresis; Crys
-00001d10: 7461 6c6c 6f67 7261 7068 793b 2052 6164  tallography; Rad
-00001d20: 696f 696d 6d75 6e6f 6173 7361 790a 2020  ioimmunoassay.  
-00001d30: 2020 2320 2754 3137 3127 2c20 2320 4c61    # 'T171', # La
-00001d40: 6e67 7561 6765 2c20 6578 2e3a 2041 726d  nguage, ex.: Arm
-00001d50: 656e 6961 6e20 6c61 6e67 7561 6765 3b20  enian language; 
-00001d60: 6272 6169 6c6c 653b 2042 696c 696e 6775  braille; Bilingu
-00001d70: 616c 6973 6d0a 2020 2020 2320 2754 3036  alism.    # 'T06
-00001d80: 3627 2c20 2320 4d61 6368 696e 6520 4163  6', # Machine Ac
-00001d90: 7469 7669 7479 2c20 6578 2e3a 2043 6f6d  tivity, ex.: Com
-00001da0: 7075 7465 7220 5369 6d75 6c61 7469 6f6e  puter Simulation
-00001db0: 3b20 4571 7569 706d 656e 7420 4661 696c  ; Equipment Fail
-00001dc0: 7572 653b 204e 6174 7572 616c 204c 616e  ure; Natural Lan
-00001dd0: 6775 6167 6520 5072 6f63 6573 7369 6e67  guage Processing
-00001de0: 0a20 2020 2023 2027 5430 3135 272c 2023  .    # 'T015', #
-00001df0: 204d 616d 6d61 6c2c 2065 782e 3a20 5572   Mammal, ex.: Ur
-00001e00: 7369 6461 6520 4661 6d69 6c79 3b20 4861  sidae Family; Ha
-00001e10: 6d73 7465 7273 3b20 4d61 6361 6361 0a20  msters; Macaca. 
-00001e20: 2020 2023 2027 5430 3733 272c 2023 204d     # 'T073', # M
-00001e30: 616e 7566 6163 7475 7265 6420 4f62 6a65  anufactured Obje
-00001e40: 6374 2c20 6578 2e3a 2063 6172 2073 6561  ct, ex.: car sea
-00001e50: 743b 2043 6f6f 6b69 6e67 2061 6e64 2045  t; Cooking and E
-00001e60: 6174 696e 6720 5574 656e 7369 6c73 3b20  ating Utensils; 
-00001e70: 476f 6767 6c65 730a 2020 2020 2754 3037  Goggles.    'T07
-00001e80: 3427 2c20 2320 4d65 6469 6361 6c20 4465  4', # Medical De
-00001e90: 7669 6365 2c20 6578 2e3a 2042 6f6e 6520  vice, ex.: Bone 
-00001ea0: 5363 7265 7773 3b20 4865 6164 6765 6172  Screws; Headgear
-00001eb0: 2c20 4f72 7468 6f64 6f6e 7469 633b 2043  , Orthodontic; C
-00001ec0: 6f6d 7072 6573 7369 6f6e 2053 746f 636b  ompression Stock
-00001ed0: 696e 6773 0a20 2020 2027 5430 3438 272c  ings.    'T048',
-00001ee0: 2023 204d 656e 7461 6c20 6f72 2042 6568   # Mental or Beh
-00001ef0: 6176 696f 7261 6c20 4479 7366 756e 6374  avioral Dysfunct
-00001f00: 696f 6e2c 2065 782e 3a20 4167 6f72 6170  ion, ex.: Agorap
-00001f10: 686f 6269 613b 2043 7963 6c6f 7468 796d  hobia; Cyclothym
-00001f20: 6963 2044 6973 6f72 6465 723b 2046 7269  ic Disorder; Fri
-00001f30: 6769 6469 7479 0a20 2020 2027 5430 3431  gidity.    'T041
-00001f40: 272c 2023 204d 656e 7461 6c20 5072 6f63  ', # Mental Proc
-00001f50: 6573 732c 2065 782e 3a20 416e 6765 723b  ess, ex.: Anger;
-00001f60: 2041 7564 6974 6f72 7920 4661 7469 6775   Auditory Fatigu
-00001f70: 653b 2041 766f 6964 616e 6365 204c 6561  e; Avoidance Lea
-00001f80: 726e 696e 670a 2020 2020 2320 2754 3036  rning.    # 'T06
-00001f90: 3327 2c20 2320 4d6f 6c65 6375 6c61 7220  3', # Molecular 
-00001fa0: 4269 6f6c 6f67 7920 5265 7365 6172 6368  Biology Research
-00001fb0: 2054 6563 686e 6971 7565 2c20 6578 2e3a   Technique, ex.:
-00001fc0: 204e 6f72 7468 6572 6e20 426c 6f74 7469   Northern Blotti
-00001fd0: 6e67 3b20 4765 6e65 7469 6320 456e 6769  ng; Genetic Engi
-00001fe0: 6e65 6572 696e 673b 2049 6e20 5369 7475  neering; In Situ
-00001ff0: 2048 7962 7269 6469 7a61 7469 6f6e 0a20   Hybridization. 
-00002000: 2020 2023 2027 5430 3434 272c 2023 204d     # 'T044', # M
-00002010: 6f6c 6563 756c 6172 2046 756e 6374 696f  olecular Functio
-00002020: 6e2c 2065 782e 3a20 4269 6e64 696e 672c  n, ex.: Binding,
-00002030: 2043 6f6d 7065 7469 7469 7665 3b20 456c   Competitive; El
-00002040: 6563 7472 6f6e 2054 7261 6e73 706f 7274  ectron Transport
-00002050: 3b20 476c 7963 6f6c 7973 6973 0a20 2020  ; Glycolysis.   
-00002060: 2023 2027 5430 3835 272c 2023 204d 6f6c   # 'T085', # Mol
-00002070: 6563 756c 6172 2053 6571 7565 6e63 652c  ecular Sequence,
-00002080: 2065 782e 3a20 4765 6e65 7469 6320 436f   ex.: Genetic Co
-00002090: 6465 3b20 486f 6d6f 6c6f 676f 7573 2053  de; Homologous S
-000020a0: 6571 7565 6e63 6573 3b20 4d6f 6c65 6375  equences; Molecu
-000020b0: 6c61 7220 5365 7175 656e 6365 0a20 2020  lar Sequence.   
-000020c0: 2023 2027 5430 3730 272c 2023 204e 6174   # 'T070', # Nat
-000020d0: 7572 616c 2050 6865 6e6f 6d65 6e6f 6e20  ural Phenomenon 
-000020e0: 6f72 2050 726f 6365 7373 2c20 6578 2e3a  or Process, ex.:
-000020f0: 2041 6972 204d 6f76 656d 656e 7473 3b20   Air Movements; 
-00002100: 436f 7272 6f73 696f 6e3b 204c 6967 6874  Corrosion; Light
-00002110: 6e69 6e67 2028 7068 656e 6f6d 656e 6f6e  ning (phenomenon
-00002120: 290a 2020 2020 2754 3139 3127 2c20 2320  ).    'T191', # 
-00002130: 4e65 6f70 6c61 7374 6963 2050 726f 6365  Neoplastic Proce
-00002140: 7373 2c20 6578 2e3a 2041 6264 6f6d 696e  ss, ex.: Abdomin
-00002150: 616c 204e 656f 706c 6173 6d73 3b20 426f  al Neoplasms; Bo
-00002160: 7765 6e27 7320 4469 7365 6173 653b 2050  wen's Disease; P
-00002170: 6f6c 7970 2069 6e20 6e61 736f 7068 6172  olyp in nasophar
-00002180: 796e 780a 2020 2020 2320 2754 3131 3427  ynx.    # 'T114'
-00002190: 2c20 2320 4e75 636c 6569 6320 4163 6964  , # Nucleic Acid
-000021a0: 2c20 4e75 636c 656f 7369 6465 2c20 6f72  , Nucleoside, or
-000021b0: 204e 7563 6c65 6f74 6964 652c 2065 782e   Nucleotide, ex.
-000021c0: 3a20 4379 746f 7369 6e65 204e 7563 6c65  : Cytosine Nucle
-000021d0: 6f74 6964 6573 3b20 4775 616e 696e 653b  otides; Guanine;
-000021e0: 204f 6c69 676f 6e75 636c 656f 7469 6465   Oligonucleotide
-000021f0: 730a 2020 2020 2320 2754 3038 3627 2c20  s.    # 'T086', 
-00002200: 2320 4e75 636c 656f 7469 6465 2053 6571  # Nucleotide Seq
-00002210: 7565 6e63 652c 2065 782e 3a20 4261 7365  uence, ex.: Base
-00002220: 2053 6571 7565 6e63 653b 2044 6972 6563   Sequence; Direc
-00002230: 7420 5265 7065 6174 3b20 524e 4120 5365  t Repeat; RNA Se
-00002240: 7175 656e 6365 0a20 2020 2023 2027 5430  quence.    # 'T0
-00002250: 3930 272c 2023 204f 6363 7570 6174 696f  90', # Occupatio
-00002260: 6e20 6f72 2044 6973 6369 706c 696e 652c  n or Discipline,
-00002270: 2065 782e 3a20 4176 6961 7469 6f6e 3b20   ex.: Aviation; 
-00002280: 4372 616e 696f 6c6f 6779 3b20 4563 6f6c  Craniology; Ecol
-00002290: 6f67 790a 2020 2020 2320 2754 3035 3727  ogy.    # 'T057'
-000022a0: 2c20 2320 4f63 6375 7061 7469 6f6e 616c  , # Occupational
-000022b0: 2041 6374 6976 6974 792c 2065 782e 3a20   Activity, ex.: 
-000022c0: 436f 6c6c 6563 7469 7665 2042 6172 6761  Collective Barga
-000022d0: 696e 696e 673b 2043 6f6d 6d65 7263 653b  ining; Commerce;
-000022e0: 2043 6f6e 7461 696e 6d65 6e74 206f 6620   Containment of 
-000022f0: 4269 6f68 617a 6172 6473 0a20 2020 2023  Biohazards.    #
-00002300: 2027 5430 3432 272c 2023 204f 7267 616e   'T042', # Organ
-00002310: 206f 7220 5469 7373 7565 2046 756e 6374   or Tissue Funct
-00002320: 696f 6e2c 2065 782e 3a20 4f73 7465 6f67  ion, ex.: Osteog
-00002330: 656e 6573 6973 3b20 5265 6e61 6c20 4369  enesis; Renal Ci
-00002340: 7263 756c 6174 696f 6e3b 2054 6f6f 7468  rculation; Tooth
-00002350: 2043 616c 6369 6669 6361 7469 6f6e 0a20   Calcification. 
-00002360: 2020 2023 2027 5431 3039 272c 2023 204f     # 'T109', # O
-00002370: 7267 616e 6963 2043 6865 6d69 6361 6c2c  rganic Chemical,
-00002380: 2065 782e 3a20 4265 6e7a 656e 6520 4465   ex.: Benzene De
-00002390: 7269 7661 7469 7665 730a 2020 2020 2320  rivatives.    # 
-000023a0: 2754 3030 3127 2c20 2320 4f72 6761 6e69  'T001', # Organi
-000023b0: 736d 2c20 6578 2e3a 204f 7267 616e 6973  sm, ex.: Organis
-000023c0: 6d3b 2049 6e66 6563 7469 6f75 7320 6167  m; Infectious ag
-000023d0: 656e 743b 2048 6574 6572 6f74 726f 7068  ent; Heterotroph
-000023e0: 0a20 2020 2023 2027 5430 3332 272c 2023  .    # 'T032', #
-000023f0: 204f 7267 616e 6973 6d20 4174 7472 6962   Organism Attrib
-00002400: 7574 652c 2065 782e 3a20 4167 653b 2042  ute, ex.: Age; B
-00002410: 6972 7468 2057 6569 6768 743b 2045 7965  irth Weight; Eye
-00002420: 2043 6f6c 6f72 0a20 2020 2027 5430 3430   Color.    'T040
-00002430: 272c 2023 204f 7267 616e 6973 6d20 4675  ', # Organism Fu
-00002440: 6e63 7469 6f6e 2c20 6578 2e3a 2042 7265  nction, ex.: Bre
-00002450: 6564 696e 673b 2048 6962 6572 6e61 7469  eding; Hibernati
-00002460: 6f6e 3b20 4d6f 746f 7220 536b 696c 6c73  on; Motor Skills
-00002470: 0a20 2020 2023 2027 5430 3932 272c 2023  .    # 'T092', #
-00002480: 204f 7267 616e 697a 6174 696f 6e2c 2065   Organization, e
-00002490: 782e 3a20 4c61 626f 7220 556e 696f 6e73  x.: Labor Unions
-000024a0: 3b20 556e 6974 6564 204e 6174 696f 6e73  ; United Nations
-000024b0: 3b20 426f 6172 6469 6e67 2073 6368 6f6f  ; Boarding schoo
-000024c0: 6c0a 2020 2020 2754 3034 3627 2c20 2320  l.    'T046', # 
-000024d0: 5061 7468 6f6c 6f67 6963 2046 756e 6374  Pathologic Funct
-000024e0: 696f 6e2c 2065 782e 3a20 496e 666c 616d  ion, ex.: Inflam
-000024f0: 6d61 7469 6f6e 3b20 5368 6f63 6b3b 2054  mation; Shock; T
-00002500: 6872 6f6d 626f 7369 730a 2020 2020 2320  hrombosis.    # 
-00002510: 2754 3130 3127 2c20 2320 5061 7469 656e  'T101', # Patien
-00002520: 7420 6f72 2044 6973 6162 6c65 6420 4772  t or Disabled Gr
-00002530: 6f75 702c 2065 782e 3a20 416d 7075 7465  oup, ex.: Ampute
-00002540: 6573 3b20 496e 7374 6974 7574 696f 6e61  es; Institutiona
-00002550: 6c69 7a65 6420 4368 696c 643b 204d 656e  lized Child; Men
-00002560: 7461 6c6c 7920 496c 6c20 5065 7273 6f6e  tally Ill Person
-00002570: 730a 2020 2020 2754 3132 3127 2c20 2320  s.    'T121', # 
-00002580: 5068 6172 6d61 636f 6c6f 6769 6320 5375  Pharmacologic Su
-00002590: 6273 7461 6e63 652c 2065 782e 3a20 416e  bstance, ex.: An
-000025a0: 7469 656d 6574 6963 733b 2043 6172 6469  tiemetics; Cardi
-000025b0: 6f76 6173 6375 6c61 7220 4167 656e 7473  ovascular Agents
-000025c0: 3b20 416c 6b61 2d53 656c 747a 6572 0a20  ; Alka-Seltzer. 
-000025d0: 2020 2027 5430 3637 272c 2023 2050 6865     'T067', # Phe
-000025e0: 6e6f 6d65 6e6f 6e20 6f72 2050 726f 6365  nomenon or Proce
-000025f0: 7373 2c20 6578 2e3a 2044 6973 6173 7465  ss, ex.: Disaste
-00002600: 7273 3b20 4d6f 746f 7220 5472 6166 6669  rs; Motor Traffi
-00002610: 6320 4163 6369 6465 6e74 733b 2044 6570  c Accidents; Dep
-00002620: 6f6c 796d 6572 697a 6174 696f 6e0a 2020  olymerization.  
-00002630: 2020 2320 2754 3037 3227 2c20 2320 5068    # 'T072', # Ph
-00002640: 7973 6963 616c 204f 626a 6563 742c 2065  ysical Object, e
-00002650: 782e 3a20 5072 696e 7465 6420 4d65 6469  x.: Printed Medi
-00002660: 613b 204d 6574 656f 7273 3b20 5068 7973  a; Meteors; Phys
-00002670: 6963 616c 206f 626a 6563 740a 2020 2020  ical object.    
-00002680: 2754 3033 3927 2c20 2320 5068 7973 696f  'T039', # Physio
-00002690: 6c6f 6769 6320 4675 6e63 7469 6f6e 2c20  logic Function, 
-000026a0: 6578 2e3a 2042 696f 7268 7974 686d 733b  ex.: Biorhythms;
-000026b0: 2048 6561 7269 6e67 3b20 5661 736f 6469   Hearing; Vasodi
-000026c0: 6c61 7469 6f6e 0a20 2020 2023 2027 5430  lation.    # 'T0
-000026d0: 3032 272c 2023 2050 6c61 6e74 2c20 6578  02', # Plant, ex
-000026e0: 2e3a 2041 6c6f 653b 2050 6f6c 6c65 6e3b  .: Aloe; Pollen;
-000026f0: 2048 656c 6961 6e74 6875 7320 7370 6563   Helianthus spec
-00002700: 6965 730a 2020 2020 2320 2754 3039 3827  ies.    # 'T098'
-00002710: 2c20 2320 506f 7075 6c61 7469 6f6e 2047  , # Population G
-00002720: 726f 7570 2c20 6578 2e3a 2041 7369 616e  roup, ex.: Asian
-00002730: 2041 6d65 7269 6361 6e73 3b20 4574 686e   Americans; Ethn
-00002740: 6963 2067 726f 7570 3b20 4164 756c 7420  ic group; Adult 
-00002750: 4f66 6665 6e64 6572 730a 2020 2020 2320  Offenders.    # 
-00002760: 2754 3039 3727 2c20 2320 5072 6f66 6573  'T097', # Profes
-00002770: 7369 6f6e 616c 206f 7220 4f63 6375 7061  sional or Occupa
-00002780: 7469 6f6e 616c 2047 726f 7570 2c20 6578  tional Group, ex
-00002790: 2e3a 2043 6c65 7267 793b 2044 656d 6f67  .: Clergy; Demog
-000027a0: 7261 7068 6572 733b 2048 6f73 7069 7461  raphers; Hospita
-000027b0: 6c20 566f 6c75 6e74 6565 7273 0a20 2020  l Volunteers.   
-000027c0: 2023 2027 5430 3934 272c 2023 2050 726f   # 'T094', # Pro
-000027d0: 6665 7373 696f 6e61 6c20 536f 6369 6574  fessional Societ
-000027e0: 792c 2065 782e 3a20 416d 6572 6963 616e  y, ex.: American
-000027f0: 204d 6564 6963 616c 2041 7373 6f63 6961   Medical Associa
-00002800: 7469 6f6e 3b20 496e 7465 726e 6174 696f  tion; Internatio
-00002810: 6e61 6c20 436f 756e 6369 6c20 6f66 204e  nal Council of N
-00002820: 7572 7365 733b 204c 6962 7261 7279 0a20  urses; Library. 
-00002830: 2020 2023 2027 5430 3830 272c 2023 2051     # 'T080', # Q
-00002840: 7561 6c69 7461 7469 7665 2043 6f6e 6365  ualitative Conce
-00002850: 7074 2c20 6578 2e3a 2043 6c69 6e69 6361  pt, ex.: Clinica
-00002860: 6c20 436f 6d70 6574 656e 6365 3b20 436f  l Competence; Co
-00002870: 6e73 756d 6572 2053 6174 6973 6661 6374  nsumer Satisfact
-00002880: 696f 6e3b 2048 6561 6c74 6820 5374 6174  ion; Health Stat
-00002890: 7573 0a20 2020 2023 2027 5430 3831 272c  us.    # 'T081',
-000028a0: 2023 2051 7561 6e74 6974 6174 6976 6520   # Quantitative 
-000028b0: 436f 6e63 6570 742c 2065 782e 3a20 4167  Concept, ex.: Ag
-000028c0: 6520 4469 7374 7269 6275 7469 6f6e 3b20  e Distribution; 
-000028d0: 4d65 7472 6963 2053 7973 7465 6d3b 2053  Metric System; S
-000028e0: 656c 6563 7469 6f6e 2042 6961 730a 2020  election Bias.  
-000028f0: 2020 2320 2754 3139 3227 2c20 2320 5265    # 'T192', # Re
-00002900: 6365 7074 6f72 2c20 6578 2e3a 2042 696e  ceptor, ex.: Bin
-00002910: 6469 6e67 2053 6974 6573 3b20 4c79 6d70  ding Sites; Lymp
-00002920: 686f 6379 7465 2061 6e74 6967 656e 2043  hocyte antigen C
-00002930: 4434 2072 6563 6570 746f 723b 2069 6e74  D4 receptor; int
-00002940: 6567 7269 6e20 616c 7068 6131 3162 6574  egrin alpha11bet
-00002950: 6131 0a20 2020 2023 2027 5430 3839 272c  a1.    # 'T089',
-00002960: 2023 2052 6567 756c 6174 696f 6e20 6f72   # Regulation or
-00002970: 204c 6177 2c20 6578 2e3a 2042 7569 6c64   Law, ex.: Build
-00002980: 696e 6720 436f 6465 733b 2043 7269 6d69  ing Codes; Crimi
-00002990: 6e61 6c20 4c61 773b 2048 6561 6c74 6820  nal Law; Health 
-000029a0: 506c 616e 6e69 6e67 2047 7569 6465 6c69  Planning Guideli
-000029b0: 6e65 730a 2020 2020 2320 2754 3031 3427  nes.    # 'T014'
-000029c0: 2c20 2320 5265 7074 696c 652c 2065 782e  , # Reptile, ex.
-000029d0: 3a20 416c 6c69 6761 746f 7273 3b20 5761  : Alligators; Wa
-000029e0: 7465 7220 4d6f 6361 7373 696e 3b20 4765  ter Mocassin; Ge
-000029f0: 6e75 7320 5079 7468 6f6e 2028 6f72 6761  nus Python (orga
-00002a00: 6e69 736d 290a 2020 2020 2320 2754 3036  nism).    # 'T06
-00002a10: 3227 2c20 2320 5265 7365 6172 6368 2041  2', # Research A
-00002a20: 6374 6976 6974 792c 2065 782e 3a20 416e  ctivity, ex.: An
-00002a30: 696d 616c 2045 7870 6572 696d 656e 7461  imal Experimenta
-00002a40: 7469 6f6e 3b20 4269 6f6d 6564 6963 616c  tion; Biomedical
-00002a50: 2052 6573 6561 7263 683b 2045 7870 6572   Research; Exper
-00002a60: 696d 656e 7461 6c20 5265 706c 6963 6174  imental Replicat
-00002a70: 696f 6e0a 2020 2020 2320 2754 3037 3527  ion.    # 'T075'
-00002a80: 2c20 2320 5265 7365 6172 6368 2044 6576  , # Research Dev
-00002a90: 6963 652c 2065 782e 3a20 456c 6563 7472  ice, ex.: Electr
-00002aa0: 6f64 6573 2c20 456e 7a79 6d65 3b20 444e  odes, Enzyme; DN
-00002ab0: 4120 4d69 6372 6f61 7272 6179 2043 6869  A Microarray Chi
-00002ac0: 703b 2050 6172 7469 636c 6520 436f 756e  p; Particle Coun
-00002ad0: 7420 616e 6420 5369 7a65 2041 6e61 6c79  t and Size Analy
-00002ae0: 7a65 720a 2020 2020 2320 2754 3039 3527  zer.    # 'T095'
-00002af0: 2c20 2320 5365 6c66 2d68 656c 7020 6f72  , # Self-help or
-00002b00: 2052 656c 6965 6620 4f72 6761 6e69 7a61   Relief Organiza
-00002b10: 7469 6f6e 2c20 6578 2e3a 2041 6c63 6f68  tion, ex.: Alcoh
-00002b20: 6f6c 6963 7320 416e 6f6e 796d 6f75 733b  olics Anonymous;
-00002b30: 2043 6861 7269 7469 6573 202d 206f 7267   Charities - org
-00002b40: 616e 697a 6174 696f 6e3b 2052 6564 2043  anization; Red C
-00002b50: 726f 7373 0a20 2020 2027 5431 3834 272c  ross.    'T184',
-00002b60: 2023 2053 6967 6e20 6f72 2053 796d 7074   # Sign or Sympt
-00002b70: 6f6d 2c20 6578 2e3a 2044 7973 706e 6561  om, ex.: Dyspnea
-00002b80: 3b20 4e61 7573 6561 3b20 5061 696e 0a20  ; Nausea; Pain. 
-00002b90: 2020 2023 2027 5430 3534 272c 2023 2053     # 'T054', # S
-00002ba0: 6f63 6961 6c20 4265 6861 7669 6f72 2c20  ocial Behavior, 
-00002bb0: 6578 2e3a 2041 6363 756c 7475 7261 7469  ex.: Acculturati
-00002bc0: 6f6e 3b20 436f 6d6d 756e 6963 6174 696f  on; Communicatio
-00002bd0: 6e3b 2049 6e74 6572 7065 7273 6f6e 616c  n; Interpersonal
-00002be0: 2052 656c 6174 696f 6e73 0a20 2020 2023   Relations.    #
-00002bf0: 2027 5430 3832 272c 2023 2053 7061 7469   'T082', # Spati
-00002c00: 616c 2043 6f6e 6365 7074 2c20 6578 2e3a  al Concept, ex.:
-00002c10: 204d 616e 6469 6275 6c61 7220 5265 7374   Mandibular Rest
-00002c20: 2050 6f73 6974 696f 6e3b 204c 6174 6572   Position; Later
-00002c30: 616c 3b20 4578 7472 696e 7369 630a 2020  al; Extrinsic.  
-00002c40: 2020 2320 2754 3136 3727 2c20 2320 5375    # 'T167', # Su
-00002c50: 6273 7461 6e63 652c 2065 782e 3a20 4169  bstance, ex.: Ai
-00002c60: 7220 2873 7562 7374 616e 6365 293b 2046  r (substance); F
-00002c70: 6f73 7369 6c73 3b20 506c 6173 7469 6373  ossils; Plastics
-00002c80: 0a20 2020 2023 2027 5430 3739 272c 2023  .    # 'T079', #
-00002c90: 2054 656d 706f 7261 6c20 436f 6e63 6570   Temporal Concep
-00002ca0: 742c 2065 782e 3a20 4269 7274 6820 496e  t, ex.: Birth In
-00002cb0: 7465 7276 616c 733b 2048 616c 662d 4c69  tervals; Half-Li
-00002cc0: 6665 3b20 506f 7374 6f70 6572 6174 6976  fe; Postoperativ
-00002cd0: 6520 5065 7269 6f64 0a20 2020 2027 5430  e Period.    'T0
-00002ce0: 3631 272c 2023 2054 6865 7261 7065 7574  61', # Therapeut
-00002cf0: 6963 206f 7220 5072 6576 656e 7469 7665  ic or Preventive
-00002d00: 2050 726f 6365 6475 7265 2c20 6578 2e3a   Procedure, ex.:
-00002d10: 2043 6573 6172 6561 6e20 7365 6374 696f   Cesarean sectio
-00002d20: 6e3b 2044 6572 6d61 6272 6173 696f 6e3b  n; Dermabrasion;
-00002d30: 2046 616d 696c 7920 7073 7963 686f 7468   Family psychoth
-00002d40: 6572 6170 790a 2020 2020 2320 2754 3032  erapy.    # 'T02
-00002d50: 3427 2c20 2320 5469 7373 7565 2c20 6578  4', # Tissue, ex
-00002d60: 2e3a 2043 6172 7469 6c61 6765 3b20 456e  .: Cartilage; En
-00002d70: 646f 7468 656c 6975 6d3b 2045 7069 6465  dothelium; Epide
-00002d80: 726d 6973 0a20 2020 2023 2027 5430 3130  rmis.    # 'T010
-00002d90: 272c 2023 2056 6572 7465 6272 6174 652c  ', # Vertebrate,
-00002da0: 2065 782e 3a20 5665 7274 6562 7261 7465   ex.: Vertebrate
-00002db0: 733b 2047 6e61 7468 6f73 746f 6d61 7461  s; Gnathostomata
-00002dc0: 2076 6572 7465 6272 6174 653b 2043 7261   vertebrate; Cra
-00002dd0: 6e69 6174 6120 3c63 686f 7264 6174 613e  niata <chordata>
-00002de0: 0a20 2020 2023 2027 5430 3035 272c 2023  .    # 'T005', #
-00002df0: 2056 6972 7573 2c20 6578 2e3a 2043 6f6c   Virus, ex.: Col
-00002e00: 6970 6861 6765 733b 2045 6368 6f76 6972  iphages; Echovir
-00002e10: 7573 3b20 5061 7276 6f76 6972 6964 6165  us; Parvoviridae
-00002e20: 0a20 2020 2023 2027 5431 3237 2720 2023  .    # 'T127'  #
-00002e30: 2056 6974 616d 696e 2c20 6578 2e3a 2035   Vitamin, ex.: 5
-00002e40: 2c32 352d 4469 6879 6472 6f78 7920 6368  ,25-Dihydroxy ch
-00002e50: 6f6c 6563 616c 6369 6665 726f 6c3b 2061  olecalciferol; a
-00002e60: 6c70 6861 2d74 6f63 6f70 6865 7279 6c20  lpha-tocopheryl 
-00002e70: 6f78 616c 6174 653b 2056 6974 616d 696e  oxalate; Vitamin
-00002e80: 2041 205b 4550 435d 0a7d 0a0a 554e 4943   A [EPC].}..UNIC
-00002e90: 4f44 455f 4441 5348 4553 203d 207b 0a20  ODE_DASHES = {. 
-00002ea0: 2020 2075 275c 7530 3032 6427 2c20 7527     u'\u002d', u'
-00002eb0: 5c75 3030 3765 272c 2075 275c 7530 3061  \u007e', u'\u00a
-00002ec0: 6427 2c20 7527 5c75 3035 3861 272c 2075  d', u'\u058a', u
-00002ed0: 275c 7530 3562 6527 2c20 7527 5c75 3134  '\u05be', u'\u14
-00002ee0: 3030 272c 0a20 2020 2075 275c 7531 3830  00',.    u'\u180
-00002ef0: 3627 2c20 7527 5c75 3230 3130 272c 2075  6', u'\u2010', u
-00002f00: 275c 7532 3031 3127 2c20 7527 5c75 3230  '\u2011', u'\u20
-00002f10: 3130 272c 2075 275c 7532 3031 3227 2c20  10', u'\u2012', 
-00002f20: 7527 5c75 3230 3133 272c 0a20 2020 2075  u'\u2013',.    u
-00002f30: 275c 7532 3031 3427 2c20 7527 5c75 3230  '\u2014', u'\u20
-00002f40: 3135 272c 2075 275c 7532 3035 3327 2c20  15', u'\u2053', 
-00002f50: 7527 5c75 3230 3762 272c 2075 275c 7532  u'\u207b', u'\u2
-00002f60: 3231 3227 2c20 7527 5c75 3230 3862 272c  212', u'\u208b',
-00002f70: 0a20 2020 2075 275c 7532 3231 3227 2c20  .    u'\u2212', 
-00002f80: 7527 5c75 3232 3132 272c 2075 275c 7532  u'\u2212', u'\u2
-00002f90: 6531 3727 2c20 7527 5c75 3265 3361 272c  e17', u'\u2e3a',
-00002fa0: 2075 275c 7532 6533 6227 2c20 7527 5c75   u'\u2e3b', u'\u
-00002fb0: 3330 3163 272c 0a20 2020 2075 275c 7533  301c',.    u'\u3
-00002fc0: 3033 3027 2c20 7527 5c75 3330 6130 272c  030', u'\u30a0',
-00002fd0: 2075 275c 7566 6533 3127 2c20 7527 5c75   u'\ufe31', u'\u
-00002fe0: 6665 3332 272c 2075 275c 7566 6535 3827  fe32', u'\ufe58'
-00002ff0: 2c20 7527 5c75 6665 3633 272c 0a20 2020  , u'\ufe63',.   
-00003000: 2075 275c 7566 6630 6427 0a7d 0a0a 2320   u'\uff0d'.}..# 
-00003010: 6c61 6e67 7561 6765 2077 6974 6820 6d69  language with mi
-00003020: 7373 696e 6720 7661 6c75 650a 2320 7769  ssing value.# wi
-00003030: 6c6c 206e 6f74 2068 6176 6520 7375 7070  ll not have supp
-00003040: 6f72 7420 666f 7220 746f 6b65 6e69 7a61  ort for tokeniza
-00003050: 7469 6f6e 0a4c 414e 4755 4147 4553 203d  tion.LANGUAGES =
-00003060: 207b 0a20 2020 2027 4241 5127 3a20 4e6f   {.    'BAQ': No
-00003070: 6e65 2c20 2020 2020 2020 2020 2020 2320  ne,           # 
-00003080: 4261 7371 7565 0a20 2020 2027 4348 4927  Basque.    'CHI'
-00003090: 3a20 4e6f 6e65 2c20 2020 2020 2020 2020  : None,         
-000030a0: 2020 2320 4368 696e 6573 650a 2020 2020    # Chinese.    
-000030b0: 2743 5a45 273a 204e 6f6e 652c 2020 2020  'CZE': None,    
-000030c0: 2020 2020 2020 2023 2043 7a65 6368 0a20         # Czech. 
-000030d0: 2020 2027 4441 4e27 3a20 2764 616e 6973     'DAN': 'danis
-000030e0: 6827 2c20 2020 2020 2020 2320 4461 6e69  h',       # Dani
-000030f0: 7368 0a20 2020 2027 4455 5427 3a20 2764  sh.    'DUT': 'd
-00003100: 7574 6368 272c 2020 2020 2020 2020 2320  utch',        # 
-00003110: 4475 7463 680a 2020 2020 2745 4e47 273a  Dutch.    'ENG':
-00003120: 2027 656e 676c 6973 6827 2c20 2020 2020   'english',     
-00003130: 2023 2045 6e67 6c69 7368 0a20 2020 2027   # English.    '
-00003140: 4553 5427 3a20 4e6f 6e65 2c20 2020 2020  EST': None,     
-00003150: 2020 2020 2020 2320 4573 746f 6e69 616e        # Estonian
-00003160: 0a20 2020 2027 4649 4e27 3a20 2766 696e  .    'FIN': 'fin
-00003170: 6e69 7368 272c 2020 2020 2020 2320 4669  nish',      # Fi
-00003180: 6e6e 6973 680a 2020 2020 2746 5245 273a  nnish.    'FRE':
-00003190: 2027 6672 656e 6368 272c 2020 2020 2020   'french',      
-000031a0: 2023 2046 7265 6e63 680a 2020 2020 2747   # French.    'G
-000031b0: 4552 273a 2027 6765 726d 616e 272c 2020  ER': 'german',  
-000031c0: 2020 2020 2023 2047 6572 6d61 6e0a 2020       # German.  
-000031d0: 2020 2747 5245 273a 2027 6772 6565 6b27    'GRE': 'greek'
-000031e0: 2c20 2020 2020 2020 2023 2047 7265 656b  ,        # Greek
-000031f0: 0a20 2020 2027 4845 4227 3a20 4e6f 6e65  .    'HEB': None
-00003200: 2c20 2020 2020 2020 2020 2020 2320 4865  ,           # He
-00003210: 6272 6577 0a20 2020 2027 4855 4e27 3a20  brew.    'HUN': 
-00003220: 2768 756e 6761 7269 616e 272c 2020 2020  'hungarian',    
-00003230: 2320 4875 6e67 6172 6961 6e0a 2020 2020  # Hungarian.    
-00003240: 2749 5441 273a 2027 6974 616c 6961 6e27  'ITA': 'italian'
-00003250: 2c20 2020 2020 2023 2049 7461 6c69 616e  ,      # Italian
-00003260: 0a20 2020 2027 4a50 4e27 3a20 4e6f 6e65  .    'JPN': None
-00003270: 2c20 2020 2020 2020 2020 2020 2320 4a61  ,           # Ja
-00003280: 7061 6e65 7365 0a20 2020 2027 4b4f 5227  panese.    'KOR'
-00003290: 3a20 4e6f 6e65 2c20 2020 2020 2020 2020  : None,         
-000032a0: 2020 2320 4b6f 7265 616e 0a20 2020 2027    # Korean.    '
-000032b0: 4c41 5627 3a20 4e6f 6e65 2c20 2020 2020  LAV': None,     
-000032c0: 2020 2020 2020 2320 4c61 7476 6961 6e0a        # Latvian.
-000032d0: 2020 2020 274e 4f52 273a 2027 6e6f 7277      'NOR': 'norw
-000032e0: 6567 6961 6e27 2c20 2020 2023 204e 6f72  egian',    # Nor
-000032f0: 7765 6769 616e 0a20 2020 2027 504f 4c27  wegian.    'POL'
-00003300: 3a20 2770 6f6c 6973 6827 2c20 2020 2020  : 'polish',     
-00003310: 2020 2320 506f 6c69 7368 0a20 2020 2027    # Polish.    '
-00003320: 504f 5227 3a20 2770 6f72 746f 6775 6573  POR': 'portogues
-00003330: 6527 2c20 2020 2320 506f 7274 7567 7565  e',   # Portugue
-00003340: 7365 0a20 2020 2027 5255 5327 3a20 2772  se.    'RUS': 'r
-00003350: 7573 7369 616e 272c 2020 2020 2020 2320  ussian',      # 
-00003360: 5275 7373 6961 6e0a 2020 2020 2753 4352  Russian.    'SCR
-00003370: 273a 204e 6f6e 652c 2020 2020 2020 2020  ': None,        
-00003380: 2020 2023 2043 726f 6174 6961 6e0a 2020     # Croatian.  
-00003390: 2020 2753 5041 273a 2027 7370 616e 6973    'SPA': 'spanis
-000033a0: 6827 2c20 2020 2020 2023 2053 7061 6e69  h',      # Spani
-000033b0: 7368 0a20 2020 2027 5357 4527 3a20 2773  sh.    'SWE': 's
-000033c0: 7765 6469 7368 272c 2020 2020 2020 2320  wedish',      # 
-000033d0: 5377 6564 6973 680a 2020 2020 2754 5552  Swedish.    'TUR
-000033e0: 273a 2027 7475 726b 6973 6827 2c20 2020  ': 'turkish',   
-000033f0: 2020 2023 2054 7572 6b69 7368 0a7d 0a0a     # Turkish.}..
-00003400: 444f 4d41 494e 5f53 5045 4349 4649 435f  DOMAIN_SPECIFIC_
-00003410: 5354 4f50 574f 5244 5320 3d20 7b0a 2020  STOPWORDS = {.  
-00003420: 2020 2774 696d 6527 0a7d 0a0a 5350 4143    'time'.}..SPAC
-00003430: 595f 4c41 4e47 5541 4745 5f4d 4150 203d  Y_LANGUAGE_MAP =
-00003440: 207b 0a20 2020 2027 454e 4727 3a20 2765   {.    'ENG': 'e
-00003450: 6e5f 636f 7265 5f77 6562 5f73 6d27 2c0a  n_core_web_sm',.
-00003460: 2020 2020 2747 4552 273a 2027 6465 5f63      'GER': 'de_c
-00003470: 6f72 655f 6e65 7773 5f73 6d27 2c0a 2020  ore_news_sm',.  
-00003480: 2020 2753 5041 273a 2027 6573 5f63 6f72    'SPA': 'es_cor
-00003490: 655f 6e65 7773 5f73 6d27 2c0a 2020 2020  e_news_sm',.    
-000034a0: 2750 4f52 273a 2027 7074 5f63 6f72 655f  'POR': 'pt_core_
-000034b0: 6e65 7773 5f73 6d27 2c0a 2020 2020 2746  news_sm',.    'F
-000034c0: 5245 273a 2027 6672 5f63 6f72 655f 6e65  RE': 'fr_core_ne
-000034d0: 7773 5f73 6d27 2c0a 2020 2020 2749 5441  ws_sm',.    'ITA
-000034e0: 273a 2027 6974 5f63 6f72 655f 6e65 7773  ': 'it_core_news
-000034f0: 5f73 6d27 2c0a 2020 2020 2744 5554 273a  _sm',.    'DUT':
-00003500: 2027 6e6c 5f63 6f72 655f 6e65 7773 5f73   'nl_core_news_s
-00003510: 6d27 2c0a 2020 2020 2758 5858 273a 2027  m',.    'XXX': '
-00003520: 7878 270a 7d0a                           xx'.}.
+00000030: 6e73 220d 0a0d 0a48 4541 4445 5253 5f4d  ns"....HEADERS_M
+00000040: 5243 4f4e 534f 203d 205b 0d0a 2020 2020  RCONSO = [..    
+00000050: 2763 7569 272c 2027 6c61 7427 2c20 2774  'cui', 'lat', 't
+00000060: 7327 2c20 276c 7569 272c 2027 7374 7427  s', 'lui', 'stt'
+00000070: 2c20 2773 7569 272c 2027 6973 7072 6566  , 'sui', 'ispref
+00000080: 272c 2027 6175 6927 2c20 2773 6175 6927  ', 'aui', 'saui'
+00000090: 2c0d 0a20 2020 2027 7363 7569 272c 2027  ,..    'scui', '
+000000a0: 7364 7569 272c 2027 7361 6227 2c20 2774  sdui', 'sab', 't
+000000b0: 7479 272c 2027 636f 6465 272c 2027 7374  ty', 'code', 'st
+000000c0: 7227 2c20 2773 726c 272c 2027 7375 7070  r', 'srl', 'supp
+000000d0: 7265 7373 272c 2027 6376 6627 0d0a 5d0d  ress', 'cvf'..].
+000000e0: 0a48 4541 4445 5253 5f4d 5253 5459 203d  .HEADERS_MRSTY =
+000000f0: 205b 0d0a 2020 2020 2763 7569 272c 2027   [..    'cui', '
+00000100: 7374 7927 2c20 2768 6965 7227 2027 6465  sty', 'hier' 'de
+00000110: 7363 272c 2027 7369 6427 2c20 276e 756d  sc', 'sid', 'num
+00000120: 270d 0a5d 0d0a 0d0a 4e45 4741 5449 4f4e  '..]....NEGATION
+00000130: 5320 3d20 7b27 6e6f 6e65 272c 2027 6e6f  S = {'none', 'no
+00000140: 6e27 2c20 276e 6569 7468 6572 272c 2027  n', 'neither', '
+00000150: 6e6f 7227 2c20 276e 6f27 2c20 276e 6f74  nor', 'no', 'not
+00000160: 277d 0d0a 0d0a 2320 5468 6520 666f 6c6c  '}....# The foll
+00000170: 6f77 696e 6720 6973 2061 206c 6973 7420  owing is a list 
+00000180: 6f66 2061 6c6c 2065 7869 7374 696e 6720  of all existing 
+00000190: 7365 6d74 7970 6573 2061 6c6f 6e67 2077  semtypes along w
+000001a0: 6974 6820 7468 6569 7220 6e61 6d65 2061  ith their name a
+000001b0: 6e64 2073 6f6d 6520 6578 616d 706c 6573  nd some examples
+000001c0: 2e20 0d0a 2320 596f 7520 6361 6e20 6561  . ..# You can ea
+000001d0: 7369 6c79 2073 656c 6563 7420 7468 6520  sily select the 
+000001e0: 6f6e 6573 2079 6f75 206e 6565 6420 6279  ones you need by
+000001f0: 2063 6f6d 6d65 6e74 696e 6720 6f75 7420   commenting out 
+00000200: 7468 6520 6c69 6e65 7320 7468 6174 2061  the lines that a
+00000210: 7265 206e 6f74 2072 656c 6576 616e 7420  re not relevant 
+00000220: 666f 7220 796f 7572 2061 7070 6c69 6361  for your applica
+00000230: 7469 6f6e 2e0d 0a0d 0a41 4343 4550 5445  tion.....ACCEPTE
+00000240: 445f 5345 4d54 5950 4553 203d 207b 0d0a  D_SEMTYPES = {..
+00000250: 2020 2020 2320 2754 3032 3027 2c20 2320      # 'T020', # 
+00000260: 4163 7175 6972 6564 2041 626e 6f72 6d61  Acquired Abnorma
+00000270: 6c69 7479 2c20 6578 2e3a 2048 656d 6f72  lity, ex.: Hemor
+00000280: 7268 6f69 6473 3b20 4865 726e 6961 2c20  rhoids; Hernia, 
+00000290: 4665 6d6f 7261 6c3b 2043 6175 6c69 666c  Femoral; Caulifl
+000002a0: 6f77 6572 2065 6172 0d0a 2020 2020 2320  ower ear..    # 
+000002b0: 2754 3035 3227 2c20 2320 4163 7469 7669  'T052', # Activi
+000002c0: 7479 2c20 6578 2e3a 2045 7870 6564 6974  ty, ex.: Expedit
+000002d0: 696f 6e73 3b20 496e 666f 726d 6174 696f  ions; Informatio
+000002e0: 6e20 4469 7374 7269 6275 7469 6f6e 3b20  n Distribution; 
+000002f0: 536f 6369 616c 2050 6c61 6e6e 696e 670d  Social Planning.
+00000300: 0a20 2020 2023 2027 5431 3030 272c 2023  .    # 'T100', #
+00000310: 2041 6765 2047 726f 7570 2c20 6578 2e3a   Age Group, ex.:
+00000320: 2041 6475 6c74 3b20 496e 6661 6e74 2c20   Adult; Infant, 
+00000330: 5072 656d 6174 7572 653b 2041 646f 6c65  Premature; Adole
+00000340: 7363 656e 7420 2861 6765 2067 726f 7570  scent (age group
+00000350: 290d 0a20 2020 2023 2027 5430 3837 272c  )..    # 'T087',
+00000360: 2023 2041 6d69 6e6f 2041 6369 6420 5365   # Amino Acid Se
+00000370: 7175 656e 6365 2c20 6578 2e3a 2053 6967  quence, ex.: Sig
+00000380: 6e61 6c20 5065 7074 6964 6573 3b20 486f  nal Peptides; Ho
+00000390: 6d6f 6c6f 676f 7573 2053 6571 7565 6e63  mologous Sequenc
+000003a0: 6573 2c20 416d 696e 6f20 4163 6964 3b20  es, Amino Acid; 
+000003b0: 4162 6e6f 726d 616c 2061 6d69 6e6f 2061  Abnormal amino a
+000003c0: 6369 640d 0a20 2020 2023 2027 5431 3136  cid..    # 'T116
+000003d0: 272c 2023 2041 6d69 6e6f 2041 6369 642c  ', # Amino Acid,
+000003e0: 2050 6570 7469 6465 2c20 6f72 2050 726f   Peptide, or Pro
+000003f0: 7465 696e 2c20 6578 2e3a 2041 6d69 6e6f  tein, ex.: Amino
+00000400: 2041 6369 6473 2c20 4379 636c 6963 3b20   Acids, Cyclic; 
+00000410: 476c 7963 6f70 6570 7469 6465 733b 204b  Glycopeptides; K
+00000420: 6572 6174 696e 0d0a 2020 2020 2320 2754  eratin..    # 'T
+00000430: 3031 3127 2c20 2320 416d 7068 6962 6961  011', # Amphibia
+00000440: 6e2c 2065 782e 3a20 5361 6c61 6d61 6e64  n, ex.: Salamand
+00000450: 7261 3b20 5572 6f64 656c 613b 2042 7261  ra; Urodela; Bra
+00000460: 7a69 6c69 616e 2068 6f72 6e65 6420 6672  zilian horned fr
+00000470: 6f67 0d0a 2020 2020 2320 2754 3139 3027  og..    # 'T190'
+00000480: 2c20 2320 416e 6174 6f6d 6963 616c 2041  , # Anatomical A
+00000490: 626e 6f72 6d61 6c69 7479 2c20 6578 2e3a  bnormality, ex.:
+000004a0: 2042 726f 6e63 6869 616c 2046 6973 7475   Bronchial Fistu
+000004b0: 6c61 3b20 466f 6f74 2044 6566 6f72 6d69  la; Foot Deformi
+000004c0: 7469 6573 3b20 4879 7065 726f 7374 6f73  ties; Hyperostos
+000004d0: 6973 206f 6620 736b 756c 6c0d 0a20 2020  is of skull..   
+000004e0: 2023 2027 5430 3137 272c 2023 2041 6e61   # 'T017', # Ana
+000004f0: 746f 6d69 6361 6c20 5374 7275 6374 7572  tomical Structur
+00000500: 652c 2065 782e 3a20 4361 6461 7665 723b  e, ex.: Cadaver;
+00000510: 2050 6861 7279 6e67 6f73 746f 6d65 3b20   Pharyngostome; 
+00000520: 416e 6174 6f6d 6963 2073 7472 7563 7475  Anatomic structu
+00000530: 7265 730d 0a20 2020 2023 2027 5430 3038  res..    # 'T008
+00000540: 272c 2023 2041 6e69 6d61 6c2c 2065 782e  ', # Animal, ex.
+00000550: 3a20 416e 696d 616c 733b 2041 6e69 6d61  : Animals; Anima
+00000560: 6c73 2c20 4c61 626f 7261 746f 7279 3b20  ls, Laboratory; 
+00000570: 4361 726e 6976 6f72 650d 0a20 2020 2027  Carnivore..    '
+00000580: 5431 3935 272c 2023 2041 6e74 6962 696f  T195', # Antibio
+00000590: 7469 632c 2065 782e 3a20 416e 7469 6269  tic, ex.: Antibi
+000005a0: 6f74 6963 733b 2062 6163 7465 7269 6369  otics; bacterici
+000005b0: 6465 3b20 5468 6965 6e61 6d79 6369 6e73  de; Thienamycins
+000005c0: 0d0a 2020 2020 2320 2754 3139 3427 2c20  ..    # 'T194', 
+000005d0: 2320 4172 6368 6165 6f6e 2c20 6578 2e3a  # Archaeon, ex.:
+000005e0: 2054 6865 726d 6f70 726f 7465 616c 6573   Thermoproteales
+000005f0: 3b20 4861 6c6f 6665 7261 7820 766f 6c63  ; Haloferax volc
+00000600: 616e 6969 3b20 4d65 7468 616e 6f73 7069  anii; Methanospi
+00000610: 7269 6c6c 756d 0d0a 2020 2020 2320 2754  rillum..    # 'T
+00000620: 3030 3727 2c20 2320 4261 6374 6572 6975  007', # Bacteriu
+00000630: 6d2c 2065 782e 3a20 4163 6574 6f62 6163  m, ex.: Acetobac
+00000640: 7465 723b 2042 6163 696c 6c75 7320 6365  ter; Bacillus ce
+00000650: 7265 7573 3b20 4379 746f 7068 6167 610d  reus; Cytophaga.
+00000660: 0a20 2020 2023 2027 5430 3533 272c 2023  .    # 'T053', #
+00000670: 2042 6568 6176 696f 722c 2065 782e 3a20   Behavior, ex.: 
+00000680: 486f 6d69 6e67 2042 6568 6176 696f 723b  Homing Behavior;
+00000690: 2053 6578 7561 6c69 7479 3b20 4861 6269   Sexuality; Habi
+000006a0: 7461 7420 5365 6c65 6374 696f 6e0d 0a20  tat Selection.. 
+000006b0: 2020 2023 2027 5430 3338 272c 2023 2042     # 'T038', # B
+000006c0: 696f 6c6f 6769 6320 4675 6e63 7469 6f6e  iologic Function
+000006d0: 2c20 6578 2e3a 2041 6e74 6962 6f64 7920  , ex.: Antibody 
+000006e0: 466f 726d 6174 696f 6e3b 2044 7275 6720  Formation; Drug 
+000006f0: 7265 7369 7374 616e 6365 3b20 486f 6d65  resistance; Home
+00000700: 6f73 7461 7369 730d 0a20 2020 2023 2027  ostasis..    # '
+00000710: 5431 3233 272c 2023 2042 696f 6c6f 6769  T123', # Biologi
+00000720: 6361 6c6c 7920 4163 7469 7665 2053 7562  cally Active Sub
+00000730: 7374 616e 6365 2c20 6578 2e3a 2043 7974  stance, ex.: Cyt
+00000740: 6f6b 696e 696e 733b 2050 6865 726f 6d6f  okinins; Pheromo
+00000750: 6e65 0d0a 2020 2020 2320 2754 3039 3127  ne..    # 'T091'
+00000760: 2c20 2320 4269 6f6d 6564 6963 616c 204f  , # Biomedical O
+00000770: 6363 7570 6174 696f 6e20 6f72 2044 6973  ccupation or Dis
+00000780: 6369 706c 696e 652c 2065 782e 3a20 4164  cipline, ex.: Ad
+00000790: 6f6c 6573 6365 6e74 204d 6564 6963 696e  olescent Medicin
+000007a0: 653b 2043 656c 6c75 6c61 7220 4e65 7572  e; Cellular Neur
+000007b0: 6f62 696f 6c6f 6779 3b20 4465 6e74 6973  obiology; Dentis
+000007c0: 7472 790d 0a20 2020 2023 2027 5431 3232  try..    # 'T122
+000007d0: 272c 2023 2042 696f 6d65 6469 6361 6c20  ', # Biomedical 
+000007e0: 6f72 2044 656e 7461 6c20 4d61 7465 7269  or Dental Materi
+000007f0: 616c 2c20 6578 2e3a 2041 6372 796c 6963  al, ex.: Acrylic
+00000800: 2052 6573 696e 733b 2042 6f6e 6520 4365   Resins; Bone Ce
+00000810: 6d65 6e74 733b 2044 656e 7469 6672 6963  ments; Dentifric
+00000820: 6573 0d0a 2020 2020 2320 2754 3031 3227  es..    # 'T012'
+00000830: 2c20 2320 4269 7264 2c20 6578 2e3a 2053  , # Bird, ex.: S
+00000840: 6572 696e 7573 3b20 4475 636b 733b 2051  erinus; Ducks; Q
+00000850: 7561 696c 0d0a 2020 2020 2754 3032 3927  uail..    'T029'
+00000860: 2c20 2320 426f 6479 204c 6f63 6174 696f  , # Body Locatio
+00000870: 6e20 6f72 2052 6567 696f 6e2c 2065 782e  n or Region, ex.
+00000880: 3a20 466f 7265 6865 6164 3b20 5375 626c  : Forehead; Subl
+00000890: 696e 6775 616c 2052 6567 696f 6e3b 2042  ingual Region; B
+000008a0: 6173 6520 6f66 2073 6b75 6c6c 2073 7472  ase of skull str
+000008b0: 7563 7475 7265 0d0a 2020 2020 2754 3032  ucture..    'T02
+000008c0: 3327 2c20 2320 426f 6479 2050 6172 742c  3', # Body Part,
+000008d0: 204f 7267 616e 2c20 6f72 204f 7267 616e   Organ, or Organ
+000008e0: 2043 6f6d 706f 6e65 6e74 2c20 6578 2e3a   Component, ex.:
+000008f0: 2041 6f72 7461 3b20 4272 6169 6e20 5374   Aorta; Brain St
+00000900: 656d 3b20 5374 7275 6374 7572 6520 6f66  em; Structure of
+00000910: 206e 6563 6b20 6f66 2066 656d 7572 0d0a   neck of femur..
+00000920: 2020 2020 2320 2754 3033 3027 2c20 2320      # 'T030', # 
+00000930: 426f 6479 2053 7061 6365 206f 7220 4a75  Body Space or Ju
+00000940: 6e63 7469 6f6e 2c20 6578 2e3a 204b 6e65  nction, ex.: Kne
+00000950: 6520 6a6f 696e 743b 2047 7265 6174 6572  e joint; Greater
+00000960: 2073 6163 206f 6620 7065 7269 746f 6e65   sac of peritone
+00000970: 756d 3b20 5379 6e61 7073 6573 0d0a 2020  um; Synapses..  
+00000980: 2020 2754 3033 3127 2c20 2320 426f 6479    'T031', # Body
+00000990: 2053 7562 7374 616e 6365 2c20 6578 2e3a   Substance, ex.:
+000009a0: 2041 6d6e 696f 7469 6320 466c 7569 643b   Amniotic Fluid;
+000009b0: 2073 616c 6976 613b 2053 6d65 676d 610d   saliva; Smegma.
+000009c0: 0a20 2020 2023 2027 5430 3232 272c 2023  .    # 'T022', #
+000009d0: 2042 6f64 7920 5379 7374 656d 2c20 6578   Body System, ex
+000009e0: 2e3a 2045 6e64 6f63 7269 6e65 2073 7973  .: Endocrine sys
+000009f0: 7465 6d3b 2052 656e 696e 2d61 6e67 696f  tem; Renin-angio
+00000a00: 7465 6e73 696e 2073 7973 7465 6d3b 2052  tensin system; R
+00000a10: 6574 6963 756c 6f65 6e64 6f74 6865 6c69  eticuloendotheli
+00000a20: 616c 2053 7973 7465 6d0d 0a20 2020 2023  al System..    #
+00000a30: 2027 5430 3838 272c 2023 2043 6172 626f   'T088', # Carbo
+00000a40: 6879 6472 6174 6520 5365 7175 656e 6365  hydrate Sequence
+00000a50: 2c20 6578 2e3a 2043 6172 626f 6879 6472  , ex.: Carbohydr
+00000a60: 6174 6520 5365 7175 656e 6365 3b20 4162  ate Sequence; Ab
+00000a70: 6e6f 726d 616c 2063 6172 626f 6879 6472  normal carbohydr
+00000a80: 6174 6520 7365 7175 656e 6365 0d0a 2020  ate sequence..  
+00000a90: 2020 2320 2754 3032 3527 2c20 2320 4365    # 'T025', # Ce
+00000aa0: 6c6c 2c20 6578 2e3a 2042 2d4c 796d 7068  ll, ex.: B-Lymph
+00000ab0: 6f63 7974 6573 3b20 4465 6e64 7269 7469  ocytes; Dendriti
+00000ac0: 6320 4365 6c6c 733b 2046 6962 726f 626c  c Cells; Fibrobl
+00000ad0: 6173 7473 0d0a 2020 2020 2320 2754 3032  asts..    # 'T02
+00000ae0: 3627 2c20 2320 4365 6c6c 2043 6f6d 706f  6', # Cell Compo
+00000af0: 6e65 6e74 2c20 6578 2e3a 2041 786f 6e3b  nent, ex.: Axon;
+00000b00: 2047 6f6c 6769 2041 7070 6172 6174 7573   Golgi Apparatus
+00000b10: 3b20 4f72 6761 6e65 6c6c 6573 0d0a 2020  ; Organelles..  
+00000b20: 2020 2320 2754 3034 3327 2c20 2320 4365    # 'T043', # Ce
+00000b30: 6c6c 2046 756e 6374 696f 6e2c 2065 782e  ll Function, ex.
+00000b40: 3a20 4365 6c6c 2043 7963 6c65 3b20 4365  : Cell Cycle; Ce
+00000b50: 6c6c 2064 6976 6973 696f 6e3b 2050 6861  ll division; Pha
+00000b60: 676f 6379 746f 7369 730d 0a20 2020 2023  gocytosis..    #
+00000b70: 2027 5430 3439 272c 2023 2043 656c 6c20   'T049', # Cell 
+00000b80: 6f72 204d 6f6c 6563 756c 6172 2044 7973  or Molecular Dys
+00000b90: 6675 6e63 7469 6f6e 2c20 6578 2e3a 2044  function, ex.: D
+00000ba0: 4e41 2044 616d 6167 653b 2057 616c 6c65  NA Damage; Walle
+00000bb0: 7269 616e 2044 6567 656e 6572 6174 696f  rian Degeneratio
+00000bc0: 6e3b 2041 7479 7069 6361 6c20 7371 7561  n; Atypical squa
+00000bd0: 6d6f 7573 206d 6574 6170 6c61 7369 610d  mous metaplasia.
+00000be0: 0a20 2020 2023 2027 5431 3033 272c 2023  .    # 'T103', #
+00000bf0: 2043 6865 6d69 6361 6c2c 2065 782e 3a20   Chemical, ex.: 
+00000c00: 4163 6964 733b 2043 6865 6d69 6361 6c73  Acids; Chemicals
+00000c10: 3b20 496f 6e69 6320 4c69 7175 6964 730d  ; Ionic Liquids.
+00000c20: 0a20 2020 2023 2027 5431 3230 272c 2023  .    # 'T120', #
+00000c30: 2043 6865 6d69 6361 6c20 5669 6577 6564   Chemical Viewed
+00000c40: 2046 756e 6374 696f 6e61 6c6c 792c 2065   Functionally, e
+00000c50: 782e 3a20 4165 726f 736f 6c20 5072 6f70  x.: Aerosol Prop
+00000c60: 656c 6c61 6e74 733b 2044 6574 6572 6765  ellants; Deterge
+00000c70: 6e74 733b 2053 7461 6269 6c69 7a69 6e67  nts; Stabilizing
+00000c80: 2041 6765 6e74 730d 0a20 2020 2023 2027   Agents..    # '
+00000c90: 5431 3034 272c 2023 2043 6865 6d69 6361  T104', # Chemica
+00000ca0: 6c20 5669 6577 6564 2053 7472 7563 7475  l Viewed Structu
+00000cb0: 7261 6c6c 792c 2065 782e 3a20 416d 6d6f  rally, ex.: Ammo
+00000cc0: 6e69 756d 2043 6f6d 706f 756e 6473 3b20  nium Compounds; 
+00000cd0: 4361 7469 6f6e 733b 2053 756c 6675 7220  Cations; Sulfur 
+00000ce0: 436f 6d70 6f75 6e64 730d 0a20 2020 2023  Compounds..    #
+00000cf0: 2027 5431 3835 272c 2023 2043 6c61 7373   'T185', # Class
+00000d00: 6966 6963 6174 696f 6e2c 2065 782e 3a20  ification, ex.: 
+00000d10: 416e 6174 6f6d 7920 284d 6553 4820 4361  Anatomy (MeSH Ca
+00000d20: 7465 676f 7279 293b 2054 756d 6f72 2053  tegory); Tumor S
+00000d30: 7461 6765 2043 6c61 7373 6966 6963 6174  tage Classificat
+00000d40: 696f 6e3b 2061 7869 7320 690d 0a20 2020  ion; axis i..   
+00000d50: 2027 5432 3031 272c 2023 2043 6c69 6e69   'T201', # Clini
+00000d60: 6361 6c20 4174 7472 6962 7574 652c 2065  cal Attribute, e
+00000d70: 782e 3a20 426f 6e65 2044 656e 7369 7479  x.: Bone Density
+00000d80: 3b20 6865 6172 7420 7261 7465 3b20 5261  ; heart rate; Ra
+00000d90: 6e67 6520 6f66 204d 6f74 696f 6e2c 2041  nge of Motion, A
+00000da0: 7274 6963 756c 6172 0d0a 2020 2020 2754  rticular..    'T
+00000db0: 3230 3027 2c20 2320 436c 696e 6963 616c  200', # Clinical
+00000dc0: 2044 7275 672c 2065 782e 3a20 5261 6e69   Drug, ex.: Rani
+00000dd0: 7469 6469 6e65 2033 3030 204d 4720 4f72  tidine 300 MG Or
+00000de0: 616c 2054 6162 6c65 7420 5b5a 616e 7461  al Tablet [Zanta
+00000df0: 635d 3b20 4173 7069 7269 6e20 3330 3020  c]; Aspirin 300 
+00000e00: 4d47 2044 656c 6179 6564 2052 656c 6561  MG Delayed Relea
+00000e10: 7365 204f 7261 6c0d 0a20 2020 2023 2027  se Oral..    # '
+00000e20: 5430 3737 272c 2023 2043 6f6e 6365 7074  T077', # Concept
+00000e30: 7561 6c20 456e 7469 7479 2c20 6578 2e3a  ual Entity, ex.:
+00000e40: 2047 656f 6772 6170 6869 6320 4661 6374   Geographic Fact
+00000e50: 6f72 733b 2046 7261 6374 616c 733b 2053  ors; Fractals; S
+00000e60: 6563 756c 6172 6973 6d0d 0a20 2020 2023  ecularism..    #
+00000e70: 2027 5430 3139 272c 2023 2043 6f6e 6765   'T019', # Conge
+00000e80: 6e69 7461 6c20 4162 6e6f 726d 616c 6974  nital Abnormalit
+00000e90: 792c 2065 782e 3a20 416c 6269 6e69 736d  y, ex.: Albinism
+00000ea0: 3b20 436c 6566 7420 7061 6c61 7465 2077  ; Cleft palate w
+00000eb0: 6974 6820 636c 6566 7420 6c69 703b 2050  ith cleft lip; P
+00000ec0: 6f6c 7964 6163 7479 6c79 206f 6620 746f  olydactyly of to
+00000ed0: 6573 0d0a 2020 2020 2320 2754 3035 3627  es..    # 'T056'
+00000ee0: 2c20 2320 4461 696c 7920 6f72 2052 6563  , # Daily or Rec
+00000ef0: 7265 6174 696f 6e61 6c20 4163 7469 7669  reational Activi
+00000f00: 7479 2c20 6578 2e3a 2042 6164 6d69 6e74  ty, ex.: Badmint
+00000f10: 6f6e 3b20 4461 6e63 696e 673b 2053 7769  on; Dancing; Swi
+00000f20: 6d6d 696e 670d 0a20 2020 2027 5430 3630  mming..    'T060
+00000f30: 272c 2023 2044 6961 676e 6f73 7469 6320  ', # Diagnostic 
+00000f40: 5072 6f63 6564 7572 652c 2065 782e 3a20  Procedure, ex.: 
+00000f50: 4269 6f70 7379 3b20 4865 6172 7420 4175  Biopsy; Heart Au
+00000f60: 7363 756c 7461 7469 6f6e 3b20 4d61 676e  scultation; Magn
+00000f70: 6574 6963 2052 6573 6f6e 616e 6365 2049  etic Resonance I
+00000f80: 6d61 6769 6e67 0d0a 2020 2020 2754 3034  maging..    'T04
+00000f90: 3727 2c20 2320 4469 7365 6173 6520 6f72  7', # Disease or
+00000fa0: 2053 796e 6472 6f6d 652c 2065 782e 3a20   Syndrome, ex.: 
+00000fb0: 4469 6162 6574 6573 204d 656c 6c69 7475  Diabetes Mellitu
+00000fc0: 733b 2044 7275 6720 416c 6c65 7267 793b  s; Drug Allergy;
+00000fd0: 204d 616c 6162 736f 7270 7469 6f6e 2053   Malabsorption S
+00000fe0: 796e 6472 6f6d 650d 0a20 2020 2027 5432  yndrome..    'T2
+00000ff0: 3033 272c 2023 2044 7275 6720 4465 6c69  03', # Drug Deli
+00001000: 7665 7279 2044 6576 6963 652c 2065 782e  very Device, ex.
+00001010: 3a20 4e6f 7264 6574 7465 2032 3120 4461  : Nordette 21 Da
+00001020: 7920 5061 636b 3b20 7b37 2028 5465 7261  y Pack; {7 (Tera
+00001030: 7a6f 7369 6e20 3120 4d47 204f 7261 6c20  zosin 1 MG Oral 
+00001040: 5461 626c 6574 2920 2f20 3720 2854 6572  Tablet) / 7 (Ter
+00001050: 617a 6f73 696e 2032 204d 470d 0a20 2020  azosin 2 MG..   
+00001060: 2023 2027 5430 3635 272c 2023 2045 6475   # 'T065', # Edu
+00001070: 6361 7469 6f6e 616c 2041 6374 6976 6974  cational Activit
+00001080: 792c 2065 782e 3a20 4163 6164 656d 6963  y, ex.: Academic
+00001090: 2054 7261 696e 696e 673b 2046 616d 696c   Training; Famil
+000010a0: 7920 506c 616e 6e69 6e67 2054 7261 696e  y Planning Train
+000010b0: 696e 673b 2050 7265 6365 7074 6f72 7368  ing; Preceptorsh
+000010c0: 6970 0d0a 2020 2020 2320 2754 3139 3627  ip..    # 'T196'
+000010d0: 2c20 2320 456c 656d 656e 742c 2049 6f6e  , # Element, Ion
+000010e0: 2c20 6f72 2049 736f 746f 7065 2c20 6578  , or Isotope, ex
+000010f0: 2e3a 2043 6172 626f 6e3b 2043 6872 6f6d  .: Carbon; Chrom
+00001100: 6975 6d20 4973 6f74 6f70 6573 3b20 5261  ium Isotopes; Ra
+00001110: 6469 6f69 736f 746f 7065 730d 0a20 2020  dioisotopes..   
+00001120: 2023 2027 5430 3138 272c 2023 2045 6d62   # 'T018', # Emb
+00001130: 7279 6f6e 6963 2053 7472 7563 7475 7265  ryonic Structure
+00001140: 2c20 6578 2e3a 2042 6c61 7374 6f64 6572  , ex.: Blastoder
+00001150: 6d3b 2046 6574 7573 3b20 4e65 7572 616c  m; Fetus; Neural
+00001160: 2043 7265 7374 0d0a 2020 2020 2320 2754   Crest..    # 'T
+00001170: 3037 3127 2c20 2320 456e 7469 7479 2c20  071', # Entity, 
+00001180: 6578 2e3a 2047 6966 7473 2c20 4669 6e61  ex.: Gifts, Fina
+00001190: 6e63 6961 6c3b 2049 6d61 6765 3b20 5072  ncial; Image; Pr
+000011a0: 6f64 7563 7420 5061 7274 0d0a 2020 2020  oduct Part..    
+000011b0: 2320 2754 3036 3927 2c20 2320 456e 7669  # 'T069', # Envi
+000011c0: 726f 6e6d 656e 7461 6c20 4566 6665 6374  ronmental Effect
+000011d0: 206f 6620 4875 6d61 6e73 2c20 6578 2e3a   of Humans, ex.:
+000011e0: 2041 6972 2050 6f6c 6c75 7469 6f6e 3b20   Air Pollution; 
+000011f0: 4465 7365 7274 6966 6963 6174 696f 6e3b  Desertification;
+00001200: 2042 696f 7265 6d65 6469 6174 696f 6e0d   Bioremediation.
+00001210: 0a20 2020 2023 2027 5431 3236 272c 2023  .    # 'T126', #
+00001220: 2045 6e7a 796d 652c 2065 782e 3a20 4754   Enzyme, ex.: GT
+00001230: 5020 4379 636c 6f68 7964 726f 6c61 7365  P Cyclohydrolase
+00001240: 2049 493b 2065 6e7a 796d 6520 7375 6273   II; enzyme subs
+00001250: 7472 6174 6520 636f 6d70 6c65 783b 2061  trate complex; a
+00001260: 7267 696e 696e 6520 616d 6964 6173 650d  rginine amidase.
+00001270: 0a20 2020 2023 2027 5432 3034 272c 2023  .    # 'T204', #
+00001280: 2045 756b 6172 796f 7465 2c20 6578 2e3a   Eukaryote, ex.:
+00001290: 204f 7264 6572 2041 6361 7269 6e61 3b20   Order Acarina; 
+000012a0: 4265 6573 3b20 506c 6173 6d6f 6469 756d  Bees; Plasmodium
+000012b0: 206d 616c 6172 6961 650d 0a20 2020 2023   malariae..    #
+000012c0: 2027 5430 3531 272c 2023 2045 7665 6e74   'T051', # Event
+000012d0: 2c20 6578 2e3a 2041 6e6e 6976 6572 7361  , ex.: Anniversa
+000012e0: 7269 6573 3b20 4578 706f 7375 7265 2074  ries; Exposure t
+000012f0: 6f20 4d75 6d70 7320 7669 7275 7320 2865  o Mumps virus (e
+00001300: 7665 6e74 293b 2044 6576 6963 6520 556e  vent); Device Un
+00001310: 6174 7465 6e64 6564 0d0a 2020 2020 2320  attended..    # 
+00001320: 2754 3035 3027 2c20 2320 4578 7065 7269  'T050', # Experi
+00001330: 6d65 6e74 616c 204d 6f64 656c 206f 6620  mental Model of 
+00001340: 4469 7365 6173 652c 2065 782e 3a20 416c  Disease, ex.: Al
+00001350: 6c6f 7861 6e20 4469 6162 6574 6573 3b20  loxan Diabetes; 
+00001360: 4c69 7665 7220 4369 7272 686f 7369 732c  Liver Cirrhosis,
+00001370: 2045 7870 6572 696d 656e 7461 6c3b 2054   Experimental; T
+00001380: 7261 6e73 6965 6e74 2047 656e 6520 4b6e  ransient Gene Kn
+00001390: 6f63 6b2d 4f75 740d 0a20 2020 2023 2027  ock-Out..    # '
+000013a0: 5430 3939 272c 2023 2046 616d 696c 7920  T099', # Family 
+000013b0: 4772 6f75 702c 2065 782e 3a20 4461 7567  Group, ex.: Daug
+000013c0: 6874 6572 3b20 4973 2061 6e20 6f6e 6c79  hter; Is an only
+000013d0: 2063 6869 6c64 3b20 556e 6d61 7272 6965   child; Unmarrie
+000013e0: 6420 4661 7468 6572 730d 0a20 2020 2027  d Fathers..    '
+000013f0: 5430 3333 272c 2023 2046 696e 6469 6e67  T033', # Finding
+00001400: 2c20 6578 2e3a 2042 6972 7468 2048 6973  , ex.: Birth His
+00001410: 746f 7279 3b20 446f 776e 7761 7264 2064  tory; Downward d
+00001420: 6973 706c 6163 656d 656e 7420 6f66 2064  isplacement of d
+00001430: 6961 7068 7261 676d 3b20 4465 6372 6561  iaphragm; Decrea
+00001440: 7365 6420 676c 7563 6f73 6520 6c65 7665  sed glucose leve
+00001450: 6c0d 0a20 2020 2023 2027 5430 3133 272c  l..    # 'T013',
+00001460: 2023 2046 6973 682c 2065 782e 3a20 4261   # Fish, ex.: Ba
+00001470: 7373 3b20 5361 6c6d 6f6e 6964 6165 3b20  ss; Salmonidae; 
+00001480: 5768 6974 6566 6973 680d 0a20 2020 2023  Whitefish..    #
+00001490: 2027 5431 3638 272c 2023 2046 6f6f 642c   'T168', # Food,
+000014a0: 2065 782e 3a20 4265 7665 7261 6765 733b   ex.: Beverages;
+000014b0: 2045 6767 2059 6f6c 6b20 2844 6965 7461   Egg Yolk (Dieta
+000014c0: 7279 293b 2049 6365 2043 7265 616d 0d0a  ry); Ice Cream..
+000014d0: 2020 2020 2320 2754 3032 3127 2c20 2320      # 'T021', # 
+000014e0: 4675 6c6c 7920 466f 726d 6564 2041 6e61  Fully Formed Ana
+000014f0: 746f 6d69 6361 6c20 5374 7275 6374 7572  tomical Structur
+00001500: 652c 2065 782e 3a20 456e 7469 7265 2062  e, ex.: Entire b
+00001510: 6f64 7920 6173 2061 2077 686f 6c65 3b20  ody as a whole; 
+00001520: 4665 6d61 6c65 2068 756d 616e 2062 6f64  Female human bod
+00001530: 793b 2053 6574 206f 6620 7061 7274 7320  y; Set of parts 
+00001540: 6f66 2068 756d 616e 2062 6f64 790d 0a20  of human body.. 
+00001550: 2020 2023 2027 5431 3639 272c 2023 2046     # 'T169', # F
+00001560: 756e 6374 696f 6e61 6c20 436f 6e63 6570  unctional Concep
+00001570: 742c 2065 782e 3a20 496e 7465 7276 6965  t, ex.: Intervie
+00001580: 7765 7220 4566 6665 6374 3b20 5072 6f62  wer Effect; Prob
+00001590: 6c65 6d20 466f 726d 756c 6174 696f 6e3b  lem Formulation;
+000015a0: 2045 6e64 6f67 656e 6f75 730d 0a20 2020   Endogenous..   
+000015b0: 2023 2027 5430 3034 272c 2023 2046 756e   # 'T004', # Fun
+000015c0: 6775 732c 2065 782e 3a20 4173 7065 7267  gus, ex.: Asperg
+000015d0: 696c 6c75 7320 636c 6176 6174 7573 3b20  illus clavatus; 
+000015e0: 426c 6173 746f 6d79 6365 733b 204e 6575  Blastomyces; Neu
+000015f0: 726f 7370 6f72 610d 0a20 2020 2023 2027  rospora..    # '
+00001600: 5430 3238 272c 2023 2047 656e 6520 6f72  T028', # Gene or
+00001610: 2047 656e 6f6d 652c 2065 782e 3a20 416c   Genome, ex.: Al
+00001620: 6c65 6c65 733b 2047 656e 6f6d 652c 2048  leles; Genome, H
+00001630: 756d 616e 3b20 7252 4e41 204f 7065 726f  uman; rRNA Opero
+00001640: 6e0d 0a20 2020 2023 2027 5430 3435 272c  n..    # 'T045',
+00001650: 2023 2047 656e 6574 6963 2046 756e 6374   # Genetic Funct
+00001660: 696f 6e2c 2065 782e 3a20 4561 726c 7920  ion, ex.: Early 
+00001670: 4765 6e65 2054 7261 6e73 6372 6970 7469  Gene Transcripti
+00001680: 6f6e 3b20 4765 6e65 2041 6d70 6c69 6669  on; Gene Amplifi
+00001690: 6361 7469 6f6e 3b20 524e 4120 5370 6c69  cation; RNA Spli
+000016a0: 6369 6e67 0d0a 2020 2020 2320 2754 3038  cing..    # 'T08
+000016b0: 3327 2c20 2320 4765 6f67 7261 7068 6963  3', # Geographic
+000016c0: 2041 7265 612c 2065 782e 3a20 4261 6c74   Area, ex.: Balt
+000016d0: 696d 6f72 653b 2043 616e 6164 613b 2046  imore; Canada; F
+000016e0: 6172 2045 6173 740d 0a20 2020 2023 2027  ar East..    # '
+000016f0: 5430 3634 272c 2023 2047 6f76 6572 6e6d  T064', # Governm
+00001700: 656e 7461 6c20 6f72 2052 6567 756c 6174  ental or Regulat
+00001710: 6f72 7920 4163 7469 7669 7479 2c20 6578  ory Activity, ex
+00001720: 2e3a 2043 6572 7469 6669 6361 7469 6f6e  .: Certification
+00001730: 3b20 4372 6564 656e 7469 616c 696e 673b  ; Credentialing;
+00001740: 2050 7562 6c69 6320 506f 6c69 6379 0d0a   Public Policy..
+00001750: 2020 2020 2320 2754 3039 3627 2c20 2320      # 'T096', # 
+00001760: 4772 6f75 702c 2065 782e 3a20 466f 6375  Group, ex.: Focu
+00001770: 7320 4772 6f75 7073 3b20 6a75 7279 3b20  s Groups; jury; 
+00001780: 7465 616d 730d 0a20 2020 2023 2027 5431  teams..    # 'T1
+00001790: 3032 272c 2023 2047 726f 7570 2041 7474  02', # Group Att
+000017a0: 7269 6275 7465 2c20 6578 2e3a 2046 616d  ribute, ex.: Fam
+000017b0: 696c 7920 5369 7a65 3b20 4772 6f75 7020  ily Size; Group 
+000017c0: 5374 7275 6374 7572 653b 204c 6966 6520  Structure; Life 
+000017d0: 4578 7065 6374 616e 6379 0d0a 2020 2020  Expectancy..    
+000017e0: 2320 2754 3133 3127 2c20 2320 4861 7a61  # 'T131', # Haza
+000017f0: 7264 6f75 7320 6f72 2050 6f69 736f 6e6f  rdous or Poisono
+00001800: 7573 2053 7562 7374 616e 6365 2c20 6578  us Substance, ex
+00001810: 2e3a 2043 6172 6369 6e6f 6765 6e73 3b20  .: Carcinogens; 
+00001820: 4675 6d69 6761 6e74 3b20 4d75 7461 6765  Fumigant; Mutage
+00001830: 6e73 0d0a 2020 2020 2754 3035 3827 2c20  ns..    'T058', 
+00001840: 2320 4865 616c 7468 2043 6172 6520 4163  # Health Care Ac
+00001850: 7469 7669 7479 2c20 6578 2e3a 2061 6d62  tivity, ex.: amb
+00001860: 756c 6174 6f72 7920 6361 7265 2073 6572  ulatory care ser
+00001870: 7669 6365 733b 2043 6c69 6e69 6320 4163  vices; Clinic Ac
+00001880: 7469 7669 7469 6573 3b20 5072 6576 656e  tivities; Preven
+00001890: 7469 7665 2048 6561 6c74 6820 5365 7276  tive Health Serv
+000018a0: 6963 6573 0d0a 2020 2020 2320 2754 3039  ices..    # 'T09
+000018b0: 3327 2c20 2320 4865 616c 7468 2043 6172  3', # Health Car
+000018c0: 6520 5265 6c61 7465 6420 4f72 6761 6e69  e Related Organi
+000018d0: 7a61 7469 6f6e 2c20 6578 2e3a 2043 656e  zation, ex.: Cen
+000018e0: 7465 7273 2066 6f72 2044 6973 6561 7365  ters for Disease
+000018f0: 2043 6f6e 7472 6f6c 2061 6e64 2050 7265   Control and Pre
+00001900: 7665 6e74 696f 6e20 2855 2e53 2e29 3b20  vention (U.S.); 
+00001910: 4861 6c66 7761 7920 486f 7573 6573 3b0d  Halfway Houses;.
+00001920: 0a20 2020 2023 2027 5431 3235 272c 2023  .    # 'T125', #
+00001930: 2048 6f72 6d6f 6e65 2c20 6578 2e3a 2045   Hormone, ex.: E
+00001940: 6e74 6572 6963 2048 6f72 6d6f 6e65 733b  nteric Hormones;
+00001950: 2074 6879 6d69 6320 6875 6d6f 7261 6c20   thymic humoral 
+00001960: 6661 6374 6f72 3b20 5072 6f68 6f72 6d6f  factor; Prohormo
+00001970: 6e65 0d0a 2020 2020 2320 2754 3031 3627  ne..    # 'T016'
+00001980: 2c20 2320 4875 6d61 6e2c 2065 782e 3a20  , # Human, ex.: 
+00001990: 486f 6d6f 2073 6170 6965 6e73 3b20 6a65  Homo sapiens; je
+000019a0: 616e 2070 6961 6765 743b 204d 656d 6265  an piaget; Membe
+000019b0: 7220 6f66 2070 7562 6c69 630d 0a20 2020  r of public..   
+000019c0: 2023 2027 5430 3638 272c 2023 2048 756d   # 'T068', # Hum
+000019d0: 616e 2d63 6175 7365 6420 5068 656e 6f6d  an-caused Phenom
+000019e0: 656e 6f6e 206f 7220 5072 6f63 6573 732c  enon or Process,
+000019f0: 2065 782e 3a20 4261 6279 2042 6f6f 6d3b   ex.: Baby Boom;
+00001a00: 2043 756c 7475 7261 6c20 4576 6f6c 7574   Cultural Evolut
+00001a10: 696f 6e3b 204d 6173 7320 4d65 6469 610d  ion; Mass Media.
+00001a20: 0a20 2020 2023 2027 5430 3738 272c 2023  .    # 'T078', #
+00001a30: 2049 6465 6120 6f72 2043 6f6e 6365 7074   Idea or Concept
+00001a40: 2c20 6578 2e3a 2043 6170 6974 616c 6973  , ex.: Capitalis
+00001a50: 6d3b 2043 6976 696c 2052 6967 6874 733b  m; Civil Rights;
+00001a60: 2045 7468 6963 730d 0a20 2020 2023 2027   Ethics..    # '
+00001a70: 5431 3239 272c 2023 2049 6d6d 756e 6f6c  T129', # Immunol
+00001a80: 6f67 6963 2046 6163 746f 722c 2065 782e  ogic Factor, ex.
+00001a90: 3a20 416e 7469 6765 6e73 3b20 496d 6d75  : Antigens; Immu
+00001aa0: 6e6f 6c6f 6769 6320 4661 6374 6f72 733b  nologic Factors;
+00001ab0: 2042 6c6f 6f64 2067 726f 7570 2061 6e74   Blood group ant
+00001ac0: 6967 656e 2050 0d0a 2020 2020 2754 3133  igen P..    'T13
+00001ad0: 3027 2c20 2320 496e 6469 6361 746f 722c  0', # Indicator,
+00001ae0: 2052 6561 6765 6e74 2c20 6f72 2044 6961   Reagent, or Dia
+00001af0: 676e 6f73 7469 6320 4169 642c 2065 782e  gnostic Aid, ex.
+00001b00: 3a20 466c 756f 7265 7363 656e 7420 4479  : Fluorescent Dy
+00001b10: 6573 3b20 496e 6469 6361 746f 7273 2061  es; Indicators a
+00001b20: 6e64 2052 6561 6765 6e74 733b 2049 6e64  nd Reagents; Ind
+00001b30: 6961 2069 6e6b 2073 7461 696e 0d0a 2020  ia ink stain..  
+00001b40: 2020 2320 2754 3035 3527 2c20 2320 496e    # 'T055', # In
+00001b50: 6469 7669 6475 616c 2042 6568 6176 696f  dividual Behavio
+00001b60: 722c 2065 782e 3a20 4173 7365 7274 6976  r, ex.: Assertiv
+00001b70: 656e 6573 733b 2047 726f 6f6d 696e 673b  eness; Grooming;
+00001b80: 2052 6973 6b2d 5461 6b69 6e67 0d0a 2020   Risk-Taking..  
+00001b90: 2020 2754 3033 3727 2c20 2320 496e 6a75    'T037', # Inju
+00001ba0: 7279 206f 7220 506f 6973 6f6e 696e 672c  ry or Poisoning,
+00001bb0: 2065 782e 3a20 4163 6369 6465 6e74 616c   ex.: Accidental
+00001bc0: 2046 616c 6c73 3b20 4361 7262 6f6e 204d   Falls; Carbon M
+00001bd0: 6f6e 6f78 6964 6520 506f 6973 6f6e 696e  onoxide Poisonin
+00001be0: 673b 2053 6e61 6b65 2042 6974 6573 0d0a  g; Snake Bites..
+00001bf0: 2020 2020 2320 2754 3139 3727 2c20 2320      # 'T197', # 
+00001c00: 496e 6f72 6761 6e69 6320 4368 656d 6963  Inorganic Chemic
+00001c10: 616c 2c20 6578 2e3a 2043 6172 626f 6e69  al, ex.: Carboni
+00001c20: 6320 4163 6964 3b20 616c 756d 696e 756d  c Acid; aluminum
+00001c30: 206e 6974 7269 6465 3b20 6665 7272 6963   nitride; ferric
+00001c40: 2063 6974 7261 7465 0d0a 2020 2020 2754   citrate..    'T
+00001c50: 3137 3027 2c20 2320 496e 7465 6c6c 6563  170', # Intellec
+00001c60: 7475 616c 2050 726f 6475 6374 2c20 6578  tual Product, ex
+00001c70: 2e3a 2044 6563 6973 696f 6e20 5375 7070  .: Decision Supp
+00001c80: 6f72 7420 5465 6368 6e69 7175 6573 3b20  ort Techniques; 
+00001c90: 496e 666f 726d 6174 696f 6e20 5379 7374  Information Syst
+00001ca0: 656d 733b 204c 6974 6572 6174 7572 650d  ems; Literature.
+00001cb0: 0a20 2020 2027 5430 3334 272c 2023 204c  .    'T034', # L
+00001cc0: 6162 6f72 6174 6f72 7920 6f72 2054 6573  aboratory or Tes
+00001cd0: 7420 5265 7375 6c74 2c20 6578 2e3a 2042  t Result, ex.: B
+00001ce0: 6c6f 6f64 2046 6c6f 7720 5665 6c6f 6369  lood Flow Veloci
+00001cf0: 7479 3b20 5365 7275 6d20 4361 6c63 6975  ty; Serum Calciu
+00001d00: 6d20 4c65 7665 6c3b 2053 7069 6e61 6c20  m Level; Spinal 
+00001d10: 466c 7569 6420 5072 6573 7375 7265 0d0a  Fluid Pressure..
+00001d20: 2020 2020 2754 3035 3927 2c20 2320 4c61      'T059', # La
+00001d30: 626f 7261 746f 7279 2050 726f 6365 6475  boratory Procedu
+00001d40: 7265 2c20 6578 2e3a 2042 6c6f 6f64 2050  re, ex.: Blood P
+00001d50: 726f 7465 696e 2045 6c65 6374 726f 7068  rotein Electroph
+00001d60: 6f72 6573 6973 3b20 4372 7973 7461 6c6c  oresis; Crystall
+00001d70: 6f67 7261 7068 793b 2052 6164 696f 696d  ography; Radioim
+00001d80: 6d75 6e6f 6173 7361 790d 0a20 2020 2023  munoassay..    #
+00001d90: 2027 5431 3731 272c 2023 204c 616e 6775   'T171', # Langu
+00001da0: 6167 652c 2065 782e 3a20 4172 6d65 6e69  age, ex.: Armeni
+00001db0: 616e 206c 616e 6775 6167 653b 2062 7261  an language; bra
+00001dc0: 696c 6c65 3b20 4269 6c69 6e67 7561 6c69  ille; Bilinguali
+00001dd0: 736d 0d0a 2020 2020 2320 2754 3036 3627  sm..    # 'T066'
+00001de0: 2c20 2320 4d61 6368 696e 6520 4163 7469  , # Machine Acti
+00001df0: 7669 7479 2c20 6578 2e3a 2043 6f6d 7075  vity, ex.: Compu
+00001e00: 7465 7220 5369 6d75 6c61 7469 6f6e 3b20  ter Simulation; 
+00001e10: 4571 7569 706d 656e 7420 4661 696c 7572  Equipment Failur
+00001e20: 653b 204e 6174 7572 616c 204c 616e 6775  e; Natural Langu
+00001e30: 6167 6520 5072 6f63 6573 7369 6e67 0d0a  age Processing..
+00001e40: 2020 2020 2320 2754 3031 3527 2c20 2320      # 'T015', # 
+00001e50: 4d61 6d6d 616c 2c20 6578 2e3a 2055 7273  Mammal, ex.: Urs
+00001e60: 6964 6165 2046 616d 696c 793b 2048 616d  idae Family; Ham
+00001e70: 7374 6572 733b 204d 6163 6163 610d 0a20  sters; Macaca.. 
+00001e80: 2020 2023 2027 5430 3733 272c 2023 204d     # 'T073', # M
+00001e90: 616e 7566 6163 7475 7265 6420 4f62 6a65  anufactured Obje
+00001ea0: 6374 2c20 6578 2e3a 2063 6172 2073 6561  ct, ex.: car sea
+00001eb0: 743b 2043 6f6f 6b69 6e67 2061 6e64 2045  t; Cooking and E
+00001ec0: 6174 696e 6720 5574 656e 7369 6c73 3b20  ating Utensils; 
+00001ed0: 476f 6767 6c65 730d 0a20 2020 2027 5430  Goggles..    'T0
+00001ee0: 3734 272c 2023 204d 6564 6963 616c 2044  74', # Medical D
+00001ef0: 6576 6963 652c 2065 782e 3a20 426f 6e65  evice, ex.: Bone
+00001f00: 2053 6372 6577 733b 2048 6561 6467 6561   Screws; Headgea
+00001f10: 722c 204f 7274 686f 646f 6e74 6963 3b20  r, Orthodontic; 
+00001f20: 436f 6d70 7265 7373 696f 6e20 5374 6f63  Compression Stoc
+00001f30: 6b69 6e67 730d 0a20 2020 2027 5430 3438  kings..    'T048
+00001f40: 272c 2023 204d 656e 7461 6c20 6f72 2042  ', # Mental or B
+00001f50: 6568 6176 696f 7261 6c20 4479 7366 756e  ehavioral Dysfun
+00001f60: 6374 696f 6e2c 2065 782e 3a20 4167 6f72  ction, ex.: Agor
+00001f70: 6170 686f 6269 613b 2043 7963 6c6f 7468  aphobia; Cycloth
+00001f80: 796d 6963 2044 6973 6f72 6465 723b 2046  ymic Disorder; F
+00001f90: 7269 6769 6469 7479 0d0a 2020 2020 2754  rigidity..    'T
+00001fa0: 3034 3127 2c20 2320 4d65 6e74 616c 2050  041', # Mental P
+00001fb0: 726f 6365 7373 2c20 6578 2e3a 2041 6e67  rocess, ex.: Ang
+00001fc0: 6572 3b20 4175 6469 746f 7279 2046 6174  er; Auditory Fat
+00001fd0: 6967 7565 3b20 4176 6f69 6461 6e63 6520  igue; Avoidance 
+00001fe0: 4c65 6172 6e69 6e67 0d0a 2020 2020 2320  Learning..    # 
+00001ff0: 2754 3036 3327 2c20 2320 4d6f 6c65 6375  'T063', # Molecu
+00002000: 6c61 7220 4269 6f6c 6f67 7920 5265 7365  lar Biology Rese
+00002010: 6172 6368 2054 6563 686e 6971 7565 2c20  arch Technique, 
+00002020: 6578 2e3a 204e 6f72 7468 6572 6e20 426c  ex.: Northern Bl
+00002030: 6f74 7469 6e67 3b20 4765 6e65 7469 6320  otting; Genetic 
+00002040: 456e 6769 6e65 6572 696e 673b 2049 6e20  Engineering; In 
+00002050: 5369 7475 2048 7962 7269 6469 7a61 7469  Situ Hybridizati
+00002060: 6f6e 0d0a 2020 2020 2320 2754 3034 3427  on..    # 'T044'
+00002070: 2c20 2320 4d6f 6c65 6375 6c61 7220 4675  , # Molecular Fu
+00002080: 6e63 7469 6f6e 2c20 6578 2e3a 2042 696e  nction, ex.: Bin
+00002090: 6469 6e67 2c20 436f 6d70 6574 6974 6976  ding, Competitiv
+000020a0: 653b 2045 6c65 6374 726f 6e20 5472 616e  e; Electron Tran
+000020b0: 7370 6f72 743b 2047 6c79 636f 6c79 7369  sport; Glycolysi
+000020c0: 730d 0a20 2020 2023 2027 5430 3835 272c  s..    # 'T085',
+000020d0: 2023 204d 6f6c 6563 756c 6172 2053 6571   # Molecular Seq
+000020e0: 7565 6e63 652c 2065 782e 3a20 4765 6e65  uence, ex.: Gene
+000020f0: 7469 6320 436f 6465 3b20 486f 6d6f 6c6f  tic Code; Homolo
+00002100: 676f 7573 2053 6571 7565 6e63 6573 3b20  gous Sequences; 
+00002110: 4d6f 6c65 6375 6c61 7220 5365 7175 656e  Molecular Sequen
+00002120: 6365 0d0a 2020 2020 2320 2754 3037 3027  ce..    # 'T070'
+00002130: 2c20 2320 4e61 7475 7261 6c20 5068 656e  , # Natural Phen
+00002140: 6f6d 656e 6f6e 206f 7220 5072 6f63 6573  omenon or Proces
+00002150: 732c 2065 782e 3a20 4169 7220 4d6f 7665  s, ex.: Air Move
+00002160: 6d65 6e74 733b 2043 6f72 726f 7369 6f6e  ments; Corrosion
+00002170: 3b20 4c69 6768 746e 696e 6720 2870 6865  ; Lightning (phe
+00002180: 6e6f 6d65 6e6f 6e29 0d0a 2020 2020 2754  nomenon)..    'T
+00002190: 3139 3127 2c20 2320 4e65 6f70 6c61 7374  191', # Neoplast
+000021a0: 6963 2050 726f 6365 7373 2c20 6578 2e3a  ic Process, ex.:
+000021b0: 2041 6264 6f6d 696e 616c 204e 656f 706c   Abdominal Neopl
+000021c0: 6173 6d73 3b20 426f 7765 6e27 7320 4469  asms; Bowen's Di
+000021d0: 7365 6173 653b 2050 6f6c 7970 2069 6e20  sease; Polyp in 
+000021e0: 6e61 736f 7068 6172 796e 780d 0a20 2020  nasopharynx..   
+000021f0: 2023 2027 5431 3134 272c 2023 204e 7563   # 'T114', # Nuc
+00002200: 6c65 6963 2041 6369 642c 204e 7563 6c65  leic Acid, Nucle
+00002210: 6f73 6964 652c 206f 7220 4e75 636c 656f  oside, or Nucleo
+00002220: 7469 6465 2c20 6578 2e3a 2043 7974 6f73  tide, ex.: Cytos
+00002230: 696e 6520 4e75 636c 656f 7469 6465 733b  ine Nucleotides;
+00002240: 2047 7561 6e69 6e65 3b20 4f6c 6967 6f6e   Guanine; Oligon
+00002250: 7563 6c65 6f74 6964 6573 0d0a 2020 2020  ucleotides..    
+00002260: 2320 2754 3038 3627 2c20 2320 4e75 636c  # 'T086', # Nucl
+00002270: 656f 7469 6465 2053 6571 7565 6e63 652c  eotide Sequence,
+00002280: 2065 782e 3a20 4261 7365 2053 6571 7565   ex.: Base Seque
+00002290: 6e63 653b 2044 6972 6563 7420 5265 7065  nce; Direct Repe
+000022a0: 6174 3b20 524e 4120 5365 7175 656e 6365  at; RNA Sequence
+000022b0: 0d0a 2020 2020 2320 2754 3039 3027 2c20  ..    # 'T090', 
+000022c0: 2320 4f63 6375 7061 7469 6f6e 206f 7220  # Occupation or 
+000022d0: 4469 7363 6970 6c69 6e65 2c20 6578 2e3a  Discipline, ex.:
+000022e0: 2041 7669 6174 696f 6e3b 2043 7261 6e69   Aviation; Crani
+000022f0: 6f6c 6f67 793b 2045 636f 6c6f 6779 0d0a  ology; Ecology..
+00002300: 2020 2020 2320 2754 3035 3727 2c20 2320      # 'T057', # 
+00002310: 4f63 6375 7061 7469 6f6e 616c 2041 6374  Occupational Act
+00002320: 6976 6974 792c 2065 782e 3a20 436f 6c6c  ivity, ex.: Coll
+00002330: 6563 7469 7665 2042 6172 6761 696e 696e  ective Bargainin
+00002340: 673b 2043 6f6d 6d65 7263 653b 2043 6f6e  g; Commerce; Con
+00002350: 7461 696e 6d65 6e74 206f 6620 4269 6f68  tainment of Bioh
+00002360: 617a 6172 6473 0d0a 2020 2020 2320 2754  azards..    # 'T
+00002370: 3034 3227 2c20 2320 4f72 6761 6e20 6f72  042', # Organ or
+00002380: 2054 6973 7375 6520 4675 6e63 7469 6f6e   Tissue Function
+00002390: 2c20 6578 2e3a 204f 7374 656f 6765 6e65  , ex.: Osteogene
+000023a0: 7369 733b 2052 656e 616c 2043 6972 6375  sis; Renal Circu
+000023b0: 6c61 7469 6f6e 3b20 546f 6f74 6820 4361  lation; Tooth Ca
+000023c0: 6c63 6966 6963 6174 696f 6e0d 0a20 2020  lcification..   
+000023d0: 2023 2027 5431 3039 272c 2023 204f 7267   # 'T109', # Org
+000023e0: 616e 6963 2043 6865 6d69 6361 6c2c 2065  anic Chemical, e
+000023f0: 782e 3a20 4265 6e7a 656e 6520 4465 7269  x.: Benzene Deri
+00002400: 7661 7469 7665 730d 0a20 2020 2023 2027  vatives..    # '
+00002410: 5430 3031 272c 2023 204f 7267 616e 6973  T001', # Organis
+00002420: 6d2c 2065 782e 3a20 4f72 6761 6e69 736d  m, ex.: Organism
+00002430: 3b20 496e 6665 6374 696f 7573 2061 6765  ; Infectious age
+00002440: 6e74 3b20 4865 7465 726f 7472 6f70 680d  nt; Heterotroph.
+00002450: 0a20 2020 2023 2027 5430 3332 272c 2023  .    # 'T032', #
+00002460: 204f 7267 616e 6973 6d20 4174 7472 6962   Organism Attrib
+00002470: 7574 652c 2065 782e 3a20 4167 653b 2042  ute, ex.: Age; B
+00002480: 6972 7468 2057 6569 6768 743b 2045 7965  irth Weight; Eye
+00002490: 2043 6f6c 6f72 0d0a 2020 2020 2754 3034   Color..    'T04
+000024a0: 3027 2c20 2320 4f72 6761 6e69 736d 2046  0', # Organism F
+000024b0: 756e 6374 696f 6e2c 2065 782e 3a20 4272  unction, ex.: Br
+000024c0: 6565 6469 6e67 3b20 4869 6265 726e 6174  eeding; Hibernat
+000024d0: 696f 6e3b 204d 6f74 6f72 2053 6b69 6c6c  ion; Motor Skill
+000024e0: 730d 0a20 2020 2023 2027 5430 3932 272c  s..    # 'T092',
+000024f0: 2023 204f 7267 616e 697a 6174 696f 6e2c   # Organization,
+00002500: 2065 782e 3a20 4c61 626f 7220 556e 696f   ex.: Labor Unio
+00002510: 6e73 3b20 556e 6974 6564 204e 6174 696f  ns; United Natio
+00002520: 6e73 3b20 426f 6172 6469 6e67 2073 6368  ns; Boarding sch
+00002530: 6f6f 6c0d 0a20 2020 2027 5430 3436 272c  ool..    'T046',
+00002540: 2023 2050 6174 686f 6c6f 6769 6320 4675   # Pathologic Fu
+00002550: 6e63 7469 6f6e 2c20 6578 2e3a 2049 6e66  nction, ex.: Inf
+00002560: 6c61 6d6d 6174 696f 6e3b 2053 686f 636b  lammation; Shock
+00002570: 3b20 5468 726f 6d62 6f73 6973 0d0a 2020  ; Thrombosis..  
+00002580: 2020 2320 2754 3130 3127 2c20 2320 5061    # 'T101', # Pa
+00002590: 7469 656e 7420 6f72 2044 6973 6162 6c65  tient or Disable
+000025a0: 6420 4772 6f75 702c 2065 782e 3a20 416d  d Group, ex.: Am
+000025b0: 7075 7465 6573 3b20 496e 7374 6974 7574  putees; Institut
+000025c0: 696f 6e61 6c69 7a65 6420 4368 696c 643b  ionalized Child;
+000025d0: 204d 656e 7461 6c6c 7920 496c 6c20 5065   Mentally Ill Pe
+000025e0: 7273 6f6e 730d 0a20 2020 2027 5431 3231  rsons..    'T121
+000025f0: 272c 2023 2050 6861 726d 6163 6f6c 6f67  ', # Pharmacolog
+00002600: 6963 2053 7562 7374 616e 6365 2c20 6578  ic Substance, ex
+00002610: 2e3a 2041 6e74 6965 6d65 7469 6373 3b20  .: Antiemetics; 
+00002620: 4361 7264 696f 7661 7363 756c 6172 2041  Cardiovascular A
+00002630: 6765 6e74 733b 2041 6c6b 612d 5365 6c74  gents; Alka-Selt
+00002640: 7a65 720d 0a20 2020 2027 5430 3637 272c  zer..    'T067',
+00002650: 2023 2050 6865 6e6f 6d65 6e6f 6e20 6f72   # Phenomenon or
+00002660: 2050 726f 6365 7373 2c20 6578 2e3a 2044   Process, ex.: D
+00002670: 6973 6173 7465 7273 3b20 4d6f 746f 7220  isasters; Motor 
+00002680: 5472 6166 6669 6320 4163 6369 6465 6e74  Traffic Accident
+00002690: 733b 2044 6570 6f6c 796d 6572 697a 6174  s; Depolymerizat
+000026a0: 696f 6e0d 0a20 2020 2023 2027 5430 3732  ion..    # 'T072
+000026b0: 272c 2023 2050 6879 7369 6361 6c20 4f62  ', # Physical Ob
+000026c0: 6a65 6374 2c20 6578 2e3a 2050 7269 6e74  ject, ex.: Print
+000026d0: 6564 204d 6564 6961 3b20 4d65 7465 6f72  ed Media; Meteor
+000026e0: 733b 2050 6879 7369 6361 6c20 6f62 6a65  s; Physical obje
+000026f0: 6374 0d0a 2020 2020 2754 3033 3927 2c20  ct..    'T039', 
+00002700: 2320 5068 7973 696f 6c6f 6769 6320 4675  # Physiologic Fu
+00002710: 6e63 7469 6f6e 2c20 6578 2e3a 2042 696f  nction, ex.: Bio
+00002720: 7268 7974 686d 733b 2048 6561 7269 6e67  rhythms; Hearing
+00002730: 3b20 5661 736f 6469 6c61 7469 6f6e 0d0a  ; Vasodilation..
+00002740: 2020 2020 2320 2754 3030 3227 2c20 2320      # 'T002', # 
+00002750: 506c 616e 742c 2065 782e 3a20 416c 6f65  Plant, ex.: Aloe
+00002760: 3b20 506f 6c6c 656e 3b20 4865 6c69 616e  ; Pollen; Helian
+00002770: 7468 7573 2073 7065 6369 6573 0d0a 2020  thus species..  
+00002780: 2020 2320 2754 3039 3827 2c20 2320 506f    # 'T098', # Po
+00002790: 7075 6c61 7469 6f6e 2047 726f 7570 2c20  pulation Group, 
+000027a0: 6578 2e3a 2041 7369 616e 2041 6d65 7269  ex.: Asian Ameri
+000027b0: 6361 6e73 3b20 4574 686e 6963 2067 726f  cans; Ethnic gro
+000027c0: 7570 3b20 4164 756c 7420 4f66 6665 6e64  up; Adult Offend
+000027d0: 6572 730d 0a20 2020 2023 2027 5430 3937  ers..    # 'T097
+000027e0: 272c 2023 2050 726f 6665 7373 696f 6e61  ', # Professiona
+000027f0: 6c20 6f72 204f 6363 7570 6174 696f 6e61  l or Occupationa
+00002800: 6c20 4772 6f75 702c 2065 782e 3a20 436c  l Group, ex.: Cl
+00002810: 6572 6779 3b20 4465 6d6f 6772 6170 6865  ergy; Demographe
+00002820: 7273 3b20 486f 7370 6974 616c 2056 6f6c  rs; Hospital Vol
+00002830: 756e 7465 6572 730d 0a20 2020 2023 2027  unteers..    # '
+00002840: 5430 3934 272c 2023 2050 726f 6665 7373  T094', # Profess
+00002850: 696f 6e61 6c20 536f 6369 6574 792c 2065  ional Society, e
+00002860: 782e 3a20 416d 6572 6963 616e 204d 6564  x.: American Med
+00002870: 6963 616c 2041 7373 6f63 6961 7469 6f6e  ical Association
+00002880: 3b20 496e 7465 726e 6174 696f 6e61 6c20  ; International 
+00002890: 436f 756e 6369 6c20 6f66 204e 7572 7365  Council of Nurse
+000028a0: 733b 204c 6962 7261 7279 0d0a 2020 2020  s; Library..    
+000028b0: 2320 2754 3038 3027 2c20 2320 5175 616c  # 'T080', # Qual
+000028c0: 6974 6174 6976 6520 436f 6e63 6570 742c  itative Concept,
+000028d0: 2065 782e 3a20 436c 696e 6963 616c 2043   ex.: Clinical C
+000028e0: 6f6d 7065 7465 6e63 653b 2043 6f6e 7375  ompetence; Consu
+000028f0: 6d65 7220 5361 7469 7366 6163 7469 6f6e  mer Satisfaction
+00002900: 3b20 4865 616c 7468 2053 7461 7475 730d  ; Health Status.
+00002910: 0a20 2020 2023 2027 5430 3831 272c 2023  .    # 'T081', #
+00002920: 2051 7561 6e74 6974 6174 6976 6520 436f   Quantitative Co
+00002930: 6e63 6570 742c 2065 782e 3a20 4167 6520  ncept, ex.: Age 
+00002940: 4469 7374 7269 6275 7469 6f6e 3b20 4d65  Distribution; Me
+00002950: 7472 6963 2053 7973 7465 6d3b 2053 656c  tric System; Sel
+00002960: 6563 7469 6f6e 2042 6961 730d 0a20 2020  ection Bias..   
+00002970: 2023 2027 5431 3932 272c 2023 2052 6563   # 'T192', # Rec
+00002980: 6570 746f 722c 2065 782e 3a20 4269 6e64  eptor, ex.: Bind
+00002990: 696e 6720 5369 7465 733b 204c 796d 7068  ing Sites; Lymph
+000029a0: 6f63 7974 6520 616e 7469 6765 6e20 4344  ocyte antigen CD
+000029b0: 3420 7265 6365 7074 6f72 3b20 696e 7465  4 receptor; inte
+000029c0: 6772 696e 2061 6c70 6861 3131 6265 7461  grin alpha11beta
+000029d0: 310d 0a20 2020 2023 2027 5430 3839 272c  1..    # 'T089',
+000029e0: 2023 2052 6567 756c 6174 696f 6e20 6f72   # Regulation or
+000029f0: 204c 6177 2c20 6578 2e3a 2042 7569 6c64   Law, ex.: Build
+00002a00: 696e 6720 436f 6465 733b 2043 7269 6d69  ing Codes; Crimi
+00002a10: 6e61 6c20 4c61 773b 2048 6561 6c74 6820  nal Law; Health 
+00002a20: 506c 616e 6e69 6e67 2047 7569 6465 6c69  Planning Guideli
+00002a30: 6e65 730d 0a20 2020 2023 2027 5430 3134  nes..    # 'T014
+00002a40: 272c 2023 2052 6570 7469 6c65 2c20 6578  ', # Reptile, ex
+00002a50: 2e3a 2041 6c6c 6967 6174 6f72 733b 2057  .: Alligators; W
+00002a60: 6174 6572 204d 6f63 6173 7369 6e3b 2047  ater Mocassin; G
+00002a70: 656e 7573 2050 7974 686f 6e20 286f 7267  enus Python (org
+00002a80: 616e 6973 6d29 0d0a 2020 2020 2320 2754  anism)..    # 'T
+00002a90: 3036 3227 2c20 2320 5265 7365 6172 6368  062', # Research
+00002aa0: 2041 6374 6976 6974 792c 2065 782e 3a20   Activity, ex.: 
+00002ab0: 416e 696d 616c 2045 7870 6572 696d 656e  Animal Experimen
+00002ac0: 7461 7469 6f6e 3b20 4269 6f6d 6564 6963  tation; Biomedic
+00002ad0: 616c 2052 6573 6561 7263 683b 2045 7870  al Research; Exp
+00002ae0: 6572 696d 656e 7461 6c20 5265 706c 6963  erimental Replic
+00002af0: 6174 696f 6e0d 0a20 2020 2023 2027 5430  ation..    # 'T0
+00002b00: 3735 272c 2023 2052 6573 6561 7263 6820  75', # Research 
+00002b10: 4465 7669 6365 2c20 6578 2e3a 2045 6c65  Device, ex.: Ele
+00002b20: 6374 726f 6465 732c 2045 6e7a 796d 653b  ctrodes, Enzyme;
+00002b30: 2044 4e41 204d 6963 726f 6172 7261 7920   DNA Microarray 
+00002b40: 4368 6970 3b20 5061 7274 6963 6c65 2043  Chip; Particle C
+00002b50: 6f75 6e74 2061 6e64 2053 697a 6520 416e  ount and Size An
+00002b60: 616c 797a 6572 0d0a 2020 2020 2320 2754  alyzer..    # 'T
+00002b70: 3039 3527 2c20 2320 5365 6c66 2d68 656c  095', # Self-hel
+00002b80: 7020 6f72 2052 656c 6965 6620 4f72 6761  p or Relief Orga
+00002b90: 6e69 7a61 7469 6f6e 2c20 6578 2e3a 2041  nization, ex.: A
+00002ba0: 6c63 6f68 6f6c 6963 7320 416e 6f6e 796d  lcoholics Anonym
+00002bb0: 6f75 733b 2043 6861 7269 7469 6573 202d  ous; Charities -
+00002bc0: 206f 7267 616e 697a 6174 696f 6e3b 2052   organization; R
+00002bd0: 6564 2043 726f 7373 0d0a 2020 2020 2754  ed Cross..    'T
+00002be0: 3138 3427 2c20 2320 5369 676e 206f 7220  184', # Sign or 
+00002bf0: 5379 6d70 746f 6d2c 2065 782e 3a20 4479  Symptom, ex.: Dy
+00002c00: 7370 6e65 613b 204e 6175 7365 613b 2050  spnea; Nausea; P
+00002c10: 6169 6e0d 0a20 2020 2023 2027 5430 3534  ain..    # 'T054
+00002c20: 272c 2023 2053 6f63 6961 6c20 4265 6861  ', # Social Beha
+00002c30: 7669 6f72 2c20 6578 2e3a 2041 6363 756c  vior, ex.: Accul
+00002c40: 7475 7261 7469 6f6e 3b20 436f 6d6d 756e  turation; Commun
+00002c50: 6963 6174 696f 6e3b 2049 6e74 6572 7065  ication; Interpe
+00002c60: 7273 6f6e 616c 2052 656c 6174 696f 6e73  rsonal Relations
+00002c70: 0d0a 2020 2020 2320 2754 3038 3227 2c20  ..    # 'T082', 
+00002c80: 2320 5370 6174 6961 6c20 436f 6e63 6570  # Spatial Concep
+00002c90: 742c 2065 782e 3a20 4d61 6e64 6962 756c  t, ex.: Mandibul
+00002ca0: 6172 2052 6573 7420 506f 7369 7469 6f6e  ar Rest Position
+00002cb0: 3b20 4c61 7465 7261 6c3b 2045 7874 7269  ; Lateral; Extri
+00002cc0: 6e73 6963 0d0a 2020 2020 2320 2754 3136  nsic..    # 'T16
+00002cd0: 3727 2c20 2320 5375 6273 7461 6e63 652c  7', # Substance,
+00002ce0: 2065 782e 3a20 4169 7220 2873 7562 7374   ex.: Air (subst
+00002cf0: 616e 6365 293b 2046 6f73 7369 6c73 3b20  ance); Fossils; 
+00002d00: 506c 6173 7469 6373 0d0a 2020 2020 2320  Plastics..    # 
+00002d10: 2754 3037 3927 2c20 2320 5465 6d70 6f72  'T079', # Tempor
+00002d20: 616c 2043 6f6e 6365 7074 2c20 6578 2e3a  al Concept, ex.:
+00002d30: 2042 6972 7468 2049 6e74 6572 7661 6c73   Birth Intervals
+00002d40: 3b20 4861 6c66 2d4c 6966 653b 2050 6f73  ; Half-Life; Pos
+00002d50: 746f 7065 7261 7469 7665 2050 6572 696f  toperative Perio
+00002d60: 640d 0a20 2020 2027 5430 3631 272c 2023  d..    'T061', #
+00002d70: 2054 6865 7261 7065 7574 6963 206f 7220   Therapeutic or 
+00002d80: 5072 6576 656e 7469 7665 2050 726f 6365  Preventive Proce
+00002d90: 6475 7265 2c20 6578 2e3a 2043 6573 6172  dure, ex.: Cesar
+00002da0: 6561 6e20 7365 6374 696f 6e3b 2044 6572  ean section; Der
+00002db0: 6d61 6272 6173 696f 6e3b 2046 616d 696c  mabrasion; Famil
+00002dc0: 7920 7073 7963 686f 7468 6572 6170 790d  y psychotherapy.
+00002dd0: 0a20 2020 2023 2027 5430 3234 272c 2023  .    # 'T024', #
+00002de0: 2054 6973 7375 652c 2065 782e 3a20 4361   Tissue, ex.: Ca
+00002df0: 7274 696c 6167 653b 2045 6e64 6f74 6865  rtilage; Endothe
+00002e00: 6c69 756d 3b20 4570 6964 6572 6d69 730d  lium; Epidermis.
+00002e10: 0a20 2020 2023 2027 5430 3130 272c 2023  .    # 'T010', #
+00002e20: 2056 6572 7465 6272 6174 652c 2065 782e   Vertebrate, ex.
+00002e30: 3a20 5665 7274 6562 7261 7465 733b 2047  : Vertebrates; G
+00002e40: 6e61 7468 6f73 746f 6d61 7461 2076 6572  nathostomata ver
+00002e50: 7465 6272 6174 653b 2043 7261 6e69 6174  tebrate; Craniat
+00002e60: 6120 3c63 686f 7264 6174 613e 0d0a 2020  a <chordata>..  
+00002e70: 2020 2320 2754 3030 3527 2c20 2320 5669    # 'T005', # Vi
+00002e80: 7275 732c 2065 782e 3a20 436f 6c69 7068  rus, ex.: Coliph
+00002e90: 6167 6573 3b20 4563 686f 7669 7275 733b  ages; Echovirus;
+00002ea0: 2050 6172 766f 7669 7269 6461 650d 0a20   Parvoviridae.. 
+00002eb0: 2020 2023 2027 5431 3237 2720 2023 2056     # 'T127'  # V
+00002ec0: 6974 616d 696e 2c20 6578 2e3a 2035 2c32  itamin, ex.: 5,2
+00002ed0: 352d 4469 6879 6472 6f78 7920 6368 6f6c  5-Dihydroxy chol
+00002ee0: 6563 616c 6369 6665 726f 6c3b 2061 6c70  ecalciferol; alp
+00002ef0: 6861 2d74 6f63 6f70 6865 7279 6c20 6f78  ha-tocopheryl ox
+00002f00: 616c 6174 653b 2056 6974 616d 696e 2041  alate; Vitamin A
+00002f10: 205b 4550 435d 0d0a 7d0d 0a0d 0a55 4e49   [EPC]..}....UNI
+00002f20: 434f 4445 5f44 4153 4845 5320 3d20 7b0d  CODE_DASHES = {.
+00002f30: 0a20 2020 2075 275c 7530 3032 6427 2c20  .    u'\u002d', 
+00002f40: 7527 5c75 3030 3765 272c 2075 275c 7530  u'\u007e', u'\u0
+00002f50: 3061 6427 2c20 7527 5c75 3035 3861 272c  0ad', u'\u058a',
+00002f60: 2075 275c 7530 3562 6527 2c20 7527 5c75   u'\u05be', u'\u
+00002f70: 3134 3030 272c 0d0a 2020 2020 7527 5c75  1400',..    u'\u
+00002f80: 3138 3036 272c 2075 275c 7532 3031 3027  1806', u'\u2010'
+00002f90: 2c20 7527 5c75 3230 3131 272c 2075 275c  , u'\u2011', u'\
+00002fa0: 7532 3031 3027 2c20 7527 5c75 3230 3132  u2010', u'\u2012
+00002fb0: 272c 2075 275c 7532 3031 3327 2c0d 0a20  ', u'\u2013',.. 
+00002fc0: 2020 2075 275c 7532 3031 3427 2c20 7527     u'\u2014', u'
+00002fd0: 5c75 3230 3135 272c 2075 275c 7532 3035  \u2015', u'\u205
+00002fe0: 3327 2c20 7527 5c75 3230 3762 272c 2075  3', u'\u207b', u
+00002ff0: 275c 7532 3231 3227 2c20 7527 5c75 3230  '\u2212', u'\u20
+00003000: 3862 272c 0d0a 2020 2020 7527 5c75 3232  8b',..    u'\u22
+00003010: 3132 272c 2075 275c 7532 3231 3227 2c20  12', u'\u2212', 
+00003020: 7527 5c75 3265 3137 272c 2075 275c 7532  u'\u2e17', u'\u2
+00003030: 6533 6127 2c20 7527 5c75 3265 3362 272c  e3a', u'\u2e3b',
+00003040: 2075 275c 7533 3031 6327 2c0d 0a20 2020   u'\u301c',..   
+00003050: 2075 275c 7533 3033 3027 2c20 7527 5c75   u'\u3030', u'\u
+00003060: 3330 6130 272c 2075 275c 7566 6533 3127  30a0', u'\ufe31'
+00003070: 2c20 7527 5c75 6665 3332 272c 2075 275c  , u'\ufe32', u'\
+00003080: 7566 6535 3827 2c20 7527 5c75 6665 3633  ufe58', u'\ufe63
+00003090: 272c 0d0a 2020 2020 7527 5c75 6666 3064  ',..    u'\uff0d
+000030a0: 270d 0a7d 0d0a 0d0a 2320 6c61 6e67 7561  '..}....# langua
+000030b0: 6765 2077 6974 6820 6d69 7373 696e 6720  ge with missing 
+000030c0: 7661 6c75 650d 0a23 2077 696c 6c20 6e6f  value..# will no
+000030d0: 7420 6861 7665 2073 7570 706f 7274 2066  t have support f
+000030e0: 6f72 2074 6f6b 656e 697a 6174 696f 6e0d  or tokenization.
+000030f0: 0a4c 414e 4755 4147 4553 203d 207b 0d0a  .LANGUAGES = {..
+00003100: 2020 2020 2742 4151 273a 204e 6f6e 652c      'BAQ': None,
+00003110: 2020 2020 2020 2020 2020 2023 2042 6173             # Bas
+00003120: 7175 650d 0a20 2020 2027 4348 4927 3a20  que..    'CHI': 
+00003130: 4e6f 6e65 2c20 2020 2020 2020 2020 2020  None,           
+00003140: 2320 4368 696e 6573 650d 0a20 2020 2027  # Chinese..    '
+00003150: 435a 4527 3a20 4e6f 6e65 2c20 2020 2020  CZE': None,     
+00003160: 2020 2020 2020 2320 437a 6563 680d 0a20        # Czech.. 
+00003170: 2020 2027 4441 4e27 3a20 2764 616e 6973     'DAN': 'danis
+00003180: 6827 2c20 2020 2020 2020 2320 4461 6e69  h',       # Dani
+00003190: 7368 0d0a 2020 2020 2744 5554 273a 2027  sh..    'DUT': '
+000031a0: 6475 7463 6827 2c20 2020 2020 2020 2023  dutch',        #
+000031b0: 2044 7574 6368 0d0a 2020 2020 2745 4e47   Dutch..    'ENG
+000031c0: 273a 2027 656e 676c 6973 6827 2c20 2020  ': 'english',   
+000031d0: 2020 2023 2045 6e67 6c69 7368 0d0a 2020     # English..  
+000031e0: 2020 2745 5354 273a 204e 6f6e 652c 2020    'EST': None,  
+000031f0: 2020 2020 2020 2020 2023 2045 7374 6f6e           # Eston
+00003200: 6961 6e0d 0a20 2020 2027 4649 4e27 3a20  ian..    'FIN': 
+00003210: 2766 696e 6e69 7368 272c 2020 2020 2020  'finnish',      
+00003220: 2320 4669 6e6e 6973 680d 0a20 2020 2027  # Finnish..    '
+00003230: 4652 4527 3a20 2766 7265 6e63 6827 2c20  FRE': 'french', 
+00003240: 2020 2020 2020 2320 4672 656e 6368 0d0a        # French..
+00003250: 2020 2020 2747 4552 273a 2027 6765 726d      'GER': 'germ
+00003260: 616e 272c 2020 2020 2020 2023 2047 6572  an',       # Ger
+00003270: 6d61 6e0d 0a20 2020 2027 4752 4527 3a20  man..    'GRE': 
+00003280: 2767 7265 656b 272c 2020 2020 2020 2020  'greek',        
+00003290: 2320 4772 6565 6b0d 0a20 2020 2027 4845  # Greek..    'HE
+000032a0: 4227 3a20 4e6f 6e65 2c20 2020 2020 2020  B': None,       
+000032b0: 2020 2020 2320 4865 6272 6577 0d0a 2020      # Hebrew..  
+000032c0: 2020 2748 554e 273a 2027 6875 6e67 6172    'HUN': 'hungar
+000032d0: 6961 6e27 2c20 2020 2023 2048 756e 6761  ian',    # Hunga
+000032e0: 7269 616e 0d0a 2020 2020 2749 5441 273a  rian..    'ITA':
+000032f0: 2027 6974 616c 6961 6e27 2c20 2020 2020   'italian',     
+00003300: 2023 2049 7461 6c69 616e 0d0a 2020 2020   # Italian..    
+00003310: 274a 504e 273a 204e 6f6e 652c 2020 2020  'JPN': None,    
+00003320: 2020 2020 2020 2023 204a 6170 616e 6573         # Japanes
+00003330: 650d 0a20 2020 2027 4b4f 5227 3a20 4e6f  e..    'KOR': No
+00003340: 6e65 2c20 2020 2020 2020 2020 2020 2320  ne,           # 
+00003350: 4b6f 7265 616e 0d0a 2020 2020 274c 4156  Korean..    'LAV
+00003360: 273a 204e 6f6e 652c 2020 2020 2020 2020  ': None,        
+00003370: 2020 2023 204c 6174 7669 616e 0d0a 2020     # Latvian..  
+00003380: 2020 274e 4f52 273a 2027 6e6f 7277 6567    'NOR': 'norweg
+00003390: 6961 6e27 2c20 2020 2023 204e 6f72 7765  ian',    # Norwe
+000033a0: 6769 616e 0d0a 2020 2020 2750 4f4c 273a  gian..    'POL':
+000033b0: 2027 706f 6c69 7368 272c 2020 2020 2020   'polish',      
+000033c0: 2023 2050 6f6c 6973 680d 0a20 2020 2027   # Polish..    '
+000033d0: 504f 5227 3a20 2770 6f72 746f 6775 6573  POR': 'portogues
+000033e0: 6527 2c20 2020 2320 506f 7274 7567 7565  e',   # Portugue
+000033f0: 7365 0d0a 2020 2020 2752 5553 273a 2027  se..    'RUS': '
+00003400: 7275 7373 6961 6e27 2c20 2020 2020 2023  russian',      #
+00003410: 2052 7573 7369 616e 0d0a 2020 2020 2753   Russian..    'S
+00003420: 4352 273a 204e 6f6e 652c 2020 2020 2020  CR': None,      
+00003430: 2020 2020 2023 2043 726f 6174 6961 6e0d       # Croatian.
+00003440: 0a20 2020 2027 5350 4127 3a20 2773 7061  .    'SPA': 'spa
+00003450: 6e69 7368 272c 2020 2020 2020 2320 5370  nish',      # Sp
+00003460: 616e 6973 680d 0a20 2020 2027 5357 4527  anish..    'SWE'
+00003470: 3a20 2773 7765 6469 7368 272c 2020 2020  : 'swedish',    
+00003480: 2020 2320 5377 6564 6973 680d 0a20 2020    # Swedish..   
+00003490: 2027 5455 5227 3a20 2774 7572 6b69 7368   'TUR': 'turkish
+000034a0: 272c 2020 2020 2020 2320 5475 726b 6973  ',      # Turkis
+000034b0: 680d 0a7d 0d0a 0d0a 444f 4d41 494e 5f53  h..}....DOMAIN_S
+000034c0: 5045 4349 4649 435f 5354 4f50 574f 5244  PECIFIC_STOPWORD
+000034d0: 5320 3d20 7b0d 0a20 2020 2027 7469 6d65  S = {..    'time
+000034e0: 270d 0a7d 0d0a 0d0a 5350 4143 595f 4c41  '..}....SPACY_LA
+000034f0: 4e47 5541 4745 5f4d 4150 203d 207b 0d0a  NGUAGE_MAP = {..
+00003500: 2020 2020 2745 4e47 273a 2027 656e 5f63      'ENG': 'en_c
+00003510: 6f72 655f 7765 625f 736d 272c 0d0a 2020  ore_web_sm',..  
+00003520: 2020 2747 4552 273a 2027 6465 5f63 6f72    'GER': 'de_cor
+00003530: 655f 6e65 7773 5f73 6d27 2c0d 0a20 2020  e_news_sm',..   
+00003540: 2027 5350 4127 3a20 2765 735f 636f 7265   'SPA': 'es_core
+00003550: 5f6e 6577 735f 736d 272c 0d0a 2020 2020  _news_sm',..    
+00003560: 2750 4f52 273a 2027 7074 5f63 6f72 655f  'POR': 'pt_core_
+00003570: 6e65 7773 5f73 6d27 2c0d 0a20 2020 2027  news_sm',..    '
+00003580: 4652 4527 3a20 2766 725f 636f 7265 5f6e  FRE': 'fr_core_n
+00003590: 6577 735f 736d 272c 0d0a 2020 2020 2749  ews_sm',..    'I
+000035a0: 5441 273a 2027 6974 5f63 6f72 655f 6e65  TA': 'it_core_ne
+000035b0: 7773 5f73 6d27 2c0d 0a20 2020 2027 4455  ws_sm',..    'DU
+000035c0: 5427 3a20 276e 6c5f 636f 7265 5f6e 6577  T': 'nl_core_new
+000035d0: 735f 736d 272c 0d0a 2020 2020 2758 5858  s_sm',..    'XXX
+000035e0: 273a 2027 7878 270d 0a7d 0d0a            ': 'xx'..}..
```

### Comparing `medspacy_quickumls-2.7.1a0/quickumls/core.py` & `medspacy_quickumls-3.0/quickumls/core.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,481 +1,481 @@
-# future statements for Python 2 compatibility
-from __future__ import (
-    unicode_literals, division, print_function, absolute_import)
-
-# built in modules
-import os
-import sys
-import datetime
-from six.moves import xrange
-
-# installed modules
-import spacy
-import nltk
-from unidecode import unidecode
-
-# project modules
-from . import toolbox
-from . import constants
-
-
-class QuickUMLS(object):
-    """The main class to interact with the matcher.
-    """
-    def __init__(
-            self, quickumls_fp,
-            overlapping_criteria='score', threshold=0.7, window=5,
-            similarity_name='jaccard', min_match_length=3,
-            accepted_semtypes=constants.ACCEPTED_SEMTYPES,
-            verbose=False, keep_uppercase=False,
-            spacy_component = False):
-        """Instantiate QuickUMLS object
-
-            This is the main interface through which text can be processed.
-
-        Args:
-            quickumls_fp (str): Path to which QuickUMLS was installed
-            overlapping_criteria (str, optional):
-                    One of "score" or "length". Choose how results are ranked.
-                    Choose "score" for best matching score first or "length" for longest match first.. Defaults to 'score'.
-            threshold (float, optional): Minimum similarity between strings. Defaults to 0.7.
-            window (int, optional): Maximum amount of tokens to consider for matching. Defaults to 5.
-            similarity_name (str, optional): One of "dice", "jaccard", "cosine", or "overlap".
-                    Similarity measure to be used. Defaults to 'jaccard'.
-            min_match_length (int, optional): TODO: ??. Defaults to 3.
-            accepted_semtypes (List[str], optional): Set of UMLS semantic types concepts should belong to.
-                Semantic types are identified by the letter "T" followed by three numbers
-                (e.g., "T131", which identifies the type "Hazardous or Poisonous Substance").
-                Defaults to constants.ACCEPTED_SEMTYPES.
-            verbose (bool, optional): TODO:??. Defaults to False.
-            keep_uppercase (bool, optional): By default QuickUMLS converts all
-                    uppercase strings to lowercase. This option disables that
-                    functionality, which makes QuickUMLS useful for
-                    distinguishing acronyms from normal words. For this the
-                    database should be installed without the -L option.
-                    Defaults to False.
-
-        Raises:
-            ValueError: Raises a ValueError if QuickUMLS was installed for a language that is not currently supported TODO: verify this?
-            OSError: Raises an OSError if the required Spacy model was not installed.
-        """
-
-        self.verbose = verbose
-
-        valid_criteria = {'length', 'score'}
-        err_msg = (
-            '"{}" is not a valid overlapping_criteria. Choose '
-            'between {}'.format(
-                overlapping_criteria, ', '.join(valid_criteria)
-            )
-        )
-        assert overlapping_criteria in valid_criteria, err_msg
-        self.overlapping_criteria = overlapping_criteria
-
-        valid_similarities = {'dice', 'jaccard', 'cosine', 'overlap'}
-        err_msg = ('"{}" is not a valid similarity name. Choose between '
-                   '{}'.format(similarity_name, ', '.join(valid_similarities)))
-        assert not(valid_similarities in valid_similarities), err_msg
-        self.similarity_name = similarity_name
-
-        simstring_fp = os.path.join(quickumls_fp, 'umls-simstring.db')
-        cuisem_fp = os.path.join(quickumls_fp, 'cui-semtypes.db')
-
-        self.valid_punct = constants.UNICODE_DASHES
-        self.negations = constants.NEGATIONS
-
-        self.window = window
-        self.ngram_length = 3
-        self.threshold = threshold
-        self.min_match_length = min_match_length
-        self.to_lowercase_flag = os.path.exists(
-            os.path.join(quickumls_fp, 'lowercase.flag')
-        )
-        self.normalize_unicode_flag = os.path.exists(
-            os.path.join(quickumls_fp, 'normalize-unicode.flag')
-        )
-        self.keep_uppercase = keep_uppercase
-
-        # Check whether data is installed with lowercase flag and QuickUMLS initiated with keeping uppercase words
-        if self.to_lowercase_flag and self.keep_uppercase:
-            raise ValueError('Database is installed with lowercase flag and QuickUMLS is initiated with '
-                             'keep_uppercase flag. This would prevent identifying concepts that contain all uppercase'
-                             'characters. Please reinstall data without --lowercase or run QuickUMLS without'
-                             '--keep_uppercase.')
-
-        language_fp = os.path.join(quickumls_fp, 'language.flag')
-
-        # download stopwords if necessary
-        try:
-            nltk.corpus.stopwords.words()
-        except LookupError:
-            nltk.download('stopwords')
-
-        if os.path.exists(language_fp):
-            with open(language_fp) as f:
-                self.language_flag = f.read().strip()
-        else:
-            self.language_flag = 'ENG'
-
-        if self.language_flag not in constants.LANGUAGES:
-            raise ValueError('Language "{}" not supported'.format(self.language_flag))
-        elif constants.LANGUAGES[self.language_flag] is None:
-            self._stopwords = set()
-            spacy_lang = 'XXX'
-        else:
-            self._stopwords = set(
-                nltk.corpus.stopwords.words(constants.LANGUAGES[self.language_flag])
-            )
-            spacy_lang = constants.SPACY_LANGUAGE_MAP[self.language_flag]
-
-        database_backend_fp = os.path.join(quickumls_fp, 'database_backend.flag')
-        if os.path.exists(database_backend_fp):
-            with open(database_backend_fp) as f:
-                self._database_backend = f.read().strip()
-        else:
-            raise ValueError("""File database_backend.flag was not found at this location: {}.  This path may have been created with leveldb
-                             or an earlier version of QuickUMLS, but leveldb is not supported by this package version
-                             """.format(quickumls_fp))
-
-        # domain specific stopwords
-        self._stopwords = self._stopwords.union(constants.DOMAIN_SPECIFIC_STOPWORDS)
-
-        self._info = None
-
-        self.accepted_semtypes = accepted_semtypes
-
-        # if this is not being executed as as spacy component, then it must be standalone
-        if spacy_component:
-            # In this case, the pipeline is external to this current class
-            self.nlp = None
-        else:
-            try:
-                self.nlp = spacy.load(spacy_lang)
-            except OSError:
-                msg = (
-                    'Model for language "{}" is not downloaded. Please '
-                    'run "python -m spacy download {}" before launching '
-                    'QuickUMLS'
-                ).format(
-                    self.language_flag,
-                    constants.SPACY_LANGUAGE_MAP.get(self.language_flag, 'xx')
-                )
-                raise OSError(msg)
-
-        self.ss_db = toolbox.SimstringDBReader(
-            simstring_fp, similarity_name, threshold
-        )
-        self.cuisem_db = toolbox.CuiSemTypesDB(
-            cuisem_fp, database_backend=self._database_backend
-        )
-
-    def get_info(self):
-        """Computes a summary of the matcher options.
-
-        Returns:
-            Dict: Dictionary containing information on the QuicUMLS instance.
-        """
-        return self.info
-
-    def get_accepted_semtypes(self):
-        return self.accepted_semtypes
-
-    @property
-    def info(self):
-        """Computes a summary of the matcher options.
-
-        Returns:
-            Dict: Dictionary containing information on the QuicUMLS instance.
-        """
-        # useful for caching of respnses
-
-        if self._info is None:
-            self._info = {
-                'threshold': self.threshold,
-                'similarity_name': self.similarity_name,
-                'window': self.window,
-                'ngram_length': self.ngram_length,
-                'min_match_length': self.min_match_length,
-                'accepted_semtypes': sorted(self.accepted_semtypes),
-                'negations': sorted(self.negations),
-                'valid_punct': sorted(self.valid_punct)
-            }
-        return self._info
-
-    def _is_valid_token(self, tok):
-        return not(
-            tok.is_punct or tok.is_space or
-            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
-        )
-
-    def _is_valid_start_token(self, tok):
-        return not(
-            tok.like_num or
-            (self._is_stop_term(tok) and tok.lemma_ not in self.negations) or
-            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
-        )
-
-    def _is_stop_term(self, tok):
-        return tok.text in self._stopwords
-
-    def _is_valid_end_token(self, tok):
-        return not(
-            tok.is_punct or tok.is_space or self._is_stop_term(tok) or
-            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
-        )
-
-    def _is_valid_middle_token(self, tok):
-        return (
-            not(tok.is_punct or tok.is_space) or
-            tok.is_bracket or
-            tok.text in self.valid_punct
-        )
-
-    def _is_ok_semtype(self, target_semtypes):
-        if self.accepted_semtypes is None:
-            ok = True
-        else:
-            ok = any(sem in self.accepted_semtypes for sem in target_semtypes)
-        return ok
-
-    def _is_longer_than_min(self, span):
-        return (span.end_char - span.start_char) >= self.min_match_length
-
-    def _make_ngrams(self, sent):
-        sent_length = len(sent)
-
-        # do not include determiners inside a span
-        skip_in_span = {token.i for token in sent if token.pos_ == 'DET'}
-
-        # invalidate a span if it includes any on these symbols
-        invalid_mid_tokens = {
-            token.i for token in sent if not self._is_valid_middle_token(token)
-        }
-
-        for i in xrange(sent_length):
-            tok = sent[i]
-
-            if not self._is_valid_token(tok):
-                continue
-
-            # do not consider this token by itself if it is
-            # a number or a stopword.
-            if self._is_valid_start_token(tok):
-                compensate = False
-            else:
-                compensate = True
-
-            span_end = min(sent_length, i + self.window) + 1
-
-            # we take a shortcut if the token is the last one
-            # in the sentence
-            if (
-                i + 1 == sent_length and            # it's the last token
-                self._is_valid_end_token(tok) and   # it's a valid end token
-                len(tok) >= self.min_match_length   # it's of miminum length
-            ):
-                yield(tok.idx, tok.idx + len(tok), tok.text)
-
-            for j in xrange(i + 1, span_end):
-                if compensate:
-                    compensate = False
-                    continue
-
-                if sent[j - 1] in invalid_mid_tokens:
-                    break
-
-                if not self._is_valid_end_token(sent[j - 1]):
-                    continue
-
-                span = sent[i:j]
-
-                if not self._is_longer_than_min(span):
-                    continue
-
-                yield (
-                    span.start_char, span.end_char,
-                    ''.join(token.text_with_ws for token in span
-                            if token.i not in skip_in_span).strip()
-                )
-
-    def _get_all_matches(self, ngrams):
-        matches = []
-        for start, end, ngram in ngrams:
-            ngram_normalized = ngram
-
-            if self.normalize_unicode_flag:
-                ngram_normalized = unidecode(ngram_normalized)
-
-            # make it lowercase
-            if self.to_lowercase_flag:
-                ngram_normalized = ngram_normalized.lower()
-
-            # If the term is all uppercase, it might be the case that
-            # no match is found; so we convert to lowercase;
-            # however, this is never needed if the string is lowercased
-            # in the step above
-            if not self.to_lowercase_flag and ngram_normalized.isupper() and not self.keep_uppercase:
-                ngram_normalized = ngram_normalized.lower()
-
-            prev_cui = None
-            ngram_cands = list(self.ss_db.get(ngram_normalized))
-
-            ngram_dict = {}
-            for match in ngram_cands:
-                cuisem_match = sorted(self.cuisem_db.get(match))
-
-                match_similarity = toolbox.get_similarity(
-                    x=ngram_normalized,
-                    y=match,
-                    n=self.ngram_length,
-                    similarity_name=self.similarity_name
-                )
-
-                if match_similarity == 0:
-                        continue
-
-                for cui, semtypes, preferred in cuisem_match:
-
-                    if not self._is_ok_semtype(semtypes):
-                        continue
-
-                    # if cui is already in the dictionary, replace only if the new score is higher
-                    if cui in ngram_dict.keys():
-                        if match_similarity > ngram_dict[cui]['similarity']:
-                            ngram_dict[cui] = {
-                                'start': start,
-                                'end': end,
-                                'ngram': ngram,
-                                'term': toolbox.safe_unicode(match),
-                                'cui': cui,
-                                'similarity': match_similarity,
-                                'semtypes': semtypes,
-                                'preferred': preferred
-                            }
-                    else: # otherwise just add it if it is not part of the dictionary
-                        ngram_dict[cui] = {
-                            'start': start,
-                            'end': end,
-                            'ngram': ngram,
-                            'term': toolbox.safe_unicode(match),
-                            'cui': cui,
-                            'similarity': match_similarity,
-                            'semtypes': semtypes,
-                            'preferred': preferred
-                        }
-
-            ngram_matches = ngram_dict.values()
-            if len(ngram_matches) > 0:
-                matches.append(
-                    sorted(
-                        ngram_matches,
-                        key=lambda m: m['similarity'] + m['preferred'],
-                        reverse=True
-                    )
-                )
-        return matches
-
-    @staticmethod
-    def _select_score(match):
-        return (match[0]['similarity'], (match[0]['end'] - match[0]['start']))
-
-    @staticmethod
-    def _select_longest(match):
-        return ((match[0]['end'] - match[0]['start']), match[0]['similarity'])
-
-    def _select_terms(self, matches):
-        sort_func = (
-            self._select_longest if self.overlapping_criteria == 'length'
-            else self._select_score
-        )
-
-        matches = sorted(matches, key=sort_func, reverse=True)
-
-        intervals = toolbox.Intervals()
-        final_matches_subset = []
-
-        for match in matches:
-            match_interval = (match[0]['start'], match[0]['end'])
-            if match_interval not in intervals:
-                final_matches_subset.append(match)
-                intervals.append(match_interval)
-
-        return final_matches_subset
-
-    def _make_token_sequences(self, parsed):
-        for i in range(len(parsed)):
-            for j in xrange(
-                    i + 1, min(i + self.window, len(parsed)) + 1):
-                span = parsed[i:j]
-
-                if not self._is_longer_than_min(span):
-                    continue
-
-                yield (span.start_char, span.end_char, span.text)
-
-    def _print_verbose_status(self, parsed, matches):
-        if not self.verbose:
-            return False
-
-        print(
-            '[{}] {:,} extracted from {:,} tokens'.format(
-                datetime.datetime.now().isoformat(),
-                sum(len(match_group) for match_group in matches),
-                len(parsed)
-            ),
-            file=sys.stderr
-        )
-        return True
-
-    def match(self, text, best_match=True, ignore_syntax=False):
-        """Perform UMLS concept resolution for the given string.
-
-        [extended_summary]
-
-        Args:
-            text (str): Text on which to run the algorithm
-
-            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
-            ignore_syntax (bool, optional): Wether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False.
-
-        Returns:
-            List: List of all matches in the text
-            TODO: Describe format
-        """
-
-        parsed = self.nlp(u'{}'.format(text))
-        
-        # pass in parsed spacy doc to get concept matches
-        matches = self._match(parsed)
-
-        return matches
-        
-    def _match(self, doc, best_match=True, ignore_syntax=False):
-        """Gathers ngram matches given a spaCy document object.
-
-        [extended_summary]
-
-        Args:
-            text (Document): spaCy Document object to be used for extracting ngrams
-
-            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
-            ignore_syntax (bool, optional): Wether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False
-
-        Returns:
-            List: List of all matches in the text
-            TODO: Describe format
-        """
-        
-        ngrams = None
-        if ignore_syntax:
-            ngrams = self._make_token_sequences(doc)
-        else:
-            ngrams = self._make_ngrams(doc)
-
-        matches = self._get_all_matches(ngrams)
-
-        if best_match:
-            matches = self._select_terms(matches)
-
-        self._print_verbose_status(doc, matches)
-        
-        return matches
+# future statements for Python 2 compatibility
+from __future__ import (
+    unicode_literals, division, print_function, absolute_import)
+
+# built in modules
+import os
+import sys
+import datetime
+from six.moves import xrange
+
+# installed modules
+import spacy
+import nltk
+from unidecode import unidecode
+
+# project modules
+from . import toolbox
+from . import constants
+
+
+class QuickUMLS(object):
+    """The main class to interact with the matcher.
+    """
+    def __init__(
+            self, quickumls_fp,
+            overlapping_criteria='score', threshold=0.7, window=5,
+            similarity_name='jaccard', min_match_length=3,
+            accepted_semtypes=constants.ACCEPTED_SEMTYPES,
+            verbose=False, keep_uppercase=False,
+            spacy_component = False):
+        """Instantiate QuickUMLS object
+
+            This is the main interface through which text can be processed.
+
+        Args:
+            quickumls_fp (str): Path to which QuickUMLS was installed
+            overlapping_criteria (str, optional):
+                    One of "score" or "length". Choose how results are ranked.
+                    Choose "score" for best matching score first or "length" for longest match first.. Defaults to 'score'.
+            threshold (float, optional): Minimum similarity between strings. Defaults to 0.7.
+            window (int, optional): Maximum amount of tokens to consider for matching. Defaults to 5.
+            similarity_name (str, optional): One of "dice", "jaccard", "cosine", or "overlap".
+                    Similarity measure to be used. Defaults to 'jaccard'.
+            min_match_length (int, optional): TODO: ??. Defaults to 3.
+            accepted_semtypes (List[str], optional): Set of UMLS semantic types concepts should belong to.
+                Semantic types are identified by the letter "T" followed by three numbers
+                (e.g., "T131", which identifies the type "Hazardous or Poisonous Substance").
+                Defaults to constants.ACCEPTED_SEMTYPES.
+            verbose (bool, optional): TODO:??. Defaults to False.
+            keep_uppercase (bool, optional): By default QuickUMLS converts all
+                    uppercase strings to lowercase. This option disables that
+                    functionality, which makes QuickUMLS useful for
+                    distinguishing acronyms from normal words. For this the
+                    database should be installed without the -L option.
+                    Defaults to False.
+
+        Raises:
+            ValueError: Raises a ValueError if QuickUMLS was installed for a language that is not currently supported TODO: verify this?
+            OSError: Raises an OSError if the required Spacy model was not installed.
+        """
+
+        self.verbose = verbose
+
+        valid_criteria = {'length', 'score'}
+        err_msg = (
+            '"{}" is not a valid overlapping_criteria. Choose '
+            'between {}'.format(
+                overlapping_criteria, ', '.join(valid_criteria)
+            )
+        )
+        assert overlapping_criteria in valid_criteria, err_msg
+        self.overlapping_criteria = overlapping_criteria
+
+        valid_similarities = {'dice', 'jaccard', 'cosine', 'overlap'}
+        err_msg = ('"{}" is not a valid similarity name. Choose between '
+                   '{}'.format(similarity_name, ', '.join(valid_similarities)))
+        assert not(valid_similarities in valid_similarities), err_msg
+        self.similarity_name = similarity_name
+
+        simstring_fp = os.path.join(quickumls_fp, 'umls-simstring.db')
+        cuisem_fp = os.path.join(quickumls_fp, 'cui-semtypes.db')
+
+        self.valid_punct = constants.UNICODE_DASHES
+        self.negations = constants.NEGATIONS
+
+        self.window = window
+        self.ngram_length = 3
+        self.threshold = threshold
+        self.min_match_length = min_match_length
+        self.to_lowercase_flag = os.path.exists(
+            os.path.join(quickumls_fp, 'lowercase.flag')
+        )
+        self.normalize_unicode_flag = os.path.exists(
+            os.path.join(quickumls_fp, 'normalize-unicode.flag')
+        )
+        self.keep_uppercase = keep_uppercase
+
+        # Check whether data is installed with lowercase flag and QuickUMLS initiated with keeping uppercase words
+        if self.to_lowercase_flag and self.keep_uppercase:
+            raise ValueError('Database is installed with lowercase flag and QuickUMLS is initiated with '
+                             'keep_uppercase flag. This would prevent identifying concepts that contain all uppercase'
+                             'characters. Please reinstall data without --lowercase or run QuickUMLS without'
+                             '--keep_uppercase.')
+
+        language_fp = os.path.join(quickumls_fp, 'language.flag')
+
+        # download stopwords if necessary
+        try:
+            nltk.corpus.stopwords.words()
+        except LookupError:
+            nltk.download('stopwords')
+
+        if os.path.exists(language_fp):
+            with open(language_fp) as f:
+                self.language_flag = f.read().strip()
+        else:
+            self.language_flag = 'ENG'
+
+        if self.language_flag not in constants.LANGUAGES:
+            raise ValueError('Language "{}" not supported'.format(self.language_flag))
+        elif constants.LANGUAGES[self.language_flag] is None:
+            self._stopwords = set()
+            spacy_lang = 'XXX'
+        else:
+            self._stopwords = set(
+                nltk.corpus.stopwords.words(constants.LANGUAGES[self.language_flag])
+            )
+            spacy_lang = constants.SPACY_LANGUAGE_MAP[self.language_flag]
+
+        database_backend_fp = os.path.join(quickumls_fp, 'database_backend.flag')
+        if os.path.exists(database_backend_fp):
+            with open(database_backend_fp) as f:
+                self._database_backend = f.read().strip()
+        else:
+            raise ValueError("""File database_backend.flag was not found at this location: {}.  This path may have been created with leveldb
+                             or an earlier version of QuickUMLS, but leveldb is not supported by this package version
+                             """.format(quickumls_fp))
+
+        # domain specific stopwords
+        self._stopwords = self._stopwords.union(constants.DOMAIN_SPECIFIC_STOPWORDS)
+
+        self._info = None
+
+        self.accepted_semtypes = accepted_semtypes
+
+        # if this is not being executed as as spacy component, then it must be standalone
+        if spacy_component:
+            # In this case, the pipeline is external to this current class
+            self.nlp = None
+        else:
+            try:
+                self.nlp = spacy.load(spacy_lang)
+            except OSError:
+                msg = (
+                    'Model for language "{}" is not downloaded. Please '
+                    'run "python -m spacy download {}" before launching '
+                    'QuickUMLS'
+                ).format(
+                    self.language_flag,
+                    constants.SPACY_LANGUAGE_MAP.get(self.language_flag, 'xx')
+                )
+                raise OSError(msg)
+
+        self.ss_db = toolbox.SimstringDBReader(
+            simstring_fp, similarity_name, threshold
+        )
+        self.cuisem_db = toolbox.CuiSemTypesDB(
+            cuisem_fp, database_backend=self._database_backend
+        )
+
+    def get_info(self):
+        """Computes a summary of the matcher options.
+
+        Returns:
+            Dict: Dictionary containing information on the QuicUMLS instance.
+        """
+        return self.info
+
+    def get_accepted_semtypes(self):
+        return self.accepted_semtypes
+
+    @property
+    def info(self):
+        """Computes a summary of the matcher options.
+
+        Returns:
+            Dict: Dictionary containing information on the QuicUMLS instance.
+        """
+        # useful for caching of respnses
+
+        if self._info is None:
+            self._info = {
+                'threshold': self.threshold,
+                'similarity_name': self.similarity_name,
+                'window': self.window,
+                'ngram_length': self.ngram_length,
+                'min_match_length': self.min_match_length,
+                'accepted_semtypes': sorted(self.accepted_semtypes),
+                'negations': sorted(self.negations),
+                'valid_punct': sorted(self.valid_punct)
+            }
+        return self._info
+
+    def _is_valid_token(self, tok):
+        return not(
+            tok.is_punct or tok.is_space or
+            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
+        )
+
+    def _is_valid_start_token(self, tok):
+        return not(
+            tok.like_num or
+            (self._is_stop_term(tok) and tok.lemma_ not in self.negations) or
+            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
+        )
+
+    def _is_stop_term(self, tok):
+        return tok.text in self._stopwords
+
+    def _is_valid_end_token(self, tok):
+        return not(
+            tok.is_punct or tok.is_space or self._is_stop_term(tok) or
+            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
+        )
+
+    def _is_valid_middle_token(self, tok):
+        return (
+            not(tok.is_punct or tok.is_space) or
+            tok.is_bracket or
+            tok.text in self.valid_punct
+        )
+
+    def _is_ok_semtype(self, target_semtypes):
+        if self.accepted_semtypes is None:
+            ok = True
+        else:
+            ok = any(sem in self.accepted_semtypes for sem in target_semtypes)
+        return ok
+
+    def _is_longer_than_min(self, span):
+        return (span.end_char - span.start_char) >= self.min_match_length
+
+    def _make_ngrams(self, sent):
+        sent_length = len(sent)
+
+        # do not include determiners inside a span
+        skip_in_span = {token.i for token in sent if token.pos_ == 'DET'}
+
+        # invalidate a span if it includes any on these symbols
+        invalid_mid_tokens = {
+            token.i for token in sent if not self._is_valid_middle_token(token)
+        }
+
+        for i in xrange(sent_length):
+            tok = sent[i]
+
+            if not self._is_valid_token(tok):
+                continue
+
+            # do not consider this token by itself if it is
+            # a number or a stopword.
+            if self._is_valid_start_token(tok):
+                compensate = False
+            else:
+                compensate = True
+
+            span_end = min(sent_length, i + self.window) + 1
+
+            # we take a shortcut if the token is the last one
+            # in the sentence
+            if (
+                i + 1 == sent_length and            # it's the last token
+                self._is_valid_end_token(tok) and   # it's a valid end token
+                len(tok) >= self.min_match_length   # it's of miminum length
+            ):
+                yield(tok.idx, tok.idx + len(tok), tok.text)
+
+            for j in xrange(i + 1, span_end):
+                if compensate:
+                    compensate = False
+                    continue
+
+                if sent[j - 1] in invalid_mid_tokens:
+                    break
+
+                if not self._is_valid_end_token(sent[j - 1]):
+                    continue
+
+                span = sent[i:j]
+
+                if not self._is_longer_than_min(span):
+                    continue
+
+                yield (
+                    span.start_char, span.end_char,
+                    ''.join(token.text_with_ws for token in span
+                            if token.i not in skip_in_span).strip()
+                )
+
+    def _get_all_matches(self, ngrams):
+        matches = []
+        for start, end, ngram in ngrams:
+            ngram_normalized = ngram
+
+            if self.normalize_unicode_flag:
+                ngram_normalized = unidecode(ngram_normalized)
+
+            # make it lowercase
+            if self.to_lowercase_flag:
+                ngram_normalized = ngram_normalized.lower()
+
+            # If the term is all uppercase, it might be the case that
+            # no match is found; so we convert to lowercase;
+            # however, this is never needed if the string is lowercased
+            # in the step above
+            if not self.to_lowercase_flag and ngram_normalized.isupper() and not self.keep_uppercase:
+                ngram_normalized = ngram_normalized.lower()
+
+            prev_cui = None
+            ngram_cands = list(self.ss_db.get(ngram_normalized))
+
+            ngram_dict = {}
+            for match in ngram_cands:
+                cuisem_match = sorted(self.cuisem_db.get(match))
+
+                match_similarity = toolbox.get_similarity(
+                    x=ngram_normalized,
+                    y=match,
+                    n=self.ngram_length,
+                    similarity_name=self.similarity_name
+                )
+
+                if match_similarity == 0:
+                        continue
+
+                for cui, semtypes, preferred in cuisem_match:
+
+                    if not self._is_ok_semtype(semtypes):
+                        continue
+
+                    # if cui is already in the dictionary, replace only if the new score is higher
+                    if cui in ngram_dict.keys():
+                        if match_similarity > ngram_dict[cui]['similarity']:
+                            ngram_dict[cui] = {
+                                'start': start,
+                                'end': end,
+                                'ngram': ngram,
+                                'term': toolbox.safe_unicode(match),
+                                'cui': cui,
+                                'similarity': match_similarity,
+                                'semtypes': semtypes,
+                                'preferred': preferred
+                            }
+                    else: # otherwise just add it if it is not part of the dictionary
+                        ngram_dict[cui] = {
+                            'start': start,
+                            'end': end,
+                            'ngram': ngram,
+                            'term': toolbox.safe_unicode(match),
+                            'cui': cui,
+                            'similarity': match_similarity,
+                            'semtypes': semtypes,
+                            'preferred': preferred
+                        }
+
+            ngram_matches = ngram_dict.values()
+            if len(ngram_matches) > 0:
+                matches.append(
+                    sorted(
+                        ngram_matches,
+                        key=lambda m: m['similarity'] + m['preferred'],
+                        reverse=True
+                    )
+                )
+        return matches
+
+    @staticmethod
+    def _select_score(match):
+        return (match[0]['similarity'], (match[0]['end'] - match[0]['start']))
+
+    @staticmethod
+    def _select_longest(match):
+        return ((match[0]['end'] - match[0]['start']), match[0]['similarity'])
+
+    def _select_terms(self, matches):
+        sort_func = (
+            self._select_longest if self.overlapping_criteria == 'length'
+            else self._select_score
+        )
+
+        matches = sorted(matches, key=sort_func, reverse=True)
+
+        intervals = toolbox.Intervals()
+        final_matches_subset = []
+
+        for match in matches:
+            match_interval = (match[0]['start'], match[0]['end'])
+            if match_interval not in intervals:
+                final_matches_subset.append(match)
+                intervals.append(match_interval)
+
+        return final_matches_subset
+
+    def _make_token_sequences(self, parsed):
+        for i in range(len(parsed)):
+            for j in xrange(
+                    i + 1, min(i + self.window, len(parsed)) + 1):
+                span = parsed[i:j]
+
+                if not self._is_longer_than_min(span):
+                    continue
+
+                yield (span.start_char, span.end_char, span.text)
+
+    def _print_verbose_status(self, parsed, matches):
+        if not self.verbose:
+            return False
+
+        print(
+            '[{}] {:,} extracted from {:,} tokens'.format(
+                datetime.datetime.now().isoformat(),
+                sum(len(match_group) for match_group in matches),
+                len(parsed)
+            ),
+            file=sys.stderr
+        )
+        return True
+
+    def match(self, text, best_match=True, ignore_syntax=False):
+        """Perform UMLS concept resolution for the given string.
+
+        [extended_summary]
+
+        Args:
+            text (str): Text on which to run the algorithm
+
+            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
+            ignore_syntax (bool, optional): Wether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False.
+
+        Returns:
+            List: List of all matches in the text
+            TODO: Describe format
+        """
+
+        parsed = self.nlp(u'{}'.format(text))
+        
+        # pass in parsed spacy doc to get concept matches
+        matches = self._match(parsed)
+
+        return matches
+        
+    def _match(self, doc, best_match=True, ignore_syntax=False):
+        """Gathers ngram matches given a spaCy document object.
+
+        [extended_summary]
+
+        Args:
+            text (Document): spaCy Document object to be used for extracting ngrams
+
+            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
+            ignore_syntax (bool, optional): Wether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False
+
+        Returns:
+            List: List of all matches in the text
+            TODO: Describe format
+        """
+        
+        ngrams = None
+        if ignore_syntax:
+            ngrams = self._make_token_sequences(doc)
+        else:
+            ngrams = self._make_ngrams(doc)
+
+        matches = self._get_all_matches(ngrams)
+
+        if best_match:
+            matches = self._select_terms(matches)
+
+        self._print_verbose_status(doc, matches)
+        
+        return matches
```

### Comparing `medspacy_quickumls-2.7.1a0/quickumls/install.py` & `medspacy_quickumls-3.0/quickumls/install.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-from __future__ import unicode_literals, division, print_function
-
-# built in modules
-import argparse
-import codecs
-import os
-from six.moves import input
-import shutil
-import sys
-import time
-try:
-    from unidecode import unidecode
-except ImportError:
-    pass
-
-
-# third party-dependencies
-import spacy
-
-
-# project modules
-from .toolbox import countlines, CuiSemTypesDB, SimstringDBWriter, mkdir
-from .constants import HEADERS_MRCONSO, HEADERS_MRSTY, LANGUAGES, SPACY_LANGUAGE_MAP
-
-
-def get_semantic_types(path, headers):
-    sem_types = {}
-    with codecs.open(path, encoding='utf-8') as f:
-        for i, ln in enumerate(f):
-            content = dict(zip(headers, ln.strip().split('|')))
-
-            sem_types.setdefault(content['cui'], []).append(content['sty'])
-
-    return sem_types
-
-
-def get_mrconso_iterator(path, headers, lang='ENG'):
-    with codecs.open(path, encoding='utf-8') as f:
-        for i, ln in enumerate(f):
-            content = dict(zip(headers, ln.strip().split('|')))
-
-            if content['lat'] != lang:
-                continue
-
-            yield content
-
-
-def extract_from_mrconso(
-        mrconso_path, mrsty_path, opts,
-        mrconso_header=HEADERS_MRCONSO, mrsty_header=HEADERS_MRSTY):
-
-    start = time.time()
-    print('loading semantic types...', end=' ')
-    sys.stdout.flush()
-    sem_types = get_semantic_types(mrsty_path, mrsty_header)
-    print('done in {:.2f} s'.format(time.time() - start))
-
-    start = time.time()
-
-    mrconso_iterator = get_mrconso_iterator(
-        mrconso_path, mrconso_header, opts.language
-    )
-
-    total = countlines(mrconso_path)
-
-    processed = set()
-    i = 0
-
-    for content in mrconso_iterator:
-        i += 1
-
-        if i % 100000 == 0:
-            delta = time.time() - start
-            status = (
-                '{:,} in {:.2f} s ({:.2%}, {:.1e} s / term)'
-                ''.format(i, delta, i / total, delta / i if i > 0 else 0)
-            )
-            print(status)
-
-        concept_text = content['str'].strip()
-        cui = content['cui']
-        preferred = 1 if content['ispref'] == 'Y' else 0
-
-        if opts.lowercase:
-            concept_text = concept_text.lower()
-
-        if opts.normalize_unicode:
-            concept_text = unidecode(concept_text)
-
-        if (cui, concept_text) in processed:
-            continue
-        else:
-            processed.add((cui, concept_text))
-
-        yield (concept_text, cui, sem_types[cui], preferred)
-
-    delta = time.time() - start
-    status = (
-        '\nCOMPLETED: {:,} in {:.2f} s ({:.1e} s / term)'
-        ''.format(i, delta, i / total, delta / i if i > 0 else 0)
-    )
-    print(status)
-
-
-def parse_and_encode_ngrams(extracted_it, simstring_dir, cuisty_dir, database_backend):
-    # Create destination directories for the two databases
-    mkdir(simstring_dir)
-    mkdir(cuisty_dir)
-
-    ss_db = SimstringDBWriter(simstring_dir)
-    cuisty_db = CuiSemTypesDB(cuisty_dir, database_backend=database_backend)
-
-    simstring_terms = set()
-
-    for i, (term, cui, stys, preferred) in enumerate(extracted_it, start=1):
-        if term not in simstring_terms:
-            ss_db.insert(term)
-            simstring_terms.add(term)
-
-        cuisty_db.insert(term, cui, stys, preferred)
-
-
-def install_spacy(lang):
-    """Tries to create a spacy object; if it fails, downloads the dataset"""
-
-    print(f'Determining if SpaCy for language "{lang}" is installed...')
-
-    if lang in SPACY_LANGUAGE_MAP:
-        try:
-            spacy.load(SPACY_LANGUAGE_MAP[lang])
-            print(f'SpaCy is installed and avaliable for {lang}!')
-        except OSError:
-            print(f'SpaCy is not available! Attempting to download and install...')
-            spacy.cli.download(SPACY_LANGUAGE_MAP[lang])
-
-
-def parse_args():
-    ap = argparse.ArgumentParser()
-    ap.add_argument(
-        'umls_installation_path',
-        help=('Location of UMLS installation files (`MRCONSO.RRF` and '
-              '`MRSTY.RRF` files)')
-    )
-    ap.add_argument(
-        'destination_path',
-        help='Location where the necessary QuickUMLS files are installed'
-    )
-    ap.add_argument(
-        '-L', '--lowercase', action='store_true',
-        help='Consider only lowercase version of tokens'
-    )
-    ap.add_argument(
-        '-U', '--normalize-unicode', action='store_true',
-        help='Normalize unicode strings to their closest ASCII representation'
-    )
-    ap.add_argument(
-        '-d', '--database-backend', choices=('unqlite'), default='unqlite',
-        help='KV database to use to store CUIs and semantic types'
-    )
-    ap.add_argument(
-        '-E', '--language', default='ENG', choices=LANGUAGES,
-        help='Extract concepts of the specified language'
-    )
-    opts = ap.parse_args()
-    return opts
-
-
-def main():
-    opts = parse_args()
-
-    install_spacy(opts.language)
-
-    if not os.path.exists(opts.destination_path):
-        msg = ('Directory "{}" does not exists; should I create it? [y/N] '
-               ''.format(opts.destination_path))
-        create = input(msg).lower().strip() == 'y'
-
-        if create:
-            os.makedirs(opts.destination_path)
-        else:
-            print('Aborting.')
-            exit(1)
-
-    if len(os.listdir(opts.destination_path)) > 0:
-        msg = ('Directory "{}" is not empty; should I empty it? [y/N] '
-               ''.format(opts.destination_path))
-        empty = input(msg).lower().strip() == 'y'
-        if empty:
-            shutil.rmtree(opts.destination_path)
-            os.mkdir(opts.destination_path)
-        else:
-            print('Aborting.')
-            exit(1)
-
-    if opts.normalize_unicode:
-        try:
-            unidecode
-        except NameError:
-            err = ('`unidecode` is needed for unicode normalization'
-                   'please install it via the `[sudo] pip install '
-                   'unidecode` command.')
-            print(err, file=sys.stderr)
-            exit(1)
-
-        flag_fp = os.path.join(opts.destination_path, 'normalize-unicode.flag')
-        open(flag_fp, 'w').close()
-
-    if opts.lowercase:
-        flag_fp = os.path.join(opts.destination_path, 'lowercase.flag')
-        open(flag_fp, 'w').close()
-
-    flag_fp = os.path.join(opts.destination_path, 'language.flag')
-    with open(flag_fp, 'w') as f:
-        f.write(opts.language)
-
-    flag_fp = os.path.join(opts.destination_path, 'database_backend.flag')
-    with open(flag_fp, 'w') as f:
-        f.write(opts.database_backend)
-
-    mrconso_path = os.path.join(opts.umls_installation_path, 'MRCONSO.RRF')
-    mrsty_path = os.path.join(opts.umls_installation_path, 'MRSTY.RRF')
-
-    mrconso_iterator = extract_from_mrconso(mrconso_path, mrsty_path, opts)
-
-    simstring_dir = os.path.join(opts.destination_path, 'umls-simstring.db')
-    cuisty_dir = os.path.join(opts.destination_path, 'cui-semtypes.db')
-
-    parse_and_encode_ngrams(mrconso_iterator, simstring_dir, cuisty_dir,
-                            database_backend=opts.database_backend)
-
-
-if __name__ == '__main__':
-    main()
+from __future__ import unicode_literals, division, print_function
+
+# built in modules
+import argparse
+import codecs
+import os
+from six.moves import input
+import shutil
+import sys
+import time
+try:
+    from unidecode import unidecode
+except ImportError:
+    pass
+
+
+# third party-dependencies
+import spacy
+
+
+# project modules
+from .toolbox import countlines, CuiSemTypesDB, SimstringDBWriter, mkdir
+from .constants import HEADERS_MRCONSO, HEADERS_MRSTY, LANGUAGES, SPACY_LANGUAGE_MAP
+
+
+def get_semantic_types(path, headers):
+    sem_types = {}
+    with codecs.open(path, encoding='utf-8') as f:
+        for i, ln in enumerate(f):
+            content = dict(zip(headers, ln.strip().split('|')))
+
+            sem_types.setdefault(content['cui'], []).append(content['sty'])
+
+    return sem_types
+
+
+def get_mrconso_iterator(path, headers, lang='ENG'):
+    with codecs.open(path, encoding='utf-8') as f:
+        for i, ln in enumerate(f):
+            content = dict(zip(headers, ln.strip().split('|')))
+
+            if content['lat'] != lang:
+                continue
+
+            yield content
+
+
+def extract_from_mrconso(
+        mrconso_path, mrsty_path, opts,
+        mrconso_header=HEADERS_MRCONSO, mrsty_header=HEADERS_MRSTY):
+
+    start = time.time()
+    print('loading semantic types...', end=' ')
+    sys.stdout.flush()
+    sem_types = get_semantic_types(mrsty_path, mrsty_header)
+    print('done in {:.2f} s'.format(time.time() - start))
+
+    start = time.time()
+
+    mrconso_iterator = get_mrconso_iterator(
+        mrconso_path, mrconso_header, opts.language
+    )
+
+    total = countlines(mrconso_path)
+
+    processed = set()
+    i = 0
+
+    for content in mrconso_iterator:
+        i += 1
+
+        if i % 100000 == 0:
+            delta = time.time() - start
+            status = (
+                '{:,} in {:.2f} s ({:.2%}, {:.1e} s / term)'
+                ''.format(i, delta, i / total, delta / i if i > 0 else 0)
+            )
+            print(status)
+
+        concept_text = content['str'].strip()
+        cui = content['cui']
+        preferred = 1 if content['ispref'] == 'Y' else 0
+
+        if opts.lowercase:
+            concept_text = concept_text.lower()
+
+        if opts.normalize_unicode:
+            concept_text = unidecode(concept_text)
+
+        if (cui, concept_text) in processed:
+            continue
+        else:
+            processed.add((cui, concept_text))
+
+        yield (concept_text, cui, sem_types[cui], preferred)
+
+    delta = time.time() - start
+    status = (
+        '\nCOMPLETED: {:,} in {:.2f} s ({:.1e} s / term)'
+        ''.format(i, delta, i / total, delta / i if i > 0 else 0)
+    )
+    print(status)
+
+
+def parse_and_encode_ngrams(extracted_it, simstring_dir, cuisty_dir, database_backend):
+    # Create destination directories for the two databases
+    mkdir(simstring_dir)
+    mkdir(cuisty_dir)
+
+    ss_db = SimstringDBWriter(simstring_dir)
+    cuisty_db = CuiSemTypesDB(cuisty_dir, database_backend=database_backend)
+
+    simstring_terms = set()
+
+    for i, (term, cui, stys, preferred) in enumerate(extracted_it, start=1):
+        if term not in simstring_terms:
+            ss_db.insert(term)
+            simstring_terms.add(term)
+
+        cuisty_db.insert(term, cui, stys, preferred)
+
+
+def install_spacy(lang):
+    """Tries to create a spacy object; if it fails, downloads the dataset"""
+
+    print(f'Determining if SpaCy for language "{lang}" is installed...')
+
+    if lang in SPACY_LANGUAGE_MAP:
+        try:
+            spacy.load(SPACY_LANGUAGE_MAP[lang])
+            print(f'SpaCy is installed and avaliable for {lang}!')
+        except OSError:
+            print(f'SpaCy is not available! Attempting to download and install...')
+            spacy.cli.download(SPACY_LANGUAGE_MAP[lang])
+
+
+def parse_args():
+    ap = argparse.ArgumentParser()
+    ap.add_argument(
+        'umls_installation_path',
+        help=('Location of UMLS installation files (`MRCONSO.RRF` and '
+              '`MRSTY.RRF` files)')
+    )
+    ap.add_argument(
+        'destination_path',
+        help='Location where the necessary QuickUMLS files are installed'
+    )
+    ap.add_argument(
+        '-L', '--lowercase', action='store_true',
+        help='Consider only lowercase version of tokens'
+    )
+    ap.add_argument(
+        '-U', '--normalize-unicode', action='store_true',
+        help='Normalize unicode strings to their closest ASCII representation'
+    )
+    ap.add_argument(
+        '-d', '--database-backend', choices=('unqlite',), default='unqlite',
+        help='KV database to use to store CUIs and semantic types'
+    )
+    ap.add_argument(
+        '-E', '--language', default='ENG', choices=LANGUAGES,
+        help='Extract concepts of the specified language'
+    )
+    opts = ap.parse_args()
+    return opts
+
+
+def main():
+    opts = parse_args()
+
+    install_spacy(opts.language)
+
+    if not os.path.exists(opts.destination_path):
+        msg = ('Directory "{}" does not exists; should I create it? [y/N] '
+               ''.format(opts.destination_path))
+        create = input(msg).lower().strip() == 'y'
+
+        if create:
+            os.makedirs(opts.destination_path)
+        else:
+            print('Aborting.')
+            exit(1)
+
+    if len(os.listdir(opts.destination_path)) > 0:
+        msg = ('Directory "{}" is not empty; should I empty it? [y/N] '
+               ''.format(opts.destination_path))
+        empty = input(msg).lower().strip() == 'y'
+        if empty:
+            shutil.rmtree(opts.destination_path)
+            os.mkdir(opts.destination_path)
+        else:
+            print('Aborting.')
+            exit(1)
+
+    if opts.normalize_unicode:
+        try:
+            unidecode
+        except NameError:
+            err = ('`unidecode` is needed for unicode normalization'
+                   'please install it via the `[sudo] pip install '
+                   'unidecode` command.')
+            print(err, file=sys.stderr)
+            exit(1)
+
+        flag_fp = os.path.join(opts.destination_path, 'normalize-unicode.flag')
+        open(flag_fp, 'w').close()
+
+    if opts.lowercase:
+        flag_fp = os.path.join(opts.destination_path, 'lowercase.flag')
+        open(flag_fp, 'w').close()
+
+    flag_fp = os.path.join(opts.destination_path, 'language.flag')
+    with open(flag_fp, 'w') as f:
+        f.write(opts.language)
+
+    flag_fp = os.path.join(opts.destination_path, 'database_backend.flag')
+    with open(flag_fp, 'w') as f:
+        f.write(opts.database_backend)
+
+    mrconso_path = os.path.join(opts.umls_installation_path, 'MRCONSO.RRF')
+    mrsty_path = os.path.join(opts.umls_installation_path, 'MRSTY.RRF')
+
+    mrconso_iterator = extract_from_mrconso(mrconso_path, mrsty_path, opts)
+
+    simstring_dir = os.path.join(opts.destination_path, 'umls-simstring.db')
+    cuisty_dir = os.path.join(opts.destination_path, 'cui-semtypes.db')
+
+    parse_and_encode_ngrams(mrconso_iterator, simstring_dir, cuisty_dir,
+                            database_backend=opts.database_backend)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `medspacy_quickumls-2.7.1a0/quickumls/server.py` & `medspacy_quickumls-3.0/quickumls/server.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from argparse import ArgumentParser
-
-from .core import QuickUMLS
-from .network import run_server
-
-
-def run_quickumls_server(opts):
-    matcher = QuickUMLS(
-        quickumls_fp=opts.quickumls_fp,
-        threshold=opts.threshold,
-        overlapping_criteria=opts.overlapping_criteria,
-        similarity_name=opts.similarity_name,
-        window=opts.window,
-        min_match_length=opts.min_match_length,
-        verbose=opts.verbose,
-        keep_uppercase=opts.keep_uppercase
-    )
-
-    run_server(matcher, host=opts.host, port=opts.port, buffersize=4096)
-
-
-def parse_args():
-    ap = ArgumentParser(
-        prog='QuickUMLS server',
-        description=(
-            'For more detailed instructions, visit '
-            'github.com/Georgetown-IR-Lab/QuickUMLS'
-        )
-    )
-
-    # required arguments
-    ap.add_argument(
-        'quickumls_fp',
-        help='directory where the QuickUMLS data files are installed.'
-    )
-
-    # server configuration
-    ap.add_argument(
-        '-H', '--host', default='localhost',
-        help='host of the server'
-    )
-    ap.add_argument(
-        '-P', '--port', default=4645, type=int,
-        help='port on which the script responds'
-    )
-
-    # QuickUMLS options
-    ap.add_argument(
-        '-t', '--threshold', default=0.7, type=float,
-        help='minimum similarity value between strings'
-    )
-    ap.add_argument(
-        '-o', '--overlapping_criteria', default='score',
-        choices=['score', 'length'],
-        help='criteria used to deal with overlapping concepts'
-    )
-
-    ap.add_argument(
-        '-s', '--similarity_name', default='jaccard',
-        choices=['dice', 'jaccard', 'cosine', 'overlap'],
-        help='name of similarity to use'
-    )
-    ap.add_argument(
-        '-w', '--window', default=5, type=int,
-        help='maximum number of tokens to consider for matching'
-    )
-    ap.add_argument(
-        '-l', '--min-match-length', default=3, type=int,
-        help='minimum length of a match'
-    )
-    ap.add_argument(
-        '-v', '--verbose', action='store_true',
-        help='return verbose information while running'
-    )
-    ap.add_argument(
-        '-u', '--keep_uppercase', action='store_true',
-        help='By default QuickUMLS converts all uppercase strings to lowercase'
-             '. This option disables that functionality, which makes QuickUMLS '
-             'useful for distinguishing acronyms from normal words. For this '
-             'the database should be installed without the -L option.'
-    )
-    return ap.parse_args()
-
-
-def main():
-    opts = parse_args()
-    run_quickumls_server(opts)
-
-
-if __name__ == '__main__':
-    main()
+from argparse import ArgumentParser
+
+from .core import QuickUMLS
+from .network import run_server
+
+
+def run_quickumls_server(opts):
+    matcher = QuickUMLS(
+        quickumls_fp=opts.quickumls_fp,
+        threshold=opts.threshold,
+        overlapping_criteria=opts.overlapping_criteria,
+        similarity_name=opts.similarity_name,
+        window=opts.window,
+        min_match_length=opts.min_match_length,
+        verbose=opts.verbose,
+        keep_uppercase=opts.keep_uppercase
+    )
+
+    run_server(matcher, host=opts.host, port=opts.port, buffersize=4096)
+
+
+def parse_args():
+    ap = ArgumentParser(
+        prog='QuickUMLS server',
+        description=(
+            'For more detailed instructions, visit '
+            'github.com/Georgetown-IR-Lab/QuickUMLS'
+        )
+    )
+
+    # required arguments
+    ap.add_argument(
+        'quickumls_fp',
+        help='directory where the QuickUMLS data files are installed.'
+    )
+
+    # server configuration
+    ap.add_argument(
+        '-H', '--host', default='localhost',
+        help='host of the server'
+    )
+    ap.add_argument(
+        '-P', '--port', default=4645, type=int,
+        help='port on which the script responds'
+    )
+
+    # QuickUMLS options
+    ap.add_argument(
+        '-t', '--threshold', default=0.7, type=float,
+        help='minimum similarity value between strings'
+    )
+    ap.add_argument(
+        '-o', '--overlapping_criteria', default='score',
+        choices=['score', 'length'],
+        help='criteria used to deal with overlapping concepts'
+    )
+
+    ap.add_argument(
+        '-s', '--similarity_name', default='jaccard',
+        choices=['dice', 'jaccard', 'cosine', 'overlap'],
+        help='name of similarity to use'
+    )
+    ap.add_argument(
+        '-w', '--window', default=5, type=int,
+        help='maximum number of tokens to consider for matching'
+    )
+    ap.add_argument(
+        '-l', '--min-match-length', default=3, type=int,
+        help='minimum length of a match'
+    )
+    ap.add_argument(
+        '-v', '--verbose', action='store_true',
+        help='return verbose information while running'
+    )
+    ap.add_argument(
+        '-u', '--keep_uppercase', action='store_true',
+        help='By default QuickUMLS converts all uppercase strings to lowercase'
+             '. This option disables that functionality, which makes QuickUMLS '
+             'useful for distinguishing acronyms from normal words. For this '
+             'the database should be installed without the -L option.'
+    )
+    return ap.parse_args()
+
+
+def main():
+    opts = parse_args()
+    run_quickumls_server(opts)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `medspacy_quickumls-2.7.1a0/quickumls/spacy_component.py` & `medspacy_quickumls-3.0/quickumls/spacy_component.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-from sys import platform
-from os import path
-from pathlib import Path
-from typing import Literal
-
-import spacy
-from spacy.tokens import Span
-from spacy.strings import StringStore
-from spacy.language import Language
-
-from .core import QuickUMLS
-from . import constants
-from .umls_match import UmlsMatch
-from .constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
-
-@Language.factory("medspacy_quickumls")
-class SpacyQuickUMLS(object):
-
-    def __init__(self, nlp, name = "medspacy_quickumls", quickumls_fp=None,
-                 overlapping_criteria='score',
-                 threshold=0.7,
-                 window=5,
-                 similarity_name='jaccard',
-                 min_match_length=3,
-                 accepted_semtypes=constants.ACCEPTED_SEMTYPES,
-                 verbose=False,
-                 keep_uppercase=False,
-                 best_match=True,
-                 ignore_syntax=False,
-                 result_type: Literal["ents", "group"] = "ents",
-                 span_group_name: str = MEDSPACY_DEFAULT_SPAN_GROUP_NAME,
-                 ):
-        """Instantiate SpacyQuickUMLS object
-
-            This creates a QuickUMLS spaCy component which can be used in modular pipelines.  
-            This module adds either entity Spans (default) or Span Groups to the document where the  label is the UMLS CUI and the Span's
-                "underscore" object is extended to contain additional information about matched concepts.
-            Note that this implementation follows and enforces a known spacy convention on entities
-                that entity Spans cannot overlap on a single token.  If SpanGroups are selected instead, they may overlap
-
-        Args:
-            nlp: Existing spaCy pipeline.  This is needed to update the vocabulary with UMLS CUI values
-            quickumls_fp (str): Path to QuickUMLS data
-            overlapping_criteria (str, optional):
-                    One of "score" or "length". Choose how results are ranked.
-                    Choose "score" for best matching score first or "length" for longest match first.. Defaults to 'score'.
-            threshold (float, optional): Minimum similarity between strings. Defaults to 0.7.
-            window (int, optional): Maximum amount of tokens to consider for matching. Defaults to 5.
-            similarity_name (str, optional): One of "dice", "jaccard", "cosine", or "overlap".
-                    Similarity measure to be used. Defaults to 'jaccard'.
-            min_match_length (int, optional): TODO: ??. Defaults to 3.
-            accepted_semtypes (List[str], optional): Set of UMLS semantic types concepts should belong to.
-                Semantic types are identified by the letter "T" followed by three numbers
-                (e.g., "T131", which identifies the type "Hazardous or Poisonous Substance").
-                Defaults to constants.ACCEPTED_SEMTYPES.
-            verbose (bool, optional): TODO:??. Defaults to False.
-            keep_uppercase (bool, optional): By default QuickUMLS converts all
-                    uppercase strings to lowercase. This option disables that
-                    functionality, which makes QuickUMLS useful for
-                    distinguishing acronyms from normal words. For this the
-                    database should be installed without the -L option.
-                    Defaults to False.
-            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
-            ignore_syntax (bool, optional): Whether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False
-            result_type: "ents" (default), or "group". Determines where component will put the matched spans.
-                "ents" will add spans to doc.ents and add to any existing entities, but does not allow overlapping.
-                "group" will add spans to doc.spans under the specified group name.
-            span_group_name: The name of the span group used to store results when result_type is "group". Default is
-                "medspacy_spans".
-        """
-
-        if quickumls_fp is None:
-            # let's use a default sample that we provide in medspacy
-            # NOTE: Currently QuickUMLS uses an older fork of simstring where databases
-            # cannot be shared between Windows and POSIX systems so we distribute the sample for both:
-
-            quickumls_platform_dir = "QuickUMLS_SAMPLE_lowercase_POSIX_unqlite"
-            if platform.startswith("win"):
-                quickumls_platform_dir = "QuickUMLS_SAMPLE_lowercase_Windows_unqlite"
-
-            quickumls_fp = path.join(
-                Path(__file__).resolve().parents[1], "resources", "quickumls/{0}".format(quickumls_platform_dir)
-            )
-            print("Loading QuickUMLS resources from a default SAMPLE of UMLS data from here: {}".format(quickumls_fp))
-        
-        self.quickumls = QuickUMLS(quickumls_fp, 
-            # By default, the QuickUMLS objects creates its own internal spacy pipeline but this is not needed
-            # when we're using it as a component in a pipeline
-            spacy_component = True,
-            overlapping_criteria=overlapping_criteria,
-            threshold=threshold,
-            window=window,
-            similarity_name=similarity_name,
-            min_match_length=min_match_length,
-            accepted_semtypes=accepted_semtypes,
-            verbose=verbose,
-            keep_uppercase=keep_uppercase
-            )
-        
-        # save this off so that we can get vocab values of labels later
-        self.nlp = nlp
-        self.name = name
-        
-        # keep these for matching
-        self.best_match = best_match
-        self.ignore_syntax = ignore_syntax
-        self.verbose = verbose
-
-        self._result_type = result_type
-        self._span_group_name = span_group_name
-
-        # let's extend this with some proprties that we want
-        # NOTE: These two might be deprecated at some point since we now have
-        # umls_matches below which contains more information and enables overlapping
-        if not Span.has_extension("similarity"):
-            Span.set_extension('similarity', default = -1.0)
-        if not Span.has_extension("semtypes"): 
-            Span.set_extension('semtypes', default = -1.0)
-
-        # match objects are a set, since span objects with the same start/end keys
-        # would have the same values for custom attributes in spacy
-        if not Span.has_extension("umls_matches"):
-            Span.set_extension('umls_matches', default=set())
-
-    @property
-    def result_type(self) -> str:
-        """
-        The result type of the component. "ents" indicates that calling TargetMatcher will store the results in
-        doc.ents, "group" indicates that the results will be stored in the span group indicated by `span_group_name`,
-
-        Returns:
-            The result type string.
-        """
-        return self._result_type
-
-    @result_type.setter
-    def result_type(self, result_type: Literal["ents", "group"]):
-        if not (result_type == "group" or result_type == "ents"):
-            raise ValueError('result_type must be "ents", or "group".')
-        self._result_type = result_type
-
-    @property
-    def span_group_name(self) -> str:
-        """
-        The name of the span group used by this component. If `result_type` is "group", calling this component will
-        place results in the span group with this name.
-
-        Returns:
-            The span group name.
-        """
-        return self._span_group_name
-
-    @span_group_name.setter
-    def span_group_name(self, name: str):
-        if not name or not isinstance(name, str):
-            raise ValueError("Span group name must be a string.")
-        self._span_group_name = name
-        
-    def __call__(self, doc):
-        # pass in the document which has been parsed to this point in the pipeline for ngrams and matches
-        matches = self.quickumls._match(doc, best_match=self.best_match, ignore_syntax=self.ignore_syntax)
-        
-        # NOTE: Spacy spans do not allow overlapping tokens, so we prevent the overlap here
-        # For more information, see: https://github.com/explosion/spaCy/issues/3608
-        tokens_in_ents_set = set()
-
-        if self.result_type.lower() == "group":
-            # set up an empty list if there are no spans yet
-            doc.spans.setdefault(self.span_group_name, [])
-        
-        # let's track any other entities which may have been attached via upstream components
-        for ent in doc.ents:
-            for token_index in range(ent.start, ent.end):
-                tokens_in_ents_set.add(token_index)
-        
-        # Convert QuickUMLS match objects into Spans
-        for match in matches:
-            # each match may match multiple ngrams
-            for ngram_match_dict in match:
-                start_char_idx = int(ngram_match_dict['start'])
-                end_char_idx = int(ngram_match_dict['end'])
-                
-                cui = ngram_match_dict['cui']
-                # add the string to the spacy vocab
-                self.nlp.vocab.strings.add(cui)
-                # pull out the value
-                cui_label_value = self.nlp.vocab.strings[cui]
-                
-                # char_span() creates a Span from these character indices
-                # UMLS CUI should work well as the label here
-                span = doc.char_span(start_char_idx, end_char_idx, label = cui_label_value)
-                
-                # before we add this, let's make sure that this entity does not overlap any tokens added thus far
-                candidate_token_indexes = set(range(span.start, span.end))
-                
-                # check the intersection and skip this if there is any overlap
-                if self.result_type.lower() == "ents" and len(tokens_in_ents_set.intersection(candidate_token_indexes)) > 0:
-                    continue
-                    
-                # track this to make sure we do not introduce overlap later
-                tokens_in_ents_set.update(candidate_token_indexes)
-                
-                # add some custom metadata to the spans
-                span._.similarity = ngram_match_dict['similarity']
-                span._.semtypes = ngram_match_dict['semtypes']
-
-                # let's create this more fully featured match object
-                umls_match = UmlsMatch(cui,
-                                       ngram_match_dict['semtypes'],
-                                       ngram_match_dict['similarity'])
-
-                span._.umls_matches.add(umls_match)
-
-                if self.result_type.lower() == "ents":
-                    doc.ents = list(doc.ents) + [span]
-                elif self.result_type.lower() == "group":
-                    doc.spans[self.span_group_name].append(span)
-                
-        return doc
+from sys import platform
+from os import path
+from pathlib import Path
+from typing import Literal
+
+import spacy
+from spacy.tokens import Span
+from spacy.strings import StringStore
+from spacy.language import Language
+
+from .core import QuickUMLS
+from . import constants
+from .umls_match import UmlsMatch
+from .constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
+
+@Language.factory("medspacy_quickumls")
+class SpacyQuickUMLS(object):
+
+    def __init__(self, nlp, name = "medspacy_quickumls", quickumls_fp=None,
+                 overlapping_criteria='score',
+                 threshold=0.7,
+                 window=5,
+                 similarity_name='jaccard',
+                 min_match_length=3,
+                 accepted_semtypes=constants.ACCEPTED_SEMTYPES,
+                 verbose=False,
+                 keep_uppercase=False,
+                 best_match=True,
+                 ignore_syntax=False,
+                 result_type: Literal["ents", "group"] = "ents",
+                 span_group_name: str = MEDSPACY_DEFAULT_SPAN_GROUP_NAME,
+                 ):
+        """Instantiate SpacyQuickUMLS object
+
+            This creates a QuickUMLS spaCy component which can be used in modular pipelines.  
+            This module adds either entity Spans (default) or Span Groups to the document where the  label is the UMLS CUI and the Span's
+                "underscore" object is extended to contain additional information about matched concepts.
+            Note that this implementation follows and enforces a known spacy convention on entities
+                that entity Spans cannot overlap on a single token.  If SpanGroups are selected instead, they may overlap
+
+        Args:
+            nlp: Existing spaCy pipeline.  This is needed to update the vocabulary with UMLS CUI values
+            quickumls_fp (str): Path to QuickUMLS data
+            overlapping_criteria (str, optional):
+                    One of "score" or "length". Choose how results are ranked.
+                    Choose "score" for best matching score first or "length" for longest match first.. Defaults to 'score'.
+            threshold (float, optional): Minimum similarity between strings. Defaults to 0.7.
+            window (int, optional): Maximum amount of tokens to consider for matching. Defaults to 5.
+            similarity_name (str, optional): One of "dice", "jaccard", "cosine", or "overlap".
+                    Similarity measure to be used. Defaults to 'jaccard'.
+            min_match_length (int, optional): TODO: ??. Defaults to 3.
+            accepted_semtypes (List[str], optional): Set of UMLS semantic types concepts should belong to.
+                Semantic types are identified by the letter "T" followed by three numbers
+                (e.g., "T131", which identifies the type "Hazardous or Poisonous Substance").
+                Defaults to constants.ACCEPTED_SEMTYPES.
+            verbose (bool, optional): TODO:??. Defaults to False.
+            keep_uppercase (bool, optional): By default QuickUMLS converts all
+                    uppercase strings to lowercase. This option disables that
+                    functionality, which makes QuickUMLS useful for
+                    distinguishing acronyms from normal words. For this the
+                    database should be installed without the -L option.
+                    Defaults to False.
+            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
+            ignore_syntax (bool, optional): Whether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False
+            result_type: "ents" (default), or "group". Determines where component will put the matched spans.
+                "ents" will add spans to doc.ents and add to any existing entities, but does not allow overlapping.
+                "group" will add spans to doc.spans under the specified group name.
+            span_group_name: The name of the span group used to store results when result_type is "group". Default is
+                "medspacy_spans".
+        """
+
+        if quickumls_fp is None:
+            # let's use a default sample that we provide in medspacy
+            # NOTE: Currently QuickUMLS uses an older fork of simstring where databases
+            # cannot be shared between Windows and POSIX systems so we distribute the sample for both:
+
+            quickumls_platform_dir = "QuickUMLS_SAMPLE_lowercase_POSIX_unqlite"
+            if platform.startswith("win"):
+                quickumls_platform_dir = "QuickUMLS_SAMPLE_lowercase_Windows_unqlite"
+
+            quickumls_fp = path.join(
+                Path(__file__).resolve().parents[1], "resources", "quickumls/{0}".format(quickumls_platform_dir)
+            )
+            print("Loading QuickUMLS resources from a default SAMPLE of UMLS data from here: {}".format(quickumls_fp))
+        
+        self.quickumls = QuickUMLS(quickumls_fp, 
+            # By default, the QuickUMLS objects creates its own internal spacy pipeline but this is not needed
+            # when we're using it as a component in a pipeline
+            spacy_component = True,
+            overlapping_criteria=overlapping_criteria,
+            threshold=threshold,
+            window=window,
+            similarity_name=similarity_name,
+            min_match_length=min_match_length,
+            accepted_semtypes=accepted_semtypes,
+            verbose=verbose,
+            keep_uppercase=keep_uppercase
+            )
+        
+        # save this off so that we can get vocab values of labels later
+        self.nlp = nlp
+        self.name = name
+        
+        # keep these for matching
+        self.best_match = best_match
+        self.ignore_syntax = ignore_syntax
+        self.verbose = verbose
+
+        self._result_type = result_type
+        self._span_group_name = span_group_name
+
+        # let's extend this with some proprties that we want
+        # NOTE: These two might be deprecated at some point since we now have
+        # umls_matches below which contains more information and enables overlapping
+        if not Span.has_extension("similarity"):
+            Span.set_extension('similarity', default = -1.0)
+        if not Span.has_extension("semtypes"): 
+            Span.set_extension('semtypes', default = -1.0)
+
+        # match objects are a set, since span objects with the same start/end keys
+        # would have the same values for custom attributes in spacy
+        if not Span.has_extension("umls_matches"):
+            Span.set_extension('umls_matches', default=set())
+
+    @property
+    def result_type(self) -> str:
+        """
+        The result type of the component. "ents" indicates that calling TargetMatcher will store the results in
+        doc.ents, "group" indicates that the results will be stored in the span group indicated by `span_group_name`,
+
+        Returns:
+            The result type string.
+        """
+        return self._result_type
+
+    @result_type.setter
+    def result_type(self, result_type: Literal["ents", "group"]):
+        if not (result_type == "group" or result_type == "ents"):
+            raise ValueError('result_type must be "ents", or "group".')
+        self._result_type = result_type
+
+    @property
+    def span_group_name(self) -> str:
+        """
+        The name of the span group used by this component. If `result_type` is "group", calling this component will
+        place results in the span group with this name.
+
+        Returns:
+            The span group name.
+        """
+        return self._span_group_name
+
+    @span_group_name.setter
+    def span_group_name(self, name: str):
+        if not name or not isinstance(name, str):
+            raise ValueError("Span group name must be a string.")
+        self._span_group_name = name
+        
+    def __call__(self, doc):
+        # pass in the document which has been parsed to this point in the pipeline for ngrams and matches
+        matches = self.quickumls._match(doc, best_match=self.best_match, ignore_syntax=self.ignore_syntax)
+        
+        # NOTE: Spacy spans do not allow overlapping tokens, so we prevent the overlap here
+        # For more information, see: https://github.com/explosion/spaCy/issues/3608
+        tokens_in_ents_set = set()
+
+        if self.result_type.lower() == "group":
+            # set up an empty list if there are no spans yet
+            doc.spans.setdefault(self.span_group_name, [])
+        
+        # let's track any other entities which may have been attached via upstream components
+        for ent in doc.ents:
+            for token_index in range(ent.start, ent.end):
+                tokens_in_ents_set.add(token_index)
+        
+        # Convert QuickUMLS match objects into Spans
+        for match in matches:
+            # each match may match multiple ngrams
+            for ngram_match_dict in match:
+                start_char_idx = int(ngram_match_dict['start'])
+                end_char_idx = int(ngram_match_dict['end'])
+                
+                cui = ngram_match_dict['cui']
+                # add the string to the spacy vocab
+                self.nlp.vocab.strings.add(cui)
+                # pull out the value
+                cui_label_value = self.nlp.vocab.strings[cui]
+                
+                # char_span() creates a Span from these character indices
+                # UMLS CUI should work well as the label here
+                span = doc.char_span(start_char_idx, end_char_idx, label = cui_label_value)
+                
+                # before we add this, let's make sure that this entity does not overlap any tokens added thus far
+                candidate_token_indexes = set(range(span.start, span.end))
+                
+                # check the intersection and skip this if there is any overlap
+                if self.result_type.lower() == "ents" and len(tokens_in_ents_set.intersection(candidate_token_indexes)) > 0:
+                    continue
+                    
+                # track this to make sure we do not introduce overlap later
+                tokens_in_ents_set.update(candidate_token_indexes)
+                
+                # add some custom metadata to the spans
+                span._.similarity = ngram_match_dict['similarity']
+                span._.semtypes = ngram_match_dict['semtypes']
+
+                # let's create this more fully featured match object
+                umls_match = UmlsMatch(cui,
+                                       ngram_match_dict['semtypes'],
+                                       ngram_match_dict['similarity'])
+
+                span._.umls_matches.add(umls_match)
+
+                if self.result_type.lower() == "ents":
+                    doc.ents = list(doc.ents) + [span]
+                elif self.result_type.lower() == "group":
+                    doc.spans[self.span_group_name].append(span)
+                
+        return doc
```

### Comparing `medspacy_quickumls-2.7.1a0/quickumls/toolbox.py` & `medspacy_quickumls-3.0/quickumls/toolbox.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-from __future__ import unicode_literals, division, print_function
-
-# build-in modules
-import re
-import os
-from functools import wraps
-import six
-import unicodedata
-from string import punctuation
-from itertools import takewhile, repeat
-from six.moves import xrange
-
-# installed modules
-import numpy
-
-try:
-    import unqlite
-    UNQLITE_AVAILABLE = True
-except ImportError:
-    UNQLITE_AVAILABLE = False
-
-# project imports
-from quickumls_simstring import simstring
-
-
-# Python version specific imports
-if six.PY2:
-    import cPickle as pickle
-else:
-    import pickle
-
-
-def pickle_loading(data):
-    pass
-
-
-def pickle_dumping(data):
-    pass
-
-
-def mkdir(path):
-    try:
-        os.makedirs(path)
-        return True
-    except OSError:
-        return False
-
-
-def count_ngrams(s, n):
-    return len(s) + n - 1
-
-
-def safe_unicode(s):
-    if six.PY2:
-        # in python 3, there no ambiguity on whether
-        # a string is encoded in bytes format or not
-        try:
-            s = u'%s' % s
-        except UnicodeDecodeError:
-            s = u'%s' % s.decode('utf-8')
-
-    return u'{}'.format(unicodedata.normalize('NFKD', s))
-
-
-def prepare_string_for_db_input(s):
-    if six.PY2:
-        return s.encode('utf-8')
-    else:
-        return s
-
-
-def make_ngrams(s, n):
-    # s = u'{t}{s}{t}'.format(s=safe_unicode(s), t=('$' * (n - 1)))
-    n = len(s) if len(s) < n else n
-    return (s[i:i + n] for i in xrange(len(s) - n + 1))
-
-
-def get_similarity(x, y, n, similarity_name):
-    if len(x) == 0 or len(y) == 0:
-        # we define similarity between two strings
-        # to be 0 if any of the two is empty.
-        return 0.
-
-    X, Y = set(make_ngrams(x, n)), set(make_ngrams(y, n))
-    intersec = len(X.intersection(Y))
-
-    if similarity_name == 'dice':
-        return 2 * intersec / (len(X) + len(Y))
-    elif similarity_name == 'jaccard':
-        return intersec / (len(X) + len(Y) - intersec)
-    elif similarity_name == 'cosine':
-        return intersec / numpy.sqrt(len(X) * len(Y))
-    elif similarity_name == 'overlap':
-        return intersec
-    else:
-        msg = 'Similarity {} not recognized'.format(similarity_name)
-        raise TypeError(msg)
-
-
-class SimpleTokenizer(object):
-    def __init__(self, stopwords=None, min_length=1, split_sym=None):
-        if stopwords == 'default':
-            stopwords = [
-                'a', 'an', 'and', 'are', 'as', 'at', 'be', 'by', 'for',
-                'from', 'has', 'he', 'in', 'is', 'its', 'of', 'on', 'or',
-                'that', 'the', 'to', 'was ', 'were', 'will', 'with'
-            ]
-        elif stopwords is None:
-            stopwords = []
-
-        self.stopwords = set(stopwords)
-
-        if split_sym is None:
-            split_sym = []
-
-        split_sym = punctuation + ''.join(split_sym)
-
-        self.min_length = min_length
-        self.re_tokenize = re.compile(r'&\w+;|\W+|_')
-
-    def tokenize(self, text, lower=True):
-        """Tokenize text"""
-        if lower:
-            text = text.lower()
-        for tok in self.re_tokenize.split(text):
-            if len(tok) >= self.min_length and tok not in self.stopwords:
-                yield tok
-
-    def tokenize_list(self, text, lower=True):
-        if lower:
-            text = text.lower()
-        return [
-            tok for tok in self.re_tokenize.split(text)
-            if len(tok) >= self.min_length and tok not in self.stopwords
-        ]
-
-
-def db_key_encode(term):
-    if six.PY2:
-        return term
-    else:
-        return term.encode('utf-8')
-
-
-def countlines(fn):
-    """Count lines in fn. Slightly modified version of
-    http://stackoverflow.com/a/27518377"""
-    with open(fn, 'rb') as f:
-        bufgen = takewhile(
-            lambda x: x, (f.read(1024 * 1024) for _ in repeat(None)))
-        ln = sum(buf.count(b'\n') for buf in bufgen)
-    return ln
-
-
-class SimstringDBWriter(object):
-    def __init__(self, path):
-
-        if not(os.path.exists(path)) or not(os.path.isdir(path)):
-            err_msg = (
-                '"{}" does not exists or it is not a directory.'
-            ).format(path)
-            raise IOError(err_msg)
-        else:
-            try:
-                os.makedirs(path)
-            except OSError:
-                pass
-
-        self.db = simstring.writer(
-            prepare_string_for_db_input(
-                os.path.join(path, 'umls-terms.simstring')
-            ),
-            3, False, True
-        )
-
-    def insert(self, term):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        self.db.insert(term)
-
-
-class SimstringDBReader(object):
-    def __init__(self, path, similarity_name, threshold):
-        if not(os.path.exists(path)) or not(os.path.isdir(path)):
-            err_msg = (
-                '"{}" does not exists or it is not a directory.'
-            ).format(path)
-            raise IOError(err_msg)
-
-        self.db = simstring.reader(
-            prepare_string_for_db_input(
-                os.path.join(path, 'umls-terms.simstring')
-            )
-        )
-        self.db.measure = getattr(simstring, similarity_name)
-        self.db.threshold = threshold
-
-    def get(self, term):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        return self.db.retrieve(term)
-
-
-class Intervals(object):
-    def __init__(self):
-        self.intervals = []
-
-    def _is_overlapping_intervals(self, a, b):
-        if b[0] < a[1] and b[1] > a[0]:
-            return True
-        elif a[0] < b[1] and a[1] > b[0]:
-            return True
-        else:
-            return False
-
-    def __contains__(self, interval):
-        return any(
-            self._is_overlapping_intervals(interval, other)
-            for other in self.intervals
-        )
-
-    def append(self, interval):
-        self.intervals.append(interval)
-
-
-class CuiSemTypesDB(object):
-    def __init__(self, path, database_backend='unqlite'):
-        if not (os.path.exists(path) or os.path.isdir(path)):
-            err_msg = (
-                '"{}" is not a valid directory').format(path)
-            raise IOError(err_msg)
-
-        if database_backend == 'unqlite':
-            assert UNQLITE_AVAILABLE, (
-                'You selected unqlite as database backend, but it is not '
-                'installed. Please install it via `pip install unqlite`'
-            )
-            self.cui_db = unqlite.UnQLite(os.path.join(path, 'cui.unqlite'))
-            self.cui_db_put = self.cui_db.store
-            self.cui_db_get = self.cui_db.fetch
-            self.semtypes_db = unqlite.UnQLite(os.path.join(path, 'semtypes.unqlite'))
-            self.semtypes_db_put = self.semtypes_db.store
-            self.semtypes_db_get = self.semtypes_db.fetch
-        elif database_backend == 'leveldb':
-            raise ValueError(f'database_backend {database_backend} is no longer supported')
-        else:
-            raise ValueError(f'database_backend {database_backend} not recognized')
-
-    def has_term(self, term):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        try:
-            self.cui_db_get(db_key_encode(term))
-            return True
-        except KeyError:
-            return
-
-    def insert(self, term, cui, semtypes, is_preferred):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        cui = prepare_string_for_db_input(safe_unicode(cui))
-
-        # some terms have multiple cuis associated with them,
-        # so we store them all
-        try:
-            cuis = pickle.loads(self.cui_db_get(db_key_encode(term)))
-        except KeyError:
-            cuis = set()
-
-        cuis.add((cui, is_preferred))
-        self.cui_db_put(db_key_encode(term), pickle.dumps(cuis))
-
-        try:
-            self.semtypes_db_get(db_key_encode(cui))
-        except KeyError:
-            self.semtypes_db_put(
-                db_key_encode(cui), pickle.dumps(set(semtypes))
-            )
-
-    def get(self, term):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        try:
-            cuis = pickle.loads(self.cui_db_get(db_key_encode(term)))
-        except KeyError:
-            cuis = set()
-
-        matches = (
-            (
-                cui,
-                pickle.loads(self.semtypes_db_get(db_key_encode(cui))),
-                is_preferred
-            )
-            for cui, is_preferred in cuis
-        )
-        return matches
+from __future__ import unicode_literals, division, print_function
+
+# build-in modules
+import re
+import os
+from functools import wraps
+import six
+import unicodedata
+from string import punctuation
+from itertools import takewhile, repeat
+from six.moves import xrange
+
+# installed modules
+import numpy
+
+try:
+    import unqlite
+    UNQLITE_AVAILABLE = True
+except ImportError:
+    UNQLITE_AVAILABLE = False
+
+# project imports
+from pysimstring import simstring
+
+
+# Python version specific imports
+if six.PY2:
+    import cPickle as pickle
+else:
+    import pickle
+
+
+def pickle_loading(data):
+    pass
+
+
+def pickle_dumping(data):
+    pass
+
+
+def mkdir(path):
+    try:
+        os.makedirs(path)
+        return True
+    except OSError:
+        return False
+
+
+def count_ngrams(s, n):
+    return len(s) + n - 1
+
+
+def safe_unicode(s):
+    if six.PY2:
+        # in python 3, there no ambiguity on whether
+        # a string is encoded in bytes format or not
+        try:
+            s = u'%s' % s
+        except UnicodeDecodeError:
+            s = u'%s' % s.decode('utf-8')
+
+    return u'{}'.format(unicodedata.normalize('NFKD', s))
+
+
+def prepare_string_for_db_input(s):
+    if six.PY2:
+        return s.encode('utf-8')
+    else:
+        return s
+
+
+def make_ngrams(s, n):
+    # s = u'{t}{s}{t}'.format(s=safe_unicode(s), t=('$' * (n - 1)))
+    n = len(s) if len(s) < n else n
+    return (s[i:i + n] for i in xrange(len(s) - n + 1))
+
+
+def get_similarity(x, y, n, similarity_name):
+    if len(x) == 0 or len(y) == 0:
+        # we define similarity between two strings
+        # to be 0 if any of the two is empty.
+        return 0.
+
+    X, Y = set(make_ngrams(x, n)), set(make_ngrams(y, n))
+    intersec = len(X.intersection(Y))
+
+    if similarity_name == 'dice':
+        return 2 * intersec / (len(X) + len(Y))
+    elif similarity_name == 'jaccard':
+        return intersec / (len(X) + len(Y) - intersec)
+    elif similarity_name == 'cosine':
+        return intersec / numpy.sqrt(len(X) * len(Y))
+    elif similarity_name == 'overlap':
+        return intersec
+    else:
+        msg = 'Similarity {} not recognized'.format(similarity_name)
+        raise TypeError(msg)
+
+
+class SimpleTokenizer(object):
+    def __init__(self, stopwords=None, min_length=1, split_sym=None):
+        if stopwords == 'default':
+            stopwords = [
+                'a', 'an', 'and', 'are', 'as', 'at', 'be', 'by', 'for',
+                'from', 'has', 'he', 'in', 'is', 'its', 'of', 'on', 'or',
+                'that', 'the', 'to', 'was ', 'were', 'will', 'with'
+            ]
+        elif stopwords is None:
+            stopwords = []
+
+        self.stopwords = set(stopwords)
+
+        if split_sym is None:
+            split_sym = []
+
+        split_sym = punctuation + ''.join(split_sym)
+
+        self.min_length = min_length
+        self.re_tokenize = re.compile(r'&\w+;|\W+|_')
+
+    def tokenize(self, text, lower=True):
+        """Tokenize text"""
+        if lower:
+            text = text.lower()
+        for tok in self.re_tokenize.split(text):
+            if len(tok) >= self.min_length and tok not in self.stopwords:
+                yield tok
+
+    def tokenize_list(self, text, lower=True):
+        if lower:
+            text = text.lower()
+        return [
+            tok for tok in self.re_tokenize.split(text)
+            if len(tok) >= self.min_length and tok not in self.stopwords
+        ]
+
+
+def db_key_encode(term):
+    if six.PY2:
+        return term
+    else:
+        return term.encode('utf-8')
+
+
+def countlines(fn):
+    """Count lines in fn. Slightly modified version of
+    http://stackoverflow.com/a/27518377"""
+    with open(fn, 'rb') as f:
+        bufgen = takewhile(
+            lambda x: x, (f.read(1024 * 1024) for _ in repeat(None)))
+        ln = sum(buf.count(b'\n') for buf in bufgen)
+    return ln
+
+
+class SimstringDBWriter(object):
+    def __init__(self, path):
+
+        if not(os.path.exists(path)) or not(os.path.isdir(path)):
+            err_msg = (
+                '"{}" does not exists or it is not a directory.'
+            ).format(path)
+            raise IOError(err_msg)
+        else:
+            try:
+                os.makedirs(path)
+            except OSError:
+                pass
+
+        self.db = simstring.writer(
+            prepare_string_for_db_input(
+                os.path.join(path, 'umls-terms.simstring')
+            ),
+            3, False, True
+        )
+
+    def insert(self, term):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        self.db.insert(term)
+
+
+class SimstringDBReader(object):
+    def __init__(self, path, similarity_name, threshold):
+        if not(os.path.exists(path)) or not(os.path.isdir(path)):
+            err_msg = (
+                '"{}" does not exists or it is not a directory.'
+            ).format(path)
+            raise IOError(err_msg)
+
+        self.db = simstring.reader(
+            prepare_string_for_db_input(
+                os.path.join(path, 'umls-terms.simstring')
+            )
+        )
+        self.db.measure = getattr(simstring, similarity_name)
+        self.db.threshold = threshold
+
+    def get(self, term):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        return self.db.retrieve(term)
+
+
+class Intervals(object):
+    def __init__(self):
+        self.intervals = []
+
+    def _is_overlapping_intervals(self, a, b):
+        if b[0] < a[1] and b[1] > a[0]:
+            return True
+        elif a[0] < b[1] and a[1] > b[0]:
+            return True
+        else:
+            return False
+
+    def __contains__(self, interval):
+        return any(
+            self._is_overlapping_intervals(interval, other)
+            for other in self.intervals
+        )
+
+    def append(self, interval):
+        self.intervals.append(interval)
+
+
+class CuiSemTypesDB(object):
+    def __init__(self, path, database_backend='unqlite'):
+        if not (os.path.exists(path) or os.path.isdir(path)):
+            err_msg = (
+                '"{}" is not a valid directory').format(path)
+            raise IOError(err_msg)
+
+        if database_backend == 'unqlite':
+            assert UNQLITE_AVAILABLE, (
+                'You selected unqlite as database backend, but it is not '
+                'installed. Please install it via `pip install unqlite`'
+            )
+            self.cui_db = unqlite.UnQLite(os.path.join(path, 'cui.unqlite'))
+            self.cui_db_put = self.cui_db.store
+            self.cui_db_get = self.cui_db.fetch
+            self.semtypes_db = unqlite.UnQLite(os.path.join(path, 'semtypes.unqlite'))
+            self.semtypes_db_put = self.semtypes_db.store
+            self.semtypes_db_get = self.semtypes_db.fetch
+        elif database_backend == 'leveldb':
+            raise ValueError(f'database_backend {database_backend} is no longer supported')
+        else:
+            raise ValueError(f'database_backend {database_backend} not recognized')
+
+    def has_term(self, term):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        try:
+            self.cui_db_get(db_key_encode(term))
+            return True
+        except KeyError:
+            return
+
+    def insert(self, term, cui, semtypes, is_preferred):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        cui = prepare_string_for_db_input(safe_unicode(cui))
+
+        # some terms have multiple cuis associated with them,
+        # so we store them all
+        try:
+            cuis = pickle.loads(self.cui_db_get(db_key_encode(term)))
+        except KeyError:
+            cuis = set()
+
+        cuis.add((cui, is_preferred))
+        self.cui_db_put(db_key_encode(term), pickle.dumps(cuis))
+
+        try:
+            self.semtypes_db_get(db_key_encode(cui))
+        except KeyError:
+            self.semtypes_db_put(
+                db_key_encode(cui), pickle.dumps(set(semtypes))
+            )
+
+    def get(self, term):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        try:
+            cuis = pickle.loads(self.cui_db_get(db_key_encode(term)))
+        except KeyError:
+            cuis = set()
+
+        matches = (
+            (
+                cui,
+                pickle.loads(self.semtypes_db_get(db_key_encode(cui))),
+                is_preferred
+            )
+            for cui, is_preferred in cuis
+        )
+        return matches
```

### Comparing `medspacy_quickumls-2.7.1a0/quickumls/umls_match.py` & `medspacy_quickumls-3.0/quickumls/umls_match.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Set
-
-
-class UmlsMatch:
-
-    def __init__(self,
-                 cui: str,
-                 semtypes: Set[str],
-                 similarity: float):
-        """Instantiate UmlsMatch object
-
-                    This creates a QuickUMLS spaCy component which can be used in modular pipelines.
-                    This module adds entity Spans to the document where the entity label is the UMLS CUI and the Span's "underscore" object is extended to contains "similarity" and "semtypes" for matched concepts.
-                    Note that this implementation follows and enforces a known spacy convention that entity Spans cannot overlap on a single token.
-
-                Args:
-                    cui: UMLS controlled unique identifier (CUI) value (e.g., "C0243095")
-                    semtypes (Set[str]): List of UMLS semantic types as Type Unique Identifier values (TUI)
-                            for this matched concept (e.g., "T203")
-                    similarity (float): Similarity score between match and UMLS concept
-                """
-        self.cui = cui
-        self.semtypes = semtypes
-        self.similarity = similarity
+from typing import Set
+
+
+class UmlsMatch:
+
+    def __init__(self,
+                 cui: str,
+                 semtypes: Set[str],
+                 similarity: float):
+        """Instantiate UmlsMatch object
+
+                    This creates a QuickUMLS spaCy component which can be used in modular pipelines.
+                    This module adds entity Spans to the document where the entity label is the UMLS CUI and the Span's "underscore" object is extended to contains "similarity" and "semtypes" for matched concepts.
+                    Note that this implementation follows and enforces a known spacy convention that entity Spans cannot overlap on a single token.
+
+                Args:
+                    cui: UMLS controlled unique identifier (CUI) value (e.g., "C0243095")
+                    semtypes (Set[str]): List of UMLS semantic types as Type Unique Identifier values (TUI)
+                            for this matched concept (e.g., "T203")
+                    similarity (float): Similarity score between match and UMLS concept
+                """
+        self.cui = cui
+        self.semtypes = semtypes
+        self.similarity = similarity
```

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy_quickumls-3.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-2.7.1a0/setup.py` & `medspacy_quickumls-3.0/setup.py`

 * *Files identical despite different names*

