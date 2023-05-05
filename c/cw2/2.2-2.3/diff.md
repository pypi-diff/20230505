# Comparing `tmp/cw2-2.2.tar.gz` & `tmp/cw2-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cw2-2.2.tar", last modified: Mon Apr 24 13:12:53 2023, max compression
+gzip compressed data, was "cw2-2.3.tar", last modified: Fri May  5 09:06:59 2023, max compression
```

## Comparing `cw2-2.2.tar` & `cw2-2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.947887 cw2-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-24 13:12:39.000000 cw2-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-24 13:12:53.947887 cw2-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-24 13:12:39.000000 cw2-2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:39.000000 cw2-2.2/cw2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-24 13:12:39.000000 cw2-2.2/cw2/alternative_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cluster_work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2/cw_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/conf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/conf_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/conf_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/conf_unfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/cw_conf_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/cw_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2/cw_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/cw_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/cw_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/cw_pd_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/cw_wandb_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2/cw_slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_slurm/cw_slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_slurm/cw_slurm_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-24 13:12:39.000000 cw2-2.2/cw2/default_sbatch.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-24 13:12:39.000000 cw2-2.2/cw2/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-24 13:12:39.000000 cw2-2.2/cw2/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14026 2023-04-24 13:12:39.000000 cw2-2.2/cw2/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-24 13:12:39.000000 cw2-2.2/cw2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-24 13:12:39.000000 cw2-2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:12:53.947887 cw2-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-24 13:12:39.000000 cw2-2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-24 13:12:39.000000 cw2-2.2/test/test_cw_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:59.972740 cw2-2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-05 09:06:44.000000 cw2-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-05 09:06:59.972740 cw2-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-05 09:06:44.000000 cw2-2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:59.968740 cw2-2.3/cw2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:44.000000 cw2-2.3/cw2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-05 09:06:44.000000 cw2-2.3/cw2/alternative_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cluster_work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:59.972740 cw2-2.3/cw2/cw_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_config/conf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_config/conf_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_config/conf_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_config/conf_unfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_config/cw_conf_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_config/cw_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:59.972740 cw2-2.3/cw2/cw_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_data/cw_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_data/cw_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_data/cw_pd_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_data/cw_wandb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:59.972740 cw2-2.3/cw2/cw_slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_slurm/cw_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 09:06:44.000000 cw2-2.3/cw2/cw_slurm/cw_slurm_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-05 09:06:44.000000 cw2-2.3/cw2/default_sbatch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-05 09:06:44.000000 cw2-2.3/cw2/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-05 09:06:44.000000 cw2-2.3/cw2/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-05 09:06:44.000000 cw2-2.3/cw2/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-05 09:06:44.000000 cw2-2.3/cw2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:59.968740 cw2-2.3/cw2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-05 09:06:59.000000 cw2-2.3/cw2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 09:06:59.000000 cw2-2.3/cw2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:06:59.000000 cw2-2.3/cw2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 09:06:59.000000 cw2-2.3/cw2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 09:06:59.000000 cw2-2.3/cw2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 09:06:44.000000 cw2-2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:06:59.972740 cw2-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-05 09:06:44.000000 cw2-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:06:59.972740 cw2-2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-05 09:06:44.000000 cw2-2.3/test/test_cw_config.py
```

### Comparing `cw2-2.2/LICENSE` & `cw2-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cw2-2.2/PKG-INFO` & `cw2-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cw2
-Version: 2.2
+Version: 2.3
 Summary: A reengineered framework to run experiments on a computing cluster.
 Home-page: https://github.com/ALRhub/cw2
 Author: Maximilian Li
 Author-email: maximilian.xiling.li@gmail.com
 License: MIT
 Keywords: scientific,experiments,distributed computing,mpi,research
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cw2-2.2/README.md` & `cw2-2.3/README.md`

 * *Files identical despite different names*

### Comparing `cw2-2.2/cw2/alternative_schedulers.py` & `cw2-2.3/cw2/alternative_schedulers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,157 +1,192 @@
 import abc
+import concurrent.futures as con
+import multiprocessing
 import os
+import queue
 from typing import List
 
 from joblib import Parallel, delayed
-import multiprocessing
-
-import concurrent.futures as con
-import queue
 
 from cw2 import cw_error, job
 from cw2.cw_config import cw_config
 from cw2.cw_slurm import cw_slurm
-
 from cw2.scheduler import GPUDistributingLocalScheduler
 
 
 class StarmapGPUDistributingLocalScheduler(GPUDistributingLocalScheduler):
-
     def run(self, overwrite: bool = False):
         print("Using StarmapGPUDistributingLocalScheduler")
         num_parallel = self.joblist[0].n_parallel
         for j in self.joblist:
-            assert j.n_parallel == num_parallel, "All jobs in list must have same n_parallel"
-            assert j.n_parallel == self._queue_elements, "Mismatch between GPUs Queue Elements and Jobs executed in" \
-                                                         "parallel. Fix for optimal resource usage!!"
+            assert (
+                j.n_parallel == num_parallel
+            ), "All jobs in list must have same n_parallel"
+            assert j.n_parallel == self._queue_elements, (
+                "Mismatch between GPUs Queue Elements and Jobs executed in"
+                "parallel. Fix for optimal resource usage!!"
+            )
 
         with multiprocessing.Pool(processes=num_parallel) as pool:
             # setup gpu resource queue
             m = multiprocessing.Manager()
             gpu_queue = m.Queue(maxsize=self._queue_elements)
             for i in range(self._queue_elements):
                 gpu_queue.put(i)
 
             for j in self.joblist:
-                args = [(j, c, gpu_queue, self._gpus_per_rep, overwrite) for c in j.tasks]
-                pool.starmap_async(StarmapGPUDistributingLocalScheduler._execute_task, args)
+                args = [
+                    (j, c, gpu_queue, self._gpus_per_rep, overwrite) for c in j.tasks
+                ]
+                pool.starmap_async(
+                    StarmapGPUDistributingLocalScheduler._execute_task, args
+                )
             pool.close()
             pool.join()
 
     @staticmethod
-    def _execute_task(j: job.Job,
-                      c: dict,
-                      q: multiprocessing.Queue,
-                      gpus_per_job: int,
-                      overwrite: bool = False):
+    def _execute_task(
+        j: job.Job,
+        c: dict,
+        q: multiprocessing.Queue,
+        gpus_per_job: int,
+        overwrite: bool = False,
+    ):
         gpu_idx = q.get()
-        s = ("{}," * gpus_per_job).format(*[gpu_idx * gpus_per_job + i for i in range(gpus_per_job)])[:-1]
+        s = ("{}," * gpus_per_job).format(
+            *[gpu_idx * gpus_per_job + i for i in range(gpus_per_job)]
+        )[:-1]
         try:
             os.environ["CUDA_VISIBLE_DEVICES"] = s
             j.run_task(c, overwrite)
         except cw_error.ExperimentSurrender as _:
             return
         finally:
             q.put(gpu_idx)
 
 
 class ConcurrentGPUDistributingLocalScheduler(GPUDistributingLocalScheduler):
-
     def run(self, overwrite: bool = False):
         print("Using ConcurrentGPUDistributingLocalScheduler")
         num_parallel = self.joblist[0].n_parallel
         for j in self.joblist:
-            assert j.n_parallel == num_parallel, "All jobs in list must have same n_parallel"
-            assert j.n_parallel == self._queue_elements, "Mismatch between GPUs Queue Elements and Jobs executed in" \
-                                                         "parallel. Fix for optimal resource usage!!"
+            assert (
+                j.n_parallel == num_parallel
+            ), "All jobs in list must have same n_parallel"
+            assert j.n_parallel == self._queue_elements, (
+                "Mismatch between GPUs Queue Elements and Jobs executed in"
+                "parallel. Fix for optimal resource usage!!"
+            )
 
         with con.ProcessPoolExecutor(max_workers=num_parallel) as pool:
             # setup gpu resource queue
-            #gpu_queue = queue.Queue(maxsize=self._queue_elements)
-            #for i in range(self._queue_elements):
+            # gpu_queue = queue.Queue(maxsize=self._queue_elements)
+            # for i in range(self._queue_elements):
             #    gpu_queue.put(i)
 
             results = []
             for j in self.joblist:
                 for i, c in enumerate(j.tasks):
-                    results.append(pool.submit(ConcurrentGPUDistributingLocalScheduler._execute_task, j, c, i,
-                                               self._gpus_per_rep, overwrite))
+                    results.append(
+                        pool.submit(
+                            ConcurrentGPUDistributingLocalScheduler._execute_task,
+                            j,
+                            c,
+                            i,
+                            self._gpus_per_rep,
+                            overwrite,
+                        )
+                    )
             for r in results:
                 r.result()
 
     @staticmethod
-    def _execute_task(j: job.Job,
-                      c: dict,
-                      idx: int,
-                      #q: multiprocessing.Queue,
-                      gpus_per_job: int,
-                      overwrite: bool = False):
-        #gpu_idx = q.get()
-        s = ("{}," * gpus_per_job).format(*[idx * gpus_per_job + i for i in range(gpus_per_job)])[:-1]
+    def _execute_task(
+        j: job.Job,
+        c: dict,
+        idx: int,
+        # q: multiprocessing.Queue,
+        gpus_per_job: int,
+        overwrite: bool = False,
+    ):
+        # gpu_idx = q.get()
+        s = ("{}," * gpus_per_job).format(
+            *[idx * gpus_per_job + i for i in range(gpus_per_job)]
+        )[:-1]
         try:
             os.environ["CUDA_VISIBLE_DEVICES"] = s
             j.run_task(c, overwrite)
         except cw_error.ExperimentSurrender as _:
             return
-       # finally:
-            #q.put(gpu_idx)
 
+    # finally:
+    # q.put(gpu_idx)
 
-class JoblibGPUDistributingLocalScheduler(GPUDistributingLocalScheduler):
 
+class JoblibGPUDistributingLocalScheduler(GPUDistributingLocalScheduler):
     def run(self, overwrite: bool = False):
         print("Using JoblibGPUDistributingLocalScheduler")
         for j in self.joblist:
-            Parallel(n_jobs=j.n_parallel)(delayed(self.execute_task)(j, c, i, self._gpus_per_rep, overwrite)
-                                          for i, c in enumerate(j.tasks))
-
-    def execute_task(self, j: job.Job, c: dict, idx: int, gpus_per_job: int, overwrite: bool = False):
-        s = ("{}," * gpus_per_job).format(*[idx * gpus_per_job + i for i in range(gpus_per_job)])[:-1]
+            Parallel(n_jobs=j.n_parallel)(
+                delayed(self.execute_task)(j, c, i, self._gpus_per_rep, overwrite)
+                for i, c in enumerate(j.tasks)
+            )
+
+    def execute_task(
+        self, j: job.Job, c: dict, idx: int, gpus_per_job: int, overwrite: bool = False
+    ):
+        s = ("{}," * gpus_per_job).format(
+            *[idx * gpus_per_job + i for i in range(gpus_per_job)]
+        )[:-1]
         try:
             os.environ["CUDA_VISIBLE_DEVICES"] = s
             j.run_task(c, overwrite)
         except cw_error.ExperimentSurrender as _:
             return
 
 
 class RayGPUDistributingLocalScheduler(GPUDistributingLocalScheduler):
-
     def run(self, overwrite: bool = False):
         print("Using RayGPUDistributingLocalScheduler")
 
         import ray
         from ray.util.queue import Queue
 
         @ray.remote
-        def _execute_task(j: job.Job,
-                          c: dict,
-                          q,
-                          gpus_per_job: int,
-                          overwrite: bool = False):
+        def _execute_task(
+            j: job.Job, c: dict, q, gpus_per_job: int, overwrite: bool = False
+        ):
             gpu_idx = q.get()
             print("I got gpu idx", gpu_idx)
-            s = ("{}," * gpus_per_job).format(*[gpu_idx * gpus_per_job + i for i in range(gpus_per_job)])[:-1]
+            s = ("{}," * gpus_per_job).format(
+                *[gpu_idx * gpus_per_job + i for i in range(gpus_per_job)]
+            )[:-1]
             try:
                 os.environ["CUDA_VISIBLE_DEVICES"] = s
                 j.run_task(c, overwrite)
             except cw_error.ExperimentSurrender as _:
                 return
             finally:
                 print("giving back gpu idx", gpu_idx)
                 q.put(gpu_idx)
 
         ray.init()
         num_parallel = self.joblist[0].n_parallel
         for j in self.joblist:
-            assert j.n_parallel == num_parallel, "All jobs in list must have same n_parallel"
-            assert j.n_parallel == self._queue_elements, "Mismatch between GPUs Queue Elements and Jobs executed in" \
-                                                         "parallel. Fix for optimal resource usage!!"
+            assert (
+                j.n_parallel == num_parallel
+            ), "All jobs in list must have same n_parallel"
+            assert j.n_parallel == self._queue_elements, (
+                "Mismatch between GPUs Queue Elements and Jobs executed in"
+                "parallel. Fix for optimal resource usage!!"
+            )
         gpu_queue = Queue(maxsize=self._queue_elements)
 
         for i in range(self._queue_elements):
             gpu_queue.put(i)
         results = []
         for j in self.joblist:
             for i, c in enumerate(j.tasks):
