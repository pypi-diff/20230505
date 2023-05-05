# Comparing `tmp/rq-1.8.1.tar.gz` & `tmp/rq-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rq-1.8.1.tar", last modified: Mon May 17 07:06:52 2021, max compression
+gzip compressed data, was "dist/rq-1.9.0.tar", last modified: Wed Jun 30 07:21:37 2021, max compression
```

## Comparing `rq-1.8.1.tar` & `rq-1.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-05-17 07:06:52.000000 rq-1.8.1/
--rw-r--r--   0 selwin     (501) staff       (20)     1532 2021-05-17 07:06:52.000000 rq-1.8.1/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)     1502 2018-03-03 00:21:08.000000 rq-1.8.1/LICENSE
--rw-r--r--   0 selwin     (501) staff       (20)       26 2020-09-05 09:18:48.000000 rq-1.8.1/requirements.txt
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-05-17 07:06:52.000000 rq-1.8.1/rq.egg-info/
--rw-r--r--   0 selwin     (501) staff       (20)     1532 2021-05-17 07:06:52.000000 rq-1.8.1/rq.egg-info/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)        1 2017-11-01 09:12:31.000000 rq-1.8.1/rq.egg-info/not-zip-safe
--rw-r--r--   0 selwin     (501) staff       (20)      774 2021-05-17 07:06:52.000000 rq-1.8.1/rq.egg-info/SOURCES.txt
--rw-r--r--   0 selwin     (501) staff       (20)       82 2021-05-17 07:06:52.000000 rq-1.8.1/rq.egg-info/entry_points.txt
--rw-r--r--   0 selwin     (501) staff       (20)       26 2021-05-17 07:06:52.000000 rq-1.8.1/rq.egg-info/requires.txt
--rw-r--r--   0 selwin     (501) staff       (20)        3 2021-05-17 07:06:52.000000 rq-1.8.1/rq.egg-info/top_level.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2021-05-17 07:06:52.000000 rq-1.8.1/rq.egg-info/dependency_links.txt
--rw-r--r--   0 selwin     (501) staff       (20)       82 2020-10-04 04:23:00.000000 rq-1.8.1/MANIFEST.in
--rw-r--r--   0 selwin     (501) staff       (20)      171 2020-09-05 09:18:48.000000 rq-1.8.1/.deepsource.toml
--rw-r--r--   0 selwin     (501) staff       (20)     3753 2021-04-20 01:04:12.000000 rq-1.8.1/README.md
--rw-r--r--   0 selwin     (501) staff       (20)     3020 2021-05-17 06:59:23.000000 rq-1.8.1/setup.py
--rw-r--r--   0 selwin     (501) staff       (20)      160 2021-05-17 07:06:52.000000 rq-1.8.1/setup.cfg
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-05-17 07:06:52.000000 rq-1.8.1/rq/
--rw-r--r--   0 selwin     (501) staff       (20)    25120 2021-05-15 11:27:29.000000 rq-1.8.1/rq/queue.py
--rw-r--r--   0 selwin     (501) staff       (20)    47092 2021-05-17 06:51:49.000000 rq-1.8.1/rq/worker.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-05-17 07:06:52.000000 rq-1.8.1/rq/compat/
--rw-r--r--   0 selwin     (501) staff       (20)      501 2020-03-08 09:20:54.000000 rq-1.8.1/rq/compat/connections.py
--rw-r--r--   0 selwin     (501) staff       (20)     2305 2020-11-14 00:57:51.000000 rq-1.8.1/rq/compat/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)    22853 2021-05-15 11:27:29.000000 rq-1.8.1/rq/compat/dictconfig.py
--rw-r--r--   0 selwin     (501) staff       (20)     2530 2021-04-20 01:04:12.000000 rq-1.8.1/rq/command.py
--rw-r--r--   0 selwin     (501) staff       (20)      152 2021-05-15 11:27:29.000000 rq-1.8.1/rq/version.py
--rw-r--r--   0 selwin     (501) staff       (20)    12463 2021-05-17 06:51:49.000000 rq-1.8.1/rq/registry.py
--rw-r--r--   0 selwin     (501) staff       (20)    12854 2021-05-15 11:27:29.000000 rq-1.8.1/rq/local.py
--rw-r--r--   0 selwin     (501) staff       (20)    33449 2021-05-17 06:51:49.000000 rq-1.8.1/rq/job.py
--rw-r--r--   0 selwin     (501) staff       (20)     1298 2020-11-28 05:08:20.000000 rq-1.8.1/rq/serializers.py
--rw-r--r--   0 selwin     (501) staff       (20)     2048 2020-03-08 09:20:54.000000 rq-1.8.1/rq/connections.py
--rw-r--r--   0 selwin     (501) staff       (20)      469 2021-01-19 01:19:58.000000 rq-1.8.1/rq/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      750 2020-03-08 09:20:54.000000 rq-1.8.1/rq/suspension.py
--rw-r--r--   0 selwin     (501) staff       (20)     2425 2021-05-15 11:27:29.000000 rq-1.8.1/rq/timeouts.py
--rw-r--r--   0 selwin     (501) staff       (20)     1763 2020-09-05 09:18:48.000000 rq-1.8.1/rq/logutils.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-05-17 07:06:52.000000 rq-1.8.1/rq/cli/
--rw-r--r--   0 selwin     (501) staff       (20)      210 2020-03-08 09:20:54.000000 rq-1.8.1/rq/cli/__init__.py
--rwxr-xr-x   0 selwin     (501) staff       (20)    12472 2021-05-15 11:27:29.000000 rq-1.8.1/rq/cli/cli.py
--rw-r--r--   0 selwin     (501) staff       (20)     8032 2021-05-15 11:27:29.000000 rq-1.8.1/rq/cli/helpers.py
--rw-r--r--   0 selwin     (501) staff       (20)       80 2020-09-05 09:18:48.000000 rq-1.8.1/rq/cli/__main__.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-05-17 07:06:52.000000 rq-1.8.1/rq/contrib/
--rw-r--r--   0 selwin     (501) staff       (20)     1063 2020-03-08 09:20:54.000000 rq-1.8.1/rq/contrib/legacy.py
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:20:54.000000 rq-1.8.1/rq/contrib/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      466 2020-09-05 09:18:48.000000 rq-1.8.1/rq/contrib/sentry.py
--rw-r--r--   0 selwin     (501) staff       (20)     8705 2021-05-15 11:27:43.000000 rq-1.8.1/rq/utils.py
--rw-r--r--   0 selwin     (501) staff       (20)      607 2020-09-05 09:18:48.000000 rq-1.8.1/rq/exceptions.py
--rw-r--r--   0 selwin     (501) staff       (20)      435 2021-05-15 11:27:29.000000 rq-1.8.1/rq/defaults.py
--rw-r--r--   0 selwin     (501) staff       (20)     9389 2021-05-15 11:27:29.000000 rq-1.8.1/rq/scheduler.py
--rw-r--r--   0 selwin     (501) staff       (20)      670 2020-03-08 09:20:54.000000 rq-1.8.1/rq/dummy.py
--rw-r--r--   0 selwin     (501) staff       (20)     2130 2021-04-20 01:04:12.000000 rq-1.8.1/rq/worker_registration.py
--rw-r--r--   0 selwin     (501) staff       (20)     2603 2021-05-15 11:27:29.000000 rq-1.8.1/rq/decorators.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-06-30 07:21:37.000000 rq-1.9.0/
+-rw-r--r--   0 selwin     (501) staff       (20)     1532 2021-06-30 07:21:37.000000 rq-1.9.0/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)     1502 2018-03-03 00:21:08.000000 rq-1.9.0/LICENSE
+-rw-r--r--   0 selwin     (501) staff       (20)       26 2020-09-05 09:18:48.000000 rq-1.9.0/requirements.txt
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-06-30 07:21:37.000000 rq-1.9.0/rq.egg-info/
+-rw-r--r--   0 selwin     (501) staff       (20)     1532 2021-06-30 07:21:37.000000 rq-1.9.0/rq.egg-info/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2017-11-01 09:12:31.000000 rq-1.9.0/rq.egg-info/not-zip-safe
+-rw-r--r--   0 selwin     (501) staff       (20)      774 2021-06-30 07:21:37.000000 rq-1.9.0/rq.egg-info/SOURCES.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       82 2021-06-30 07:21:37.000000 rq-1.9.0/rq.egg-info/entry_points.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       26 2021-06-30 07:21:37.000000 rq-1.9.0/rq.egg-info/requires.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        3 2021-06-30 07:21:37.000000 rq-1.9.0/rq.egg-info/top_level.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2021-06-30 07:21:37.000000 rq-1.9.0/rq.egg-info/dependency_links.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       82 2020-10-04 04:23:00.000000 rq-1.9.0/MANIFEST.in
+-rw-r--r--   0 selwin     (501) staff       (20)      171 2020-09-05 09:18:48.000000 rq-1.9.0/.deepsource.toml
+-rw-r--r--   0 selwin     (501) staff       (20)     3753 2021-04-20 01:04:12.000000 rq-1.9.0/README.md
+-rw-r--r--   0 selwin     (501) staff       (20)     3020 2021-05-28 09:18:22.000000 rq-1.9.0/setup.py
+-rw-r--r--   0 selwin     (501) staff       (20)      160 2021-06-30 07:21:37.000000 rq-1.9.0/setup.cfg
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-06-30 07:21:37.000000 rq-1.9.0/rq/
+-rw-r--r--   0 selwin     (501) staff       (20)    28815 2021-06-30 07:00:07.000000 rq-1.9.0/rq/queue.py
+-rw-r--r--   0 selwin     (501) staff       (20)    49078 2021-06-30 07:00:07.000000 rq-1.9.0/rq/worker.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-06-30 07:21:37.000000 rq-1.9.0/rq/compat/
+-rw-r--r--   0 selwin     (501) staff       (20)      501 2020-03-08 09:20:54.000000 rq-1.9.0/rq/compat/connections.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2305 2020-11-14 00:57:51.000000 rq-1.9.0/rq/compat/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)    22853 2021-05-15 11:27:29.000000 rq-1.9.0/rq/compat/dictconfig.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2530 2021-04-20 01:04:12.000000 rq-1.9.0/rq/command.py
+-rw-r--r--   0 selwin     (501) staff       (20)      152 2021-06-20 10:19:06.000000 rq-1.9.0/rq/version.py
+-rw-r--r--   0 selwin     (501) staff       (20)    12463 2021-05-28 09:20:06.000000 rq-1.9.0/rq/registry.py
+-rw-r--r--   0 selwin     (501) staff       (20)    12854 2021-05-15 11:27:29.000000 rq-1.9.0/rq/local.py
+-rw-r--r--   0 selwin     (501) staff       (20)    35029 2021-06-30 07:00:07.000000 rq-1.9.0/rq/job.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1298 2020-11-28 05:08:20.000000 rq-1.9.0/rq/serializers.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2048 2020-03-08 09:20:54.000000 rq-1.9.0/rq/connections.py
+-rw-r--r--   0 selwin     (501) staff       (20)      469 2021-01-19 01:19:58.000000 rq-1.9.0/rq/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      750 2020-03-08 09:20:54.000000 rq-1.9.0/rq/suspension.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2425 2021-05-15 11:27:29.000000 rq-1.9.0/rq/timeouts.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1763 2020-09-05 09:18:48.000000 rq-1.9.0/rq/logutils.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-06-30 07:21:37.000000 rq-1.9.0/rq/cli/
+-rw-r--r--   0 selwin     (501) staff       (20)      210 2020-03-08 09:20:54.000000 rq-1.9.0/rq/cli/__init__.py
+-rwxr-xr-x   0 selwin     (501) staff       (20)    12472 2021-05-15 11:27:29.000000 rq-1.9.0/rq/cli/cli.py
+-rw-r--r--   0 selwin     (501) staff       (20)     8546 2021-06-12 04:54:45.000000 rq-1.9.0/rq/cli/helpers.py
+-rw-r--r--   0 selwin     (501) staff       (20)       80 2020-09-05 09:18:48.000000 rq-1.9.0/rq/cli/__main__.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2021-06-30 07:21:37.000000 rq-1.9.0/rq/contrib/
+-rw-r--r--   0 selwin     (501) staff       (20)     1063 2020-03-08 09:20:54.000000 rq-1.9.0/rq/contrib/legacy.py
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:20:54.000000 rq-1.9.0/rq/contrib/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      466 2020-09-05 09:18:48.000000 rq-1.9.0/rq/contrib/sentry.py
+-rw-r--r--   0 selwin     (501) staff       (20)     9946 2021-06-30 07:00:07.000000 rq-1.9.0/rq/utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)      657 2021-06-12 04:54:45.000000 rq-1.9.0/rq/exceptions.py
+-rw-r--r--   0 selwin     (501) staff       (20)      457 2021-06-30 07:00:07.000000 rq-1.9.0/rq/defaults.py
+-rw-r--r--   0 selwin     (501) staff       (20)     9389 2021-05-15 11:27:29.000000 rq-1.9.0/rq/scheduler.py
+-rw-r--r--   0 selwin     (501) staff       (20)      670 2020-03-08 09:20:54.000000 rq-1.9.0/rq/dummy.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2130 2021-04-20 01:04:12.000000 rq-1.9.0/rq/worker_registration.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2603 2021-05-15 11:27:29.000000 rq-1.9.0/rq/decorators.py
```

### Comparing `rq-1.8.1/PKG-INFO` & `rq-1.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rq
-Version: 1.8.1
+Version: 1.9.0
 Summary: RQ is a simple, lightweight, library for creating background jobs, and processing them.
 Home-page: https://github.com/nvie/rq/
 Author: Vincent Driessen
 Author-email: vincent@3rdcloud.com
 License: BSD
 Description: 
         rq is a simple, lightweight, library for creating background jobs, and
