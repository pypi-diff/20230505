# Comparing `tmp/pg_force_execute-0.0.5.tar.gz` & `tmp/pg_force_execute-0.0.6.tar.gz`

## Comparing `pg_force_execute-0.0.5.tar` & `pg_force_execute-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pg_force_execute-0.0.5/pg_force_execute.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.5/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.5/LICENSE
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pg_force_execute-0.0.5/README.md
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pg_force_execute-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 pg_force_execute-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/pg_force_execute.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 pg_force_execute-0.0.6/PKG-INFO
```

### Comparing `pg_force_execute-0.0.5/pg_force_execute.py` & `pg_force_execute-0.0.6/pg_force_execute.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
+import contextlib
 import datetime
 import logging
 from threading import Event, Thread
 
 import sqlalchemy as sa
 
 
-def pg_force_execute(statement, conn, engine,
-                     parameters=None, execution_options=None,
+@contextlib.contextmanager
+def pg_force_execute(conn, engine,
                      delay=datetime.timedelta(minutes=5),
                      check_interval=datetime.timedelta(seconds=1),
                      termination_thread_timeout=datetime.timedelta(seconds=10),
                      logger=logging.getLogger("pg_force_execute"),
 ):
     cancel_exception = None
 
     def force_unblock(pid, exit):
         nonlocal cancel_exception
 
         try:
             exit.wait(timeout=(delay - check_interval).total_seconds())
 
-            # Repeatedly check for other backends that block `statement`, and cancel them if
-            # they are. The repeat check is to avoid race conditions - if another backend
-            # blocks this backend just after pg_blocking_pids returns its PIDs. If it's
-            # determined that PostgreSQL forbids this case the looping can be removed
+            # Repeatedly check for other backends that block conn, and terminates them if they are
+            # The loop addreses the case that as the client context progresses, it might run queries
+            # that get blocked by clients not caught in the initial pg_blocking_pids call
             while not exit.wait(timeout=check_interval.total_seconds()):
-                logger.info('Cancelling queries blocking PID %s running %s', pid, statement)
+                logger.info('Cancelling queries blocking PID %s', pid)
                 with engine.begin() as conn:
                     # pg_cancel_backend isn't strong enough - the blocking PIDs might not be
                     # actually running a query, so there is nothing to cancel. They might
                     # just be holding locks. To force release of the locks, we have to call
                     # pg_terminate_backend
                     cancelled_queries = conn.execute(
                         sa.text("""
@@ -55,13 +55,13 @@
         sa.text('SELECT pg_backend_pid()')
     ).fetchall()[0][0]
     exit = Event()
     t = Thread(target=force_unblock, args=(pid, exit))
     t.start()
 
     try:
-        return conn.execute(statement, parameters=parameters, execution_options=execution_options)
+        yield
     finally:
         exit.set()
         t.join(timeout=termination_thread_timeout.total_seconds())
         if cancel_exception is not None:
             raise cancel_exception
```

### Comparing `pg_force_execute-0.0.5/.gitignore` & `pg_force_execute-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.5/LICENSE` & `pg_force_execute-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.5/pyproject.toml` & `pg_force_execute-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-force-execute"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
-description = "Utility function to run a PostgreSQL query with SQLAlchemy, terminating any other clients that block it"
+description = "Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that block them"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