-                results.append(_execute_task.remote(j, c, gpu_queue, self._gpus_per_rep, overwrite))
+                results.append(
+                    _execute_task.remote(j, c, gpu_queue, self._gpus_per_rep, overwrite)
+                )
         ray.get(results)
```

### Comparing `cw2-2.2/cw2/cli_parser.py` & `cw2-2.3/cw2/cli_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,68 @@
 import argparse
 
 
 class Arguments:
     def __init__(self):
         p = argparse.ArgumentParser()
-        p.add_argument('config', metavar='CONFIG.yml')
-        p.add_argument('-j', '--job', type=int, default=None,
-                       help='Run only the specified job. CAVEAT: Should only be used with slurm arrays.')
+        p.add_argument("config", metavar="CONFIG.yml")
+        p.add_argument(
+            "-j",
+            "--job",
+            type=int,
+            default=None,
+            help="Run only the specified job. CAVEAT: Should only be used with slurm arrays.",
+        )
 
         # XXX: Disable delete for now
         # p.add_argument('-d', '--delete', action='store_true',
         #                help='CAUTION deletes results of previous runs.')
 
-        p.add_argument('-e', '--experiments', nargs='+', default=None,
-                       help='Allows to specify which experiments should be run.')
-        p.add_argument('-s', '--slurm', action='store_true',
-                       help='Run using SLURM Workload Manager.')
-        p.add_argument('-o', '--overwrite', action='store_true',
-                       help='Overwrite existing results.')
-        p.add_argument('--nocodecopy', action='store_true', help='Skip code copy.')
-        p.add_argument('--zip', action='store_true', help='Make a Zip Copy of the Code.')
-        p.add_argument('--skipsizecheck', action='store_true', help='Skip check if code copy src < 200MByte')
-        p.add_argument('--multicopy', action='store_true', help='Create a code copy for each job seperately')
-        p.add_argument('--noconsolelog', action='store_true', help='Disables writing internal console log files')
-        p.add_argument('--debug', action='store_true', default=False, help='Enable debug mode.')
-        p.add_argument('--debugall', action='store_true', default=False, help='Enable debug mode for arguments.')
+        p.add_argument(
+            "-e",
+            "--experiments",
+            nargs="+",
+            default=None,
+            help="Allows to specify which experiments should be run.",
+        )
+        p.add_argument(
+            "-s",
+            "--slurm",
+            action="store_true",
+            help="Run using SLURM Workload Manager.",
+        )
+        p.add_argument(
+            "-o", "--overwrite", action="store_true", help="Overwrite existing results."
+        )
+        p.add_argument("--nocodecopy", action="store_true", help="Skip code copy.")
+        p.add_argument(
+            "--zip", action="store_true", help="Make a Zip Copy of the Code."
+        )
+        p.add_argument(
+            "--skipsizecheck",
+            action="store_true",
+            help="Skip check if code copy src < 200MByte",
+        )
+        p.add_argument(
+            "--multicopy",
+            action="store_true",
+            help="Create a code copy for each job seperately",
+        )
+        p.add_argument(
+            "--noconsolelog",
+            action="store_true",
+            help="Disables writing internal console log files",
+        )
+        p.add_argument(
+            "--debug", action="store_true", default=False, help="Enable debug mode."
+        )
+        p.add_argument(
+            "--debugall",
+            action="store_true",
+            default=False,
+            help="Enable debug mode for arguments.",
+        )
 
         self.args = p.parse_args(namespace=self)
 
     def get(self) -> dict:
         return vars(self.args)
```

### Comparing `cw2-2.2/cw2/cluster_work.py` & `cw2-2.3/cw2/cluster_work.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,77 +3,88 @@
 from cw2 import cli_parser, experiment, job, scheduler
 from cw2.cw_config import cw_config
 from cw2.cw_data import cw_loading, cw_logging
 
 
 class ClusterWork:
     def __init__(self, exp_cls: Type[experiment.AbstractExperiment] = None):
-
         self.args = cli_parser.Arguments().get()
         self.exp_cls = exp_cls
-        self.config = cw_config.Config(self.args['config'],
-                                       self.args['experiments'],
-                                       self.args['debug'],
-                                       self.args['debugall'])
+        self.config = cw_config.Config(
+            self.args["config"],
+            self.args["experiments"],
+            self.args["debug"],
+            self.args["debugall"],
+        )
 
         self.logArray = cw_logging.LoggerArray()
 
-        if not self.args['noconsolelog']:
+        if not self.args["noconsolelog"]:
             self.add_logger(cw_logging.PythonLogger())
         self.joblist = None
 
     def add_logger(self, logger: cw_logging.AbstractLogger) -> None:
         """add a logger to the ClusterWork pipeline
 
         Args:
             logger (cw_logging.AbstractLogger): logger object to be called during execution
         """
         self.logArray.add(logger)
 
-    def _get_jobs(self, delete: bool = False, root_dir: str = "", read_only: bool = False) -> List[job.Job]:
+    def _get_jobs(
+        self, delete: bool = False, root_dir: str = "", read_only: bool = False
+    ) -> List[job.Job]:
         """private method. creates and returns all configured jobs.
 
         Args:
             delete (bool, optional): delete all old data inside the job directories. Defaults to False.
             root_dir (str, optional): [description]. Defaults to "".
 
         Returns:
             List[job.Job]: list of all configured job objects
         """
         if self.joblist is None:
             factory = job.JobFactory(
-                self.exp_cls, self.logArray, delete, root_dir, read_only)
+                self.exp_cls, self.logArray, delete, root_dir, read_only
+            )
             self.joblist = factory.create_jobs(self.config.exp_configs)
         return self.joblist
 
     def run(self, root_dir: str = "", sch: scheduler.AbstractScheduler = None):
         """Run ClusterWork computations.
 
         Args:
             root_dir (str, optional): [description]. Defaults to "".
         """
         if self.exp_cls is None:
             raise NotImplementedError(
-                "Cannot run with missing experiment.AbstractExperiment Implementation.")
+                "Cannot run with missing experiment.AbstractExperiment Implementation."
+            )
 
         self.config.to_yaml(relpath=True)
 
         args = self.args
 
         # Handle SLURM execution
-        if args['slurm']:
+        if args["slurm"]:
             s = scheduler.SlurmScheduler(self.config)
         else:
             # Do Local execution
             if sch is None:
-                if scheduler.GPUDistributingLocalScheduler.use_distributed_gpu_scheduling(self.config):
-                    scheduler_cls = scheduler.get_gpu_scheduler_cls(self.config.slurm_config.get("scheduler", "mp"))
+                if scheduler.GPUDistributingLocalScheduler.use_distributed_gpu_scheduling(
+                    self.config
+                ):
+                    scheduler_cls = scheduler.get_gpu_scheduler_cls(
+                        self.config.slurm_config.get("scheduler", "mp")
+                    )
                     s = scheduler_cls(self.config)
 
-                elif scheduler.CpuDistributingLocalScheduler.use_distributed_cpu_scheduling(self.config):
+                elif scheduler.CpuDistributingLocalScheduler.use_distributed_cpu_scheduling(
+                    self.config
+                ):
                     s = scheduler.CpuDistributingLocalScheduler(self.config)
 
                 else:
                     s = scheduler.LocalScheduler()
             else:
                 s = sch
 
@@ -89,19 +100,24 @@
             pd.DataFrame: saved data in Dataframe form.
         """
 
         loader = cw_loading.Loader()
 
         return self._run_scheduler(loader, root_dir, True)
 
-    def _run_scheduler(self, s: scheduler.AbstractScheduler, root_dir: str = "", read_only: bool = False):
+    def _run_scheduler(
+        self,
+        s: scheduler.AbstractScheduler,
+        root_dir: str = "",
+        read_only: bool = False,
+    ):
         if self.logArray.is_empty():
             cw_logging.getLogger().warning("No Logger has been added. Are you sure?")
 
         args = self.args
         job_list = self._get_jobs(False, root_dir, read_only)
 
-        if args['job'] is not None:
-            job_list = [job_list[args['job']]]
+        if args["job"] is not None:
+            job_list = [job_list[args["job"]]]
 
         s.assign(job_list)
-        return s.run(overwrite=args['overwrite'])
+        return s.run(overwrite=args["overwrite"])
```

### Comparing `cw2-2.2/cw2/cw_config/conf_io.py` & `cw2-2.3/cw2/cw_config/conf_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 from typing import List, Tuple
+
 import yaml
 
 from cw2.cw_config import cw_conf_keys as KEY
-from cw2.cw_error import MissingConfigError, ExperimentNotFoundError
+from cw2.cw_error import ExperimentNotFoundError, MissingConfigError
 
 
-def get_configs(config_path: str, experiment_selections: List[str]) -> Tuple[dict, dict, List[dict]]:
+def get_configs(
+    config_path: str, experiment_selections: List[str]
+) -> Tuple[dict, dict, List[dict]]:
     """reads and seperates the experiment configs from a yaml file
 
     Args:
         config_path (str): path to the yaml file
         experiment_selections (List[str]): a list of selected experiment names
 
     Returns:
@@ -30,23 +33,24 @@
         List[dict]: all configs found in the yaml file
     """
     if not os.path.exists(config_path):
         raise MissingConfigError("Could not find {}".format(config_path))
 
     all_configs = []
 
-    with open(config_path, 'r') as f:
+    with open(config_path, "r") as f:
         for exp_conf in yaml.load_all(f, yaml.FullLoader):
             if exp_conf is not None:
                 all_configs.append(exp_conf)
     return all_configs
 
 
-def separate_configs(all_configs: List[dict], experiment_selections: List[str],
-                     suppress: bool = False) -> Tuple[List[dict], dict, List[dict]]:
+def separate_configs(
+    all_configs: List[dict], experiment_selections: List[str], suppress: bool = False
+) -> Tuple[List[dict], dict, List[dict]]:
     """separates the list of individual configs into the 'special' SLURM, DEFAULT and normal experiment configs
 
     Arguments:
         all_configs (List[dict]): a list of all configurations
         experiment_selections (List[str], optional): List of specific experiments to run. If None runs all. Defaults to None.
 
     Returns:
@@ -77,9 +81,9 @@
     """write a yaml file
 
     Args:
         fpath : path
         data : payload
     """
     os.makedirs(os.path.dirname(fpath), exist_ok=True)
-    with open(fpath, 'w') as f:
+    with open(fpath, "w") as f:
         yaml.dump_all(data, f, default_flow_style=False)
```

### Comparing `cw2-2.2/cw2/cw_config/conf_path.py` & `cw2-2.3/cw2/cw_config/conf_path.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import os
-from typing import List, Dict, Any
+from typing import Any, Dict, List
 
 from cw2.cw_config import cw_conf_keys as KEY
 
 
