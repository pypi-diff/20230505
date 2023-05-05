# Comparing `tmp/unique_char_counter_cli_kir_boh-1.5.4.tar.gz` & `tmp/unique_char_counter_cli_kir_boh-1.5.5.tar.gz`

## Comparing `unique_char_counter_cli_kir_boh-1.5.4.tar` & `unique_char_counter_cli_kir_boh-1.5.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/Task 5 Package.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/misc.xml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/modules.xml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/vcs.xml
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/tests/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/Task 5 Package.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/misc.xml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/modules.xml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/__init__.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/tests/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/LICENSE
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/PKG-INFO
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.4/.idea/workspace.xml` & `unique_char_counter_cli_kir_boh-1.5.5/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/v/cache/nodeids` & `unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.4/LICENSE` & `unique_char_counter_cli_kir_boh-1.5.5/LICENSE`

 * *Files identical despite different names*