```

### Comparing `rq-1.8.1/LICENSE` & `rq-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq.egg-info/PKG-INFO` & `rq-1.9.0/rq.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rq
-Version: 1.8.1
+Version: 1.9.0
 Summary: RQ is a simple, lightweight, library for creating background jobs, and processing them.
 Home-page: https://github.com/nvie/rq/
 Author: Vincent Driessen
 Author-email: vincent@3rdcloud.com
 License: BSD
 Description: 
         rq is a simple, lightweight, library for creating background jobs, and
```

### Comparing `rq-1.8.1/rq.egg-info/SOURCES.txt` & `rq-1.9.0/rq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/README.md` & `rq-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/setup.py` & `rq-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/queue.py` & `rq-1.9.0/rq/queue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 
 import uuid
 import warnings
 
+from collections import namedtuple
 from datetime import datetime, timezone
 
 from distutils.version import StrictVersion
 from redis import WatchError
 
 from .compat import as_text, string_types, total_ordering
 from .connections import resolve_connection
@@ -19,14 +20,25 @@
 from .utils import backend_class, get_version, import_attribute, parse_timeout, utcnow
 
 
 def compact(lst):
     return [item for item in lst if item is not None]
 
 
+class EnqueueData(namedtuple('EnqueueData', ["func", "args", "kwargs", "timeout",
+                                             "result_ttl", "ttl", "failure_ttl",
+                                             "description", "job_id",
+                                             "at_front", "meta", "retry"])):
+    """Helper type to use when calling enqueue_many
+    NOTE: Does not support `depends_on` yet.
+    """
+
+    __slots__ = ()
+
+
 @total_ordering
 class Queue:
     job_class = Job
     DEFAULT_TIMEOUT = 180  # Default timeout seconds.
     redis_queue_namespace_prefix = 'rq:queue:'
     redis_queues_keys = 'rq:queues'
 