-def normalize_expanded_paths(expanded_config_list: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+def normalize_expanded_paths(
+    expanded_config_list: List[Dict[str, Any]]
+) -> List[Dict[str, Any]]:
     """normalizes path key after expansion operation
 
     Args:
         expanded_config_list (List[Dict[str, Any]]): list fo expanded experiment configs
 
     Returns:
         List[Dict[str, Any]]: noramlized expanded experiment configs
     """
     # Set Path and LogPath Args depending on the name
     for _config in expanded_config_list:
-        _config[KEY.PATH] = os.path.join(_config[KEY.i_BASIC_PATH],
-                                         _config[KEY.i_NEST_DIR], _config[KEY.i_EXP_NAME])
-        _config[KEY.LOG_PATH] = os.path.join(_config[KEY.PATH], 'log')
+        _config[KEY.PATH] = os.path.join(
+            _config[KEY.i_BASIC_PATH], _config[KEY.i_NEST_DIR], _config[KEY.i_EXP_NAME]
+        )
+        _config[KEY.LOG_PATH] = os.path.join(_config[KEY.PATH], "log")
     return expanded_config_list
 
 
 def make_rel_paths(config: Dict[str, Any], base_path: str) -> Dict[str, Any]:
     """converts relevant paths of the config into relative paths
 
     Args:
@@ -29,16 +32,16 @@
         base_path (str): base path
 
     Returns:
         Dict[str, Any]: experiment config with paths relative to base_path
     """
     c = config.copy()
     _basic_path = base_path
-    c[KEY.LOG_PATH] = os.path.join(".",
-                                   os.path.relpath(c[KEY.LOG_PATH], _basic_path))
-    c[KEY.i_REP_LOG_PATH] = os.path.join(".",
-                                         os.path.relpath(c[KEY.i_REP_LOG_PATH], _basic_path))
-    c[KEY.PATH] = os.path.join(".",
-                               os.path.relpath(c[KEY.PATH], _basic_path))
-    c[KEY.i_BASIC_PATH] = os.path.join(".",
-                                       os.path.relpath(c[KEY.i_BASIC_PATH], _basic_path))
+    c[KEY.LOG_PATH] = os.path.join(".", os.path.relpath(c[KEY.LOG_PATH], _basic_path))
+    c[KEY.i_REP_LOG_PATH] = os.path.join(
+        ".", os.path.relpath(c[KEY.i_REP_LOG_PATH], _basic_path)
+    )
+    c[KEY.PATH] = os.path.join(".", os.path.relpath(c[KEY.PATH], _basic_path))
+    c[KEY.i_BASIC_PATH] = os.path.join(
+        ".", os.path.relpath(c[KEY.i_BASIC_PATH], _basic_path)
+    )
     return c
```

### Comparing `cw2-2.2/cw2/cw_config/conf_resolver.py` & `cw2-2.3/cw2/cw_config/conf_resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from cw2 import util
 from cw2.cw_config import conf_io
 from cw2.cw_config import cw_conf_keys as KEY
 from cw2.cw_error import ConfigKeyError, MissingConfigError
 
 
-def resolve_dependencies(default_config: dict, experiment_configs: List[dict], conf_path: str) -> List[dict]:
+def resolve_dependencies(
+    default_config: dict, experiment_configs: List[dict], conf_path: str
+) -> List[dict]:
     """resolves all internal (DEFAULT) and external (import) dependencies
 
     Args:
         default_config (dict): DEFAULT exp configuration
         experiment_configs (List[dict]): list of experiment configurations
         conf_path (str): path of the "calling" config file
 
@@ -43,15 +45,17 @@
     for c in experiment_configs:
         merge_c = deepcopy(default_config)
         merge_c = util.deep_update(merge_c, c)
         expanded_exp_configs.append(merge_c)
     return expanded_exp_configs
 
 
-def import_external_yml(experiment_configs: List[dict], abs_path: str, traversal_dict: dict = None) -> List[dict]:
+def import_external_yml(
+    experiment_configs: List[dict], abs_path: str, traversal_dict: dict = None
+) -> List[dict]:
     """recursively imports external yaml files
     The external yaml files are first merged with their own DEFAULT configuration,
     then their external dependencies get resolved.
 
     Args:
         experiment_configs (List[dict]): list of experiment configurations
         abs_path (str): Absolute file path of the YAML file which gets resolved..
@@ -63,17 +67,15 @@
         MissingConfigError: if the linked config cannot be found
 
     Returns:
         List[dict]: a list of resolved experiment configurations.
     """
 
     if traversal_dict is None:
-        traversal_dict = {
-            abs_path: []
-        }
+        traversal_dict = {abs_path: []}
 
     resolved_configs = []
     for config in experiment_configs:
         # SKIP
         if KEY.IMPORT_PATH not in config and KEY.IMPORT_EXP not in config:
             resolved_configs.append(config)
             continue
@@ -83,44 +85,51 @@
 
         import_yml = abs_path
         if KEY.IMPORT_PATH in config:
             import_yml = config[KEY.IMPORT_PATH]
 
         # Get absolute Path for import
         import_yml = os.path.abspath(
-            os.path.join(os.path.dirname(abs_path), import_yml))
+            os.path.join(os.path.dirname(abs_path), import_yml)
+        )
 
         all_external_configs = conf_io.read_yaml(import_yml)
 
         ext_exp_name = KEY.DEFAULT
         if custom_import_exp(config):
             ext_exp_name = config[KEY.IMPORT_EXP]
 
         # Recursion Anchor:
         if import_yml in traversal_dict and ext_exp_name in traversal_dict[import_yml]:
             raise ConfigKeyError(
-                "Cyclic YML import with {} : {}".format(import_yml, ext_exp_name))
+                "Cyclic YML import with {} : {}".format(import_yml, ext_exp_name)
+            )
 
         # Default Merge External
-        _, external, ext_selection = conf_io.separate_configs(all_external_configs, [ext_exp_name], suppress=True)
+        _, external, ext_selection = conf_io.separate_configs(
+            all_external_configs, [ext_exp_name], suppress=True
+        )
 
         if custom_import_exp(config):
             if len(ext_selection) == 0:
                 raise MissingConfigError(
-                    "Could not import {} from {}".format(ext_exp_name, import_yml))
+                    "Could not import {} from {}".format(ext_exp_name, import_yml)
+                )
 
             external = merge_default(external, ext_selection)[0]
 
         # Register new Anchor
         if import_yml not in traversal_dict:
             traversal_dict[import_yml] = []
         traversal_dict[import_yml].append(ext_exp_name)
 
         # Recursion call
-        ext_resolved_conf = import_external_yml([external], import_yml, traversal_dict)[0]
+        ext_resolved_conf = import_external_yml([external], import_yml, traversal_dict)[
+            0
+        ]
 
         # Delete Anchor when coming back
         del traversal_dict[import_yml]
 
         resolved_conf = merge_default(ext_resolved_conf, [config])[0]
         resolved_conf = archive_import_keys(resolved_conf)
         resolved_configs.append(resolved_conf)
@@ -155,8 +164,8 @@
     removal_keys = [KEY.IMPORT_PATH, KEY.IMPORT_EXP]
     replacement_keys = [KEY.i_IMPORT_PATH_ARCHIVE, KEY.i_IMPORT_EXP_ARCHIVE]
 
     for removal, replacement in zip(removal_keys, replacement_keys):
         if removal in config:
             config[replacement] = config[removal]
             del config[removal]
-    return config
+    return config
```

### Comparing `cw2-2.2/cw2/cw_config/cw_conf_keys.py` & `cw2-2.3/cw2/cw_config/cw_conf_keys.py`

 * *Files identical despite different names*

### Comparing `cw2-2.2/cw2/cw_config/cw_config.py` & `cw2-2.3/cw2/cw_config/cw_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 import os
 import socket
 from typing import List, Tuple
 
 import cw2.cw_config.cw_conf_keys as KEY
-from cw2.cw_config import conf_io, conf_resolver, conf_path, conf_unfolder
+from cw2.cw_config import conf_io, conf_path, conf_resolver, conf_unfolder
 
 
 class Config:
-    def __init__(self, config_path: str = None,
-                 experiment_selections: List[str] = None,
-                 debug: bool = False, debug_all: bool = False):
+    def __init__(
+        self,
+        config_path: str = None,
+        experiment_selections: List[str] = None,
+        debug: bool = False,
+        debug_all: bool = False,
+    ):
         self.slurm_config = None
         self.exp_configs = None
 
         self.f_name = None
         self.config_path = config_path
         self.exp_selections = experiment_selections
 
         if config_path is not None:
             self.load_config(config_path, experiment_selections, debug, debug_all)
 
-    def load_config(self,
-                    config_path: str,
-                    experiment_selections: List[str] = None,
-                    debug: bool = False,
-                    debug_all: bool = False) -> None:
+    def load_config(
+        self,
+        config_path: str,
+        experiment_selections: List[str] = None,
+        debug: bool = False,
+        debug_all: bool = False,
+    ) -> None:
         """Loads config from YAML file
         The config can include multiple experiments, DEFAULT paramters and a SLURM configuration
 
         Arguments:
             config_path {str} -- path to a YAML configuraton file
             experiment_selections (List[str], optional): List of specific experiments to run. If None runs all. Defaults to None.
         """
 
         self.config_path = config_path
         self.f_name = os.path.basename(config_path)
 
         self.exp_selections = experiment_selections
 
         slurm_configs, self.exp_configs = self._parse_configs(
-            config_path, experiment_selections, debug, debug_all)
+            config_path, experiment_selections, debug, debug_all
+        )
         self.slurm_config = self._filter_slurm_configs(slurm_configs)
 
     @staticmethod
     def _filter_slurm_configs(slurm_configs: List[dict]) -> dict:
         """Returns machine/cluster specific slurm conf (identified by hostname)
            if available, otherwise returns the default one (if available)
 
@@ -64,32 +71,41 @@
             elif c[KEY.NAME].split("_")[1].lower() in hostname:
                 print("Setting specific slurm config: {}".format(c[KEY.NAME]))
                 specific_conf = c
                 specific_conf[KEY.NAME] = KEY.SLURM
 
         return specific_conf if specific_conf is not None else default_conf
 
-    def _parse_configs(self, config_path: str, experiment_selections: List[str] = None,
-                       debug: bool = False, debug_all: bool = False) \
-            -> Tuple[List[dict], List[dict]]:
+    def _parse_configs(
+        self,
+        config_path: str,
+        experiment_selections: List[str] = None,
+        debug: bool = False,
+        debug_all: bool = False,
+    ) -> Tuple[List[dict], List[dict]]:
         """parse the config file, including separating the SLURM configuration and expanding grid / list search params
 
         Arguments:
             config_path {str} -- path to the configuration file
             experiment_selections (List[str], optional): List of specific experiments to run. If None runs all. Defaults to None.
 
         Returns:
             Tuple[dict, dict] -- SLURM configuration, list of expanded experiment configurations
         """
 
-        slurm_config, default_config, experiment_configs = conf_io.get_configs(config_path, experiment_selections)
-
-        experiment_configs = conf_resolver.resolve_dependencies(default_config, experiment_configs,
-                                                                self.config_path)
-        experiment_configs = conf_unfolder.unfold_exps(experiment_configs, debug, debug_all)
+        slurm_config, default_config, experiment_configs = conf_io.get_configs(
+            config_path, experiment_selections
+        )
+
+        experiment_configs = conf_resolver.resolve_dependencies(
+            default_config, experiment_configs, self.config_path
+        )
+        experiment_configs = conf_unfolder.unfold_exps(
+            experiment_configs, debug, debug_all
+        )
 
         return slurm_config, experiment_configs
 
     def to_yaml(self, dir_path: str = "", relpath: bool = True) -> None:
         """write config back into a YAML file.
 
         Args:
@@ -98,35 +114,41 @@
         """
 
         if dir_path == "":
             dir_path = self.exp_configs[0][KEY.i_BASIC_PATH]
 
         original_yml_name = os.path.splitext(self.f_name)[0]
 
-
         # List so it can be merged easily
         slurm_config = []
         if self.slurm_config is not None:
             slurm_config.append(dict(self.slurm_config))
 
         readable_configs = self._readable_exp_configs(relpath)
 
         # Save all named experiment configs in subdir
         grouped_configs = self._group_configs_by_name(readable_configs)
         for exp_name in grouped_configs.keys():
-            fpath = os.path.join(dir_path, exp_name, "relative_{}_{}.yml".format(
-                original_yml_name, exp_name))
+            fpath = os.path.join(
+                dir_path,
+                exp_name,
+                "relative_{}_{}.yml".format(original_yml_name, exp_name),
+            )
             conf_io.write_yaml(fpath, slurm_config + grouped_configs[exp_name])
 
         # Save global configs
         fpath = os.path.join(dir_path, "relative_" + self.f_name)
 
         if self.exp_selections is not None:
-            fpath = os.path.splitext(
-                fpath)[0] + "_" + "_".join(self.exp_selections) + ".yml"
+            fpath = (
+                os.path.splitext(fpath)[0]
+                + "_"
+                + "_".join(self.exp_selections)
+                + ".yml"
+            )
 
         # Merge into single list
         data = slurm_config + readable_configs
         conf_io.write_yaml(fpath, data)
 
     def _readable_exp_configs(self, relpath: bool = True) -> List[dict]:
         """Internal function to get more readable objects when written as yaml
```

### Comparing `cw2-2.2/cw2/cw_data/cw_loading.py` & `cw2-2.3/cw2/cw_data/cw_loading.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,36 +10,38 @@
     def run(self, overwrite: bool = False):
         cw_res = CWResult()
 
         for j in self.joblist:
             cw_res._load_job(j)
 
         cw_res._compile()
-        return cw_res.data().set_index(['name', 'r'])
+        return cw_res.data().set_index(["name", "r"])
 
 
-class CWResult():
+class CWResult:
     def __init__(self, df: pd.DataFrame = None):
         self.data_list = []
         self.df = df
 
     def _compile(self):
         self.df = pd.DataFrame(self.data_list)
         self.data_list = None
 
     def _load_job(self, j: job.Job) -> None:
         for c in j.tasks:
             rep_data = j.load_task(c)
-            rep_data.update({
-                'name': c['name'],
-                'r': c['_rep_idx'],
-                'rep_path': c['_rep_log_path'],
-                'params': c['params']
-            })
-            rep_data.update(util.flatten_dict(c['params']))
+            rep_data.update(
+                {
+                    "name": c["name"],
+                    "r": c["_rep_idx"],
+                    "rep_path": c["_rep_log_path"],
+                    "params": c["params"],
+                }
+            )
+            rep_data.update(util.flatten_dict(c["params"]))
             self.data_list.append(rep_data)
 
     def data(self) -> pd.DataFrame:
         return self.df
 
 
 @pd.api.extensions.register_dataframe_accessor("cw2")
@@ -70,30 +72,34 @@
         Args:
             r (int): repetition number
 
         Returns:
             pd.DataFrame: filtered result
         """
         df = self._obj
-        return df[df['r'] == r]
+        return df[df["r"] == r]
 
     def name(self, name: str):
         """only select experiments with a specific name
 
         Args:
             name (str): experiment name
 
         Returns:
             pd.DataFrame: filtered result
         """
         df = self._obj
-        return df[df['name'] == name]
+        return df[df["name"] == name]
 
-    def logger(self, l_name: str = "", l_obj: cw_logging.AbstractLogger = None,
-               l_cls: Type[cw_logging.AbstractLogger] = None):
+    def logger(
+        self,
+        l_name: str = "",
+        l_obj: cw_logging.AbstractLogger = None,
+        l_cls: Type[cw_logging.AbstractLogger] = None,
+    ):
         """select the column containg the results from a specific logger
 
         Args:
             l_name (str, optional): the class name of the logger. Defaults to "".
             l_obj (cw_logging.AbstractLogger, optional): an instance object of the logger. Defaults to None.
             l_cls (Type[cw_logging.AbstractLogger], optional): the class object of the logger. Defaults to None.
 
@@ -122,11 +128,11 @@
             outer_row = row.drop(pd_log_col)
             for c, v in outer_row.iteritems():
                 if isinstance(v, dict):
                     nested_df[c] = str(v)
                     nested_df[c] = nested_df[c].map(eval)
                     continue
                 nested_df[c] = v
-            nested_df['name'] = idx[0]
-            nested_df['r'] = idx[1]
+            nested_df["name"] = idx[0]
+            nested_df["r"] = idx[1]
             new_df = new_df.append(nested_df, ignore_index=True)
-        return new_df.set_index(['name', 'r', 'iter'])
+        return new_df.set_index(["name", "r", "iter"])
```

### Comparing `cw2-2.2/cw2/cw_data/cw_logging.py` & `cw2-2.3/cw2/cw_data/cw_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import abc
 import logging
 import os
 import pprint
 import sys
-from typing import Iterable, Optional, Dict, List
+from typing import Dict, Iterable, List, Optional
 
 
 class AbstractLogger(abc.ABC):
-    """Abstract Base Class for all Loggers
-    """
+    """Abstract Base Class for all Loggers"""
 
-    def __init__(self, ignore_keys: Optional[Iterable] = None, allow_keys: Optional[Iterable] = None):
+    def __init__(
+        self,
+        ignore_keys: Optional[Iterable] = None,
+        allow_keys: Optional[Iterable] = None,
+    ):
         """
         Initialize a logger that records based on (a subset of) the provided keys
         :param ignore_keys: A list of keys
         :param allow_keys:
         """
-        assert ignore_keys is None or allow_keys is None, \
-            "Logging keys can either be whitelisted ('ignore_keys') or blacklisted ('allow_keys'), but not both"
+        assert (
+            ignore_keys is None or allow_keys is None
+        ), "Logging keys can either be whitelisted ('ignore_keys') or blacklisted ('allow_keys'), but not both"
         self.ignore_keys = ignore_keys
         self.allow_keys = allow_keys
 
     def filter(self, data: Dict) -> Dict:
         """
         Base Function. Either filters out ignored keys or looks for allowed ones
 
         Args:
             data: data payload dict
         """
         if self.ignore_keys is not None:  # blacklist ignored keys
-            return {key: value for key, value in data.items() if key not in self.ignore_keys}
+            return {
+                key: value for key, value in data.items() if key not in self.ignore_keys
+            }
         elif self.allow_keys is not None:  # whitelist allowed keys
             return {key: value for key, value in data.items() if key in self.allow_keys}
         else:  # use all keys
             return data
 
     def preprocess(self, *args):
         """
@@ -126,16 +132,15 @@
         return iter(self._logger_array)
 
     def is_empty(self) -> bool:
         return len(self._logger_array) == 0
 
 
 class Printer(AbstractLogger):
-    """Prints the result of each iteration to the console.
-    """
+    """Prints the result of each iteration to the console."""
 
     def initialize(self, config: dict, rep: int, rep_log_path: str) -> None:
         pass
 
     def process(self, data: dict) -> None:
         data_ = self.filter(data)
         pprint.pprint(data_)
@@ -152,20 +157,22 @@
     Logger which writes calls to logging.getLogger('cw2') on to disk
     """
 
     def __init__(self):
         self.logger = getLogger()
 
     def initialize(self, config: dict, rep: int, rep_log_path: str) -> None:
-        self.outh = logging.FileHandler(os.path.join(rep_log_path, 'out.log'), delay=True)
+        self.outh = logging.FileHandler(
+            os.path.join(rep_log_path, "out.log"), delay=True
+        )
         self.outh.setLevel(logging.INFO)
         self.outh.setFormatter(_formatter)
         self.logger.addHandler(self.outh)
 
-        self.errh = logging.FileHandler(os.path.join(rep_log_path, 'err.log'))
+        self.errh = logging.FileHandler(os.path.join(rep_log_path, "err.log"))
         self.errh.setLevel(logging.ERROR)
         self.errh.setFormatter(_formatter)
         self.logger.addHandler(self.errh)
 
     def process(self, data: dict) -> None:
         pass
 
@@ -177,23 +184,24 @@
 
     def load(self):
         pass
 
 
 ### logging module functionality ####
 
+
 class _CWFormatter(logging.Formatter):
-    """Taken From CW V1
-    """
+    """Taken From CW V1"""
 
     def __init__(self):
         # self.std_formatter = logging.Formatter('[%(asctime)s] [%(name)s] [%(levelname)s] %(message)s')
-        self.std_formatter = logging.Formatter('[%(name)s] [%(levelname)s] %(message)s')
+        self.std_formatter = logging.Formatter("[%(name)s] [%(levelname)s] %(message)s")
         self.red_formatter = logging.Formatter(
-            '[%(asctime)s]:[%(name)s] [%(levelname)s] %(message)s')
+            "[%(asctime)s]:[%(name)s] [%(levelname)s] %(message)s"
+        )
 
     def format(self, record: logging.LogRecord):
         if record.levelno < logging.ERROR:
             return self.std_formatter.format(record)
         else:
             return self.red_formatter.format(record)
 
@@ -204,15 +212,15 @@
 def getLogger() -> logging.Logger:
     """creates a logging.getLogger('cw2') object with initialization.
     Parallelization via joblib needs a more sophisticated getLogger function.
 
     Returns:
         logging.Logger
     """
-    _logging_logger = logging.getLogger('cw2')
+    _logging_logger = logging.getLogger("cw2")
 
     if _logging_logger.getEffectiveLevel() > logging.INFO:
         ch = logging.StreamHandler(sys.stdout)
         ch.setLevel(logging.INFO)
         ch.setFormatter(_formatter)
 
         _logging_logger.setLevel(logging.INFO)
```

### Comparing `cw2-2.2/cw2/cw_data/cw_pd_logger.py` & `cw2-2.3/cw2/cw_data/cw_pd_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import os
+from typing import Dict, Iterable, Optional
 
 import pandas as pd
 
 from cw2.cw_data import cw_logging
-from typing import Optional, Iterable, Dict
 
 
 class PandasLogger(cw_logging.AbstractLogger):
     """Writes the results of each repetition seperately to disk
     Each repetition is saved in its own directory. Write occurs after every iteration.
     """
 
-    def __init__(self, ignore_keys: Optional[Iterable] = None, allow_keys: Optional[Iterable] = None):
+    def __init__(
+        self,
+        ignore_keys: Optional[Iterable] = None,
+        allow_keys: Optional[Iterable] = None,
+    ):
         super().__init__(ignore_keys=ignore_keys, allow_keys=allow_keys)
         self.log_path = ""
         self.csv_name = "rep.csv"
         self.pkl_name = "rep.pkl"
         self.df = pd.DataFrame()
 
     def initialize(self, config: Dict, rep: int, rep_log_path: str):
         self.log_path = rep_log_path
-        self.csv_name = os.path.join(self.log_path, 'rep_{}.csv'.format(rep))
-        self.pkl_name = os.path.join(self.log_path, 'rep_{}.pkl'.format(rep))
+        self.csv_name = os.path.join(self.log_path, "rep_{}.csv".format(rep))
+        self.pkl_name = os.path.join(self.log_path, "rep_{}.pkl".format(rep))
         self.df = pd.DataFrame()
 
     def process(self, log_data: dict) -> None:
         data = self.filter(log_data)
 
         self.df = self.df.append(data, ignore_index=True)
 
         try:
-            self.df.to_csv(self.csv_name, index_label='index')
+            self.df.to_csv(self.csv_name, index_label="index")
         except:
-            cw_logging.getLogger().warning('Could not save {}'.format(self.csv_name))
+            cw_logging.getLogger().warning("Could not save {}".format(self.csv_name))
 
         try:
             self.df.to_pickle(self.pkl_name)
         except:
-            cw_logging.getLogger().warning('Could not save {}'.format(self.pkl_name))
+            cw_logging.getLogger().warning("Could not save {}".format(self.pkl_name))
 
     def finalize(self) -> None:
         pass
 
     def load(self):
         payload = {}
         df: pd.DataFrame = None
```

### Comparing `cw2-2.2/cw2/cw_data/cw_wandb_logger.py` & `cw2-2.3/cw2/cw_data/cw_wandb_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import warnings
-from time import sleep
 from random import random
+from time import sleep
 
 # To prevent conflicts between wandb and the joblib scheduler
 # see https://github.com/wandb/client/issues/1525 for reference
 os.environ["WANDB_START_METHOD"] = "thread"
 
-import wandb
-from typing import Optional, Iterable, List, Dict
 from itertools import groupby
+from typing import Dict, Iterable, List, Optional
+
 import pandas as pd
+import wandb
 
 from cw2.cw_data import cw_logging
 from cw2.util import get_file_names_in_directory
 
 
 def reset_wandb_env():
     exclude = {
@@ -25,15 +26,15 @@
     }
     for k, v in os.environ.items():
         if k.startswith("WANDB_") and k not in exclude:
             del os.environ[k]
 
 
 def group_parameters(list_of_strings: List[str]):
-    """ groups different strings that start with a common substring (using "." as delimiter)
+    """groups different strings that start with a common substring (using "." as delimiter)
         and outputs a single, more concise string.
     Example:
         outstring = group_parameters['local', 'mod.enc.tidentity', 'mod.hea.nhl5', 'mod.hea.ioFalse', 'mod.enc.hd64']
         % outstring will be 'local,mod_[enc_[hd64,tidentity],hea_[ioFalse,nhl5]]'
     """
     groups = []
     uniquekeys = []
@@ -57,43 +58,48 @@
                 else:
                     substring += k + "_" + subgroups + ","
                 num_subgroups += num_subs
     return substring[:-1], len(groups)
 
 
 class WandBLogger(cw_logging.AbstractLogger):
-
-    def __init__(self, ignore_keys: Optional[Iterable] = None, allow_keys: Optional[Iterable] = None):
-        super(WandBLogger, self).__init__(ignore_keys=ignore_keys, allow_keys=allow_keys)
+    def __init__(
+        self,
+        ignore_keys: Optional[Iterable] = None,
+        allow_keys: Optional[Iterable] = None,
+    ):
+        super(WandBLogger, self).__init__(
+            ignore_keys=ignore_keys, allow_keys=allow_keys
+        )
         self.log_path = ""
         self.run = None
 
     def initialize(self, config: Dict, rep: int, rep_log_path: str) -> None:
         if "wandb" in config.keys():
             self.init_fields(config, rep, rep_log_path)
             self.connect_to_wandb()
 
         else:
             warnings.warn("No 'wandb' field in yaml - Ignoring Weights & Biases Logger")
 
-    def init_fields(self,  config: Dict, rep: int, rep_log_path: str):
+    def init_fields(self, config: Dict, rep: int, rep_log_path: str):
         self.log_path = rep_log_path
         self.rep = rep
-        self.config = config['wandb']
+        self.config = config["wandb"]
         self.cw2_config = config
         reset_wandb_env()
-        self.job_name = config['_experiment_name'].replace("__", "_")
+        self.job_name = config["_experiment_name"].replace("__", "_")
         self.use_group_parameters = self.config.get("use_group_parameters", False)
         if self.use_group_parameters:
             self.job_name = group_parameters(self.job_name.split("_"))[0]
         self.runname = self.job_name + "_rep_{:02d}".format(rep)
 
         # optional: change the job_type to a fixed alias if the option is present
         if "job_type" in self.config:
-            self.job_name = self.config['job_type']
+            self.job_name = self.config["job_type"]
         # have entity and group config entry optional
         self.entity = self.config.get("entity", None)
         self.group = self.config.get("group", None)
         # Get the model logging directory
         self.wandb_log_model = self.config.get("log_model", False)
         if self.wandb_log_model:
             self.save_model_dir = os.path.join(self.log_path, "model")
@@ -101,51 +107,62 @@
             self.model_name = self.config.get("model_name", "model")
         else:
             self.save_model_dir = None
 
     def connect_to_wandb(self):
         last_error = None
         for i in range(10):
-
             try:
-                self.run = wandb.init(project=self.cw2_config['wandb']['project'],
-                                      entity=self.entity,
-                                      group=self.group,
-                                      job_type=self.job_name[:63],
-                                      name=self.runname[:63],
-                                      config=self.cw2_config['params'],
-                                      dir=self.log_path,
-                                      settings=wandb.Settings(_disable_stats=self.cw2_config['wandb'].get("disable_stats",
-                                                                                              False)),
-                                      mode="online" if self.cw2_config['wandb'].get("enabled", True) else "disabled",
-                                      )
+                self.run = wandb.init(
+                    project=self.cw2_config["wandb"]["project"],
+                    entity=self.entity,
+                    group=self.group,
+                    job_type=self.job_name[:63],
+                    name=self.runname[:63],
+                    config=self.cw2_config["params"],
+                    dir=self.log_path,
+                    settings=wandb.Settings(
+                        _disable_stats=self.cw2_config["wandb"].get(
+                            "disable_stats", False
+                        )
+                    ),
+                    mode="online"
+                    if self.cw2_config["wandb"].get("enabled", True)
+                    else "disabled",
+                )
                 return  # if starting the run is successful, exit the loop (and in this case the function)
             except Exception as e:
                 last_error = e
                 # implement a simple randomized exponential backoff if starting a run fails
-                waiting_time = ((random() / 50) + 0.01) * (2 ** i)
+                waiting_time = ((random() / 50) + 0.01) * (2**i)
                 # wait between 0.01 and 10.24 seconds depending on the random seed and the iteration of the exponent
 
-                warnings.warn("Problem with starting wandb: {}. Trying again in {} seconds".format(e, waiting_time))
+                warnings.warn(
+                    "Problem with starting wandb: {}. Trying again in {} seconds".format(
+                        e, waiting_time
+                    )
+                )
                 sleep(waiting_time)
         warnings.warn("wandb init failed several times.")
         raise last_error
 
     def process(self, data: dict) -> None:
         if self.run is not None:
-
             # Skip logging if interval is defined but not satisfied
             log_interval = self.config.get("log_interval", None)
             if log_interval is not None and data["iter"] % log_interval != 0:
                 return
 
             if "histogram" in self.config:
-                for el in self.config['histogram']:
+                for el in self.config["histogram"]:
                     if el in data:
-                        self.run.log({el: wandb.Histogram(np_histogram=data[el])}, step=data["iter"])
+                        self.run.log(
+                            {el: wandb.Histogram(np_histogram=data[el])},
+                            step=data["iter"],
+                        )
             filtered_data = self.filter(data)
             step = data.get("iter", None)
             self.run.log(filtered_data, step=step)
 
     def finalize(self) -> None:
         if self.run is not None:
             self.log_model()
@@ -181,14 +198,20 @@
         aliases = ["latest", f"finished-rep-{self.rep}"]
 
         # Log and upload
         self.run.log_artifact(model_artifact, aliases=aliases)
 
     def log_plot(self, x, y, column_names=("x", "y"), plot_id="plot", title="Plot"):
         data = [list(i) for i in zip(x, y)]
-        table = wandb.Table(data=data, columns = column_names)
-        self.run.log({plot_id : wandb.plot.line(table, column_names[0], column_names[0], title=title)})
-        
-    def log_table(self, data, table_id='table'):
+        table = wandb.Table(data=data, columns=column_names)
+        self.run.log(
+            {
+                plot_id: wandb.plot.line(
+                    table, column_names[0], column_names[0], title=title
+                )
+            }
+        )
+
+    def log_table(self, data, table_id="table"):
         assert type(data) is pd.DataFrame
         table = wandb.Table(dataframe=data)
         self.run.log({table_id: table})
```

### Comparing `cw2-2.2/cw2/cw_error.py` & `cw2-2.3/cw2/cw_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 class ConfigKeyError(Exception):
     """raised when a key is missing in the configuration."""
+
     pass
 
 
 class MissingConfigError(Exception):
     """raise when a config document is missing in the configuration."""
+
     pass
 
 
 class ExperimentNotFoundError(Exception):
     """raise when experiment selection could not be found in the configuration"""
+
     pass
 
 
 class ExperimentSurrender(Exception):
     def __init__(self, payload: dict = None):
         if payload is None:
             payload = {}
```

### Comparing `cw2-2.2/cw2/cw_slurm/cw_slurm.py` & `cw2-2.3/cw2/cw_slurm/cw_slurm.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,48 +2,50 @@
 import os
 import shutil
 import subprocess
 import sys
 
 import __main__
 
+import cw2.cw_config.cw_conf_keys as CKEYS
+import cw2.cw_slurm.cw_slurm_keys as SKEYS
 from cw2 import cli_parser, cw_error, util
 from cw2.cw_config import cw_config
 from cw2.cw_data import cw_logging
-import cw2.cw_slurm.cw_slurm_keys as SKEYS
-import cw2.cw_config.cw_conf_keys as CKEYS
 
 
 class SlurmConfig:
     def __init__(self, conf: cw_config.Config) -> None:
         self.conf = conf
         self.slurm_conf = conf.slurm_config
 
         if self.slurm_conf is None:
             raise cw_error.MissingConfigError(
-                "No SLURM configuration found in {}".format(self.conf.config_path))
+                "No SLURM configuration found in {}".format(self.conf.config_path)
+            )
 
         self._check_template()
 
     def _check_template(self):
         """check if an sbatch.sh template is present.
         If no costum template has been specified, the default will be used.
         """
 
         if SKEYS.TEMPLATE_PATH not in self.slurm_conf:
             self.slurm_conf[SKEYS.TEMPLATE_PATH] = os.path.join(
-                os.path.dirname(__file__), '../default_sbatch.sh')
+                os.path.dirname(__file__), "../default_sbatch.sh"
+            )
 
         if not os.path.exists(self.slurm_conf[SKEYS.TEMPLATE_PATH]):
             raise cw_error.ConfigKeyError(
-                "Could not find default sbatch template. Please specify your own 'path_to_template'.")
+                "Could not find default sbatch template. Please specify your own 'path_to_template'."
+            )
 
     def _complete_optionals(self):
