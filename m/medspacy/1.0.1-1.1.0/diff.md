# Comparing `tmp/medspacy-1.0.1.tar.gz` & `tmp/medspacy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspacy-1.0.1.tar", last modified: Mon Nov 28 20:19:52 2022, max compression
+gzip compressed data, was "medspacy-1.1.0.tar", last modified: Fri May  5 21:50:45 2023, max compression
```

## Comparing `medspacy-1.0.1.tar` & `medspacy-1.1.0.tar`

### file list

```diff
@@ -1,145 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.609281 medspacy-1.0.1/
--rw-rw-rw-   0        0        0     1086 2022-10-17 23:12:39.000000 medspacy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     7128 2022-11-28 20:19:52.608280 medspacy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2022-10-17 23:12:39.000000 medspacy-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.460780 medspacy-1.0.1/medspacy/
--rw-rw-rw-   0        0        0      225 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/__init__.py
--rw-rw-rw-   0        0        0     9786 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/_extensions.py
--rw-rw-rw-   0        0        0       23 2022-11-28 20:17:59.000000 medspacy-1.0.1/medspacy/_version.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.219281 medspacy-1.0.1/medspacy/common/
--rw-rw-rw-   0        0        0       33 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/__init__.py
--rw-rw-rw-   0        0        0     2130 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/base_rule.py
--rw-rw-rw-   0        0        0     6003 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/medspacy_matcher.py
--rw-rw-rw-   0        0        0     6845 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/regex_matcher.py
--rw-rw-rw-   0        0        0     6335 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/util.py
--rw-rw-rw-   0        0        0      518 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/components.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.288280 medspacy-1.0.1/medspacy/context/
--rw-rw-rw-   0        0        0      354 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/__init__.py
--rw-rw-rw-   0        0        0    13692 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context.py
--rw-rw-rw-   0        0        0     4572 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_graph.py
--rw-rw-rw-   0        0        0    15439 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_modifier.py
--rw-rw-rw-   0        0        0    11079 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_rule.py
--rw-rw-rw-   0        0        0      687 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/util.py
--rw-rw-rw-   0        0        0     1934 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/custom_tokenizer.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.386281 medspacy-1.0.1/medspacy/io/
--rw-rw-rw-   0        0        0      250 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/__init__.py
--rw-rw-rw-   0        0        0     5027 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/config_example.py
--rw-rw-rw-   0        0        0      133 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db.py
--rw-rw-rw-   0        0        0     3415 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_connect.py
--rw-rw-rw-   0        0        0      910 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_reader.py
--rw-rw-rw-   0        0        0     5737 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_writer.py
--rw-rw-rw-   0        0        0    11707 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/doc_consumer.py
--rw-rw-rw-   0        0        0     2847 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/pipeline.py
--rw-rw-rw-   0        0        0       98 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/ner.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.447780 medspacy-1.0.1/medspacy/postprocess/
--rw-rw-rw-   0        0        0      298 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/__init__.py
--rw-rw-rw-   0        0        0     8954 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_functions.py
--rw-rw-rw-   0        0        0     1529 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_pattern.py
--rw-rw-rw-   0        0        0     3450 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_rule.py
--rw-rw-rw-   0        0        0     4313 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessor.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.478281 medspacy-1.0.1/medspacy/preprocess/
--rw-rw-rw-   0        0        0      142 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/__init__.py
--rw-rw-rw-   0        0        0     4507 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/preprocessing_rule.py
--rw-rw-rw-   0        0        0     1840 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/preprocessor.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.530780 medspacy-1.0.1/medspacy/section_detection/
--rw-rw-rw-   0        0        0      192 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/__init__.py
--rw-rw-rw-   0        0        0     5399 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/section.py
--rw-rw-rw-   0        0        0     6085 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/section_rule.py
--rw-rw-rw-   0        0        0    22288 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/sectionizer.py
--rw-rw-rw-   0        0        0     1627 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/util.py
--rw-rw-rw-   0        0        0      765 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/sentence_splitting.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.569781 medspacy-1.0.1/medspacy/target_matcher/
--rw-rw-rw-   0        0        0      123 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/__init__.py
--rw-rw-rw-   0        0        0     2873 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/concept_tagger.py
--rw-rw-rw-   0        0        0     7355 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/target_matcher.py
--rw-rw-rw-   0        0        0     5196 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/target_rule.py
--rw-rw-rw-   0        0        0     8771 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/util.py
--rw-rw-rw-   0        0        0    11337 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/visualization.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.531280 medspacy-1.0.1/medspacy.egg-info/
--rw-rw-rw-   0        0        0     7128 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9130 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.564783 medspacy-1.0.1/resources/
--rw-rw-rw-   0        0        0    29201 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/context_rules.json
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.351781 medspacy-1.0.1/resources/quickumls/
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.601782 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
--rw-rw-rw-   0        0        0      183 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.619279 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-rw-rw-   0        0        0        7 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
--rw-rw-rw-   0        0        0        3 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.835780 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
--rw-rw-rw-   0        0        0     6116 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
--rw-rw-rw-   0        0        0     6892 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-rw-rw-   0        0        0     2788 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-rw-rw-   0        0        0     2664 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-rw-rw-   0        0        0     2744 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-rw-rw-   0        0        0     3016 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-rw-rw-   0        0        0     2904 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-rw-rw-   0        0        0     3140 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-rw-rw-   0        0        0     3228 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-rw-rw-   0        0        0     3460 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-rw-rw-   0        0        0     3148 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-rw-rw-   0        0        0     7344 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-rw-rw-   0        0        0     3224 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-rw-rw-   0        0        0     4984 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-rw-rw-   0        0        0     5152 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-rw-rw-   0        0        0     5024 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-rw-rw-   0        0        0     3384 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-rw-rw-   0        0        0     3824 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-rw-rw-   0        0        0     3544 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-rw-rw-   0        0        0     4064 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-rw-rw-   0        0        0     3624 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-rw-rw-   0        0        0     5160 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-rw-rw-   0        0        0     3788 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-rw-rw-   0        0        0     5368 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-rw-rw-   0        0        0     2384 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.863781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
--rw-rw-rw-   0        0        0      183 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.881781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
--rw-rw-rw-   0        0        0    20480 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-rw-rw-   0        0        0        7 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
--rw-rw-rw-   0        0        0        3 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.164781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
--rw-rw-rw-   0        0        0     2912 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
--rw-rw-rw-   0        0        0     6162 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-rw-rw-   0        0        0     2540 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-rw-rw-   0        0        0     2574 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-rw-rw-   0        0        0     2642 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-rw-rw-   0        0        0     2884 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-rw-rw-   0        0        0     2778 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-rw-rw-   0        0        0     2990 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-rw-rw-   0        0        0     3066 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-rw-rw-   0        0        0     3262 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-rw-rw-   0        0        0     2984 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-rw-rw-   0        0        0     5574 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-rw-rw-   0        0        0     3050 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-rw-rw-   0        0        0     4526 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-rw-rw-   0        0        0     3546 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-rw-rw-   0        0        0     4616 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-rw-rw-   0        0        0     3186 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-rw-rw-   0        0        0     3576 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-rw-rw-   0        0        0     3322 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-rw-rw-   0        0        0     3780 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-rw-rw-   0        0        0     3390 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-rw-rw-   0        0        0     4696 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-rw-rw-   0        0        0     3528 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-rw-rw-   0        0        0     4828 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-rw-rw-   0        0        0     2336 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
--rw-rw-rw-   0        0        0    24473 2022-11-28 20:06:06.000000 medspacy-1.0.1/resources/rush_rules.tsv
--rw-rw-rw-   0        0        0    12637 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/section_patterns.json
--rw-rw-rw-   0        0        0       42 2022-11-28 20:19:52.609781 medspacy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2529 2022-11-28 20:17:36.000000 medspacy-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.605780 medspacy-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     3078 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_extensions.py
--rw-rw-rw-   0        0        0     7542 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_medspacy.py
--rw-rw-rw-   0        0        0     3678 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:45.577851 medspacy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 21:50:40.000000 medspacy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-05-05 21:50:45.577851 medspacy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-05-05 21:50:40.000000 medspacy-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 21:50:40.000000 medspacy-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:45.577851 medspacy-1.1.0/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:45.577851 medspacy-1.1.0/resources/medspacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-05-05 21:50:45.000000 medspacy-1.1.0/resources/medspacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 21:50:45.000000 medspacy-1.1.0/resources/medspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:50:45.000000 medspacy-1.1.0/resources/medspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 21:50:45.000000 medspacy-1.1.0/resources/medspacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 21:50:45.000000 medspacy-1.1.0/resources/medspacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:50:45.577851 medspacy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-05 21:50:40.000000 medspacy-1.1.0/setup.py
```

### Comparing `medspacy-1.0.1/LICENSE` & `medspacy-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 medspacy
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 medspacy
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `medspacy-1.0.1/PKG-INFO` & `medspacy-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,156 +1,146 @@
-Metadata-Version: 2.1
-Name: medspacy
-Version: 1.0.1
-Summary: Library for clinical NLP with spaCy.
-Author: medSpaCy
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
-
-# medspacy
-Library for clinical NLP with spaCy. 
-
-![alt text](./images/medspacy_logo.png "medSpaCy logo")
-
-**MedSpaCy is currently in beta.**
-
-
-# Overview
-MedSpaCy is a library of tools for performing clinical NLP and text processing tasks with the popular [spaCy](https://spacy.io) 
-framework. The `medspacy` package brings together a number of other packages, each of which implements specific 
-functionality for common clinical text processing specific to the clinical domain, such as sentence segmentation, 
-contextual analysis and attribute assertion, and section detection.
-
-`medspacy` is modularized so that each component can be used independently. All of `medspacy` is designed to be used 
-as part of a `spacy` processing pipeline. Each of the following modules is available as part of `medspacy`:
-- `medspacy.preprocess`: Destructive preprocessing for modifying clinical text before processing
-- `medspacy.sentence_splitter`: Clinical sentence segmentation
-- `medspacy.ner`: Utilities for extracting concepts from clinical text
-- `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
-for detecting semantic modifiers and attributes of entities, including negation and uncertainty
-- `medspacy.section_detection`: Clinical section detection and segmentation
-- `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
-- `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
-- `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
-- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS).  More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
-	- NOTE: This component is installed by default on MacOS and Linux but not Windows.  For more defails and Windows installation: [QuickUMLS on Windows](windows_and_quickumls.md)
-
-Future work could include I/O, relations extraction, and pre-trained clinical models.
-
-**As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
-
-# Usage
-## Installation
-
-You can install `medspacy` using `setup.py`:
-```bash
-python setup.py install
-```
-
-Or with pip:
-```bash
-pip install medspacy
-```
-
-To install a previous version which uses spaCy 2:
-```bash
-pip install medspacy==medspacy 0.1.0.2
-```
-
-### Requirements
-The following packages are required and installed when `medspacy` is installed:
-- spaCy v3
-- [pyrush](https://github.com/medspacy/PyRuSH)
-
-If you download other models, you can use them by providing the model itself or model name to `medspacy.load(model_name)`:
-```python
-import spacy; import medspacy
-# Option 1: Load default
-nlp = medspacy.load()
-
-# Option 2: Load from existing model
-nlp = spacy.load("en_core_web_sm", disable={"ner"})
-nlp = medspacy.load(nlp)
-
-# Option 3: Load from model name
-nlp = medspacy.load("en_core_web_sm", disable={"ner"})
-```
-    
-## Basic Usage
-Here is a simple example showing how to implement and visualize a simple rule-based pipeline using `medspacy`:
-```python
-import medspacy
-from medspacy.ner import TargetRule
-from medspacy.visualization import visualize_ent
-
-# Load medspacy model
-nlp = medspacy.load()
-print(nlp.pipe_names)
-
-text = """
-Past Medical History:
-1. Atrial fibrillation
-2. Type II Diabetes Mellitus
-
-Assessment and Plan:
-There is no evidence of pneumonia. Continue warfarin for Afib. Follow up for management of type 2 DM.
-"""
-
-# Add rules for target concept extraction
-target_matcher = nlp.get_pipe("medspacy_target_matcher")
-target_rules = [
-    TargetRule("atrial fibrillation", "PROBLEM"),
-    TargetRule("atrial fibrillation", "PROBLEM", pattern=[{"LOWER": "afib"}]),
-    TargetRule("pneumonia", "PROBLEM"),
-    TargetRule("Type II Diabetes Mellitus", "PROBLEM", 
-              pattern=[
-                  {"LOWER": "type"},
-                  {"LOWER": {"IN": ["2", "ii", "two"]}},
-                  {"LOWER": {"IN": ["dm", "diabetes"]}},
-                  {"LOWER": "mellitus", "OP": "?"}
-              ]),
-    TargetRule("warfarin", "MEDICATION")
-]
-target_matcher.add(target_rules)
-
-doc = nlp(text)
-visualize_ent(doc)
-```
-
-`Output:`
-![alt text](./images/simple_text_visualization.png "Example of clinical text processed by medSpaCy")
-
-For more detailed examples and explanations of each component, see the [notebooks](./notebooks) folder.
-
-# Citing medspaCy
-If you use medspaCy in your work, consider citing our paper! Presented at the AMIA Annual Symposium 2021, [preprint available on Arxiv](http://arxiv.org/abs/2106.07799).
-
-```
-H. Eyre, A.B. Chapman, K.S. Peterson, J. Shi, P.R. Alba, M.M. Jones, T.L. Box, S.L. DuVall, O. V Patterson,
-Launching into clinical space with medspaCy: a new clinical text processing toolkit in Python,
-AMIA Annu. Symp. Proc. 2021 (in Press. (n.d.). 
-http://arxiv.org/abs/2106.07799.
-```
-
-```
-@Article{medspacy,
-   Author="Eyre, H.  and Chapman, A. B.  and Peterson, K. S.  and Shi, J.  and Alba, P. R.  and Jones, M. M.  and Box, T. L.  and DuVall, S. L.  and Patterson, O. V. ",
-   Title="{{L}aunching into clinical space with medspa{C}y: a new clinical text processing toolkit in {P}ython}",
-   Journal="AMIA Annu Symp Proc",
-   Year="2021",
-   Volume="2021",
-   Pages="438--447"
-}
-
-}
-```
-
-# Made with medSpaCy
-Here are some links to projects or tutorials which use medSpacy. If you have a project which uses medSpaCy which you'd like to use, let us know!
-- [VA_COVID-19_NLP_BSV](https://github.com/abchapman93/VA_COVID-19_NLP_BSV): An NLP pipeline for [identifying positive cases of COVID-19](https://aclanthology.org/2020.nlpcovid19-acl.10/) from clinical text. Deployed as part of the Department of Veterans Affairs response to COVID-19
-- [clinspacy](https://ml4lhs.github.io/clinspacy/index.html): An R wrapper for spaCy, sciSpaCy, and medSpaCy for performing clinical NLP and UMLS linking in R
-- [mimic34md2020_materials](https://github.com/Melbourne-BMDS/mimic34md2020_materials): A crash course in clinical data science from the University of Melbourne. For medSpaCy materials, see `notebooks/nlp-*.ipynb`
-- [ReHouSED NLP](https://github.com/abchapman93/ReHouSED): An NLP pipeline for [studying Veteran housing stability](https://www.sciencedirect.com/science/article/pii/S153204642100232X) and distinguishing between Veterans who are currently unstably housed and those who have exited homelessness
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
+
+# medspacy
+Library for clinical NLP with spaCy. 
+
+![alt text](./images/medspacy_logo.png "medSpaCy logo")
+
+**MedSpaCy is currently in beta.**
+
+
+# Overview
+MedSpaCy is a library of tools for performing clinical NLP and text processing tasks with the popular [spaCy](https://spacy.io) 
+framework. The `medspacy` package brings together a number of other packages, each of which implements specific 
+functionality for common clinical text processing specific to the clinical domain, such as sentence segmentation, 
+contextual analysis and attribute assertion, and section detection.
+
+`medspacy` is modularized so that each component can be used independently. All of `medspacy` is designed to be used 
+as part of a `spacy` processing pipeline. Each of the following modules is available as part of `medspacy`:
+- `medspacy.preprocess`: Destructive preprocessing for modifying clinical text before processing
+- `medspacy.sentence_splitter`: Clinical sentence segmentation
+- `medspacy.ner`: Utilities for extracting concepts from clinical text
+- `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
+for detecting semantic modifiers and attributes of entities, including negation and uncertainty
+- `medspacy.section_detection`: Clinical section detection and segmentation
+- `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
+- `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
+- `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
+- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [our fork](https://github.com/medspacy/QuickUMLS) of [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS). More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
+
+Future work could include I/O, relations extraction, and pre-trained clinical models.
+
+**As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
+
+# Usage
+## Installation
+
+You can install `medspacy` using `setup.py`:
+```bash
+python setup.py install
+```
+
+Or with pip:
+```bash
+pip install medspacy
+```
+
+To install a previous version which uses spaCy 2:
+```bash
+pip install medspacy==medspacy 0.1.0.2
+```
+
+### Requirements
+The following packages are required and installed when `medspacy` is installed:
+- spaCy v3
+- [pyrush](https://github.com/medspacy/PyRuSH)
+
+If you download other models, you can use them by providing the model itself or model name to `medspacy.load(model_name)`:
+```python
+import spacy; import medspacy
+# Option 1: Load default
+nlp = medspacy.load()
+
+# Option 2: Load from existing model
+nlp = spacy.load("en_core_web_sm", disable={"ner"})
+nlp = medspacy.load(nlp)
+
+# Option 3: Load from model name
+nlp = medspacy.load("en_core_web_sm", disable={"ner"})
+```
+    
+## Basic Usage
+Here is a simple example showing how to implement and visualize a simple rule-based pipeline using `medspacy`:
+```python
+import medspacy
+from medspacy.ner import TargetRule
+from medspacy.visualization import visualize_ent
+
+# Load medspacy model
+nlp = medspacy.load()
+print(nlp.pipe_names)
+
+text = """
+Past Medical History:
+1. Atrial fibrillation
+2. Type II Diabetes Mellitus
+
+Assessment and Plan:
+There is no evidence of pneumonia. Continue warfarin for Afib. Follow up for management of type 2 DM.
+"""
+
+# Add rules for target concept extraction
+target_matcher = nlp.get_pipe("medspacy_target_matcher")
+target_rules = [
+    TargetRule("atrial fibrillation", "PROBLEM"),
+    TargetRule("atrial fibrillation", "PROBLEM", pattern=[{"LOWER": "afib"}]),
+    TargetRule("pneumonia", "PROBLEM"),
+    TargetRule("Type II Diabetes Mellitus", "PROBLEM", 
+              pattern=[
+                  {"LOWER": "type"},
+                  {"LOWER": {"IN": ["2", "ii", "two"]}},
+                  {"LOWER": {"IN": ["dm", "diabetes"]}},
+                  {"LOWER": "mellitus", "OP": "?"}
+              ]),
+    TargetRule("warfarin", "MEDICATION")
+]
+target_matcher.add(target_rules)
+
+doc = nlp(text)
+visualize_ent(doc)
+```
+
+`Output:`
+![alt text](./images/simple_text_visualization.png "Example of clinical text processed by medSpaCy")
+
+For more detailed examples and explanations of each component, see the [notebooks](./notebooks) folder.
+
+# Citing medspaCy
+If you use medspaCy in your work, consider citing our paper! Presented at the AMIA Annual Symposium 2021, [preprint available on Arxiv](http://arxiv.org/abs/2106.07799).
+
+```
+H. Eyre, A.B. Chapman, K.S. Peterson, J. Shi, P.R. Alba, M.M. Jones, T.L. Box, S.L. DuVall, O. V Patterson,
+Launching into clinical space with medspaCy: a new clinical text processing toolkit in Python,
+AMIA Annu. Symp. Proc. 2021 (in Press. (n.d.). 
+http://arxiv.org/abs/2106.07799.
+```
+
+```
+@Article{medspacy,
+   Author="Eyre, H.  and Chapman, A. B.  and Peterson, K. S.  and Shi, J.  and Alba, P. R.  and Jones, M. M.  and Box, T. L.  and DuVall, S. L.  and Patterson, O. V. ",
+   Title="{{L}aunching into clinical space with medspa{C}y: a new clinical text processing toolkit in {P}ython}",
+   Journal="AMIA Annu Symp Proc",
+   Year="2021",
+   Volume="2021",
+   Pages="438--447"
+}
+
+}
+```
+
+# Made with medSpaCy
+Here are some links to projects or tutorials which use medSpacy. If you have a project which uses medSpaCy which you'd like to use, let us know!
+- [VA_COVID-19_NLP_BSV](https://github.com/abchapman93/VA_COVID-19_NLP_BSV): An NLP pipeline for [identifying positive cases of COVID-19](https://aclanthology.org/2020.nlpcovid19-acl.10/) from clinical text. Deployed as part of the Department of Veterans Affairs response to COVID-19
+- [clinspacy](https://ml4lhs.github.io/clinspacy/index.html): An R wrapper for spaCy, sciSpaCy, and medSpaCy for performing clinical NLP and UMLS linking in R
+- [mimic34md2020_materials](https://github.com/Melbourne-BMDS/mimic34md2020_materials): A crash course in clinical data science from the University of Melbourne. For medSpaCy materials, see `notebooks/nlp-*.ipynb`
+- [ReHouSED NLP](https://github.com/abchapman93/ReHouSED): An NLP pipeline for [studying Veteran housing stability](https://www.sciencedirect.com/science/article/pii/S153204642100232X) and distinguishing between Veterans who are currently unstably housed and those who have exited homelessness
```