@@ -276,15 +288,16 @@
             connection.lpush(self.key, job_id)
         else:
             connection.rpush(self.key, job_id)
 
     def create_job(self, func, args=None, kwargs=None, timeout=None,
                    result_ttl=None, ttl=None, failure_ttl=None,
                    description=None, depends_on=None, job_id=None,
-                   meta=None, status=JobStatus.QUEUED, retry=None):
+                   meta=None, status=JobStatus.QUEUED, retry=None, *,
+                   on_success=None, on_failure=None):
         """Creates a job based on parameters given."""
         timeout = parse_timeout(timeout)
 
         if timeout is None:
             timeout = self._default_timeout
         elif timeout == 0:
             raise ValueError('0 timeout is not allowed. Use -1 for infinite timeout')
@@ -297,78 +310,143 @@
             raise ValueError('Job ttl must be greater than 0')
 
         job = self.job_class.create(
             func, args=args, kwargs=kwargs, connection=self.connection,
             result_ttl=result_ttl, ttl=ttl, failure_ttl=failure_ttl,
             status=status, description=description,
             depends_on=depends_on, timeout=timeout, id=job_id,
-            origin=self.name, meta=meta, serializer=self.serializer
+            origin=self.name, meta=meta, serializer=self.serializer, on_success=on_success,
+            on_failure=on_failure
         )
 
         if retry:
             job.retries_left = retry.max
             job.retry_intervals = retry.intervals
 
         return job
 
+    def setup_dependencies(
+        self,
+        job,
+        pipeline=None
+    ):
+        # If a _dependent_ job depends on any unfinished job, register all the
+        # _dependent_ job's dependencies instead of enqueueing it.
+        #
+        # `Job#fetch_dependencies` sets WATCH on all dependencies. If
+        # WatchError is raised in the when the pipeline is executed, that means
+        # something else has modified either the set of dependencies or the
+        # status of one of them. In this case, we simply retry.
+        if len(job._dependency_ids) > 0:
+            pipe = pipeline if pipeline is not None else self.connection.pipeline()
+            while True:
+                try:
+                    # Also calling watch even if caller
+                    # passed in a pipeline since Queue#create_job
+                    # is called from within this method.
+                    pipe.watch(job.dependencies_key)
+
+                    dependencies = job.fetch_dependencies(
+                        watch=True,
+                        pipeline=pipe
+                    )
+
+                    pipe.multi()
+
+                    for dependency in dependencies:
+                        if dependency.get_status(refresh=False) != JobStatus.FINISHED:
+                            job.set_status(JobStatus.DEFERRED, pipeline=pipe)
+                            job.register_dependency(pipeline=pipe)
+                            job.save(pipeline=pipe)
+                            job.cleanup(ttl=job.ttl, pipeline=pipe)
+                            if pipeline is None:
+                                pipe.execute()
+                            return job
+                    break
+                except WatchError:
+                    if pipeline is None:
+                        continue
+                    else:
+                        # if pipeline comes from caller, re-raise to them
+                        raise
+        elif pipeline is not None:
+            pipeline.multi()  # Ensure pipeline in multi mode before returning to caller
+        return job
+
     def enqueue_call(self, func, args=None, kwargs=None, timeout=None,
-                     result_ttl=None, ttl=None, failure_ttl=None,
-                     description=None, depends_on=None, job_id=None,
-                     at_front=False, meta=None, retry=None):
+                     result_ttl=None, ttl=None, failure_ttl=None, description=None,
+                     depends_on=None, job_id=None, at_front=False, meta=None,
+                     retry=None, on_success=None, on_failure=None, pipeline=None):
         """Creates a job to represent the delayed function call and enqueues
         it.
 nd
         It is much like `.enqueue()`, except that it takes the function's args
         and kwargs as explicit arguments.  Any kwargs passed to this function
         contain options for RQ itself.
         """
 
         job = self.create_job(
             func, args=args, kwargs=kwargs, result_ttl=result_ttl, ttl=ttl,
             failure_ttl=failure_ttl, description=description, depends_on=depends_on,
             job_id=job_id, meta=meta, status=JobStatus.QUEUED, timeout=timeout,
-            retry=retry
+            retry=retry, on_success=on_success, on_failure=on_failure
         )
 