-        """Fill in any optional values.
-        """
+        """Fill in any optional values."""
 
         sc: dict = self.slurm_conf
 
         exp_output_path = self.conf.exp_configs[0][CKEYS.i_BASIC_PATH]
 
         # CREATE OPTIONAL COLLECTIONS
         # Must be done first:
@@ -52,16 +54,17 @@
         # SET DEFAULT VALUES
         sc.setdefault(SKEYS.SLURM_LOG, os.path.join(exp_output_path, "slurmlog"))
         sc.setdefault(SKEYS.SLURM_OUT, os.path.join(exp_output_path, "sbatch.sh"))
         sc.setdefault(SKEYS.ACCOUNT, "")
 
         # COMPLEX CONVERSIONS
         if isinstance(sc[SKEYS.TIME], int):
-            sc[SKEYS.TIME] = '{:d}:{:d}:00'.format(
-                sc[SKEYS.TIME] // 60, sc[SKEYS.TIME] % 60)
+            sc[SKEYS.TIME] = "{:d}:{:d}:00".format(
+                sc[SKEYS.TIME] // 60, sc[SKEYS.TIME] % 60
+            )
 
         if SKEYS.CPU_MEM in sc:
             sc[SKEYS.SBATCH_ARGS][SKEYS.CPU_MEM] = sc.get(SKEYS.CPU_MEM)
 
         # DEFAULT OR COMPLEX CONVERSION
         if SKEYS.VENV in sc:
             sc[SKEYS.VENV] = "source activate {}".format(sc[SKEYS.VENV])
@@ -70,38 +73,35 @@
 
         if SKEYS.SH_LINES in sc:
             sc[SKEYS.SH_LINES] = "\n".join(sc[SKEYS.SH_LINES])
         else:
             sc[SKEYS.SH_LINES] = ""
 
     def _complete_cli_args(self):
-        """identify and process the relevant CLI flags from the original call.
-        """
+        """identify and process the relevant CLI flags from the original call."""
         sc = self.slurm_conf
         cw_options = cli_parser.Arguments().get()
 
         sc[SKEYS.CW_ARGS] = ""
-        if cw_options['overwrite']:
+        if cw_options["overwrite"]:
             sc[SKEYS.CW_ARGS] += " -o"
-        if cw_options['experiments'] is not None:
+        if cw_options["experiments"] is not None:
             sc[SKEYS.CW_ARGS] += " -e " + " ".join(cw_options["experiments"])
 
     def _complete_sbatch_args(self):
-        """if optional SBATCH arguments are present, build a corresponding string.
-        """
+        """if optional SBATCH arguments are present, build a corresponding string."""
         sc = self.slurm_conf
 
         if SKEYS.SBATCH_ARGS not in sc:  # Check if empty
             sc[SKEYS.SBATCH_ARGS] = ""
             return
         else:  # Else build String
             sbatch_args = sc.get(SKEYS.SBATCH_ARGS)
 
-            args_list = ["#SBATCH --{} {}".format(k, v)
-                         for k, v in sbatch_args.items()]
+            args_list = ["#SBATCH --{} {}".format(k, v) for k, v in sbatch_args.items()]
             sc[SKEYS.SBATCH_ARGS] = "\n".join(args_list)
 
     def finalize(self, num_jobs: int):
         """enrich slurm configuration with dynamically computed values
 
         Args:
             num_jobs (int): total number of defined jobs
@@ -149,26 +149,30 @@
         if SKEYS.EXP_CP_SRC not in sc:
             cp_error_count += 1
             missing_arg = SKEYS.EXP_CP_SRC
 
         # MODE SWITCH
         if cp_error_count == 1:
             raise cw_error.ConfigKeyError(
-                "Incomplete SLURM experiment copy config. Missing key: {}".format(missing_arg))
+                "Incomplete SLURM experiment copy config. Missing key: {}".format(
+                    missing_arg
+                )
+            )
 
         cw_options = cli_parser.Arguments().get()
-        if cw_options.get('zip'):
+        if cw_options.get("zip"):
             return self.MODE_ZIP
 
-        if cw_options.get('multicopy'):
+        if cw_options.get("multicopy"):
             if cp_error_count == 0:
                 return self.MODE_MULTI
             else:
                 raise cw_error.ConfigKeyError(
-                    "Incomplete SLURM experiment copy config. Please define SRC and DST for --multicopy")
+                    "Incomplete SLURM experiment copy config. Please define SRC and DST for --multicopy"
+                )
 
         if cp_error_count == 0:
             return self.MODE_COPY
         return self.MODE_NOCOPY
 
     def dir_size_validation(self, src):
         """validates that the SRC for code copy is below 200MB in size
@@ -176,23 +180,27 @@
         Args:
             src: src path
 
         Raises:
             cw_error.ConfigKeyError: if directory is greater than 200MB
         """
         cw_options = cli_parser.Arguments().get()
-        if cw_options.get('skipsizecheck'):
+        if cw_options.get("skipsizecheck"):
             return
 
         dirsize = util.get_size(src)
         if dirsize > 200.0:
-            cw_logging.getLogger().warning("SourceDir {} is greater than 200MByte".format(src))
-            msg = "Directory {} is greater than 200MByte." \
-                  " If you are sure you want to copy/zip this dir, use --skipsizecheck." \
-                  "\nElse check experiment_copy__ configuration keys".format(src)
+            cw_logging.getLogger().warning(
+                "SourceDir {} is greater than 200MByte".format(src)
+            )
+            msg = (
+                "Directory {} is greater than 200MByte."
+                " If you are sure you want to copy/zip this dir, use --skipsizecheck."
+                "\nElse check experiment_copy__ configuration keys".format(src)
+            )
             raise cw_error.ConfigKeyError(msg)
 
     def get_exp_src(self) -> str:
         """retrieves the code-copy src.
         Uses CWD as default unless specified
 
         Returns:
@@ -206,34 +214,34 @@
         Uses CWD as default unless specified
 
         Returns:
             src path
         """
         sc = self.slurm_config.slurm_conf
         if SKEYS.EXP_CP_AUTO in sc and SKEYS.EXP_CP_DST not in sc:
-            sc[SKEYS.EXP_CP_DST] = os.path.join(sc.get(SKEYS.EXP_CP_AUTO),
-                                                datetime.datetime.now().strftime("%Y%m%d%G%M%S"))
+            sc[SKEYS.EXP_CP_DST] = os.path.join(
+                sc.get(SKEYS.EXP_CP_AUTO),
+                datetime.datetime.now().strftime("%Y%m%d%G%M%S"),
+            )
         if SKEYS.EXP_CP_DST in sc:
             return sc[SKEYS.EXP_CP_DST]
         else:
             exp_output_path = self.conf.exp_configs[0][CKEYS.i_BASIC_PATH]
-            return os.path.join(exp_output_path, 'code')
+            return os.path.join(exp_output_path, "code")
 
     def zip_exp(self):
-        """procedure for creating a zip backup
-        """
+        """procedure for creating a zip backup"""
         src = self.get_exp_src()
         dst = self.get_exp_dst()
         self.dir_size_validation(src)
 
-        shutil.make_archive(dst, 'zip', src)
+        shutil.make_archive(dst, "zip", src)
 
     def create_single_copy(self):
-        """creates a copy of the exp for slurm execution
-        """
+        """creates a copy of the exp for slurm execution"""
         src = self.get_exp_src()
         dst = self.get_exp_dst()
         self._copy_files(src, dst)
 
     def create_multi_copy(self, num_jobs: int):
         """creates multiple copies of the exp, one for each slurm job
 
@@ -244,16 +252,17 @@
         dst_base = self.get_exp_dst()
 
         for i in range(num_jobs):
             dst = os.path.join(dst_base, str(i))
             self._copy_files(src, dst)
 
         # Add MultiCopy ChangeDir to Slurmconf
-        self.slurm_config.slurm_conf[SKEYS.SH_LINES] += "\ncd {} \n".format(os.path.join(self.get_exp_dst(),
-                                                                                         "$SLURM_ARRAY_TASK_ID"))
+        self.slurm_config.slurm_conf[SKEYS.SH_LINES] += "\ncd {} \n".format(
+            os.path.join(self.get_exp_dst(), "$SLURM_ARRAY_TASK_ID")
+        )
 
     def _copy_files(self, src, dst):
         """copies files from src to dst
 
         Args:
             src: source directory
             dst: destination directory
@@ -263,24 +272,25 @@
             cw_error.ConfigKeyError: if the dst already exists and overwrite is not forced.
         """
         self.dir_size_validation(src)
 
         # Check Filesystem
         if util.check_subdir(src, dst):
             raise cw_error.ConfigKeyError(
-                "experiment_copy_dst is a subdirectory of experiment_copy_src. Recursive Copying is bad.")
+                "experiment_copy_dst is a subdirectory of experiment_copy_src. Recursive Copying is bad."
+            )
         try:
-            os.makedirs(
-                dst, exist_ok=cli_parser.Arguments().get()['overwrite'])
+            os.makedirs(dst, exist_ok=cli_parser.Arguments().get()["overwrite"])
         except FileExistsError:
             raise cw_error.ConfigKeyError(
-                "{} already exists. Please define a different 'experiment_copy_dst', use '-o' to overwrite or '--nocodecopy' to skip.")
+                "{} already exists. Please define a different 'experiment_copy_dst', use '-o' to overwrite or '--nocodecopy' to skip."
+            )
 
         # Copy files
-        ign = shutil.ignore_patterns('*.pyc', 'tmp*', '.git*')
+        ign = shutil.ignore_patterns("*.pyc", "tmp*", ".git*")
         for item in os.listdir(src):
             s = os.path.join(src, item)
             d = os.path.join(dst, item)
             if os.path.isdir(s):
                 shutil.copytree(s, d, ignore=ign)
             else:
                 shutil.copy2(s, d)
@@ -288,16 +298,16 @@
     def move_files(self, num_jobs: int):
         """moves exp files according to detected copy mode
         Args:
             num_jobs: number of slurm jobs for multi-copy
         """
         # Check Skip Flag
         cw_options = cli_parser.Arguments().get()
-        if cw_options.get('nocodecopy'):
-            print('Skipping Code Copy')
+        if cw_options.get("nocodecopy"):
+            print("Skipping Code Copy")
             return
 
         if self.m == self.MODE_COPY:
             self.create_single_copy()
 
         if self.m == self.MODE_MULTI:
             self.create_multi_copy(num_jobs)
