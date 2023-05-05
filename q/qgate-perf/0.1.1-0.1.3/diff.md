# Comparing `tmp/qgate_perf-0.1.1.tar.gz` & `tmp/qgate_perf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_perf-0.1.1.tar", last modified: Fri May  5 07:13:58 2023, max compression
+gzip compressed data, was "qgate_perf-0.1.3.tar", last modified: Fri May  5 13:23:04 2023, max compression
```

## Comparing `qgate_perf-0.1.1.tar` & `qgate_perf-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 07:13:58.513334 qgate_perf-0.1.1/
--rw-rw-rw-   0        0        0    11558 2023-04-29 14:14:55.000000 qgate_perf-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6322 2023-05-05 07:13:58.513334 qgate_perf-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5912 2023-05-05 07:06:42.000000 qgate_perf-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 07:13:58.482518 qgate_perf-0.1.1/qgate_perf/
--rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_perf-0.1.1/qgate_perf/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-05-04 18:36:53.000000 qgate_perf-0.1.1/qgate_perf/file_format.py
--rw-rw-rw-   0        0        0    10431 2023-05-04 20:39:19.000000 qgate_perf-0.1.1/qgate_perf/parallel_executor.py
--rw-rw-rw-   0        0        0     5423 2023-05-04 20:44:25.000000 qgate_perf-0.1.1/qgate_perf/parallel_return.py
--rw-rw-rw-   0        0        0     1329 2023-05-04 18:43:18.000000 qgate_perf-0.1.1/qgate_perf/run_setup.py
--rw-rw-rw-   0        0        0      215 2023-05-05 07:11:06.000000 qgate_perf-0.1.1/qgate_perf/version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:13:58.513334 qgate_perf-0.1.1/qgate_perf.egg-info/
--rw-rw-rw-   0        0        0     6322 2023-05-05 07:13:58.000000 qgate_perf-0.1.1/qgate_perf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-05 07:13:58.000000 qgate_perf-0.1.1/qgate_perf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 07:13:58.000000 qgate_perf-0.1.1/qgate_perf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 07:13:58.000000 qgate_perf-0.1.1/qgate_perf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-05 07:13:58.000000 qgate_perf-0.1.1/qgate_perf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 07:13:58.513334 qgate_perf-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1264 2023-05-05 07:12:43.000000 qgate_perf-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:23:04.476765 qgate_perf-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-29 14:14:55.000000 qgate_perf-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6322 2023-05-05 13:23:04.476765 qgate_perf-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5912 2023-05-05 07:06:42.000000 qgate_perf-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 13:23:04.449498 qgate_perf-0.1.3/qgate_perf/
+-rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_perf-0.1.3/qgate_perf/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-05-04 18:36:53.000000 qgate_perf-0.1.3/qgate_perf/file_format.py
+-rw-rw-rw-   0        0        0    11172 2023-05-05 13:03:19.000000 qgate_perf-0.1.3/qgate_perf/parallel_executor.py
+-rw-rw-rw-   0        0        0     5424 2023-05-05 13:10:57.000000 qgate_perf-0.1.3/qgate_perf/parallel_return.py
+-rw-rw-rw-   0        0        0     1329 2023-05-04 18:43:18.000000 qgate_perf-0.1.3/qgate_perf/run_setup.py
+-rw-rw-rw-   0        0        0      215 2023-05-05 13:19:59.000000 qgate_perf-0.1.3/qgate_perf/version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:23:04.476765 qgate_perf-0.1.3/qgate_perf.egg-info/
+-rw-rw-rw-   0        0        0     6322 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-05 13:23:04.000000 qgate_perf-0.1.3/qgate_perf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:23:04.476765 qgate_perf-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-05-05 07:12:43.000000 qgate_perf-0.1.3/setup.py
```

### Comparing `qgate_perf-0.1.1/LICENSE` & `qgate_perf-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qgate_perf-0.1.1/PKG-INFO` & `qgate_perf-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate_perf
-Version: 0.1.1
+Version: 0.1.3
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

### Comparing `qgate_perf-0.1.1/README.md` & `qgate_perf-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qgate_perf-0.1.1/qgate_perf/file_format.py` & `qgate_perf-0.1.3/qgate_perf/file_format.py`

 * *Files identical despite different names*