-        # If a _dependent_ job depends on any unfinished job, register all the
-        # _dependent_ job's dependencies instead of enqueueing it.
-        #
-        # `Job#fetch_dependencies` sets WATCH on all dependencies. If
-        # WatchError is raised in the when the pipeline is executed, that means
-        # something else has modified either the set of dependencies or the
-        # status of one of them. In this case, we simply retry.
-        if depends_on is not None:
-            with self.connection.pipeline() as pipe:
-                while True:
-                    try:
-
-                        pipe.watch(job.dependencies_key)
-
-                        dependencies = job.fetch_dependencies(
-                            watch=True,
-                            pipeline=pipe
-                        )
-
-                        pipe.multi()
-
-                        for dependency in dependencies:
-                            if dependency.get_status(refresh=False) != JobStatus.FINISHED:
-                                job.set_status(JobStatus.DEFERRED, pipeline=pipe)
-                                job.register_dependency(pipeline=pipe)
-                                job.save(pipeline=pipe)
-                                job.cleanup(ttl=job.ttl, pipeline=pipe)
-                                pipe.execute()
-                                return job
+        job = self.setup_dependencies(
+            job,
+            pipeline=pipeline
+        )
+        # If we do not depend on an unfinished job, enqueue the job.
+        if job.get_status(refresh=False) != JobStatus.DEFERRED:
+            return self.enqueue_job(job, pipeline=pipeline, at_front=at_front)
+        return job
 
-                        break
-                    except WatchError:
-                        continue
+    @staticmethod
+    def prepare_data(func, args=None, kwargs=None, timeout=None,
+                     result_ttl=None, ttl=None, failure_ttl=None,
+                     description=None, job_id=None,
+                     at_front=False, meta=None, retry=None):
+        # Need this till support dropped for python_version < 3.7, where defaults can be specified for named tuples
+        # And can keep this logic within EnqueueData
+        return EnqueueData(
+            func, args, kwargs, timeout,
+            result_ttl, ttl, failure_ttl,
+            description, job_id,
+            at_front, meta, retry
+        )
 
-        job = self.enqueue_job(job, at_front=at_front)
-        return job
+    def enqueue_many(
+        self,
+        job_datas,
+        pipeline=None
+    ):
+        """
+        Creates multiple jobs (created via `Queue.prepare_data` calls)
+        to represent the delayed function calls and enqueues them.
+        """
+        pipe = pipeline if pipeline is not None else self.connection.pipeline()
+        jobs = [
+            self.enqueue_job(
+                self.create_job(
+                    job_data.func, args=job_data.args, kwargs=job_data.kwargs, result_ttl=job_data.result_ttl,
+                    ttl=job_data.ttl,
+                    failure_ttl=job_data.failure_ttl, description=job_data.description,
+                    depends_on=None,
+                    job_id=job_data.job_id, meta=job_data.meta, status=JobStatus.QUEUED,
+                    timeout=job_data.timeout,
+                    retry=job_data.retry
+                ),
+                pipeline=pipe,
+                at_front=job_data.at_front
+            )
+            for job_data in job_datas
+        ]
+        if pipeline is None:
+            pipe.execute()
+        return jobs
 
     def run_job(self, job):
         job.perform()
         job.set_status(JobStatus.FINISHED)
         job.save(include_meta=False)
         job.cleanup(DEFAULT_RESULT_TTL)
         return job
@@ -397,47 +475,55 @@
         ttl = kwargs.pop('ttl', None)
         failure_ttl = kwargs.pop('failure_ttl', None)
         depends_on = kwargs.pop('depends_on', None)
         job_id = kwargs.pop('job_id', None)
         at_front = kwargs.pop('at_front', False)
         meta = kwargs.pop('meta', None)
         retry = kwargs.pop('retry', None)
+        on_success = kwargs.pop('on_success', None)
+        on_failure = kwargs.pop('on_failure', None)
+        pipeline = kwargs.pop('pipeline', None)
 
         if 'args' in kwargs or 'kwargs' in kwargs:
             assert args == (), 'Extra positional arguments cannot be used when using explicit args and kwargs'  # noqa
             args = kwargs.pop('args', None)
             kwargs = kwargs.pop('kwargs', None)
 
         return (f, timeout, description, result_ttl, ttl, failure_ttl,
-                depends_on, job_id, at_front, meta, retry, args, kwargs)
+                depends_on, job_id, at_front, meta, retry, on_success, on_failure,
+                pipeline, args, kwargs)
 
     def enqueue(self, f, *args, **kwargs):
         """Creates a job to represent the delayed function call and enqueues it."""
 
         (f, timeout, description, result_ttl, ttl, failure_ttl,
-         depends_on, job_id, at_front, meta, retry, args, kwargs) = Queue.parse_args(f, *args, **kwargs)
+         depends_on, job_id, at_front, meta, retry, on_success,
+         on_failure, pipeline, args, kwargs) = Queue.parse_args(f, *args, **kwargs)
 
         return self.enqueue_call(
             func=f, args=args, kwargs=kwargs, timeout=timeout,
             result_ttl=result_ttl, ttl=ttl, failure_ttl=failure_ttl,
             description=description, depends_on=depends_on, job_id=job_id,
-            at_front=at_front, meta=meta, retry=retry
+            at_front=at_front, meta=meta, retry=retry, on_success=on_success, on_failure=on_failure,
+            pipeline=pipeline
         )
 
     def enqueue_at(self, datetime, f, *args, **kwargs):
         """Schedules a job to be enqueued at specified time"""
 
         (f, timeout, description, result_ttl, ttl, failure_ttl,
-         depends_on, job_id, at_front, meta, retry, args, kwargs) = Queue.parse_args(f, *args, **kwargs)
+         depends_on, job_id, at_front, meta, retry, on_success, on_failure,
+         pipeline, args, kwargs) = Queue.parse_args(f, *args, **kwargs)
         job = self.create_job(f, status=JobStatus.SCHEDULED, args=args, kwargs=kwargs,
                               timeout=timeout, result_ttl=result_ttl, ttl=ttl,
                               failure_ttl=failure_ttl, description=description,
-                              depends_on=depends_on, job_id=job_id, meta=meta, retry=retry)
+                              depends_on=depends_on, job_id=job_id, meta=meta, retry=retry,
+                              on_success=on_success, on_failure=on_failure)
 