@@ -330,16 +340,17 @@
 
         src = self.get_exp_src()
         dst = self.get_exp_dst()
 
         if self.m == self.MODE_MULTI:
             dst = os.path.join(dst, "$SLURM_ARRAY_TASK_ID")
 
-        new_path = [x.replace(os.path.abspath(src), os.path.abspath(dst))
-                    for x in pypath]
+        new_path = [
+            x.replace(os.path.abspath(src), os.path.abspath(dst)) for x in pypath
+        ]
         # return "export PYTHONPATH=" + ":".join(new_path)
         # Maybe this is better?
         return "export PYTHONPATH=$PYTHONPATH:" + ":".join(new_path)
 
 
 def run_slurm(conf: cw_config.Config, num_jobs: int) -> None:
     """starts slurm execution
@@ -376,49 +387,49 @@
     conf = slurm_conf.conf
 
     template_path = sc[SKEYS.TEMPLATE_PATH]
     output_path = sc[SKEYS.SLURM_OUT]
 
     exp_main_file = os.path.relpath(__main__.__file__, os.getcwd())
 
-    fid_in = open(template_path, 'r')
-    fid_out = open(output_path, 'w')
+    fid_in = open(template_path, "r")
+    fid_out = open(output_path, "w")
 
     tline = fid_in.readline()
 
     while tline:
-        tline = tline.replace('%%partition%%', sc['partition'])
-        tline = tline.replace('%%account%%', sc[SKEYS.ACCOUNT])
-        tline = tline.replace('%%job-name%%', sc['job-name'])
+        tline = tline.replace("%%partition%%", sc["partition"])
+        tline = tline.replace("%%account%%", sc[SKEYS.ACCOUNT])
+        tline = tline.replace("%%job-name%%", sc["job-name"])
 
-        tline = tline.replace('%%last_job_idx%%',
-                              '{:d}'.format(sc[SKEYS.LAST_IDX]))
-        tline = tline.replace('%%num_parallel_jobs%%',
-                              '{:d}'.format(sc['num_parallel_jobs']))
+        tline = tline.replace("%%last_job_idx%%", "{:d}".format(sc[SKEYS.LAST_IDX]))
+        tline = tline.replace(
+            "%%num_parallel_jobs%%", "{:d}".format(sc["num_parallel_jobs"])
+        )
 
-        tline = tline.replace('%%experiment_execution_dir%%',
-                              dir_mgr.get_exp_exec_dir())
+        tline = tline.replace(
+            "%%experiment_execution_dir%%", dir_mgr.get_exp_exec_dir()
+        )
 
-        tline = tline.replace('%%slurm_log%%', sc[SKEYS.SLURM_LOG])
+        tline = tline.replace("%%slurm_log%%", sc[SKEYS.SLURM_LOG])
 
-        tline = tline.replace('%%ntasks%%', '{:d}'.format(sc['ntasks']))
-        tline = tline.replace('%%cpus-per-task%%',
-                              '{:d}'.format(sc['cpus-per-task']))
-        tline = tline.replace('%%time%%', sc[SKEYS.TIME])
+        tline = tline.replace("%%ntasks%%", "{:d}".format(sc["ntasks"]))
+        tline = tline.replace("%%cpus-per-task%%", "{:d}".format(sc["cpus-per-task"]))
+        tline = tline.replace("%%time%%", sc[SKEYS.TIME])
 
-        tline = tline.replace('%%sh_lines%%', sc[SKEYS.SH_LINES])
+        tline = tline.replace("%%sh_lines%%", sc[SKEYS.SH_LINES])
 
-        tline = tline.replace('%%venv%%', sc[SKEYS.VENV])
-        tline = tline.replace('%%pythonpath%%', dir_mgr.get_py_path())
+        tline = tline.replace("%%venv%%", sc[SKEYS.VENV])
+        tline = tline.replace("%%pythonpath%%", dir_mgr.get_py_path())
 
-        tline = tline.replace('%%python_script%%', exp_main_file)
-        tline = tline.replace('%%path_to_yaml_config%%', conf.config_path)
+        tline = tline.replace("%%python_script%%", exp_main_file)
+        tline = tline.replace("%%path_to_yaml_config%%", conf.config_path)
 
-        tline = tline.replace('%%cw_args%%', sc[SKEYS.CW_ARGS])
-        tline = tline.replace('%%sbatch_args%%', sc[SKEYS.SBATCH_ARGS])
+        tline = tline.replace("%%cw_args%%", sc[SKEYS.CW_ARGS])
+        tline = tline.replace("%%sbatch_args%%", sc[SKEYS.SBATCH_ARGS])
 
         fid_out.write(tline)
 
         tline = fid_in.readline()
     fid_in.close()
     fid_out.close()
-    return output_path
+    return output_path
```

### Comparing `cw2-2.2/cw2/default_sbatch.sh` & `cw2-2.3/cw2/default_sbatch.sh`

 * *Files identical despite different names*

### Comparing `cw2-2.2/cw2/experiment.py` & `cw2-2.3/cw2/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 from cw2.cw_data import cw_logging
 from cw2.cw_error import ExperimentSurrender
 
 
 class AbstractExperiment(abc.ABC):
     @abc.abstractmethod
-    def initialize(self, cw_config: dict, rep: int, logger: cw_logging.LoggerArray) -> None:
+    def initialize(
+        self, cw_config: dict, rep: int, logger: cw_logging.LoggerArray
+    ) -> None:
         """needs to be implemented by subclass.
         Called once at the start of each repition for initialization purposes.
 
         Arguments:
             cw_config {dict} -- clusterwork experiment configuration
             rep {int} -- repition counter
             logger {cw_logging.LoggerArray} -- initialized loggers for preprocessing
```

### Comparing `cw2-2.2/cw2/job.py` & `cw2-2.3/cw2/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,95 +1,103 @@
 import os
-from typing import List, Type, Dict
+from typing import Dict, List, Type
 
 from cw2 import cw_error, experiment
 from cw2.cw_config import cw_conf_keys as KEYS
 from cw2.cw_data import cw_logging
 
 
-class Job():
+class Job:
     """Class defining a computation job.
     Can contain 1..n tasks. Each job should encapsulate all information necessary for execution.
     A task is an experiment configuration with unique repetition idx.
     """
 
-    def __init__(self, tasks: List[Dict], exp_cls: experiment.AbstractExperiment.__class__,
-                 logger: cw_logging.AbstractLogger, delete_old_files: bool = False, root_dir: str = "",
-                 read_only: bool = False):
+    def __init__(
+        self,
+        tasks: List[Dict],
+        exp_cls: experiment.AbstractExperiment.__class__,
+        logger: cw_logging.AbstractLogger,
+        delete_old_files: bool = False,
+        root_dir: str = "",
+        read_only: bool = False,
+    ):
         self.tasks = tasks
 
         if exp_cls is not None:
             self.exp = exp_cls()
         self.logger = logger
 
         self.n_parallel = 1
         if KEYS.REPS_PARALL in tasks[0]:
             self.n_parallel = tasks[0][KEYS.REPS_PARALL]
 
         self._root_dir = root_dir
 
         if not read_only:
-            self.__create_experiment_directory(
-                tasks, delete_old_files, root_dir)
+            self.__create_experiment_directory(tasks, delete_old_files, root_dir)
 
-    def __create_experiment_directory(self, tasks: List[Dict], delete_old_files=False, root_dir=""):
+    def __create_experiment_directory(
+        self, tasks: List[Dict], delete_old_files=False, root_dir=""
+    ):
         """internal function creating the directories in which the job will write its data.
 
         Args:
             task (List[attrdict.Attrdict]): a list of experiment tasks
             delete_old_files (bool, optional): Should the directory be emptied beforehand?. Defaults to False.
             root_dir (str, optional): [description]. Defaults to "".
         """
         for conf in tasks:
             # create experiment path and subdir
             os.makedirs(os.path.join(root_dir, conf[KEYS.PATH]), exist_ok=True)
 
             # create a directory for the log path
-            os.makedirs(os.path.join(
-                root_dir, conf[KEYS.LOG_PATH]), exist_ok=True)
+            os.makedirs(os.path.join(root_dir, conf[KEYS.LOG_PATH]), exist_ok=True)
 
             # create log path for each repetition
-            rep_path = os.path.join(
-                root_dir, conf[KEYS.i_REP_LOG_PATH])
+            rep_path = os.path.join(root_dir, conf[KEYS.i_REP_LOG_PATH])
 
             # XXX: Disable Delete for now
             """
             if delete_old_files:
                 pass
             """
             os.makedirs(rep_path, exist_ok=True)
 
     def run_task(self, c: Dict, overwrite: bool):
-        """Execute a single task of the job. 
+        """Execute a single task of the job.
 
         Args:
             c (attrdict.AttrDict): task configuration
         """
         rep_path = c[KEYS.i_REP_LOG_PATH]
         r = c[KEYS.i_REP_IDX]
         print(rep_path)
 
         if not overwrite and self._check_task_exists(c, r):
             cw_logging.getLogger().warning(
-                "Skipping run, as {} is not empty. Use -o to overwrite.".format(rep_path))
+                "Skipping run, as {} is not empty. Use -o to overwrite.".format(
+                    rep_path
+                )
+            )
             return
 
         surrender = None
         crash = False
 
         self.logger.initialize(c, r, rep_path)
         try:
             self.exp.initialize(c, r, self.logger)
             self.exp.run(c, r, self.logger)
         except cw_error.ExperimentSurrender as s:
-            cw_logging.getLogger().warning('SURRENDER: {}'.format(rep_path))
+            cw_logging.getLogger().warning("SURRENDER: {}".format(rep_path))
             surrender = s
         except:
             crash = True
-            cw_logging.getLogger().exception('EXCEPTION: {}'.format(rep_path))
+            cw_logging.getLogger().exception("EXCEPTION: {}".format(rep_path))
 
         self.exp.finalize(surrender, crash)
         self.logger.finalize()
 
     def load_task(self, c: Dict) -> Dict:
         """Load the results of a single task.
 
@@ -118,16 +126,22 @@
 
 
 class JobFactory:
     """Facotry class to create single jobs from experiment configuration.
     Specifially used to map experiment repetitions to Jobs.
     """
 
-    def __init__(self, exp_cls: Type[experiment.AbstractExperiment], logger: cw_logging.AbstractLogger,
-                 delete_old_files: bool = False, root_dir: str = "", read_only: bool = False):
+    def __init__(
+        self,
+        exp_cls: Type[experiment.AbstractExperiment],
+        logger: cw_logging.AbstractLogger,
+        delete_old_files: bool = False,
+        root_dir: str = "",
+        read_only: bool = False,
+    ):
         self.exp_cls = exp_cls
         self.logger = logger
         self.delete_old_files = delete_old_files
         self.root_dir = root_dir
         self.read_only = read_only
 
     def _group_exp_tasks(self, task_confs: List[Dict]) -> Dict:
