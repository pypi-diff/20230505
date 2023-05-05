# Comparing `tmp/firebirdsql-run-1.0.1.tar.gz` & `tmp/firebirdsql_run-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebirdsql-run-1.0.1.tar", max compression
+gzip compressed data, was "firebirdsql_run-1.0.2a1.tar", max compression
```

## Comparing `firebirdsql-run-1.0.1.tar` & `firebirdsql_run-1.0.2a1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1065 2022-08-03 13:01:52.959298 firebirdsql-run-1.0.1/LICENSE
--rw-r--r--   0        0        0     2067 2022-08-03 13:01:52.959298 firebirdsql-run-1.0.1/README.md
--rw-r--r--   0        0        0     2064 2022-08-03 13:01:52.959298 firebirdsql-run-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3056 2022-08-03 13:01:52.959298 firebirdsql-run-1.0.1/src/firebirdsql_run/__init__.py
--rw-r--r--   0        0        0     2904 2022-08-03 13:02:03.452026 firebirdsql-run-1.0.1/setup.py
--rw-r--r--   0        0        0     2785 2022-08-03 13:02:03.452377 firebirdsql-run-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-05 09:18:10.769010 firebirdsql_run-1.0.2a1/LICENSE
+-rw-r--r--   0        0        0     2067 2023-05-05 09:18:10.769010 firebirdsql_run-1.0.2a1/README.md
+-rw-r--r--   0        0        0     2243 2023-05-05 09:18:25.929360 firebirdsql_run-1.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0     3134 2023-05-05 09:18:10.769010 firebirdsql_run-1.0.2a1/src/firebirdsql_run/__init__.py
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.2a1/PKG-INFO
```

### Comparing `firebirdsql-run-1.0.1/LICENSE` & `firebirdsql_run-1.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `firebirdsql-run-1.0.1/README.md` & `firebirdsql_run-1.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `firebirdsql-run-1.0.1/pyproject.toml` & `firebirdsql_run-1.0.2a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,89 @@
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+
 [tool.poetry]
 name = "firebirdsql-run"
-version = "1.0.1"
+version = "1.0.2-alpha.1"
 description = "Firebirdsql wrapper inspired by subprocess.run"
-authors = ["DeadNews <uhjnnn@gmail.com>"]
+authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/firebirdsql-run"
 repository = "https://github.com/DeadNews/firebirdsql-run"
 keywords = ["firebird", "sql", "api"]
 classifiers = ["Operating System :: OS Independent", "Topic :: Database"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 firebirdsql = "^1.2.2"
 
-[tool.poetry.dev-dependencies]
-bandit = "^1.7.4"
-black = "^22.3.0"
-flake8 = "^5.0.3"
-flake8-bugbear = "^22.4.25"
-flake8-comprehensions = "^3.10.0"
-flake8-implicit-str-concat = "^0.3.0"
-flake8-pytest-style = "^1.6.0"
-flake8-simplify = "^0.19.3"
-flake8-unused-arguments = "^0.0.11"
-isort = "^5.10.1"
-mypy = "^0.971"
-pep8-naming = "^0.13.0"
-poethepoet = "^0.16.0"
-pre-commit = "^2.19.0"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-safety = "^2.0.0"
+[tool.poetry.group.ci.dependencies]
+black = "^23.3.0"
+mypy = "^1.2.0"
+poethepoet = "^0.20.0"
+ruff = "^0.0.264"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poe.tasks]
+ruff = "ruff check ."
+black = "black --check ."
+mypy = "mypy ."
+ci.sequence = ["ruff", "black", "mypy"]
 
-[tool.black]
-line-length = 88
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
 
-[tool.isort]
-line_length = 88
-profile = "black"
+[tool.black]
+line-length = 99
 
 [tool.mypy]
 disallow_untyped_defs = true
 follow_imports = "silent"
 ignore_missing_imports = true
 show_column_numbers = true
 show_error_codes = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 allow_untyped_defs = true
 
-[tool.bandit]
-exclude_dirs = ["tests"]
-skips = [
-  "B404", # Importing subprocess
-  "B603", # Calling subprocess.Popen without shell=True
-]
-
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src"
 testpaths = ["tests"]
-markers = ["docker", "slow"]
+markers = ["docker", "key_required"]
 
 [tool.coverage.report]
-exclude_lines = ["if __name__ == .__main__.:"]
+exclude_lines = ["if TYPE_CHECKING:", "if __name__ == .__main__.:"]
 