-        return self.schedule_job(job, datetime)
+        return self.schedule_job(job, datetime, pipeline=pipeline)
 
     def schedule_job(self, job, datetime, pipeline=None):
         """Puts job on ScheduledJobRegistry"""
         from .registry import ScheduledJobRegistry
         registry = ScheduledJobRegistry(queue=self)
 
         pipe = pipeline if pipeline is not None else self.connection.pipeline()
```

### Comparing `rq-1.8.1/rq/worker.py` & `rq-1.9.0/rq/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 import redis.exceptions
 
 from . import worker_registration
 from .command import parse_payload, PUBSUB_CHANNEL_TEMPLATE, handle_command
 from .compat import as_text, string_types, text_type
 from .connections import get_current_connection, push_connection, pop_connection
 
-from .defaults import (DEFAULT_RESULT_TTL,
+from .defaults import (CALLBACK_TIMEOUT, DEFAULT_RESULT_TTL,
                        DEFAULT_WORKER_TTL, DEFAULT_JOB_MONITORING_INTERVAL,
                        DEFAULT_LOGGING_FORMAT, DEFAULT_LOGGING_DATE_FORMAT)
-from .exceptions import DequeueTimeout, ShutDownImminentException
+from .exceptions import DeserializationError, DequeueTimeout, ShutDownImminentException
 from .job import Job, JobStatus
 from .logutils import setup_loghandlers
 from .queue import Queue
 from .registry import FailedJobRegistry, StartedJobRegistry, clean_registries
 from .scheduler import RQScheduler
 from .suspension import is_suspended
 from .timeouts import JobTimeoutException, HorseMonitorTimeoutException, UnixSignalDeathPenalty
@@ -172,21 +172,14 @@
                  prepare_for_work=True, serializer=None):  # noqa
         if connection is None:
             connection = get_current_connection()
         self.connection = connection
 
         self.redis_server_version = None
 
