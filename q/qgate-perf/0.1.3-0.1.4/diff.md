# Comparing `tmp/qgate_perf-0.1.3.tar.gz` & `tmp/qgate_perf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_perf-0.1.3.tar", last modified: Fri May  5 13:23:04 2023, max compression
+gzip compressed data, was "qgate_perf-0.1.4.tar", last modified: Fri May  5 20:07:14 2023, max compression
```

## Comparing `qgate_perf-0.1.3.tar` & `qgate_perf-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:23:04.476765 qgate_perf-0.1.3/
--rw-rw-rw-   0        0        0    11558 2023-04-29 14:14:55.000000 qgate_perf-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6322 2023-05-05 13:23:04.476765 qgate_perf-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5912 2023-05-05 07:06:42.000000 qgate_perf-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 13:23:04.449498 qgate_perf-0.1.3/qgate_perf/
--rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_perf-0.1.3/qgate_perf/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-05-04 18:36:53.000000 qgate_perf-0.1.3/qgate_perf/file_format.py
--rw-rw-rw-   0        0        0    11172 2023-05-05 13:03:19.000000 qgate_perf-0.1.3/qgate_perf/parallel_executor.py
--rw-rw-rw-   0        0        0     5424 2023-05-05 13:10:57.000000 qgate_perf-0.1.3/qgate_perf/parallel_return.py
--rw-rw-rw-   0        0        0     1329 2023-05-04 18:43:18.000000 qgate_perf-0.1.3/qgate_perf/run_setup.py
--rw-rw-rw-   0        0        0      215 2023-05-05 13:19:59.000000 qgate_perf-0.1.3/qgate_perf/version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:23:04.476765 qgate_perf-0.1.3/qgate_perf.egg-info/
--rw-rw-rw-   0        0        0     6322 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 13:23:04.476765 qgate_perf-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1264 2023-05-05 07:12:43.000000 qgate_perf-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:07:14.835423 qgate_perf-0.1.4/
+-rw-rw-rw-   0        0        0    11558 2023-04-29 14:14:55.000000 qgate_perf-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6253 2023-05-05 20:07:14.819139 qgate_perf-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5843 2023-05-05 20:03:12.000000 qgate_perf-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 20:07:14.747079 qgate_perf-0.1.4/qgate_perf/
+-rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_perf-0.1.4/qgate_perf/__init__.py
+-rw-rw-rw-   0        0        0      373 2023-05-05 17:10:51.000000 qgate_perf-0.1.4/qgate_perf/bundle_helper.py
+-rw-rw-rw-   0        0        0     4598 2023-05-05 17:10:51.000000 qgate_perf-0.1.4/qgate_perf/executor_helper.py
+-rw-rw-rw-   0        0        0     1053 2023-05-04 18:36:53.000000 qgate_perf-0.1.4/qgate_perf/file_format.py
+-rw-rw-rw-   0        0        0    10741 2023-05-05 19:53:35.000000 qgate_perf-0.1.4/qgate_perf/parallel_executor.py
+-rw-rw-rw-   0        0        0     5424 2023-05-05 13:10:57.000000 qgate_perf-0.1.4/qgate_perf/parallel_return.py
+-rw-rw-rw-   0        0        0     1057 2023-05-05 19:53:35.000000 qgate_perf-0.1.4/qgate_perf/run_setup.py
+-rw-rw-rw-   0        0        0      215 2023-05-05 20:04:58.000000 qgate_perf-0.1.4/qgate_perf/version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:07:14.803505 qgate_perf-0.1.4/qgate_perf.egg-info/
+-rw-rw-rw-   0        0        0     6253 2023-05-05 20:07:14.000000 qgate_perf-0.1.4/qgate_perf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-05-05 20:07:14.000000 qgate_perf-0.1.4/qgate_perf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 20:07:14.000000 qgate_perf-0.1.4/qgate_perf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 20:07:14.000000 qgate_perf-0.1.4/qgate_perf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-05 20:07:14.000000 qgate_perf-0.1.4/qgate_perf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 20:07:14.835423 qgate_perf-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-05-05 07:12:43.000000 qgate_perf-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:07:14.819139 qgate_perf-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-05 17:45:29.000000 qgate_perf-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     3356 2023-05-05 19:57:29.000000 qgate_perf-0.1.4/tests/test_run.py
```

### Comparing `qgate_perf-0.1.3/LICENSE` & `qgate_perf-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qgate_perf-0.1.3/PKG-INFO` & `qgate_perf-0.1.4/qgate_perf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qgate_perf
-Version: 0.1.3
+Name: qgate-perf
+Version: 0.1.4
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
@@ -20,41 +20,38 @@
 
 ```lang-python
 from qgate_perf.parallel_executor import ParallelExecutor
 from qgate_perf.parallel_return import ParallelReturn
 from qgate_perf.run_setup import RunSetup
 import time
 
-# Function for performance testing
 def prf_GIL_impact(return_key, return_dict, run_setup: RunSetup):
+    """ Function for performance testing"""
     try:
-        # init (contain executor synchonization, if needed)
-        performance=ParallelReturn(run_setup)
+        # INIT - contain executor synchonization, if needed
+        performance = ParallelReturn(run_setup)
 
-        while(True):
-        
-            # START - performance measure for specific part of code
-            performance.start()
+        while (True):
 
+            # START - performance test, only for this specific code part
+            performance.start()
+            
             for r in range(run_setup.bulk_row * run_setup.bulk_col):
                 time.sleep(0)
-
-            # STOP - performance measure specific part of code
+            
+            # STOP - performance test
             if performance.stop():
                 break
 
-        # return outputs
-        if return_dict is not None:
-            return_dict[return_key] = performance
-
+        # RETURN - data from performance
+        return_dict[return_key] = performance
+        
     except Exception as ex:
-        # return outputs in case of error
-        if return_dict is not None:
-            return_dict[return_key] = ParallelReturn(None, ex)
-
+        # RETURN - error
+        return_dict[return_key] = ParallelReturn(None, ex)
 
 generator = ParallelExecutor(prf_GIL_impact,
                              label="GIL_impact",
                              detail_output=True,
                              output_file="prf_gil_impact_01.txt")
 
 generator.run_bulk_executor(bulk_list=[[1, 1]],
```

