# Comparing `tmp/exclusionms-0.2.0.tar.gz` & `tmp/exclusionms-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exclusionms-0.2.0.tar", last modified: Thu May  4 23:47:44 2023, max compression
+gzip compressed data, was "exclusionms-0.2.1.tar", last modified: Fri May  5 00:33:49 2023, max compression
```

## Comparing `exclusionms-0.2.0.tar` & `exclusionms-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:47:44.344184 exclusionms-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-04 23:47:30.000000 exclusionms-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-04 23:47:44.344184 exclusionms-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-04 23:47:30.000000 exclusionms-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-04 23:47:30.000000 exclusionms-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 23:47:44.348184 exclusionms-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-04 23:47:30.000000 exclusionms-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:47:44.344184 exclusionms-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:47:44.344184 exclusionms-0.2.0/src/exclusionms/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 23:47:30.000000 exclusionms-0.2.0/src/exclusionms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20868 2023-05-04 23:47:30.000000 exclusionms-0.2.0/src/exclusionms/apihandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-05-04 23:47:30.000000 exclusionms-0.2.0/src/exclusionms/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-05-04 23:47:30.000000 exclusionms-0.2.0/src/exclusionms/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-04 23:47:30.000000 exclusionms-0.2.0/src/exclusionms/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-05-04 23:47:30.000000 exclusionms-0.2.0/src/exclusionms/stress_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:47:44.344184 exclusionms-0.2.0/src/exclusionms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-04 23:47:44.000000 exclusionms-0.2.0/src/exclusionms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-04 23:47:44.000000 exclusionms-0.2.0/src/exclusionms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:47:44.000000 exclusionms-0.2.0/src/exclusionms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-04 23:47:44.000000 exclusionms-0.2.0/src/exclusionms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-04 23:47:44.000000 exclusionms-0.2.0/src/exclusionms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 23:47:44.000000 exclusionms-0.2.0/src/exclusionms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:47:44.344184 exclusionms-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20490 2023-05-04 23:47:30.000000 exclusionms-0.2.0/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    20717 2023-05-04 23:47:30.000000 exclusionms-0.2.0/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:33:49.685451 exclusionms-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 00:33:37.000000 exclusionms-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-05 00:33:49.685451 exclusionms-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-05 00:33:37.000000 exclusionms-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-05 00:33:37.000000 exclusionms-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 00:33:49.685451 exclusionms-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-05 00:33:37.000000 exclusionms-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:33:49.681451 exclusionms-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:33:49.685451 exclusionms-0.2.1/src/exclusionms/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 00:33:37.000000 exclusionms-0.2.1/src/exclusionms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20868 2023-05-05 00:33:37.000000 exclusionms-0.2.1/src/exclusionms/apihandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-05-05 00:33:37.000000 exclusionms-0.2.1/src/exclusionms/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-05-05 00:33:37.000000 exclusionms-0.2.1/src/exclusionms/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-05 00:33:37.000000 exclusionms-0.2.1/src/exclusionms/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-05 00:33:37.000000 exclusionms-0.2.1/src/exclusionms/stress_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:33:49.685451 exclusionms-0.2.1/src/exclusionms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-05 00:33:49.000000 exclusionms-0.2.1/src/exclusionms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 00:33:49.000000 exclusionms-0.2.1/src/exclusionms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:33:49.000000 exclusionms-0.2.1/src/exclusionms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 00:33:49.000000 exclusionms-0.2.1/src/exclusionms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 00:33:49.000000 exclusionms-0.2.1/src/exclusionms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 00:33:49.000000 exclusionms-0.2.1/src/exclusionms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:33:49.685451 exclusionms-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20490 2023-05-05 00:33:37.000000 exclusionms-0.2.1/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20717 2023-05-05 00:33:37.000000 exclusionms-0.2.1/tests/test_db.py
```

### Comparing `exclusionms-0.2.0/LICENSE` & `exclusionms-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exclusionms-0.2.0/PKG-INFO` & `exclusionms-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exclusionms
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for working with exclusionms-api and exclusionms-streamlit
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `exclusionms-0.2.0/README.md` & `exclusionms-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `exclusionms-0.2.0/pyproject.toml` & `exclusionms-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project.urls]
 home = "https://github.com/pgarrett-scripps/ExclusionMs.git"
 
 [project.scripts]
-stress_tester = "exclusionms.stress_tester:main"
+stress_test = "exclusionms.stress_test:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "exclusionms.__version__"}
 
 [tool.pylint]
 max-line-length = 120
 fail-under = 9.5
```

### Comparing `exclusionms-0.2.0/src/exclusionms/apihandler.py` & `exclusionms-0.2.1/src/exclusionms/apihandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
     Returns:
         A dictionary containing the most recent log entries.
 
     Raises:
         HTTPError: If the API request returns an error status code.
 
     """
-    response = requests.get(url=f'{exclusionms_ip}/log/entries?num_entries={num_entries}', timeout=timeout)
+    response = requests.get(url=f'{exclusionms_ip}/logs/entries?num_entries={num_entries}', timeout=timeout)
     response.raise_for_status()
     return json.loads(response.content)
 
 
 @dataclass
 class Handler:
     """A simple wrapper around the exclusion API functions.