-        if prepare_for_work:
-            self.hostname = socket.gethostname()
-            self.pid = os.getpid()
-        else:
-            self.hostname = None
-            self.pid = None
-
         self.job_class = backend_class(self, 'job_class', override=job_class)
         self.queue_class = backend_class(self, 'queue_class', override=queue_class)
         self.version = VERSION
         self.python_version = sys.version
         self.serializer = resolve_serializer(serializer)
 
         queues = [self.queue_class(name=q,
@@ -221,14 +214,24 @@
         self.birth_date = None
         self.scheduler = None
         self.pubsub = None
         self.pubsub_thread = None
 
         self.disable_default_exception_handler = disable_default_exception_handler
 
+        if prepare_for_work:
+            self.hostname = socket.gethostname()
+            self.pid = os.getpid()
+            connection.client_setname(self.name)
+            self.ip_address = [client['addr'] for client in connection.client_list() if client['name'] == self.name][0]
+        else:
+            self.hostname = None
+            self.pid = None
+            self.ip_address = None
+
         if isinstance(exception_handlers, (list, tuple)):
             for handler in exception_handlers:
                 self.push_exc_handler(handler)
         elif exception_handlers is not None:
             self.push_exc_handler(exception_handlers)
 
     def get_redis_server_version(self):
@@ -297,14 +300,15 @@
 
             mapping = {
                 'birth': now_in_string,
                 'last_heartbeat': now_in_string,
                 'queues': queues,
                 'pid': self.pid,
                 'hostname': self.hostname,
+                'ip_address': self.ip_address,
                 'version': self.version,
                 'python_version': self.python_version,
             }
 
             if self.get_redis_server_version() >= StrictVersion("4.0.0"):
                 p.hset(key, mapping=mapping)
             else:
@@ -427,15 +431,15 @@
         """
         A waiting the end of the horse process and recycling resources.
         """
         pid = None
         stat = None
         try:
             pid, stat = os.waitpid(self.horse_pid, 0)
-        except ChildProcessError as e:
+        except ChildProcessError:
             # ChildProcessError: [Errno 10] No child processes
             pass
         return pid, stat
 
     def request_force_stop(self, signum, frame):
         """Terminates the application (cold shutdown).
         """
@@ -700,21 +704,23 @@
         connection.hset(self.key, 'last_heartbeat', utcformat(utcnow()))
         self.log.debug('Sent heartbeat to prevent worker timeout. '
                        'Next one should arrive within %s seconds.', timeout)
 
     def refresh(self):
         data = self.connection.hmget(
             self.key, 'queues', 'state', 'current_job', 'last_heartbeat',
-            'birth', 'failed_job_count', 'successful_job_count',
-            'total_working_time', 'current_job_working_time', 'hostname', 'pid', 'version', 'python_version',
+            'birth', 'failed_job_count', 'successful_job_count', 'total_working_time',
+            'current_job_working_time', 'hostname', 'ip_address', 'pid', 'version', 'python_version',
         )
         (queues, state, job_id, last_heartbeat, birth, failed_job_count,
-         successful_job_count, total_working_time, current_job_working_time, hostname, pid, version, python_version) = data
+         successful_job_count, total_working_time, current_job_working_time,
+         hostname, ip_address, pid, version, python_version) = data
         queues = as_text(queues)
         self.hostname = as_text(hostname)
+        self.ip_address = as_text(ip_address)
         self.pid = int(pid) if pid else None
         self.version = as_text(version)
         self.python_version = as_text(python_version)
         self._state = as_text(state or '?')
         self._job_id = job_id or None
         if last_heartbeat:
             self.last_heartbeat = utcparse(as_text(last_heartbeat))
@@ -863,15 +869,15 @@
         random.seed()
 
         self.setup_work_horse_signals()
         self._is_horse = True
         self.log = logger
         try:
             self.perform_job(job, queue)
-        except:
+        except:  # noqa
             os._exit(1)
 
         # os._exit() is the way to exit from childs after a fork(), in
         # contrast to the regular sys.exit()
         os._exit(0)
 
     def setup_work_horse_signals(self):
@@ -992,14 +998,26 @@
                     started_job_registry.remove(job, pipeline=pipeline)
 
                     pipeline.execute()
                     break
                 except redis.exceptions.WatchError:
                     continue
 
+    def execute_success_callback(self, job, result):
+        """Executes success_callback with timeout"""
+        job.heartbeat(utcnow(), CALLBACK_TIMEOUT)
+        with self.death_penalty_class(CALLBACK_TIMEOUT, JobTimeoutException, job_id=job.id):
+            job.success_callback(job, self.connection, result)
+
+    def execute_failure_callback(self, job):
+        """Executes failure_callback with timeout"""
+        job.heartbeat(utcnow(), CALLBACK_TIMEOUT)
+        with self.death_penalty_class(CALLBACK_TIMEOUT, JobTimeoutException, job_id=job.id):
+            job.failure_callback(job, self.connection, *sys.exc_info())
+
     def perform_job(self, job, queue):
         """Performs the actual work of a job.  Will/should only be called
         inside the work horse's process.
         """
         push_connection(self.connection)
 
         started_job_registry = queue.started_job_registry
@@ -1013,21 +1031,37 @@
                 rv = job.perform()
 
             job.ended_at = utcnow()
 
             # Pickle the result in the same try-except block since we need
             # to use the same exc handling when pickling fails
             job._result = rv
+
+            if job.success_callback:
+                self.execute_success_callback(job, rv)
+
             self.handle_job_success(job=job,
                                     queue=queue,
                                     started_job_registry=started_job_registry)
         except:  # NOQA
             job.ended_at = utcnow()
             exc_info = sys.exc_info()
             exc_string = ''.join(traceback.format_exception(*exc_info))
+
+            if job.failure_callback:
+                try:
+                    self.execute_failure_callback(job)
+                except:  # noqa
+                    self.log.error(
+                        'Worker %s: error while executing failure callback',
+                        self.key, exc_info=True
+                    )
+                    exc_info = sys.exc_info()
+                    exc_string = ''.join(traceback.format_exception(*exc_info))
+
             self.handle_job_failure(job=job, exc_string=exc_string, queue=queue,
                                     started_job_registry=started_job_registry)
             self.handle_exception(job, *exc_info)
             return False
 
         finally:
             pop_connection()
@@ -1047,21 +1081,32 @@
                 self.log.info('Result will never expire, clean up result key manually')
 
         return True
 
     def handle_exception(self, job, *exc_info):
         """Walks the exception handler stack to delegate exception handling."""
         exc_string = ''.join(traceback.format_exception(*exc_info))
-        self.log.error(exc_string, extra={
-            'func': job.func_name,
-            'arguments': job.args,
-            'kwargs': job.kwargs,
-            'queue': job.origin,
-            'job_id': job.id,
-        })
+
+        # If the job cannot be deserialized, it will raise when func_name or
+        # the other properties are accessed, which will stop exceptions from
+        # being properly logged, so we guard against it here.
+        try:
+            extra = {
+                'func': job.func_name,
+                'arguments': job.args,
+                'kwargs': job.kwargs,
+            }
+        except DeserializationError:
+            extra = {}
+
+        # the properties below should be safe however
+        extra.update({'queue': job.origin, 'job_id': job.id})
+
+        # func_name
+        self.log.error(exc_string, exc_info=True, extra=extra)
 
         for handler in self._exc_handlers:
             self.log.debug('Invoking exception handler %s', handler)
             fallthrough = handler(job, *exc_info)
 
             # Only handlers with explicit return values should disable further
             # exc handling, so interpret a None return value as True.
@@ -1119,15 +1164,16 @@
 class SimpleWorker(Worker):
 
     def execute_job(self, job, queue):
         """Execute job in same thread/process, do not fork()"""
         return self.perform_job(job, queue)
 
     def get_heartbeat_ttl(self, job):
-        # "-1" means that jobs never timeout. In this case, we should _not_ do -1 + 60 = 59. We should just stick to DEFAULT_WORKER_TTL.
+        # "-1" means that jobs never timeout. In this case, we should _not_ do -1 + 60 = 59.
+        # # We should just stick to DEFAULT_WORKER_TTL.
         if job.timeout == -1:
             return DEFAULT_WORKER_TTL
         else:
             return (job.timeout or DEFAULT_WORKER_TTL) + 60
 
 
 class HerokuWorker(Worker):
```

### Comparing `rq-1.8.1/rq/compat/__init__.py` & `rq-1.9.0/rq/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/compat/dictconfig.py` & `rq-1.9.0/rq/compat/dictconfig.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/command.py` & `rq-1.9.0/rq/command.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/registry.py` & `rq-1.9.0/rq/registry.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/local.py` & `rq-1.9.0/rq/local.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/job.py` & `rq-1.9.0/rq/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from distutils.version import StrictVersion
 from enum import Enum
 from functools import partial
 from uuid import uuid4
 
 from rq.compat import as_text, decode_redis_hash, string_types
 from .connections import resolve_connection
-from .exceptions import NoSuchJobError
+from .exceptions import DeserializationError, NoSuchJobError
 from .local import LocalStack
 from .serializers import resolve_serializer
 from .utils import (get_version, import_attribute, parse_timeout, str_to_date,
-                    utcformat, utcnow, ensure_list)
+                    utcformat, utcnow, ensure_list, get_call_string)
 
 # Serialize pickle dumps using the highest pickle protocol (binary, default
 # uses ascii)
 dumps = partial(pickle.dumps, protocol=pickle.HIGHEST_PROTOCOL)
 loads = pickle.loads
 
 
@@ -41,20 +41,14 @@
 
 
 # Sentinel value to mark that some of our lazily evaluated properties have not
 # yet been evaluated.
 UNEVALUATED = object()
 
 
-def truncate_long_string(data, maxlen=75):
-    """ Truncates strings longer than maxlen
-    """
-    return (data[:maxlen] + '...') if len(data) > maxlen else data
-
-
 def cancel_job(job_id, connection=None):
     """Cancels the job with the given job ID, preventing execution.  Discards
     any job info (i.e. it can't be requeued later).
     """
     Job.fetch(job_id, connection=connection).cancel()
 
 
@@ -79,15 +73,15 @@
     redis_job_namespace_prefix = 'rq:job:'
 
     # Job construction
     @classmethod
     def create(cls, func, args=None, kwargs=None, connection=None,
                result_ttl=None, ttl=None, status=None, description=None,
                depends_on=None, timeout=None, id=None, origin=None, meta=None,
-               failure_ttl=None, serializer=None):
+               failure_ttl=None, serializer=None, *, on_success=None, on_failure=None):
         """Creates a new Job instance for the given function, arguments, and
         keyword arguments.
         """
         if args is None:
             args = ()
         if kwargs is None:
             kwargs = {}
@@ -117,14 +111,24 @@
             job._instance = func
             job._func_name = '__call__'
         else:
             raise TypeError('Expected a callable or a string, but got: {0}'.format(func))
         job._args = args
         job._kwargs = kwargs
 