### Comparing `qgate_perf-0.1.3/README.md` & `qgate_perf-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,41 +7,38 @@
 
 ```lang-python
 from qgate_perf.parallel_executor import ParallelExecutor
 from qgate_perf.parallel_return import ParallelReturn
 from qgate_perf.run_setup import RunSetup
 import time
 
-# Function for performance testing
 def prf_GIL_impact(return_key, return_dict, run_setup: RunSetup):
+    """ Function for performance testing"""
     try:
-        # init (contain executor synchonization, if needed)
-        performance=ParallelReturn(run_setup)
+        # INIT - contain executor synchonization, if needed
+        performance = ParallelReturn(run_setup)
 
-        while(True):
-        
-            # START - performance measure for specific part of code
-            performance.start()
+        while (True):
 
+            # START - performance test, only for this specific code part
+            performance.start()
+            
             for r in range(run_setup.bulk_row * run_setup.bulk_col):
                 time.sleep(0)
-
-            # STOP - performance measure specific part of code
+            
+            # STOP - performance test
             if performance.stop():
                 break
 
-        # return outputs
-        if return_dict is not None:
-            return_dict[return_key] = performance
-
+        # RETURN - data from performance
+        return_dict[return_key] = performance
+        
     except Exception as ex:
-        # return outputs in case of error
-        if return_dict is not None:
-            return_dict[return_key] = ParallelReturn(None, ex)
-
+        # RETURN - error
+        return_dict[return_key] = ParallelReturn(None, ex)
 
 generator = ParallelExecutor(prf_GIL_impact,
                              label="GIL_impact",
                              detail_output=True,
                              output_file="prf_gil_impact_01.txt")
 
 generator.run_bulk_executor(bulk_list=[[1, 1]],
```

### Comparing `qgate_perf-0.1.3/qgate_perf/file_format.py` & `qgate_perf-0.1.4/qgate_perf/file_format.py`

 * *Files identical despite different names*

### Comparing `qgate_perf-0.1.3/qgate_perf/parallel_executor.py` & `qgate_perf-0.1.4/qgate_perf/parallel_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,32 +74,28 @@
                 features.append(
                     executor.submit(func, f"{return_key}x{thread_key}", return_dict, run_setup))
 
             for future in concurrent.futures.as_completed(features):
                 future.result()
 
     def _executeCore(self, run_setup: RunSetup, return_dict, processes=2, threads=2):
-        # manager = multiprocessing.Manager()
-        # return_dict = manager.dict()
         proc = []
 
         # define synch time for run of all executors
         run_setup.set_start_time()
-#        print(f"before INIT {datetime.datetime.now()} > When Start {run_setup.when_start}")
+
         if threads == 1:
             for process_key in range(processes):
-                run_setup.set_output_handler(process_key, return_dict)
                 p = Process(target=self._func,
                             args=(process_key, return_dict, run_setup))
 #                            args=(run_setup))
 
                 proc.append(p)
         else:
             for process_key in range(processes):