@@ -564,8 +564,8 @@
 
     def load_or_clear_exclusion_list(self):
         """Calls equivalent apihandler function with the Handlers attributes"""
         return load_or_clear_exclusion_list(self.exclusion_api_ip, self.timeout)
 
     def get_log_entries(self) -> {}:
         """Calls equivalent apihandler function with the Handlers attributes"""
-        return search_intervals(self.exclusion_api_ip, self.timeout)
+        return get_log_entries(self.exclusion_api_ip, self.timeout)
```

### Comparing `exclusionms-0.2.0/src/exclusionms/components.py` & `exclusionms-0.2.1/src/exclusionms/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Parameters:
         min_bound (Union[float, None]): The minimum bound value to convert.
 
     Returns:
         float: The minimum bound value as a float.
     """
     if min_bound is None:
-        return -sys.float_info.max
+        return float('-inf')
     return min_bound
 
 
 def convert_max_bounds(max_bound: Union[float, None]) -> float:
     """
     Convert the maximum bound value to a float.
 
@@ -57,15 +57,15 @@
     Parameters:
         max_bound (Union[float, None]): The maximum bound value to convert.
 
     Returns:
         float: The maximum bound value as a float.
     """
     if max_bound is None:
-        return sys.float_info.max
+        return float('inf')
     return max_bound
 
 
 class ExclusionInterval(BaseModel):
     """
     ExclusionInterval represents an interval in a multidimensional space defined by several properties.
     These properties include mass, retention time (rt), ook0, intensity, and charge. The class provides
```

### Comparing `exclusionms-0.2.0/src/exclusionms/db.py` & `exclusionms-0.2.1/src/exclusionms/db.py`

 * *Files identical despite different names*

### Comparing `exclusionms-0.2.0/src/exclusionms/random.py` & `exclusionms-0.2.1/src/exclusionms/random.py`

 * *Files identical despite different names*

### Comparing `exclusionms-0.2.0/src/exclusionms/stress_test.py` & `exclusionms-0.2.1/src/exclusionms/stress_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,22 +207,69 @@
 
         log.info("ExclusionMS still processing intervals... %s / %s", exclusionms_len, num_intervals)
         time.sleep(1)
 
     return False
 
 
-def main(args):
+def parse_args() -> argparse.Namespace:
+    parser = argparse.ArgumentParser(description='ExclusionMS real-time plotting script.')
+
+    # Stress Tests Arguments
+    parser.add_argument('--exclusion_api_ip', type=str, default='http://127.0.0.1:8000',
+                        help='IP address of the ExclusionMS server.')
+    parser.add_argument('--num_intervals', type=int, default=100000,
+                        help='Number of intervals to add.')
+    parser.add_argument('--point_delay', type=float, default=0.1,
+                        help='Time in seconds between adding points.')
+    parser.add_argument('--num_points', type=float, default=1000,
+                        help='Number of points to search per query')
+    parser.add_argument('--num_additional_intervals', type=int, default=100,
+                        help='Additional intervals to add during runtime')
+    parser.add_argument('--additional_interval_delay', type=float, default=1,
+                        help='Additional intervals to add during runtime')
+    parser.add_argument('--run_time', type=float, default=30,
+                        help='Length of time to run the stress test for.')
+    parser.add_argument('--realtime_plot', type=bool, default=True,
+                        help='plot stress test data in real time')
+
+    # Random Arguments
+    parser.add_argument('--charge_range', metavar=('MIN', 'MAX'), type=int, nargs=2, default=[1, 5],
+                        help='range of charges (default: 1 to 5)')
+    parser.add_argument('--mass_range', metavar=('MIN', 'MAX'), type=float, nargs=2, default=[500.0, 700.0],
+                        help='range of masses (default: 500 to 5000)')
+    parser.add_argument('--rt_range', metavar=('MIN', 'MAX'), type=float, nargs=2, default=[0.0, 1000.0],
+                        help='range of retention times (default: 0 to 10000)')
+    parser.add_argument('--ook0_range', metavar=('MIN', 'MAX'), type=float, nargs=2, default=[0.5, 1.5],
+                        help='range of OOK0 values (default: 0.5 to 1.5)')
+    parser.add_argument('--intensity_range', metavar=('MIN', 'MAX'), type=float, nargs=2, default=[500.0, 50000.0],
+                        help='range of intensities (default: 500 to 50000)')
+
+    # Tolerance Arguments
+    parser.add_argument('--charge_tolerance', type=bool, default=False,
+                        help='charge tolerance value (default: False)')
+    parser.add_argument('--mass_tolerance', type=float, default=5,
+                        help='mass tolerance value (default: 5)')
+    parser.add_argument('--rt_tolerance', type=float, default=100,
+                        help='retention time tolerance value (default: 1000)')
+    parser.add_argument('--ook0_tolerance', type=float, default=None,
+                        help='OOK0 tolerance value (default: None)')
+    parser.add_argument('--intensity_tolerance', type=float, default=None,
+                        help='intensity tolerance value (default: None)')
+    args = parser.parse_args()
+    return args
+
+
+def main():
     """
     Main function for the script. It clears the intervals, adds random intervals, updates the plot, and saves the plot.
-
-    Args:
-        args (argparse.Namespace): Parsed command line arguments.
     """