+        if on_success:
+            if not inspect.isfunction(on_success) and not inspect.isbuiltin(on_success):
+                raise ValueError('on_success callback must be a function')
+            job._success_callback_name = '{0}.{1}'.format(on_success.__module__, on_success.__qualname__)
+
+        if on_failure:
+            if not inspect.isfunction(on_failure) and not inspect.isbuiltin(on_failure):
+                raise ValueError('on_failure callback must be a function')
+            job._failure_callback_name = '{0}.{1}'.format(on_failure.__module__, on_failure.__qualname__)
+
         # Extra meta data
         job.description = description or job.get_call_string()
         job.result_ttl = parse_timeout(result_ttl)
         job.failure_ttl = parse_timeout(failure_ttl)
         job.ttl = parse_timeout(ttl)
         job.timeout = parse_timeout(timeout)
         job._status = status
@@ -216,16 +220,40 @@
             return None
 
         if self.instance:
             return getattr(self.instance, func_name)
 
         return import_attribute(self.func_name)
 
+    @property
+    def success_callback(self):
+        if self._success_callback is UNEVALUATED:
+            if self._success_callback_name:
+                self._success_callback = import_attribute(self._success_callback_name)
+            else:
+                self._success_callback = None
+
+        return self._success_callback
+
+    @property
+    def failure_callback(self):
+        if self._failure_callback is UNEVALUATED:
+            if self._failure_callback_name:
+                self._failure_callback = import_attribute(self._failure_callback_name)
+            else:
+                self._failure_callback = None
+
+        return self._failure_callback
+
     def _deserialize_data(self):
-        self._func_name, self._instance, self._args, self._kwargs = self.serializer.loads(self.data)
+        try:
+            self._func_name, self._instance, self._args, self._kwargs = self.serializer.loads(self.data)
+        except Exception as e:
+            # catch anything because serializers are generic
+            raise DeserializationError() from e
 
     @property
     def data(self):
         if self._data is UNEVALUATED:
             if self._func_name is UNEVALUATED:
                 raise ValueError('Cannot build the job data')
 
@@ -338,14 +366,18 @@
         self._id = id
         self.created_at = utcnow()
         self._data = UNEVALUATED
         self._func_name = UNEVALUATED
         self._instance = UNEVALUATED
         self._args = UNEVALUATED
         self._kwargs = UNEVALUATED
+        self._success_callback_name = None
+        self._success_callback = UNEVALUATED
+        self._failure_callback_name = None
+        self._failure_callback = UNEVALUATED
         self.description = None
         self.origin = None
         self.enqueued_at = None
         self.started_at = None
         self.ended_at = None
         self._result = None
         self.exc_info = None
@@ -392,16 +424,16 @@
 
     def set_id(self, value):
         """Sets a job ID for the given job."""
         if not isinstance(value, string_types):
             raise TypeError('id must be a string, not {0}'.format(type(value)))
         self._id = value
 
-    def heartbeat(self, heartbeat, ttl, pipeline=None):
-        self.last_heartbeat = heartbeat
+    def heartbeat(self, timestamp, ttl, pipeline=None):
+        self.last_heartbeat = timestamp
         connection = pipeline if pipeline is not None else self.connection
         connection.hset(self.key, 'last_heartbeat', utcformat(self.last_heartbeat))
         self.started_job_registry.add(self, ttl, pipeline=pipeline)
 
     id = property(get_id, set_id)
 
     @classmethod
@@ -500,18 +532,24 @@
         result = obj.get('result')
         if result:
             try:
                 self._result = self.serializer.loads(obj.get('result'))
             except Exception:
                 self._result = "Unserializable return value"
         self.timeout = parse_timeout(obj.get('timeout')) if obj.get('timeout') else None
-        self.result_ttl = int(obj.get('result_ttl')) if obj.get('result_ttl') else None  # noqa
-        self.failure_ttl = int(obj.get('failure_ttl')) if obj.get('failure_ttl') else None  # noqa
+        self.result_ttl = int(obj.get('result_ttl')) if obj.get('result_ttl') else None
+        self.failure_ttl = int(obj.get('failure_ttl')) if obj.get('failure_ttl') else None
         self._status = obj.get('status').decode() if obj.get('status') else None
 
+        if obj.get('success_callback_name'):
+            self._success_callback_name = obj.get('success_callback_name').decode()
+
+        if obj.get('failure_callback_name'):
+            self._failure_callback_name = obj.get('failure_callback_name').decode()
+
         dep_ids = obj.get('dependency_ids')
         dep_id = obj.get('dependency_id')  # for backwards compatibility
         self._dependency_ids = (json.loads(dep_ids.decode()) if dep_ids
                                 else [dep_id.decode()] if dep_id else [])
 
         self.ttl = int(obj.get('ttl')) if obj.get('ttl') else None
         self.meta = self.serializer.loads(obj.get('meta')) if obj.get('meta') else {}
@@ -546,14 +584,16 @@
 
         You can exclude serializing the `meta` dictionary by setting
         `include_meta=False`.
         """
         obj = {
             'created_at': utcformat(self.created_at or utcnow()),
             'data': zlib.compress(self.data),
+            'success_callback_name': self._success_callback_name if self._success_callback_name else '',
+            'failure_callback_name': self._failure_callback_name if self._failure_callback_name else '',
             'started_at': utcformat(self.started_at) if self.started_at else '',
             'ended_at': utcformat(self.ended_at) if self.ended_at else '',
             'last_heartbeat': utcformat(self.last_heartbeat) if self.last_heartbeat else '',
             'worker_name': self.worker_name or ''
         }
 
         if self.retries_left is not None:
@@ -751,25 +791,15 @@
         return default_ttl if self.result_ttl is None else self.result_ttl
 
     # Representation
     def get_call_string(self):  # noqa
         """Returns a string representation of the call, formatted as a regular
         Python function invocation statement.
         """
-        if self.func_name is None:
-            return None
-
-        arg_list = [as_text(truncate_long_string(repr(arg))) for arg in self.args]
-
-        kwargs = ['{0}={1}'.format(k, as_text(truncate_long_string(repr(v)))) for k, v in self.kwargs.items()]
-        # Sort here because python 3.3 & 3.4 makes different call_string
-        arg_list += sorted(kwargs)
-        args = ', '.join(arg_list)
-
-        return '{0}({1})'.format(self.func_name, args)
+        return get_call_string(self.func_name, self.args, self.kwargs, max_length=75)
 
     def cleanup(self, ttl=None, pipeline=None, remove_from_queue=True):
         """Prepare job for eventual deletion (if needed). This method is usually
         called after successful execution. How long we persist the job and its
         result depends on the value of ttl:
         - If ttl is 0, cleanup the job immediately.
         - If it's a positive number, set the job to expire in X seconds.