-                run_setup.set_output_handler(process_key, return_dict)
                 p = Process(target=self._coreThreadClassPool,
                             args=(threads,process_key, return_dict, run_setup))
                 # p = Process(target=self._coreThreadClass, args=(threads, process_key, return_dict, run_setup))
                 # p = Process(target=ParallelExecutor._coreThread, args=(self.func, threads, process_key, return_dict, run_setup))
                 # p = Process(target=ParallelExecutor._coreThreadPool, args=(self.func, threads, process_key, return_dict, run_setup))
                 proc.append(p)
 
@@ -108,16 +104,14 @@
             p.start()
 
         # wait for finish
         for p in proc:
             p.join()
             p.close()
 
-        # return return_dict
-
     def _print(self, file, out: str):
         if file is not None:
             file.write(out + "\n")
         print(out)
 
     def _print_header(self, file, run_setup: RunSetup=None):
         self._start_tasks = datetime.datetime.utcnow()
@@ -246,22 +240,20 @@
 
         except Exception as e:
             self._print(file, str(e) if e is not None else '!! Noname exception !!')
         finally:
             if file is not None:
                 file.close()
 
-    def run_test(self):
+    def one_shot(self):
         """ Run test, only one shot (execution) of test function """
 
         # setup minimalistic values
         setup = RunSetup(duration_second=0, start_delay=0, parameters=None)
         setup.set_bulk(1,1)
 
         # run
         self.run(processes=1,
                  threads=1,
                  run_setup=setup)
 
-    #TODO: add dry ran
     #TODO: create dir, if not exist
-    #TODO: app default sets of executors as helper
```

### Comparing `qgate_perf-0.1.3/qgate_perf/parallel_return.py` & `qgate_perf-0.1.4/qgate_perf/parallel_return.py`

 * *Files identical despite different names*

### Comparing `qgate_perf-0.1.3/qgate_perf/run_setup.py` & `qgate_perf-0.1.4/qgate_perf/run_setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,18 +16,10 @@
 
         # collection of specific keys for project such as project_name, feature_set_name, etc.
         self.parameters=parameters
 
     def set_start_time(self):
         self.when_start = datetime.datetime.now() + datetime.timedelta(seconds=self.start_delay)
 
-    def set_output_handler(self, return_key, return_dict):
-        self.return_key=return_key
-        self.return_dict=return_dict
-
-    def set_output(self, ret = None):
-        if self.return_dict is not None:
-            self.return_dict[self.return_key] = ret
-
     def set_bulk(self, bulk_row, bulk_column):
         self.bulk_row = bulk_row if bulk_row > 0 else 1
         self.bulk_col = bulk_column if bulk_column > 0 else 1
```

### Comparing `qgate_perf-0.1.3/qgate_perf.egg-info/PKG-INFO` & `qgate_perf-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qgate-perf
-Version: 0.1.3
+Name: qgate_perf
+Version: 0.1.4
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
@@ -20,41 +20,38 @@
 
 ```lang-python
 from qgate_perf.parallel_executor import ParallelExecutor
 from qgate_perf.parallel_return import ParallelReturn
 from qgate_perf.run_setup import RunSetup
 import time
 
-# Function for performance testing
 def prf_GIL_impact(return_key, return_dict, run_setup: RunSetup):
+    """ Function for performance testing"""
     try:
-        # init (contain executor synchonization, if needed)
-        performance=ParallelReturn(run_setup)
+        # INIT - contain executor synchonization, if needed
+        performance = ParallelReturn(run_setup)
 
-        while(True):
-        
-            # START - performance measure for specific part of code
-            performance.start()
+        while (True):
 
+            # START - performance test, only for this specific code part
+            performance.start()
+            
             for r in range(run_setup.bulk_row * run_setup.bulk_col):
                 time.sleep(0)
-
-            # STOP - performance measure specific part of code
+            
+            # STOP - performance test
             if performance.stop():
                 break
 
-        # return outputs
-        if return_dict is not None:
-            return_dict[return_key] = performance
-
+        # RETURN - data from performance
+        return_dict[return_key] = performance
+        
     except Exception as ex:
-        # return outputs in case of error
-        if return_dict is not None:
-            return_dict[return_key] = ParallelReturn(None, ex)
-
+        # RETURN - error
+        return_dict[return_key] = ParallelReturn(None, ex)
 
 generator = ParallelExecutor(prf_GIL_impact,
                              label="GIL_impact",
                              detail_output=True,
                              output_file="prf_gil_impact_01.txt")
 
 generator.run_bulk_executor(bulk_list=[[1, 1]],
```

### Comparing `qgate_perf-0.1.3/setup.py` & `qgate_perf-0.1.4/setup.py`

 * *Files identical despite different names*