@@ -167,15 +181,15 @@
 
             # Use 1 Repetition per job if not defined otherwise
             rep_portion = 1
             if KEYS.REPS_P_JOB in exp_group[0]:
                 rep_portion = exp_group[0][KEYS.REPS_P_JOB]
 
             for start_rep in range(0, max_rep, rep_portion):
-                tasks.append(exp_group[start_rep:start_rep + rep_portion])
+                tasks.append(exp_group[start_rep : start_rep + rep_portion])
         return tasks
 
     def create_jobs(self, exp_configs: List[Dict]) -> List[Job]:
         """creates a list of all jobs.
 
         Args:
             exp_configs (List[attrdict.AttrDict]): list of all defined experiment configurations.
@@ -188,11 +202,11 @@
         for task in task_list:
             j = Job(
                 task,
                 self.exp_cls,
                 self.logger,
                 self.delete_old_files,
                 self.root_dir,
-                self.read_only
+                self.read_only,
             )
             joblist.append(j)
         return joblist
```

### Comparing `cw2-2.2/cw2/scheduler.py` & `cw2-2.3/cw2/scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import abc
 import concurrent.futures
+import multiprocessing
 import os
+import socket
+import warnings
 from typing import List
 
 from joblib import Parallel, delayed
-import multiprocessing
-import socket
-import warnings
+
 from cw2 import cw_error, job
+from cw2.cw_config import cw_conf_keys as KEYS
 from cw2.cw_config import cw_config
 from cw2.cw_slurm import cw_slurm
-from cw2.cw_config import cw_conf_keys as KEYS
 
 
 class AbstractScheduler(abc.ABC):
     def __init__(self, conf: cw_config.Config = None):
         self.joblist = None
         self.config = conf
 
@@ -33,208 +34,263 @@
         Args:
             overwrite (bool, optional): overwrite flag. can be passed to the job. Defaults to False.
         """
         raise NotImplementedError
 
 
 class GPUDistributingLocalScheduler(AbstractScheduler):
-
     def __init__(self, conf: cw_config.Config = None):
-
         super(GPUDistributingLocalScheduler, self).__init__(conf=conf)
-        self._total_num_gpus = int(conf.slurm_config["sbatch_args"]["gres"].rsplit(":", 1)[1])
-        self._gpus_per_rep = conf.slurm_config['gpus_per_rep']
+        self._total_num_gpus = int(
+            conf.slurm_config["sbatch_args"]["gres"].rsplit(":", 1)[1]
+        )
+        self._gpus_per_rep = conf.slurm_config["gpus_per_rep"]
         self._queue_elements = int(self._total_num_gpus / self._gpus_per_rep)
 
-        print("GPUDistributingLocalScheduler: {} GPUs available, {} GPUs per rep, {} queue elements".format(
-            self._total_num_gpus, self._gpus_per_rep, self._queue_elements))
+        print(
+            "GPUDistributingLocalScheduler: {} GPUs available, {} GPUs per rep, {} queue elements".format(
+                self._total_num_gpus, self._gpus_per_rep, self._queue_elements
+            )
+        )
 
         if self._gpus_per_rep >= 1.0:
-            assert self._gpus_per_rep == int(self._gpus_per_rep), "gpus_per_rep must be integer"
+            assert self._gpus_per_rep == int(
+                self._gpus_per_rep
+            ), "gpus_per_rep must be integer"
 
     @staticmethod
     def use_distributed_gpu_scheduling(conf: cw_config.Config) -> bool:
         if conf.slurm_config is None:
             return False
         # Use if
         # 1.) GPUs Requested
         # 2.) Number of GPUs per rep specified
         # 3.) Number of GPUs per rep != total number of gpus requested
         gpus_requested = "gres" in conf.slurm_config.get("sbatch_args", "DUMMY_DEFAULT")
         gpus_per_rep_specified = "gpus_per_rep" in conf.slurm_config
 
         if gpus_requested:
-            num_gpus_requested = int(conf.slurm_config["sbatch_args"]["gres"].rsplit(":", 1)[1])
+            num_gpus_requested = int(
+                conf.slurm_config["sbatch_args"]["gres"].rsplit(":", 1)[1]
+            )
             # e.g. gres=gpu:4 or gres=gpu:full:4
         else:
             num_gpus_requested = 0
 
-        use_distributed_gpu_scheduling = \
-            gpus_requested and gpus_per_rep_specified and num_gpus_requested != conf.slurm_config["gpus_per_rep"]
+        use_distributed_gpu_scheduling = (
+            gpus_requested
+            and gpus_per_rep_specified
+            and num_gpus_requested != conf.slurm_config["gpus_per_rep"]
+        )
 
         if not use_distributed_gpu_scheduling:
-            on_horeka_gpu = "hkn" in socket.gethostname() and conf.slurm_config["partition"] == "accelerated"
+            on_horeka_gpu = (
+                "hkn" in socket.gethostname()
+                and conf.slurm_config["partition"] == "accelerated"
+            )
             if on_horeka_gpu:
-                assert num_gpus_requested == 4, "On HoreKA, you must request 4 GPUs (gres=gpu:4)"
-            assert not on_horeka_gpu, "You are on HoreKA and not using the GPU scheduler, don't! "
+                assert (
+                    num_gpus_requested == 4
+                ), "On HoreKA, you must request 4 GPUs (gres=gpu:4)"
+            assert (
+                not on_horeka_gpu
+            ), "You are on HoreKA and not using the GPU scheduler, don't! "
 
         return use_distributed_gpu_scheduling
 
     @staticmethod
     def get_gpu_str(queue_idx: int, gpus_per_rep: float) -> str:
         if gpus_per_rep >= 1:
-            assert int(gpus_per_rep) == gpus_per_rep, "gpus_per_rep must be integer if >= 1"
+            assert (
+                int(gpus_per_rep) == gpus_per_rep
+            ), "gpus_per_rep must be integer if >= 1"
             gpus_per_rep = int(gpus_per_rep)
-            return ("{}," * gpus_per_rep).format(*[queue_idx * gpus_per_rep + i for i in range(gpus_per_rep)])[:-1]
+            return ("{}," * gpus_per_rep).format(
+                *[queue_idx * gpus_per_rep + i for i in range(gpus_per_rep)]
+            )[:-1]
         else:
             return str(int(queue_idx * gpus_per_rep) + 0.01)
 
 
 class MPGPUDistributingLocalScheduler(GPUDistributingLocalScheduler):
-
     def run(self, overwrite: bool = False):
         num_parallel = self.joblist[0].n_parallel
         for j in self.joblist:
-            assert j.n_parallel == num_parallel, "All jobs in list must have same n_parallel"
-            assert j.n_parallel == self._queue_elements, "Mismatch between GPUs Queue Elements and Jobs executed in" \
-                                                         "parallel. Fix for optimal resource usage!!"
+            assert (
+                j.n_parallel == num_parallel
+            ), "All jobs in list must have same n_parallel"
+            assert j.n_parallel == self._queue_elements, (
+                "Mismatch between GPUs Queue Elements and Jobs executed in"
+                "parallel. Fix for optimal resource usage!!"
+            )
 
         with multiprocessing.Pool(processes=num_parallel) as pool:
             # setup gpu resource queue
             m = multiprocessing.Manager()
             gpu_queue = m.Queue(maxsize=self._queue_elements)
             for i in range(self._queue_elements):
                 gpu_queue.put(i)
 
             for j in self.joblist:
                 for c in j.tasks:
-                    pool.apply_async(MPGPUDistributingLocalScheduler._execute_task, (j, c, gpu_queue,
-                                                                                     self._gpus_per_rep,
-                                                                                     overwrite))
+                    pool.apply_async(
+                        MPGPUDistributingLocalScheduler._execute_task,
+                        (j, c, gpu_queue, self._gpus_per_rep, overwrite),
+                    )
             pool.close()
             pool.join()
 
     @staticmethod
-    def _execute_task(j: job.Job,
-                      c: dict,
-                      q: multiprocessing.Queue,
-                      gpus_per_rep: int,
-                      overwrite: bool = False):
+    def _execute_task(
+        j: job.Job,
+        c: dict,
+        q: multiprocessing.Queue,
+        gpus_per_rep: int,
+        overwrite: bool = False,
+    ):
         queue_idx = q.get()
         gpu_str = MPGPUDistributingLocalScheduler.get_gpu_str(queue_idx, gpus_per_rep)
         try:
             os.environ["CUDA_VISIBLE_DEVICES"] = gpu_str
             j.run_task(c, overwrite)
         except cw_error.ExperimentSurrender as _:
             return
         finally:
             q.put(queue_idx)
 
 
 class HOREKAAffinityGPUDistributingLocalScheduler(GPUDistributingLocalScheduler):
-
     def __init__(self, conf: cw_config.Config = None):
         super(HOREKAAffinityGPUDistributingLocalScheduler, self).__init__(conf=conf)
 
-        total_cpus = conf.slurm_config['cpus-per-task'] * conf.slurm_config['ntasks']
+        total_cpus = conf.slurm_config["cpus-per-task"] * conf.slurm_config["ntasks"]
         self._cpus_per_rep = total_cpus // self._queue_elements
 
-        assert self._cpus_per_rep > 0, "Not enough CPUs for the number of GPUs requested"
+        assert (
+            self._cpus_per_rep > 0
+        ), "Not enough CPUs for the number of GPUs requested"
 
     def run(self, overwrite: bool = False):
         print("Seeing CPUs:", os.sched_getaffinity(0))
         num_parallel = self.joblist[0].n_parallel
         for j in self.joblist:
-            assert j.n_parallel == num_parallel, "All jobs in list must have same n_parallel"
-            assert j.n_parallel == self._queue_elements, "Mismatch between GPUs Queue Elements and Jobs executed in" \
-                                                         "parallel. Fix for optimal resource usage!!"
-
-        with concurrent.futures.ProcessPoolExecutor(max_workers=num_parallel,
-                                                    ) as pool:
+            assert (
+                j.n_parallel == num_parallel
+            ), "All jobs in list must have same n_parallel"
+            assert j.n_parallel == self._queue_elements, (
+                "Mismatch between GPUs Queue Elements and Jobs executed in"
+                "parallel. Fix for optimal resource usage!!"
+            )
+
+        with concurrent.futures.ProcessPoolExecutor(
+            max_workers=num_parallel,
+        ) as pool:
             # setup gpu resource queue
             m = multiprocessing.Manager()
             gpu_queue = m.Queue(maxsize=self._queue_elements)
             for i in range(self._queue_elements):
                 gpu_queue.put(i)
 
             for j in self.joblist:
                 for c in j.tasks:
                     pool.submit(
                         HOREKAAffinityGPUDistributingLocalScheduler._execute_task,
-                        j, c, gpu_queue, self._gpus_per_rep, self._cpus_per_rep,
-                        overwrite)
+                        j,
+                        c,
+                        gpu_queue,
+                        self._gpus_per_rep,
+                        self._cpus_per_rep,
+                        overwrite,
+                    )
 
     @staticmethod
-    def _execute_task(j: job.Job,
-                      c: dict,
-                      q: multiprocessing.Queue,
-                      gpus_per_rep: int,
-                      cpus_per_rep: int,
-                      overwrite: bool = False):
+    def _execute_task(
+        j: job.Job,
+        c: dict,
+        q: multiprocessing.Queue,
+        gpus_per_rep: int,
+        cpus_per_rep: int,
+        overwrite: bool = False,
+    ):
         print("Seeing CPUs:", os.sched_getaffinity(0))
         queue_idx = q.get()
-        gpu_str = HOREKAAffinityGPUDistributingLocalScheduler.get_gpu_str(queue_idx, gpus_per_rep)
+        gpu_str = HOREKAAffinityGPUDistributingLocalScheduler.get_gpu_str(
+            queue_idx, gpus_per_rep
+        )
         cpus = set(range(queue_idx * cpus_per_rep, (queue_idx + 1) * cpus_per_rep))
         print("Job {}: Using GPUs: {} and CPUs: {}".format(queue_idx, gpu_str, cpus))
         try:
             os.sched_setaffinity(0, cpus)
             c[KEYS.i_CPU_CORES] = cpus
             os.environ["CUDA_VISIBLE_DEVICES"] = gpu_str
             j.run_task(c, overwrite)
         except cw_error.ExperimentSurrender as _:
             return
         finally:
             q.put(queue_idx)
 
 
 class KlusterThreadLimitingScheduler(GPUDistributingLocalScheduler):
-
     def __init__(self, conf: cw_config.Config = None):
         super(KlusterThreadLimitingScheduler, self).__init__(conf=conf)
-        total_cpus = conf.slurm_config['cpus-per-task'] * conf.slurm_config['ntasks']
+        total_cpus = conf.slurm_config["cpus-per-task"] * conf.slurm_config["ntasks"]
         self._num_threads = total_cpus // self._queue_elements
         print("Using {} threads per Rep".format(self._num_threads))
 
     def run(self, overwrite: bool = False):
         num_parallel = self.joblist[0].n_parallel
         for j in self.joblist:
