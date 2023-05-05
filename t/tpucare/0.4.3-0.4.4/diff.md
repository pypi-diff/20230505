# Comparing `tmp/tpucare-0.4.3.tar.gz` & `tmp/tpucare-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpucare-0.4.3.tar", last modified: Fri May  5 11:57:56 2023, max compression
+gzip compressed data, was "tpucare-0.4.4.tar", last modified: Fri May  5 13:33:28 2023, max compression
```

## Comparing `tpucare-0.4.3.tar` & `tpucare-0.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 11:57:56.356714 tpucare-0.4.3/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-05-02 17:44:22.000000 tpucare-0.4.3/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-05 11:57:56.356714 tpucare-0.4.3/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     7570 2023-05-02 17:44:22.000000 tpucare-0.4.3/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-05 11:57:56.356714 tpucare-0.4.3/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1106 2023-05-05 11:57:42.000000 tpucare-0.4.3/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 11:57:56.356714 tpucare-0.4.3/tpucare/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11123 2023-05-05 11:57:30.000000 tpucare-0.4.3/tpucare/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 11:57:56.356714 tpucare-0.4.3/tpucare.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-05 11:57:56.000000 tpucare-0.4.3/tpucare.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      170 2023-05-05 11:57:56.000000 tpucare-0.4.3/tpucare.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-05 11:57:56.000000 tpucare-0.4.3/tpucare.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-05 11:57:56.000000 tpucare-0.4.3/tpucare.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 13:33:28.412765 tpucare-0.4.4/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-05-02 17:44:22.000000 tpucare-0.4.4/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-05 13:33:28.412765 tpucare-0.4.4/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7570 2023-05-02 17:44:22.000000 tpucare-0.4.4/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-05 13:33:28.412765 tpucare-0.4.4/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1106 2023-05-05 13:33:18.000000 tpucare-0.4.4/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 13:33:28.412765 tpucare-0.4.4/tpucare/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    11135 2023-05-05 13:33:03.000000 tpucare-0.4.4/tpucare/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 13:33:28.412765 tpucare-0.4.4/tpucare.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-05 13:33:28.000000 tpucare-0.4.4/tpucare.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      170 2023-05-05 13:33:28.000000 tpucare-0.4.4/tpucare.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-05 13:33:28.000000 tpucare-0.4.4/tpucare.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-05 13:33:28.000000 tpucare-0.4.4/tpucare.egg-info/top_level.txt
```

### Comparing `tpucare-0.4.3/LICENSE` & `tpucare-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tpucare-0.4.3/PKG-INFO` & `tpucare-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpucare
-Version: 0.4.3
+Version: 0.4.4
 Summary: Automatically take good care of your preemptible TPUs
 Home-page: https://github.com/clashluke/tpucare
 Author: Lucas Nestler
 Author-email: github.tpucare@nestler.sh
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tpucare-0.4.3/README.md` & `tpucare-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `tpucare-0.4.3/setup.py` & `tpucare-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.tpucare@nestler.sh",
     name='tpucare',
     license='BSD',
     description='Automatically take good care of your preemptible TPUs',
-    version='0.4.3',
+    version='0.4.4',
     long_description=README,
     url='https://github.com/clashluke/tpucare',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

### Comparing `tpucare-0.4.3/tpucare/__init__.py` & `tpucare-0.4.4/tpucare/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,16 +124,15 @@
         GLOBAL_DICT[f"tpus_{zone}"] = json.loads(call(f"{TPU_CMD} list --zone {zone} --format json"))
     return GLOBAL_DICT[f"tpus_{zone}"]
 
 
 def valid_tpu(tpu: dict, preempted: bool = True, deleting: bool = False, unhealthy: bool = True) -> bool:
     state = "state" in tpu and (deleting or tpu['state'] != "DELETING") and (preempted or tpu['state'] != "PREEMPTED")
     state |= deleting and preempted
-    healthy = "health" in tpu and (unhealthy or tpu["health"] == "HEALTHY")
-    healthy |= unhealthy
+    healthy = unhealthy or "health" not in tpu or tpu["health"] == "HEALTHY"  # we assume no health info == good
     return state and healthy
 
 
 def tpu_names(zone: str, preempted: bool = True, deleting: bool = False, unhealthy: bool = False,
               no_filter: bool = False, prefix: str = ''):
     while True:
         try:
```

### Comparing `tpucare-0.4.3/tpucare.egg-info/PKG-INFO` & `tpucare-0.4.4/tpucare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpucare
-Version: 0.4.3
+Version: 0.4.4
 Summary: Automatically take good care of your preemptible TPUs
 Home-page: https://github.com/clashluke/tpucare
 Author: Lucas Nestler
 Author-email: github.tpucare@nestler.sh
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

