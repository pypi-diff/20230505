# Comparing `tmp/pytest-sqlalchemy-session-0.2.0b1.tar.gz` & `tmp/pytest-sqlalchemy-session-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sqlalchemy-session-0.2.0b1.tar", last modified: Sat Apr 29 11:03:46 2023, max compression
+gzip compressed data, was "pytest-sqlalchemy-session-0.3.0b1.tar", last modified: Fri May  5 13:18:11 2023, max compression
```

## Comparing `pytest-sqlalchemy-session-0.2.0b1.tar` & `pytest-sqlalchemy-session-0.3.0b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-29 11:03:46.625712 pytest-sqlalchemy-session-0.2.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/tests/test_strict_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 13:18:11.000000 pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:18:11.992961 pytest-sqlalchemy-session-0.3.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-05 13:18:02.000000 pytest-sqlalchemy-session-0.3.0b1/tests/test_strict_mode.py
```

### Comparing `pytest-sqlalchemy-session-0.2.0b1/LICENSE` & `pytest-sqlalchemy-session-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.2.0b1/PKG-INFO` & `pytest-sqlalchemy-session-0.3.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sqlalchemy-session
-Version: 0.2.0b1
+Version: 0.3.0b1
 Summary: A pytest plugin for preserving test isolation that use SQLAlchemy.
 Author-email: Stanislav Shkitin <stanislav.shkitin@yandex.ru>
 License: MIT
 Keywords: pytest,sqlalchemy,transaction
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-sqlalchemy-session-0.2.0b1/pyproject.toml` & `pytest-sqlalchemy-session-0.3.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pytest-sqlalchemy-session'
-version = "0.2.0-beta1"
+version = "0.3.0-beta1"
 authors = [
     {name = "Stanislav Shkitin", email = "stanislav.shkitin@yandex.ru"},
 ]
 license = {text = "MIT"}
 description = "A pytest plugin for preserving test isolation that use SQLAlchemy."
 keywords = ["pytest", "sqlalchemy", "transaction"]
 readme = "README.md"
```

### Comparing `pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/PKG-INFO` & `pytest-sqlalchemy-session-0.3.0b1/pytest_sqlalchemy_session.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sqlalchemy-session
-Version: 0.2.0b1
+Version: 0.3.0b1
 Summary: A pytest plugin for preserving test isolation that use SQLAlchemy.
 Author-email: Stanislav Shkitin <stanislav.shkitin@yandex.ru>
 License: MIT
 Keywords: pytest,sqlalchemy,transaction
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-sqlalchemy-session-0.2.0b1/setup.cfg` & `pytest-sqlalchemy-session-0.3.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.2.0b1/tests/test_configs.py` & `pytest-sqlalchemy-session-0.3.0b1/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.2.0b1/tests/test_strict_mode.py` & `pytest-sqlalchemy-session-0.3.0b1/tests/test_strict_mode.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     result.assert_outcomes(failed=1)
     result.stdout.fnmatch_lines(
         ["*FAILED test__strict_mode__usage_only_fixture.py::test_transaction_commit*"]
     )
     result.stdout.fnmatch_lines(
         [
             "*_pytest.config.exceptions.UsageError: "
-            "You need to use pytest.mark.sqlalchemy_db when you execute db queries.*"
+            "The pytest.mark.sqlalchemy_db or pytest.mark.transactional_db marker is required to execute db queries.*"
         ]
     )
 
 
 def test__strict_mode__without_marker(db_testdir_with_strict_mode: Pytester) -> None:
     db_testdir_with_strict_mode.makepyfile(
         """
@@ -56,15 +56,15 @@
     result.assert_outcomes(failed=1)
     result.stdout.fnmatch_lines(
         ["*FAILED test__strict_mode__without_marker.py::test_transaction_commit*"]
     )
     result.stdout.fnmatch_lines(
         [
             "*_pytest.config.exceptions.UsageError: "
-            "You need to use pytest.mark.sqlalchemy_db when you execute db queries.*"
+            "The pytest.mark.sqlalchemy_db or pytest.mark.transactional_db marker is required to execute db queries.*"
         ]
     )
 
 
 def test__strict_mode__marker_dont_affect_another_test(
     db_testdir_with_strict_mode: Pytester,
 ) -> None:
@@ -98,15 +98,15 @@
         [
             "*FAILED test__strict_mode__marker_dont_affect_another_test.py::test_transaction_commit__without_marker*"
         ]
     )
     result.stdout.fnmatch_lines(
         [
             "*_pytest.config.exceptions.UsageError: "
-            "You need to use pytest.mark.sqlalchemy_db when you execute db queries.*"
+            "The pytest.mark.sqlalchemy_db or pytest.mark.transactional_db marker is required to execute db queries.*"
         ]
     )
 
 
 def test__strict_mode__usage_fixture_and_marker(
     db_testdir_with_strict_mode: Pytester,
 ) -> None:
@@ -159,7 +159,37 @@
         """
     )
 
     result = db_testdir_with_strict_mode.runpytest()
 
     logger.info(result.stdout.str())
     result.assert_outcomes(passed=2)
+
+
+def test__strict_mode__usage_transactional_marker(
+    db_testdir_with_strict_mode: Pytester,
+) -> None:
+    db_testdir_with_strict_mode.makepyfile(
+        """
+        import pytest
+        from pytest_sqlalchemy_session_test.app.tables import sample_table
+
+        @pytest.mark.transactional_db
+        def test_transaction_commit(custom_session):
+            custom_session.execute(sample_table.insert(), {"id": 1})
+            custom_session.commit()
+            instance = custom_session.execute(sample_table.select().where(sample_table.c.id == 1)).fetchone()
+
+            assert instance == (1,)
+
+        @pytest.mark.transactional_db
+        def test_transaction_commit_changes_dont_persist(custom_session):
+            instance = custom_session.execute(sample_table.select().where(sample_table.c.id == 1)).fetchone()
+
+            assert instance == (1,)
+        """
+    )
+
+    result = db_testdir_with_strict_mode.runpytest()
+
+    logger.info(result.stdout.str())
+    result.assert_outcomes(passed=2)
```