```

### Comparing `rq-1.8.1/rq/serializers.py` & `rq-1.9.0/rq/serializers.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/connections.py` & `rq-1.9.0/rq/connections.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/suspension.py` & `rq-1.9.0/rq/suspension.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/timeouts.py` & `rq-1.9.0/rq/timeouts.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/logutils.py` & `rq-1.9.0/rq/logutils.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/cli/cli.py` & `rq-1.9.0/rq/cli/cli.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/cli/helpers.py` & `rq-1.9.0/rq/cli/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 
 import sys
 import importlib
 import time
+import os
 from functools import partial
 
 import click
 import redis
 from redis import Redis
 from redis.sentinel import Sentinel
 from rq.defaults import (DEFAULT_CONNECTION_CLASS, DEFAULT_JOB_CLASS,
@@ -44,20 +45,29 @@
         socket_timeout = settings['SENTINEL'].get('SOCKET_TIMEOUT', None)
         password = settings['SENTINEL'].get('PASSWORD', None)
         db = settings['SENTINEL'].get('DB', 0)
         master_name = settings['SENTINEL'].get('MASTER_NAME', 'mymaster')
         sn = Sentinel(instances, socket_timeout=socket_timeout, password=password, db=db)
         return sn.master_for(master_name)
 
+    ssl = settings.get('REDIS_SSL', False)
+    if isinstance(ssl, str):
+        if ssl.lower() in ['y', 'yes', 't', 'true']:
+            ssl = True
+        elif ssl.lower() in ['n', 'no', 'f', 'false', '']:
+            ssl = False
+        else:
+            raise ValueError('REDIS_SSL is a boolean and must be "True" or "False".')
+
     kwargs = {
         'host': settings.get('REDIS_HOST', 'localhost'),
         'port': settings.get('REDIS_PORT', 6379),
         'db': settings.get('REDIS_DB', 0),
         'password': settings.get('REDIS_PASSWORD', None),
-        'ssl': settings.get('REDIS_SSL', False),
+        'ssl': ssl,
         'ssl_ca_certs': settings.get('REDIS_SSL_CA_CERTS', None),
     }
 
     return connection_class(**kwargs)
 
 
 def pad(s, pad_to_length):
@@ -127,15 +137,15 @@
         for worker in worker_class.all():
             workers.add(worker)
 
     if not by_queue:
 
         for worker in workers:
             queue_names = ', '.join(worker.queue_names())
-            name = '%s (%s %s)' % (worker.name, worker.hostname, worker.pid)
+            name = '%s (%s %s %s)' % (worker.name, worker.hostname, worker.ip_address, worker.pid)
             if not raw:
                 click.echo('%s: %s %s' % (name, state_symbol(worker.get_state()), queue_names))
             else:
                 click.echo('worker %s %s %s' % (name, worker.get_state(), queue_names))
 
     else:
         # Display workers by queue
@@ -231,12 +241,15 @@
             raise click.BadParameter(str(exc), param_hint='--connection-class')
 
     @property
     def connection(self):
         if self._connection is None:
             if self.url:
                 self._connection = self.connection_class.from_url(self.url)
-            else:
+            elif self.config:
                 settings = read_config_file(self.config) if self.config else {}
                 self._connection = get_redis_from_config(settings,
                                                          self.connection_class)
+            else:
+                self._connection = get_redis_from_config(os.environ,
+                                                         self.connection_class)
         return self._connection
```

### Comparing `rq-1.8.1/rq/contrib/legacy.py` & `rq-1.9.0/rq/contrib/legacy.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/utils.py` & `rq-1.9.0/rq/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -128,20 +128,25 @@
     name_bits = name.split('.')
     module_name_bits, attribute_bits = name_bits[:-1], [name_bits[-1]]
     module = None
     # When the attribute we look for is a staticmethod, module name in its
     # dotted path is not the last-before-end word
     # E.g.: package_a.package_b.module_a.ClassA.my_static_method
     # Thus we remove the bits from the end of the name until we can import it
+    #
+    # Sometimes the failure during importing is due to a genuine coding error in the imported module
+    # In this case, the exception is logged as a warning for ease of debugging.
+    # The above logic will apply anyways regardless of the cause of the import error.
     while len(module_name_bits):
         try:
             module_name = '.'.join(module_name_bits)
             module = importlib.import_module(module_name)
             break
         except ImportError:
+            logging.warning("Import error for '%s'" % module_name, exc_info=True)
             attribute_bits.insert(0, module_name_bits.pop())
 
     if module is None:
         raise ValueError('Invalid attribute name: %s' % name)
 
     attribute_name = '.'.join(attribute_bits)
     if hasattr(module, attribute_name):
@@ -288,7 +293,31 @@
 
 def split_list(a_list, segment_size):
     """
     Splits a list into multiple smaller lists having size `segment_size`
     """
     for i in range(0, len(a_list), segment_size):
         yield a_list[i:i + segment_size]
+
+
+def truncate_long_string(data, max_length=None):
+    """Truncate arguments with representation longer than max_length"""
+    if max_length is None:
+        return data
+    return (data[:max_length] + '...') if len(data) > max_length else data
+
+
+def get_call_string(func_name, args, kwargs, max_length=None):
+    """Returns a string representation of the call, formatted as a regular
+    Python function invocation statement. If max_length is not None, truncate
+    arguments with representation longer than max_length.
+    """
+    if func_name is None:
+        return None
+
+    arg_list = [as_text(truncate_long_string(repr(arg), max_length)) for arg in args]
+
+    kwargs = ['{0}={1}'.format(k, as_text(truncate_long_string(repr(v), max_length))) for k, v in kwargs.items()]
+    arg_list += sorted(kwargs)
+    args = ', '.join(arg_list)
+
+    return '{0}({1})'.format(func_name, args)
```

### Comparing `rq-1.8.1/rq/exceptions.py` & `rq-1.9.0/rq/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
                         unicode_literals)
 
 
 class NoSuchJobError(Exception):
     pass
 
 
+class DeserializationError(Exception):
+    pass
+
+
 class InvalidJobDependency(Exception):
     pass
 
 
 class InvalidJobOperationError(Exception):
     pass
```

### Comparing `rq-1.8.1/rq/scheduler.py` & `rq-1.9.0/rq/scheduler.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/dummy.py` & `rq-1.9.0/rq/dummy.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/worker_registration.py` & `rq-1.9.0/rq/worker_registration.py`

 * *Files identical despite different names*

### Comparing `rq-1.8.1/rq/decorators.py` & `rq-1.9.0/rq/decorators.py`

 * *Files identical despite different names*