### Comparing `qgate_perf-0.1.1/qgate_perf/parallel_executor.py` & `qgate_perf-0.1.3/qgate_perf/parallel_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 FileFormat.PRF_CORE_PLAN_EXECUTOR_ALL: processes * threads,
                 FileFormat.PRF_CORE_PLAN_EXECUTOR: [processes, threads],
                 FileFormat.PRF_CORE_REAL_EXECUTOR: count,
                 FileFormat.PRF_CORE_GROUP: group,
                 FileFormat.PRF_CORE_TOTAL_CALL: sum_call,
                 FileFormat.PRF_CORE_AVRG_TIME: sum_time / count,
                 FileFormat.PRF_CORE_STD_DEVIATION: sum_deviation / count,
-                FileFormat.PRF_CORE_TOTAL_CALL_PER_SEC: (1 / (sum_time / count)) * count * run_setup.bulk_row,
+                FileFormat.PRF_CORE_TOTAL_CALL_PER_SEC: 0 if (sum_time / count)==0 else (1 / (sum_time / count)) * count * run_setup.bulk_row,
                 FileFormat.PRF_CORE_TIME_END: datetime.datetime.utcnow().isoformat(' ')
             }
             self._print(file, f"  {json.dumps(out)}")
 
 
     def run_bulk_executor(self,
                               bulk_list=[[1, 1], [1, 2]],
@@ -186,15 +186,15 @@
             self.run_executor(executor_list, run_setup)
             time.sleep(sleep_between_bulks)
             gc.collect()
 
     def run_executor(self, executor_list=[[1, 1], [2, 2], [4, 1], [4, 2], [4, 4], [8, 1], [8, 2], [8, 4]],
                          run_setup: RunSetup=None):
         """ Run executor sequencies
-            :param executor_list:       list of executors for execution in format [[processes, threads], ...]
+            :param executor_list:       list of executors for execution in format [[processes, threads, 'label'], ...]
             :param run_setup:           setup of execution
         """
         file = None
         print('Execution...')
 
         try:
             if self._output_file is not None:
@@ -203,15 +203,20 @@
             self._print_header(file, run_setup)
 
             for executors in executor_list:
                 # execution
                 with multiprocessing.Manager() as manager:
                     return_dict = manager.dict()
                     self._executeCore(run_setup, return_dict, executors[0], executors[1])
-                    self._print_detail(file, run_setup, return_dict, executors[0], executors[1], executors[2])
+                    self._print_detail(file,
+                                       run_setup,
+                                       return_dict,
+                                       executors[0],
+                                       executors[1],
+                                       '' if len(executors) <= 2 else executors[2])
 
             self._print_footer(file)
 
         except Exception as e:
             self._print(file, str(e) if e is not None else '!! Noname exception !!')
         finally:
             if file is not None:
@@ -240,7 +245,23 @@
             self._print_footer(file)
 
         except Exception as e:
             self._print(file, str(e) if e is not None else '!! Noname exception !!')
         finally:
             if file is not None:
                 file.close()
+
+    def run_test(self):
+        """ Run test, only one shot (execution) of test function """
+
+        # setup minimalistic values
+        setup = RunSetup(duration_second=0, start_delay=0, parameters=None)
+        setup.set_bulk(1,1)
+
+        # run
+        self.run(processes=1,
+                 threads=1,
+                 run_setup=setup)
+
+    #TODO: add dry ran
+    #TODO: create dir, if not exist
+    #TODO: app default sets of executors as helper
```

### Comparing `qgate_perf-0.1.1/qgate_perf/parallel_return.py` & `qgate_perf-0.1.3/qgate_perf/parallel_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             self.min_duration=duration_one_shot
 
         # setup new max
         if duration_one_shot>self.max_duration:
             self.max_duration=duration_one_shot
 
         # Is it possible to end performance testing?
-        if ((self.stop_time_one_shot - self.init_time) > self.duration_second):
+        if ((self.stop_time_one_shot - self.init_time) >= self.duration_second):
             # write time
             self.track_time[FileFormat.PRF_DETAIL_TIME_END]=datetime.datetime.utcnow()
             # calc standard deviation
             self.standard_deviation=self.stddev.std
             return True
         return False
```

### Comparing `qgate_perf-0.1.1/qgate_perf/run_setup.py` & `qgate_perf-0.1.3/qgate_perf/run_setup.py`

 * *Files identical despite different names*

### Comparing `qgate_perf-0.1.1/qgate_perf.egg-info/PKG-INFO` & `qgate_perf-0.1.3/qgate_perf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.1.1
+Version: 0.1.3
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

### Comparing `qgate_perf-0.1.1/setup.py` & `qgate_perf-0.1.3/setup.py`

 * *Files identical despite different names*