-            assert j.n_parallel == num_parallel, "All jobs in list must have same n_parallel"
-            assert j.n_parallel == self._queue_elements, "Mismatch between GPUs Queue Elements and Jobs executed in" \
-                                                         "parallel. Fix for optimal resource usage!!"
+            assert (
+                j.n_parallel == num_parallel
+            ), "All jobs in list must have same n_parallel"
+            assert j.n_parallel == self._queue_elements, (
+                "Mismatch between GPUs Queue Elements and Jobs executed in"
+                "parallel. Fix for optimal resource usage!!"
+            )
 
         with multiprocessing.Pool(processes=num_parallel) as pool:
             # setup gpu resource queue
             m = multiprocessing.Manager()
             gpu_queue = m.Queue(maxsize=self._queue_elements)
             for i in range(self._queue_elements):
                 gpu_queue.put(i)
 
             for j in self.joblist:
                 for c in j.tasks:
-                    args = (j, c, gpu_queue, self._gpus_per_rep, self._num_threads, overwrite)
+                    args = (
+                        j,
+                        c,
+                        gpu_queue,
+                        self._gpus_per_rep,
+                        self._num_threads,
+                        overwrite,
+                    )
                     pool.apply_async(KlusterThreadLimitingScheduler._execute_task, args)
             pool.close()
             pool.join()
 
     @staticmethod
-    def _execute_task(j: job.Job,
-                      c: dict,
-                      q: multiprocessing.Queue,
-                      gpus_per_rep: int,
-                      num_threads: int,
-                      overwrite: bool = False):
+    def _execute_task(
+        j: job.Job,
+        c: dict,
+        q: multiprocessing.Queue,
+        gpus_per_rep: int,
+        num_threads: int,
+        overwrite: bool = False,
+    ):
         queue_idx = q.get()
         gpu_str = KlusterThreadLimitingScheduler.get_gpu_str(queue_idx, gpus_per_rep)
         try:
             os.environ["MKL_NUM_THREADS"] = str(num_threads)
             os.environ["NUMEXPR_NUM_THREADS"] = str(num_threads)
             os.environ["OMP_NUM_THREADS"] = str(num_threads)
             # Ok, that's not so nice, but I did not find better way yet
             try:
                 import torch
+
                 torch.set_num_threads(num_threads)
             except ImportError:
                 pass
 
             os.environ["CUDA_VISIBLE_DEVICES"] = gpu_str
             j.run_task(c, overwrite)
         except cw_error.ExperimentSurrender as _:
@@ -253,50 +309,68 @@
     else:
         raise NotImplementedError
 
 
 class CpuDistributingLocalScheduler(AbstractScheduler):
     def __init__(self, conf: cw_config.Config = None):
         super(CpuDistributingLocalScheduler, self).__init__(conf=conf)
-        self._total_num_cpus = conf.slurm_config['cpus-per-task'] * conf.slurm_config['ntasks']
-        self._cpus_per_rep = conf.slurm_config['cpus_per_rep']
-        assert self._cpus_per_rep == int(self._cpus_per_rep), "cpus_per_rep must be integer"
+        self._total_num_cpus = (
+            conf.slurm_config["cpus-per-task"] * conf.slurm_config["ntasks"]
+        )
+        self._cpus_per_rep = conf.slurm_config["cpus_per_rep"]
+        assert self._cpus_per_rep == int(
+            self._cpus_per_rep
+        ), "cpus_per_rep must be integer"
         self._queue_elements = int(self._total_num_cpus / self._cpus_per_rep)
-        print("CPUDistributingLocalScheduler: {} CPUs available, {} CPUs per rep, {} queue elements".format(
-            self._total_num_cpus, self._cpus_per_rep, self._queue_elements))
+        print(
+            "CPUDistributingLocalScheduler: {} CPUs available, {} CPUs per rep, {} queue elements".format(
+                self._total_num_cpus, self._cpus_per_rep, self._queue_elements
+            )
+        )
 
     def run(self, overwrite: bool = False):
         print("Seeing CPUs:", os.sched_getaffinity(0))
         num_parallel = self.joblist[0].n_parallel
         for j in self.joblist:
-            assert j.n_parallel == num_parallel, "All jobs in list must have same n_parallel"
-            assert j.n_parallel == self._queue_elements, "Mismatch between CPUs Queue Elements and Jobs executed in" \
-                                                         "parallel. Fix for optimal resource usage!!"
-
-        with concurrent.futures.ProcessPoolExecutor(max_workers=num_parallel,
-                                                    ) as pool:
+            assert (
+                j.n_parallel == num_parallel
+            ), "All jobs in list must have same n_parallel"
+            assert j.n_parallel == self._queue_elements, (
+                "Mismatch between CPUs Queue Elements and Jobs executed in"
+                "parallel. Fix for optimal resource usage!!"
+            )
+
+        with concurrent.futures.ProcessPoolExecutor(
+            max_workers=num_parallel,
+        ) as pool:
             # setup gpu resource queue
             m = multiprocessing.Manager()
             cpu_queue = m.Queue(maxsize=self._queue_elements)
             for i in range(self._queue_elements):
                 cpu_queue.put(i)
 
             for j in self.joblist:
                 for c in j.tasks:
                     pool.submit(
                         CpuDistributingLocalScheduler._execute_task,
-                        j, c, cpu_queue, self._cpus_per_rep,
-                        overwrite)
+                        j,
+                        c,
+                        cpu_queue,
+                        self._cpus_per_rep,
+                        overwrite,
+                    )
 
     @staticmethod
-    def _execute_task(j: job.Job,
-                      c: dict,
-                      q: multiprocessing.Queue,
-                      cpus_per_rep: int,
-                      overwrite: bool = False):
+    def _execute_task(
+        j: job.Job,
+        c: dict,
+        q: multiprocessing.Queue,
+        cpus_per_rep: int,
+        overwrite: bool = False,
+    ):
         print("Seeing CPUs:", os.sched_getaffinity(0))
         queue_idx = q.get()
         cpus = set(range(queue_idx * cpus_per_rep, (queue_idx + 1) * cpus_per_rep))
         print("Job {}: Using CPUs: {}".format(queue_idx, cpus))
         try:
             os.sched_setaffinity(0, cpus)
             c[KEYS.i_CPU_CORES] = cpus
@@ -307,22 +381,24 @@
             q.put(queue_idx)
 
     @staticmethod
     def use_distributed_cpu_scheduling(conf: cw_config.Config) -> bool:
         if conf.slurm_config is None:
             return False
         else:
-            scheduler = conf.slurm_config.get('scheduler', None)
-            return scheduler == 'cpu_distribute'
+            scheduler = conf.slurm_config.get("scheduler", None)
+            return scheduler == "cpu_distribute"
+
 
 class LocalScheduler(AbstractScheduler):
     def run(self, overwrite: bool = False):
         for j in self.joblist:
-            Parallel(n_jobs=j.n_parallel)(delayed(self.execute_task)(j, c, overwrite)
-                                          for c in j.tasks)
+            Parallel(n_jobs=j.n_parallel)(
+                delayed(self.execute_task)(j, c, overwrite) for c in j.tasks
+            )
 
     def execute_task(self, j: job.Job, c: dict, overwrite: bool = False):
         try:
             j.run_task(c, overwrite)
         except cw_error.ExperimentSurrender as _:
             return
```

### Comparing `cw2-2.2/cw2/util.py` & `cw2-2.3/cw2/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import os
 import re
 
 try:
-    from collections.abc import MutableMapping, Mapping, MutableSequence  # noqa
+    from collections.abc import Mapping, MutableMapping, MutableSequence  # noqa
 except ImportError:
-    from collections import MutableMapping, Mapping, MutableSequence  # noqa
+    from collections import Mapping, MutableMapping, MutableSequence  # noqa
 
 
 def deep_update(base_dict: dict, update_dict: dict) -> dict:
     """Updates the base dictionary with corresponding values from the update dictionary, including nested collections.
        Not updated values are kept as is.
 
     Arguments:
@@ -25,15 +25,15 @@
             branch = deep_update(base_dict.get(key, {}), value)
             base_dict[key] = branch
         else:
             base_dict[key] = update_dict[key]
     return base_dict
 
 
-def flatten_dict(d, parent_key='', sep='_'):
+def flatten_dict(d, parent_key="", sep="_"):
     items = []
     for k, v in d.items():
         new_key = parent_key + sep + k if parent_key else k
         if isinstance(v, MutableMapping):
             items.extend(flatten_dict(v, new_key, sep=sep).items())
         elif isinstance(v, MutableSequence):
             keys = map(lambda i: new_key + "_" + str(i), range(len(v)))
@@ -83,19 +83,19 @@
 
 
 def format_time(time_in_secs: float) -> str:
     return str(datetime.timedelta(seconds=time_in_secs))
 
 
 def shorten_param(_param_name):
-    name_parts = _param_name.split('.')
-    shortened_parts = '.'.join(map(lambda s: s[:3], name_parts[:-1]))
-    shortened_leaf = ''.join(map(lambda s: s[0], name_parts[-1].split('_')))
+    name_parts = _param_name.split(".")
+    shortened_parts = ".".join(map(lambda s: s[:3], name_parts[:-1]))
+    shortened_leaf = "".join(map(lambda s: s[0], name_parts[-1].split("_")))
     if shortened_parts:
-        return shortened_parts + '.' + shortened_leaf
+        return shortened_parts + "." + shortened_leaf
     else:
         return shortened_leaf
 
 
 def get_size(start_path: str):
     """recursively compute size of a directory
 
@@ -122,35 +122,38 @@
 
     Returns:
         bool: True if child is subdir of parent
     """
     parent_path = os.path.abspath(parent)
     child_path = os.path.abspath(child)
 
-    return os.path.commonpath([parent_path]) == os.path.commonpath([parent_path, child_path])
+    return os.path.commonpath([parent_path]) == os.path.commonpath(
+        [parent_path, child_path]
+    )
 
 
 def convert_param_names(_param_names: list, values: list) -> str:
     """create new shorthand name derived from parameter and value association
     Arguments:
         _param_names (list): parameter names for the experiment
         values (list): concrete values for each parameter
 
     Returns:
         str: shorthand name
     """
 
-    _converted_name = '_'.join("{}{}".format(
-        shorten_param(k), v) for k, v in zip(_param_names, values))
+    _converted_name = "_".join(
+        "{}{}".format(shorten_param(k), v) for k, v in zip(_param_names, values)
+    )
     # _converted_name = re.sub("[' \[\],()]", '', _converted_name)
-    _converted_name = re.sub("[' ]", '', _converted_name)
-    _converted_name = re.sub('["]', '', _converted_name)
-    _converted_name = re.sub("[(\[]", '_', _converted_name)
-    _converted_name = re.sub("[)\]]", '', _converted_name)
-    _converted_name = re.sub("[,]", '_', _converted_name)
+    _converted_name = re.sub("[' ]", "", _converted_name)
+    _converted_name = re.sub('["]', "", _converted_name)
+    _converted_name = re.sub("[(\[]", "_", _converted_name)
+    _converted_name = re.sub("[)\]]", "", _converted_name)
+    _converted_name = re.sub("[,]", "_", _converted_name)
     return _converted_name
 
 
 def get_file_names_in_directory(directory: str) -> [str]:
     """
     Get file names in given directory
     Args:
```

### Comparing `cw2-2.2/cw2.egg-info/PKG-INFO` & `cw2-2.3/cw2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cw2
-Version: 2.2
+Version: 2.3
 Summary: A reengineered framework to run experiments on a computing cluster.
 Home-page: https://github.com/ALRhub/cw2
 Author: Maximilian Li
 Author-email: maximilian.xiling.li@gmail.com
 License: MIT
 Keywords: scientific,experiments,distributed computing,mpi,research
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cw2-2.2/cw2.egg-info/SOURCES.txt` & `cw2-2.3/cw2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cw2-2.2/setup.py` & `cw2-2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,53 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='cw2',
-
+    name="cw2",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.2',
-
-    description='A reengineered framework to run experiments on a computing cluster.',
+    version="2.3",
+    description="A reengineered framework to run experiments on a computing cluster.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-
+    long_description_content_type="text/markdown",
     # The project's main homepage.
-    url='https://github.com/ALRhub/cw2',
-
+    url="https://github.com/ALRhub/cw2",
     # Author details
-    author='Maximilian Li',
-    author_email='maximilian.xiling.li@gmail.com',
-
-    license='MIT',
-
+    author="Maximilian Li",
+    author_email="maximilian.xiling.li@gmail.com",
+    license="MIT",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Education',
-        'Topic :: System :: Distributed Computing',
-        'Topic :: Scientific/Engineering',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-        'Topic :: Education',
-
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Environment :: Console'
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Education",
+        "Topic :: System :: Distributed Computing",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Education",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Environment :: Console",
     ],
-
-    python_requires='>=3',
-
+    python_requires=">=3",
     # What does your project relate to?
-    keywords=['scientific', 'experiments',
-              'distributed computing', 'mpi', 'research'],
-
+    keywords=["scientific", "experiments", "distributed computing", "mpi", "research"],
     packages=find_packages(),
-    package_data={'cw2': ['default_sbatch.sh']},
-
-    install_requires=['PyYAML', 'numpy', 'pandas', 'joblib'],
+    package_data={"cw2": ["default_sbatch.sh"]},
+    install_requires=["PyYAML", "numpy", "pandas", "joblib"],
 )
```