-    title = f"ExclusionMS Size: {args.num_intervals}, Num Points: {args.num_points}, Query Delay: {args.point_delay}, "\
+
+    args = parse_args()
+    title = f"ExclusionMS Size: {args.num_intervals}, Num Points: {args.num_points}, Query Delay: {args.point_delay}, " \
             f"Additional Intervals: {args.num_additional_intervals}, Interval Delay: {args.additional_interval_delay}"
     file_name = title.replace(':', '_').replace(',', '_').replace(' ', '')
     png_file = file_name + '.png'
 
     logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
     log = logging.getLogger(__name__)
 
@@ -309,53 +356,8 @@
     plt.figtext(0.5, 0.01, f'{str(np.mean(percents) * 100)}', wrap=True, horizontalalignment='center', fontsize=10)
     fig.savefig(png_file, dpi=300, bbox_inches='tight')
 
     log.info('Done!')
 
 
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='ExclusionMS real-time plotting script.')
-
-    # Stress Tests Arguments
-    parser.add_argument('--exclusion_api_ip', type=str, default='http://127.0.0.1:8000',
-                        help='IP address of the ExclusionMS server.')
-    parser.add_argument('--num_intervals', type=int, default=100000,
-                        help='Number of intervals to add.')
-    parser.add_argument('--point_delay', type=float, default=0.1,
-                        help='Time in seconds between adding points.')
-    parser.add_argument('--num_points', type=float, default=1000,
-                        help='Number of points to search per query')
-    parser.add_argument('--num_additional_intervals', type=int, default=100,
-                        help='Additional intervals to add during runtime')
-    parser.add_argument('--additional_interval_delay', type=float, default=1,
-                        help='Additional intervals to add during runtime')
-    parser.add_argument('--run_time', type=float, default=30,
-                        help='Length of time to run the stress test for.')
-    parser.add_argument('--realtime_plot', type=bool, default=True,
-                        help='plot stress test data in real time')
-
-    # Random Arguments
-    parser.add_argument('--charge_range', metavar=('MIN', 'MAX'), type=int, nargs=2, default=[1, 5],
-                        help='range of charges (default: 1 to 5)')
-    parser.add_argument('--mass_range', metavar=('MIN', 'MAX'), type=float, nargs=2, default=[500.0, 700.0],
-                        help='range of masses (default: 500 to 5000)')
-    parser.add_argument('--rt_range', metavar=('MIN', 'MAX'), type=float, nargs=2, default=[0.0, 1000.0],
-                        help='range of retention times (default: 0 to 10000)')
-    parser.add_argument('--ook0_range', metavar=('MIN', 'MAX'), type=float, nargs=2, default=[0.5, 1.5],
-                        help='range of OOK0 values (default: 0.5 to 1.5)')
-    parser.add_argument('--intensity_range', metavar=('MIN', 'MAX'), type=float, nargs=2, default=[500.0, 50000.0],
-                        help='range of intensities (default: 500 to 50000)')
-
-    # Tolerance Arguments
-    parser.add_argument('--charge_tolerance', type=bool, default=False,
-                        help='charge tolerance value (default: False)')
-    parser.add_argument('--mass_tolerance', type=float, default=5,
-                        help='mass tolerance value (default: 5)')
-    parser.add_argument('--rt_tolerance', type=float, default=100,
-                        help='retention time tolerance value (default: 1000)')
-    parser.add_argument('--ook0_tolerance', type=float, default=None,
-                        help='OOK0 tolerance value (default: None)')
-    parser.add_argument('--intensity_tolerance', type=float, default=None,
-                        help='intensity tolerance value (default: None)')
-    args = parser.parse_args()
-
-    main(args)
+    main()
```

### Comparing `exclusionms-0.2.0/src/exclusionms.egg-info/PKG-INFO` & `exclusionms-0.2.1/src/exclusionms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exclusionms
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for working with exclusionms-api and exclusionms-streamlit
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `exclusionms-0.2.0/tests/test_components.py` & `exclusionms-0.2.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `exclusionms-0.2.0/tests/test_db.py` & `exclusionms-0.2.1/tests/test_db.py`

 * *Files identical despite different names*