-[tool.poe.tasks]
-isort = "isort . --check-only --diff"
-black = "black . --check --diff"
-mypy = "mypy ."
-flake8 = "flake8 ."
-bandit = "bandit -c pyproject.toml -r ."
-safety = "safety check --bare"
-
-[tool.poe.tasks.ci]
-help = "CI sequence"
-sequence = ["isort", "black", "mypy", "flake8", "bandit", "safety"]
-
-[tool.poe.tasks.pc]
-help = "pre-commit"
-cmd = "pre-commit run --all-files"
+[tool.ruff]
+line-length = 99
+select = ["ALL"]
+ignore = [
+  "COM812", # Trailing comma missing
+  "D203",   # 1 blank line required before class docstring
+  "D212",   # Multi-line docstring summary should start at the first line
+  "E501",   # Line too long
+  "EXE001", # Shebang is present but file is not executable
+  "FBT001", # Boolean positional arg in function definition
+  "FBT002", # Boolean default value in function definition
+]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+"tests/*" = ["ANN", "D", "PLC1901", "PLR2004", "S"]
+
+[tool.ruff.flake8-comprehensions]
+allow-dict-calls-with-keyword-arguments = false
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.pylint]
+max-args = 8
```

### Comparing `firebirdsql-run-1.0.1/src/firebirdsql_run/__init__.py` & `firebirdsql_run-1.0.2a1/src/firebirdsql_run/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 #!/usr/bin/env python3
-"""
-Firebirdsql wrapper inspired by subprocess.run
-"""
-from __future__ import annotations
-
+"""Firebirdsql wrapper inspired by subprocess.run."""
 from datetime import datetime
 from pathlib import Path
 from socket import getfqdn
 from typing import NamedTuple, Union
 
 from firebirdsql import Connection, connect
 
 FBTypes = Union[str, float, datetime, None]
 Dataset = list[dict[str, FBTypes]]
 
 
 class CompletedTransaction(NamedTuple):
-    """
-    The return value from execute(), representing a transaction that has finished.
-    """
+    """The return value from execute(), representing a transaction that has finished."""
 
     host: str
     db: str
     user: str
     returncode: int
     error: str
     query: str
     params: tuple
     data: Dataset
 
 
+class ExecuteError(Exception):
+    """Exception raised for execute transaction errors."""
+
+
 def connection(
     db: Path | str,
     host: str = "localhost",
     port: int = 3050,
     user: str = "TWUSER",
     passwd: str | None = None,
 ) -> Connection:
-    """
-    Creating a connection to the database.
-    """
+    """Create a connection to the database."""
     return connect(
         host=getfqdn(host),
         database=f"{db}",
         port=port,
         user=user,
         password=passwd,
     )
@@ -56,14 +52,16 @@
     host: str = "localhost",
     port: int = 3050,
     user: str = "TWUSER",
     passwd: str | None = None,
     use_conn: Connection | None = None,
 ) -> CompletedTransaction:
     """
+    Execute transaction.
+
     Run the transaction described by args.
     Wait for transaction to complete, then return a CompletedTransaction named tuple.
 
     An existing connection can be used with `use_conn`, it will not be closed after execution.
     """
     conn_success = False
     try:
@@ -80,20 +78,20 @@
 
         lines = cur.fetchall()
         columns = [f"{col[0]}".lower() for col in cur.description]
         conn.commit()
 
         if use_conn is None:
             conn.close()
-    except Exception as e:
+    except Exception as e:  # noqa: BLE001
         data = []
         returncode = 1
         error = f"{e}"
     else:
-        data = [dict(zip(columns, line)) for line in lines]
+        data = [dict(zip(columns, line, strict=True)) for line in lines]
         returncode = 0
         error = ""
 
     return CompletedTransaction(
         host=conn.hostname if conn_success else host,
         db=conn.filename if conn_success else db,
         user=conn.user if conn_success else user,
@@ -111,17 +109,15 @@
     db: Path | str = "",
     host: str = "localhost",
     port: int = 3050,
     user: str = "TWUSER",
     passwd: str | None = None,
     use_conn: Connection | None = None,
 ) -> CompletedTransaction:
-    """
-    Execute procedure with params.
-    """
+    """Execute procedure with params."""
     query = f"EXECUTE PROCEDURE {procname} " + ",".join("?" * len(params))
 
     return execute(
         query=query,
         params=params,
         host=host,
         port=port,
```

### Comparing `firebirdsql-run-1.0.1/PKG-INFO` & `firebirdsql_run-1.0.2a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: firebirdsql-run
-Version: 1.0.1
+Version: 1.0.2a1
 Summary: Firebirdsql wrapper inspired by subprocess.run
 Home-page: https://github.com/DeadNews/firebirdsql-run
 License: MIT
 Keywords: firebird,sql,api
 Author: DeadNews
-Author-email: uhjnnn@gmail.com
-Requires-Python: >=3.9,<4.0
+Author-email: aurczpbgr@mozmail.com
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Requires-Dist: firebirdsql (>=1.2.2,<2.0.0)
 Project-URL: Repository, https://github.com/DeadNews/firebirdsql-run
 Description-Content-Type: text/markdown
 
 # firebirdsql-run
```