### Comparing `medspacy-1.0.1/README.md` & `medspacy-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,180 @@
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
-
-# medspacy
-Library for clinical NLP with spaCy. 
-
-![alt text](./images/medspacy_logo.png "medSpaCy logo")
-
-**MedSpaCy is currently in beta.**
-
-
-# Overview
-MedSpaCy is a library of tools for performing clinical NLP and text processing tasks with the popular [spaCy](https://spacy.io) 
-framework. The `medspacy` package brings together a number of other packages, each of which implements specific 
-functionality for common clinical text processing specific to the clinical domain, such as sentence segmentation, 
-contextual analysis and attribute assertion, and section detection.
-
-`medspacy` is modularized so that each component can be used independently. All of `medspacy` is designed to be used 
-as part of a `spacy` processing pipeline. Each of the following modules is available as part of `medspacy`:
-- `medspacy.preprocess`: Destructive preprocessing for modifying clinical text before processing
-- `medspacy.sentence_splitter`: Clinical sentence segmentation
-- `medspacy.ner`: Utilities for extracting concepts from clinical text
-- `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
-for detecting semantic modifiers and attributes of entities, including negation and uncertainty
-- `medspacy.section_detection`: Clinical section detection and segmentation
-- `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
-- `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
-- `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
-- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS).  More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
-	- NOTE: This component is installed by default on MacOS and Linux but not Windows.  For more defails and Windows installation: [QuickUMLS on Windows](windows_and_quickumls.md)
-
-Future work could include I/O, relations extraction, and pre-trained clinical models.
-
-**As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
-
-# Usage
-## Installation
-
-You can install `medspacy` using `setup.py`:
-```bash
-python setup.py install
-```
-
-Or with pip:
-```bash
-pip install medspacy
-```
-
-To install a previous version which uses spaCy 2:
-```bash
-pip install medspacy==medspacy 0.1.0.2
-```
-
-### Requirements
-The following packages are required and installed when `medspacy` is installed:
-- spaCy v3
-- [pyrush](https://github.com/medspacy/PyRuSH)
-
-If you download other models, you can use them by providing the model itself or model name to `medspacy.load(model_name)`:
-```python
-import spacy; import medspacy
-# Option 1: Load default
-nlp = medspacy.load()
-
-# Option 2: Load from existing model
-nlp = spacy.load("en_core_web_sm", disable={"ner"})
-nlp = medspacy.load(nlp)
-
-# Option 3: Load from model name
-nlp = medspacy.load("en_core_web_sm", disable={"ner"})
-```
-    
-## Basic Usage
-Here is a simple example showing how to implement and visualize a simple rule-based pipeline using `medspacy`:
-```python
-import medspacy
-from medspacy.ner import TargetRule
-from medspacy.visualization import visualize_ent
-
-# Load medspacy model
-nlp = medspacy.load()
-print(nlp.pipe_names)
-
-text = """
-Past Medical History:
-1. Atrial fibrillation
-2. Type II Diabetes Mellitus
-
-Assessment and Plan:
-There is no evidence of pneumonia. Continue warfarin for Afib. Follow up for management of type 2 DM.
-"""
-
-# Add rules for target concept extraction
-target_matcher = nlp.get_pipe("medspacy_target_matcher")
-target_rules = [
-    TargetRule("atrial fibrillation", "PROBLEM"),
-    TargetRule("atrial fibrillation", "PROBLEM", pattern=[{"LOWER": "afib"}]),
-    TargetRule("pneumonia", "PROBLEM"),
-    TargetRule("Type II Diabetes Mellitus", "PROBLEM", 
-              pattern=[
-                  {"LOWER": "type"},
-                  {"LOWER": {"IN": ["2", "ii", "two"]}},
-                  {"LOWER": {"IN": ["dm", "diabetes"]}},
-                  {"LOWER": "mellitus", "OP": "?"}
-              ]),
-    TargetRule("warfarin", "MEDICATION")
-]
-target_matcher.add(target_rules)
-
-doc = nlp(text)
-visualize_ent(doc)
-```
-
-`Output:`
-![alt text](./images/simple_text_visualization.png "Example of clinical text processed by medSpaCy")
-
-For more detailed examples and explanations of each component, see the [notebooks](./notebooks) folder.
-
-# Citing medspaCy
-If you use medspaCy in your work, consider citing our paper! Presented at the AMIA Annual Symposium 2021, [preprint available on Arxiv](http://arxiv.org/abs/2106.07799).
-
-```
-H. Eyre, A.B. Chapman, K.S. Peterson, J. Shi, P.R. Alba, M.M. Jones, T.L. Box, S.L. DuVall, O. V Patterson,
-Launching into clinical space with medspaCy: a new clinical text processing toolkit in Python,
-AMIA Annu. Symp. Proc. 2021 (in Press. (n.d.). 
-http://arxiv.org/abs/2106.07799.
-```
-
-```
-@Article{medspacy,
-   Author="Eyre, H.  and Chapman, A. B.  and Peterson, K. S.  and Shi, J.  and Alba, P. R.  and Jones, M. M.  and Box, T. L.  and DuVall, S. L.  and Patterson, O. V. ",
-   Title="{{L}aunching into clinical space with medspa{C}y: a new clinical text processing toolkit in {P}ython}",
-   Journal="AMIA Annu Symp Proc",
-   Year="2021",
-   Volume="2021",
-   Pages="438--447"
-}
-
-}
-```
-
-# Made with medSpaCy
-Here are some links to projects or tutorials which use medSpacy. If you have a project which uses medSpaCy which you'd like to use, let us know!
-- [VA_COVID-19_NLP_BSV](https://github.com/abchapman93/VA_COVID-19_NLP_BSV): An NLP pipeline for [identifying positive cases of COVID-19](https://aclanthology.org/2020.nlpcovid19-acl.10/) from clinical text. Deployed as part of the Department of Veterans Affairs response to COVID-19
-- [clinspacy](https://ml4lhs.github.io/clinspacy/index.html): An R wrapper for spaCy, sciSpaCy, and medSpaCy for performing clinical NLP and UMLS linking in R
-- [mimic34md2020_materials](https://github.com/Melbourne-BMDS/mimic34md2020_materials): A crash course in clinical data science from the University of Melbourne. For medSpaCy materials, see `notebooks/nlp-*.ipynb`
-- [ReHouSED NLP](https://github.com/abchapman93/ReHouSED): An NLP pipeline for [studying Veteran housing stability](https://www.sciencedirect.com/science/article/pii/S153204642100232X) and distinguishing between Veterans who are currently unstably housed and those who have exited homelessness
+Metadata-Version: 2.1
+Name: medspacy
+Version: 1.1.0
+Summary: Library for clinical NLP with spaCy.
+Author: medSpaCy
+License: MIT License
+        
+        Copyright (c) 2020 medspacy
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Source, https://github.com/medspacy/medspacy
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
+
+# medspacy
+Library for clinical NLP with spaCy. 
+
+![alt text](./images/medspacy_logo.png "medSpaCy logo")
+
+**MedSpaCy is currently in beta.**
+
+
+# Overview
+MedSpaCy is a library of tools for performing clinical NLP and text processing tasks with the popular [spaCy](https://spacy.io) 
+framework. The `medspacy` package brings together a number of other packages, each of which implements specific 
+functionality for common clinical text processing specific to the clinical domain, such as sentence segmentation, 
+contextual analysis and attribute assertion, and section detection.
+
+`medspacy` is modularized so that each component can be used independently. All of `medspacy` is designed to be used 
+as part of a `spacy` processing pipeline. Each of the following modules is available as part of `medspacy`:
+- `medspacy.preprocess`: Destructive preprocessing for modifying clinical text before processing
+- `medspacy.sentence_splitter`: Clinical sentence segmentation
+- `medspacy.ner`: Utilities for extracting concepts from clinical text
+- `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
+for detecting semantic modifiers and attributes of entities, including negation and uncertainty
+- `medspacy.section_detection`: Clinical section detection and segmentation
+- `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
+- `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
+- `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
+- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [our fork](https://github.com/medspacy/QuickUMLS) of [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS). More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
+
+Future work could include I/O, relations extraction, and pre-trained clinical models.
+
+**As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
+
+# Usage
+## Installation
+
+You can install `medspacy` using `setup.py`:
+```bash
+python setup.py install
+```
+
+Or with pip:
+```bash
+pip install medspacy
+```
+
+To install a previous version which uses spaCy 2:
+```bash
+pip install medspacy==medspacy 0.1.0.2
+```
+
+### Requirements
+The following packages are required and installed when `medspacy` is installed:
+- spaCy v3
+- [pyrush](https://github.com/medspacy/PyRuSH)
+
+If you download other models, you can use them by providing the model itself or model name to `medspacy.load(model_name)`:
+```python
+import spacy; import medspacy
+# Option 1: Load default
+nlp = medspacy.load()
+
+# Option 2: Load from existing model
+nlp = spacy.load("en_core_web_sm", disable={"ner"})
+nlp = medspacy.load(nlp)
+
+# Option 3: Load from model name
+nlp = medspacy.load("en_core_web_sm", disable={"ner"})
+```
+    
+## Basic Usage
+Here is a simple example showing how to implement and visualize a simple rule-based pipeline using `medspacy`:
+```python
+import medspacy
+from medspacy.ner import TargetRule
+from medspacy.visualization import visualize_ent
+
+# Load medspacy model
+nlp = medspacy.load()
+print(nlp.pipe_names)
+
+text = """
+Past Medical History:
+1. Atrial fibrillation
+2. Type II Diabetes Mellitus
+
+Assessment and Plan:
+There is no evidence of pneumonia. Continue warfarin for Afib. Follow up for management of type 2 DM.
+"""
+
+# Add rules for target concept extraction
+target_matcher = nlp.get_pipe("medspacy_target_matcher")
+target_rules = [
+    TargetRule("atrial fibrillation", "PROBLEM"),
+    TargetRule("atrial fibrillation", "PROBLEM", pattern=[{"LOWER": "afib"}]),
+    TargetRule("pneumonia", "PROBLEM"),
+    TargetRule("Type II Diabetes Mellitus", "PROBLEM", 
+              pattern=[
+                  {"LOWER": "type"},
+                  {"LOWER": {"IN": ["2", "ii", "two"]}},
+                  {"LOWER": {"IN": ["dm", "diabetes"]}},
+                  {"LOWER": "mellitus", "OP": "?"}
+              ]),
+    TargetRule("warfarin", "MEDICATION")
+]
+target_matcher.add(target_rules)
+
+doc = nlp(text)
+visualize_ent(doc)
+```
+
+`Output:`
+![alt text](./images/simple_text_visualization.png "Example of clinical text processed by medSpaCy")
+
+For more detailed examples and explanations of each component, see the [notebooks](./notebooks) folder.
+
+# Citing medspaCy
+If you use medspaCy in your work, consider citing our paper! Presented at the AMIA Annual Symposium 2021, [preprint available on Arxiv](http://arxiv.org/abs/2106.07799).
+
+```
+H. Eyre, A.B. Chapman, K.S. Peterson, J. Shi, P.R. Alba, M.M. Jones, T.L. Box, S.L. DuVall, O. V Patterson,
+Launching into clinical space with medspaCy: a new clinical text processing toolkit in Python,
+AMIA Annu. Symp. Proc. 2021 (in Press. (n.d.). 
+http://arxiv.org/abs/2106.07799.
+```
+
+```
+@Article{medspacy,
+   Author="Eyre, H.  and Chapman, A. B.  and Peterson, K. S.  and Shi, J.  and Alba, P. R.  and Jones, M. M.  and Box, T. L.  and DuVall, S. L.  and Patterson, O. V. ",
+   Title="{{L}aunching into clinical space with medspa{C}y: a new clinical text processing toolkit in {P}ython}",
+   Journal="AMIA Annu Symp Proc",
+   Year="2021",
+   Volume="2021",
+   Pages="438--447"
+}
+
+}
+```
+
+# Made with medSpaCy
+Here are some links to projects or tutorials which use medSpacy. If you have a project which uses medSpaCy which you'd like to use, let us know!
+- [VA_COVID-19_NLP_BSV](https://github.com/abchapman93/VA_COVID-19_NLP_BSV): An NLP pipeline for [identifying positive cases of COVID-19](https://aclanthology.org/2020.nlpcovid19-acl.10/) from clinical text. Deployed as part of the Department of Veterans Affairs response to COVID-19
+- [clinspacy](https://ml4lhs.github.io/clinspacy/index.html): An R wrapper for spaCy, sciSpaCy, and medSpaCy for performing clinical NLP and UMLS linking in R
+- [mimic34md2020_materials](https://github.com/Melbourne-BMDS/mimic34md2020_materials): A crash course in clinical data science from the University of Melbourne. For medSpaCy materials, see `notebooks/nlp-*.ipynb`
+- [ReHouSED NLP](https://github.com/abchapman93/ReHouSED): An NLP pipeline for [studying Veteran housing stability](https://www.sciencedirect.com/science/article/pii/S153204642100232X) and distinguishing between Veterans who are currently unstably housed and those who have exited homelessness
```

### Comparing `medspacy-1.0.1/medspacy.egg-info/PKG-INFO` & `medspacy-1.1.0/resources/medspacy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,156 +1,180 @@
-Metadata-Version: 2.1
-Name: medspacy
-Version: 1.0.1
-Summary: Library for clinical NLP with spaCy.
-Author: medSpaCy
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
-
-# medspacy
-Library for clinical NLP with spaCy. 
-
-![alt text](./images/medspacy_logo.png "medSpaCy logo")
-
-**MedSpaCy is currently in beta.**
-
-
-# Overview
-MedSpaCy is a library of tools for performing clinical NLP and text processing tasks with the popular [spaCy](https://spacy.io) 
-framework. The `medspacy` package brings together a number of other packages, each of which implements specific 
-functionality for common clinical text processing specific to the clinical domain, such as sentence segmentation, 
-contextual analysis and attribute assertion, and section detection.
-
-`medspacy` is modularized so that each component can be used independently. All of `medspacy` is designed to be used 
-as part of a `spacy` processing pipeline. Each of the following modules is available as part of `medspacy`:
-- `medspacy.preprocess`: Destructive preprocessing for modifying clinical text before processing
-- `medspacy.sentence_splitter`: Clinical sentence segmentation
-- `medspacy.ner`: Utilities for extracting concepts from clinical text
-- `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
-for detecting semantic modifiers and attributes of entities, including negation and uncertainty
-- `medspacy.section_detection`: Clinical section detection and segmentation
-- `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
-- `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
-- `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
-- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS).  More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
-	- NOTE: This component is installed by default on MacOS and Linux but not Windows.  For more defails and Windows installation: [QuickUMLS on Windows](windows_and_quickumls.md)
-
-Future work could include I/O, relations extraction, and pre-trained clinical models.
-
-**As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
-
-# Usage
-## Installation
-
-You can install `medspacy` using `setup.py`:
-```bash
-python setup.py install
-```
-
-Or with pip:
-```bash
-pip install medspacy
-```
-
-To install a previous version which uses spaCy 2:
-```bash
-pip install medspacy==medspacy 0.1.0.2
-```
-
-### Requirements
-The following packages are required and installed when `medspacy` is installed:
-- spaCy v3
-- [pyrush](https://github.com/medspacy/PyRuSH)
-
-If you download other models, you can use them by providing the model itself or model name to `medspacy.load(model_name)`:
-```python
-import spacy; import medspacy
-# Option 1: Load default
-nlp = medspacy.load()
-
-# Option 2: Load from existing model
-nlp = spacy.load("en_core_web_sm", disable={"ner"})
-nlp = medspacy.load(nlp)
-
-# Option 3: Load from model name
-nlp = medspacy.load("en_core_web_sm", disable={"ner"})
-```
-    
-## Basic Usage
-Here is a simple example showing how to implement and visualize a simple rule-based pipeline using `medspacy`:
-```python
-import medspacy
-from medspacy.ner import TargetRule
-from medspacy.visualization import visualize_ent
-
-# Load medspacy model
-nlp = medspacy.load()
-print(nlp.pipe_names)
-
-text = """
-Past Medical History:
-1. Atrial fibrillation
-2. Type II Diabetes Mellitus
-
-Assessment and Plan:
-There is no evidence of pneumonia. Continue warfarin for Afib. Follow up for management of type 2 DM.
-"""
-
-# Add rules for target concept extraction
-target_matcher = nlp.get_pipe("medspacy_target_matcher")
-target_rules = [
-    TargetRule("atrial fibrillation", "PROBLEM"),
-    TargetRule("atrial fibrillation", "PROBLEM", pattern=[{"LOWER": "afib"}]),
-    TargetRule("pneumonia", "PROBLEM"),
-    TargetRule("Type II Diabetes Mellitus", "PROBLEM", 
-              pattern=[
-                  {"LOWER": "type"},
-                  {"LOWER": {"IN": ["2", "ii", "two"]}},
-                  {"LOWER": {"IN": ["dm", "diabetes"]}},
-                  {"LOWER": "mellitus", "OP": "?"}
-              ]),
-    TargetRule("warfarin", "MEDICATION")
-]
-target_matcher.add(target_rules)
-
-doc = nlp(text)
-visualize_ent(doc)
-```
-
-`Output:`
-![alt text](./images/simple_text_visualization.png "Example of clinical text processed by medSpaCy")
-
-For more detailed examples and explanations of each component, see the [notebooks](./notebooks) folder.
-
-# Citing medspaCy
-If you use medspaCy in your work, consider citing our paper! Presented at the AMIA Annual Symposium 2021, [preprint available on Arxiv](http://arxiv.org/abs/2106.07799).
-
-```
-H. Eyre, A.B. Chapman, K.S. Peterson, J. Shi, P.R. Alba, M.M. Jones, T.L. Box, S.L. DuVall, O. V Patterson,
-Launching into clinical space with medspaCy: a new clinical text processing toolkit in Python,
-AMIA Annu. Symp. Proc. 2021 (in Press. (n.d.). 
-http://arxiv.org/abs/2106.07799.
-```
-
-```
-@Article{medspacy,
-   Author="Eyre, H.  and Chapman, A. B.  and Peterson, K. S.  and Shi, J.  and Alba, P. R.  and Jones, M. M.  and Box, T. L.  and DuVall, S. L.  and Patterson, O. V. ",
-   Title="{{L}aunching into clinical space with medspa{C}y: a new clinical text processing toolkit in {P}ython}",
-   Journal="AMIA Annu Symp Proc",
-   Year="2021",
-   Volume="2021",
-   Pages="438--447"
-}
-
-}
-```
-
-# Made with medSpaCy
-Here are some links to projects or tutorials which use medSpacy. If you have a project which uses medSpaCy which you'd like to use, let us know!
-- [VA_COVID-19_NLP_BSV](https://github.com/abchapman93/VA_COVID-19_NLP_BSV): An NLP pipeline for [identifying positive cases of COVID-19](https://aclanthology.org/2020.nlpcovid19-acl.10/) from clinical text. Deployed as part of the Department of Veterans Affairs response to COVID-19
-- [clinspacy](https://ml4lhs.github.io/clinspacy/index.html): An R wrapper for spaCy, sciSpaCy, and medSpaCy for performing clinical NLP and UMLS linking in R
-- [mimic34md2020_materials](https://github.com/Melbourne-BMDS/mimic34md2020_materials): A crash course in clinical data science from the University of Melbourne. For medSpaCy materials, see `notebooks/nlp-*.ipynb`
-- [ReHouSED NLP](https://github.com/abchapman93/ReHouSED): An NLP pipeline for [studying Veteran housing stability](https://www.sciencedirect.com/science/article/pii/S153204642100232X) and distinguishing between Veterans who are currently unstably housed and those who have exited homelessness
+Metadata-Version: 2.1
+Name: medspacy
+Version: 1.1.0
+Summary: Library for clinical NLP with spaCy.
+Author: medSpaCy
+License: MIT License
+        
+        Copyright (c) 2020 medspacy
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Source, https://github.com/medspacy/medspacy
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
+
+# medspacy
+Library for clinical NLP with spaCy. 
+
+![alt text](./images/medspacy_logo.png "medSpaCy logo")
+
+**MedSpaCy is currently in beta.**
+
+
+# Overview
+MedSpaCy is a library of tools for performing clinical NLP and text processing tasks with the popular [spaCy](https://spacy.io) 
+framework. The `medspacy` package brings together a number of other packages, each of which implements specific 
+functionality for common clinical text processing specific to the clinical domain, such as sentence segmentation, 
+contextual analysis and attribute assertion, and section detection.
+
+`medspacy` is modularized so that each component can be used independently. All of `medspacy` is designed to be used 
+as part of a `spacy` processing pipeline. Each of the following modules is available as part of `medspacy`:
+- `medspacy.preprocess`: Destructive preprocessing for modifying clinical text before processing
+- `medspacy.sentence_splitter`: Clinical sentence segmentation
+- `medspacy.ner`: Utilities for extracting concepts from clinical text
+- `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
+for detecting semantic modifiers and attributes of entities, including negation and uncertainty
+- `medspacy.section_detection`: Clinical section detection and segmentation
+- `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
+- `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
+- `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
+- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [our fork](https://github.com/medspacy/QuickUMLS) of [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS). More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
+
+Future work could include I/O, relations extraction, and pre-trained clinical models.
+
+**As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
+
+# Usage
+## Installation
+
+You can install `medspacy` using `setup.py`:
+```bash
+python setup.py install
+```
+
+Or with pip:
+```bash
+pip install medspacy
+```
+
+To install a previous version which uses spaCy 2:
+```bash
+pip install medspacy==medspacy 0.1.0.2
+```
+
+### Requirements
+The following packages are required and installed when `medspacy` is installed:
+- spaCy v3
+- [pyrush](https://github.com/medspacy/PyRuSH)
+
+If you download other models, you can use them by providing the model itself or model name to `medspacy.load(model_name)`:
+```python
+import spacy; import medspacy
+# Option 1: Load default
+nlp = medspacy.load()
+
+# Option 2: Load from existing model
+nlp = spacy.load("en_core_web_sm", disable={"ner"})
+nlp = medspacy.load(nlp)
+
+# Option 3: Load from model name
+nlp = medspacy.load("en_core_web_sm", disable={"ner"})
+```
+    
+## Basic Usage
+Here is a simple example showing how to implement and visualize a simple rule-based pipeline using `medspacy`:
+```python
+import medspacy
+from medspacy.ner import TargetRule
+from medspacy.visualization import visualize_ent
+
+# Load medspacy model
+nlp = medspacy.load()
+print(nlp.pipe_names)
+
+text = """
+Past Medical History:
+1. Atrial fibrillation
+2. Type II Diabetes Mellitus
+
+Assessment and Plan:
+There is no evidence of pneumonia. Continue warfarin for Afib. Follow up for management of type 2 DM.
+"""
+
+# Add rules for target concept extraction
+target_matcher = nlp.get_pipe("medspacy_target_matcher")
+target_rules = [
+    TargetRule("atrial fibrillation", "PROBLEM"),
+    TargetRule("atrial fibrillation", "PROBLEM", pattern=[{"LOWER": "afib"}]),
+    TargetRule("pneumonia", "PROBLEM"),
+    TargetRule("Type II Diabetes Mellitus", "PROBLEM", 
+              pattern=[
+                  {"LOWER": "type"},
+                  {"LOWER": {"IN": ["2", "ii", "two"]}},
+                  {"LOWER": {"IN": ["dm", "diabetes"]}},
+                  {"LOWER": "mellitus", "OP": "?"}
+              ]),
+    TargetRule("warfarin", "MEDICATION")
+]
+target_matcher.add(target_rules)
+
+doc = nlp(text)
+visualize_ent(doc)
+```
+
+`Output:`
+![alt text](./images/simple_text_visualization.png "Example of clinical text processed by medSpaCy")
+
+For more detailed examples and explanations of each component, see the [notebooks](./notebooks) folder.
+
+# Citing medspaCy
+If you use medspaCy in your work, consider citing our paper! Presented at the AMIA Annual Symposium 2021, [preprint available on Arxiv](http://arxiv.org/abs/2106.07799).
+
+```
+H. Eyre, A.B. Chapman, K.S. Peterson, J. Shi, P.R. Alba, M.M. Jones, T.L. Box, S.L. DuVall, O. V Patterson,
+Launching into clinical space with medspaCy: a new clinical text processing toolkit in Python,
+AMIA Annu. Symp. Proc. 2021 (in Press. (n.d.). 
+http://arxiv.org/abs/2106.07799.
+```
+
+```
+@Article{medspacy,
+   Author="Eyre, H.  and Chapman, A. B.  and Peterson, K. S.  and Shi, J.  and Alba, P. R.  and Jones, M. M.  and Box, T. L.  and DuVall, S. L.  and Patterson, O. V. ",
+   Title="{{L}aunching into clinical space with medspa{C}y: a new clinical text processing toolkit in {P}ython}",
+   Journal="AMIA Annu Symp Proc",
+   Year="2021",
+   Volume="2021",
+   Pages="438--447"
+}
+
+}
+```
+
+# Made with medSpaCy
+Here are some links to projects or tutorials which use medSpacy. If you have a project which uses medSpaCy which you'd like to use, let us know!
+- [VA_COVID-19_NLP_BSV](https://github.com/abchapman93/VA_COVID-19_NLP_BSV): An NLP pipeline for [identifying positive cases of COVID-19](https://aclanthology.org/2020.nlpcovid19-acl.10/) from clinical text. Deployed as part of the Department of Veterans Affairs response to COVID-19
+- [clinspacy](https://ml4lhs.github.io/clinspacy/index.html): An R wrapper for spaCy, sciSpaCy, and medSpaCy for performing clinical NLP and UMLS linking in R
+- [mimic34md2020_materials](https://github.com/Melbourne-BMDS/mimic34md2020_materials): A crash course in clinical data science from the University of Melbourne. For medSpaCy materials, see `notebooks/nlp-*.ipynb`
+- [ReHouSED NLP](https://github.com/abchapman93/ReHouSED): An NLP pipeline for [studying Veteran housing stability](https://www.sciencedirect.com/science/article/pii/S153204642100232X) and distinguishing between Veterans who are currently unstably housed and those who have exited homelessness
```

