# Comparing `tmp/python_rdma_qe-0.0.5.tar.gz` & `tmp/python_rdma_qe-0.0.6.tar.gz`

## Comparing `python_rdma_qe-0.0.5.tar` & `python_rdma_qe-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe_test.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/requirements-stable.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdmaqe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/common/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/common/cli.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/common/file_libs.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/common/fmf_tools.py
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/common/tc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdma/__init__.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdma/general.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdma/opa.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdma/roce.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdma/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdma/sriov/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdma/sriov/abc_sriov.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/rdma/sriov/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/.fmf/version
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/__init__.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/functional.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/init_mem.txt
--rw-r--r--   0        0        0    23541 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/init_top.txt
--rw-r--r--   0        0        0    16908 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/log
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/main.fmf
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/rdmaqe/tests/sriov/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/LICENSE
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/README.md
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe_test.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/requirements-stable.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdmaqe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/cli.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/file_libs.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/fmf_tools.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/tc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/__init__.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/general.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/opa.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/roce.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/__init__.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/abc_sriov.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/.fmf/version
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/__init__.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/functional.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/init_mem.txt
+-rw-r--r--   0        0        0    23790 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/init_top.txt
+-rw-r--r--   0        0        0    16908 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/log
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/main.fmf
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/sriov/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/LICENSE
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/README.md
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/PKG-INFO
```

### Comparing `python_rdma_qe-0.0.5/rdmaqe_test.py` & `python_rdma_qe-0.0.6/rdmaqe_test.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/requirements-stable.txt` & `python_rdma_qe-0.0.6/requirements-stable.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/common/cli.py` & `python_rdma_qe-0.0.6/rdmaqe/common/cli.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/common/file_libs.py` & `python_rdma_qe-0.0.6/rdmaqe/common/file_libs.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/common/fmf_tools.py` & `python_rdma_qe-0.0.6/rdmaqe/common/fmf_tools.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/common/tc.py` & `python_rdma_qe-0.0.6/rdmaqe/common/tc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""tc.py: Module for test case execution."""
+"""tc.py: Module for test case execution. Note: copied from libsan"""
 
 from libsan.host.cmdline import run
 from libsan.host import linux
 
 import stqe.host.logchecker
 import stqe.host.restraint
 
@@ -26,16 +26,19 @@
     run("lscpu")
     print("### List PCI Devices Of RDMA ###")
     run("lspci | grep -i -e ethernet -e infiniband -e omni -e ConnectX")
     print("### File system disk space usage: ###")
     run("df -h")
     print("### IP Settings")
     run("ip addr show")
-
-    #TODO: if we run commands ibstat/ibstatus/iblinkinfo/ibv_devinfo -v
+    print("### RDMA devices info ###")
+    run("ibstat")
+    run("ibstatus")
+    run("iblinkinfo")
+    run("ibv_devinfo -v")
 
 
 class Test:
     tc_status = {
         "pass": "PASS: ",
         "fail": "FAIL: ",
         "skip": "SKIP: "
```

### Comparing `python_rdma_qe-0.0.5/rdmaqe/rdma/general.py` & `python_rdma_qe-0.0.6/rdmaqe/rdma/general.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/rdma/opa.py` & `python_rdma_qe-0.0.6/rdmaqe/rdma/opa.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/rdma/roce.py` & `python_rdma_qe-0.0.6/rdmaqe/rdma/roce.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/rdma/sriov/abc_sriov.py` & `python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/abc_sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/rdma/sriov/sriov.py` & `python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/1.txt` & `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/1.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/functional.py` & `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/functional.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/init_top.txt` & `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/init_top.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,219 +1,188 @@
-top - 10:07:03 up  1:20,  1 user,  load average: 0.00, 0.01, 0.00
-Tasks: 290 total,   1 running, 289 sleeping,   0 stopped,   0 zombie
-%Cpu(s):  0.3 us,  0.6 sy,  0.0 ni, 99.2 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
-MiB Mem :  47972.4 total,  46347.5 free,   1633.7 used,    459.5 buff/cache
-MiB Swap:  24180.0 total,  24180.0 free,      0.0 used.  46338.8 avail Mem 
+top - 22:36:55 up 14 days, 13:50,  1 user,  load average: 0.10, 0.03, 0.01
+Tasks: 293 total,   1 running, 292 sleeping,   0 stopped,   0 zombie
+%Cpu(s):  0.3 us,  0.8 sy,  0.0 ni, 98.9 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
+MiB Mem :  47972.4 total,  44628.2 free,   2755.1 used,   2094.2 buff/cache
+MiB Swap:  24180.0 total,  24180.0 free,      0.0 used.  45217.3 avail Mem 
 
     PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND
-   4409 root      20   0   10700   4196   3392 R  11.8   0.0   0:00.03 top
-      1 root      20   0  173048  19524  10996 S   0.0   0.0   0:16.61 systemd
-      2 root      20   0       0      0      0 S   0.0   0.0   0:00.01 kthreadd
+ 532483 root      20   0   10700   4204   3392 R   5.6   0.0   0:00.03 top
+      1 root      20   0  173180  19528  10996 S   0.0   0.0   0:25.02 systemd
+      2 root      20   0       0      0      0 S   0.0   0.0   0:00.46 kthreadd
       3 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rcu_gp
       4 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rcu_par+
       5 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 slub_fl+
       6 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 netns
       8 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-     10 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
+     10 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
      12 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mm_perc+
      14 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
      15 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
      16 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
-     17 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
-     18 root      20   0       0      0      0 I   0.0   0.0   0:01.44 rcu_pre+
-     19 root      rt   0       0      0      0 S   0.0   0.0   0:00.00 migrati+
+     17 root      20   0       0      0      0 S   0.0   0.0   0:00.76 ksoftir+
+     18 root      20   0       0      0      0 I   0.0   0.0   6:30.15 rcu_pre+
+     19 root      rt   0       0      0      0 S   0.0   0.0   0:01.75 migrati+
      21 root      20   0       0      0      0 S   0.0   0.0   0:00.14 cpuhp/0
      22 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/1
-     23 root      rt   0       0      0      0 S   0.0   0.0   0:00.24 migrati+
-     24 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     23 root      rt   0       0      0      0 S   0.0   0.0   0:01.93 migrati+
+     24 root      20   0       0      0      0 S   0.0   0.0   0:00.18 ksoftir+
      26 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      27 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/2
-     28 root      rt   0       0      0      0 S   0.0   0.0   0:00.24 migrati+
-     29 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     28 root      rt   0       0      0      0 S   0.0   0.0   0:01.80 migrati+
+     29 root      20   0       0      0      0 S   0.0   0.0   0:00.05 ksoftir+
      31 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      32 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/3
-     33 root      rt   0       0      0      0 S   0.0   0.0   0:00.25 migrati+
-     34 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     33 root      rt   0       0      0      0 S   0.0   0.0   0:01.84 migrati+
+     34 root      20   0       0      0      0 S   0.0   0.0   0:00.64 ksoftir+
      36 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      37 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/4
-     38 root      rt   0       0      0      0 S   0.0   0.0   0:00.25 migrati+
-     39 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
-     40 root      20   0       0      0      0 I   0.0   0.0   0:00.35 kworker+
+     38 root      rt   0       0      0      0 S   0.0   0.0   0:01.92 migrati+
+     39 root      20   0       0      0      0 S   0.0   0.0   0:00.02 ksoftir+
      41 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      42 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/5
-     43 root      rt   0       0      0      0 S   0.0   0.0   0:00.25 migrati+
-     44 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     43 root      rt   0       0      0      0 S   0.0   0.0   0:01.87 migrati+
+     44 root      20   0       0      0      0 S   0.0   0.0   0:00.04 ksoftir+
      46 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      47 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/6
-     48 root      rt   0       0      0      0 S   0.0   0.0   0:00.26 migrati+
-     49 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     48 root      rt   0       0      0      0 S   0.0   0.0   0:01.94 migrati+
+     49 root      20   0       0      0      0 S   0.0   0.0   0:00.03 ksoftir+
      51 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      52 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/7
-     53 root      rt   0       0      0      0 S   0.0   0.0   0:00.26 migrati+
-     54 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     53 root      rt   0       0      0      0 S   0.0   0.0   0:01.98 migrati+
+     54 root      20   0       0      0      0 S   0.0   0.0   0:00.05 ksoftir+
      56 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      57 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/8
-     58 root      rt   0       0      0      0 S   0.0   0.0   0:00.26 migrati+
-     59 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     58 root      rt   0       0      0      0 S   0.0   0.0   0:01.93 migrati+
+     59 root      20   0       0      0      0 S   0.0   0.0   0:00.03 ksoftir+
      61 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      62 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/9
-     63 root      rt   0       0      0      0 S   0.0   0.0   0:00.27 migrati+
-     64 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     63 root      rt   0       0      0      0 S   0.0   0.0   0:01.91 migrati+
+     64 root      20   0       0      0      0 S   0.0   0.0   0:00.04 ksoftir+
      66 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      67 root      20   0       0      0      0 S   0.0   0.0   0:00.01 cpuhp/10
-     68 root      rt   0       0      0      0 S   0.0   0.0   0:00.34 migrati+
-     69 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     68 root      rt   0       0      0      0 S   0.0   0.0   0:02.05 migrati+
+     69 root      20   0       0      0      0 S   0.0   0.0   0:00.02 ksoftir+
      71 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      74 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/11
-     75 root      rt   0       0      0      0 S   0.0   0.0   0:00.34 migrati+
-     76 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     75 root      rt   0       0      0      0 S   0.0   0.0   0:02.04 migrati+
+     76 root      20   0       0      0      0 S   0.0   0.0   0:00.03 ksoftir+
      78 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      79 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/12
-     80 root      rt   0       0      0      0 S   0.0   0.0   0:00.35 migrati+
-     81 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     80 root      rt   0       0      0      0 S   0.0   0.0   0:01.99 migrati+
+     81 root      20   0       0      0      0 S   0.0   0.0   0:00.02 ksoftir+
      83 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      84 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/13
-     85 root      rt   0       0      0      0 S   0.0   0.0   0:00.35 migrati+
-     86 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     85 root      rt   0       0      0      0 S   0.0   0.0   0:02.02 migrati+
+     86 root      20   0       0      0      0 S   0.0   0.0   0:00.02 ksoftir+
      88 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      89 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/14
-     90 root      rt   0       0      0      0 S   0.0   0.0   0:00.36 migrati+
-     91 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
-     92 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+     90 root      rt   0       0      0      0 S   0.0   0.0   0:01.96 migrati+
+     91 root      20   0       0      0      0 S   0.0   0.0   0:00.02 ksoftir+
      93 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      94 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/15
-     95 root      rt   0       0      0      0 S   0.0   0.0   0:00.37 migrati+
-     96 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+     95 root      rt   0       0      0      0 S   0.0   0.0   0:02.06 migrati+
+     96 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
      98 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      99 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/16
-    100 root      rt   0       0      0      0 S   0.0   0.0   0:00.37 migrati+
-    101 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+    100 root      rt   0       0      0      0 S   0.0   0.0   0:02.02 migrati+
+    101 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
     103 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     104 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/17
-    105 root      rt   0       0      0      0 S   0.0   0.0   0:00.38 migrati+
-    106 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+    105 root      rt   0       0      0      0 S   0.0   0.0   0:02.02 migrati+
+    106 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
     108 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     109 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/18
-    110 root      rt   0       0      0      0 S   0.0   0.0   0:00.38 migrati+
-    111 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+    110 root      rt   0       0      0      0 S   0.0   0.0   0:02.03 migrati+
+    111 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
     113 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     114 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/19
-    115 root      rt   0       0      0      0 S   0.0   0.0   0:00.39 migrati+
-    116 root      20   0       0      0      0 S   0.0   0.0   0:00.00 ksoftir+
+    115 root      rt   0       0      0      0 S   0.0   0.0   0:01.98 migrati+
+    116 root      20   0       0      0      0 S   0.0   0.0   0:00.01 ksoftir+
     118 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     139 root      20   0       0      0      0 S   0.0   0.0   0:00.00 kdevtmp+
     140 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 inet_fr+
-    141 root      20   0       0      0      0 S   0.0   0.0   0:00.00 kauditd
-    142 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    143 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    144 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    145 root      20   0       0      0      0 I   0.0   0.0   0:04.07 kworker+
-    146 root      20   0       0      0      0 S   0.0   0.0   0:00.00 khungta+
+    141 root      20   0       0      0      0 S   0.0   0.0   0:00.01 kauditd
+    146 root      20   0       0      0      0 S   0.0   0.0   0:00.31 khungta+
     147 root      20   0       0      0      0 S   0.0   0.0   0:00.00 oom_rea+
     148 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 writeba+
-    149 root      20   0       0      0      0 S   0.0   0.0   0:00.04 kcompac+
-    150 root      20   0       0      0      0 S   0.0   0.0   0:00.03 kcompac+
+    149 root      20   0       0      0      0 S   0.0   0.0   0:09.59 kcompac+
+    150 root      20   0       0      0      0 S   0.0   0.0   0:10.44 kcompac+
     151 root      25   5       0      0      0 S   0.0   0.0   0:00.00 ksmd
-    152 root      39  19       0      0      0 S   0.0   0.0   0:00.02 khugepa+
+    152 root      39  19       0      0      0 S   0.0   0.0   0:03.18 khugepa+
     153 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 cryptd
     154 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kintegr+
     155 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kblockd
     156 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 blkcg_p+
-    158 root      20   0       0      0      0 I   0.0   0.0   0:00.07 kworker+
-    159 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    160 root      20   0       0      0      0 I   0.0   0.0   0:00.13 kworker+
-    162 root      20   0       0      0      0 I   0.0   0.0   0:00.04 kworker+
-    163 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    164 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    165 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    166 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    167 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    168 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    170 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    171 root      20   0       0      0      0 I   0.0   0.0   0:00.03 kworker+
-    172 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    173 root      20   0       0      0      0 I   0.0   0.0   0:00.03 kworker+
+    170 root      20   0       0      0      0 I   0.0   0.0   0:01.47 kworker+
     174 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 tpm_dev+
     175 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 md
     176 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 edac-po+
     177 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 watchdo+
-    178 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
+    178 root       0 -20       0      0      0 I   0.0   0.0   0:00.32 kworker+
     179 root      20   0       0      0      0 S   0.0   0.0   0:00.00 kswapd0
     180 root      20   0       0      0      0 S   0.0   0.0   0:00.00 kswapd1
-    185 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
     186 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kthrotld
-    189 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
     193 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 acpi_th+
     194 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kmpath_+
     195 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kaluad
-    197 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    198 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
-    199 root      20   0       0      0      0 I   0.0   0.0   0:00.38 kworker+
-    200 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    201 root      20   0       0      0      0 I   0.0   0.0   0:01.63 kworker+
-    202 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
+    197 root       0 -20       0      0      0 I   0.0   0.0   0:00.11 kworker+
+    198 root       0 -20       0      0      0 I   0.0   0.0   0:09.43 kworker+
+    200 root       0 -20       0      0      0 I   0.0   0.0   0:00.20 kworker+
+    202 root       0 -20       0      0      0 I   0.0   0.0   0:00.10 kworker+
     203 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mld
     204 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipv6_ad+
     205 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kstrp
     217 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 zswap-s+
     330 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     331 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     332 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    333 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    371 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    379 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    383 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    390 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
-    391 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    440 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    483 root       0 -20       0      0      0 I   0.0   0.0   0:00.01 kworker+
-    506 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    507 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
-    508 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    538 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
+    333 root       0 -20       0      0      0 I   0.0   0.0   0:00.16 kworker+
+    371 root       0 -20       0      0      0 I   0.0   0.0   0:00.21 kworker+
+    383 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
+    391 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
+    440 root       0 -20       0      0      0 I   0.0   0.0   0:02.82 kworker+
+    483 root       0 -20       0      0      0 I   0.0   0.0   0:00.19 kworker+
+    508 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
+    538 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
     539 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
     552 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 tls-strp
     572 root      20   0       0      0      0 S   0.0   0.0   0:00.00 scsi_eh+
     573 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 scsi_tm+
     580 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ata_sff
-    581 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    592 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
+    592 root       0 -20       0      0      0 I   0.0   0.0   0:00.08 kworker+
     598 root      20   0       0      0      0 S   0.0   0.0   0:00.01 scsi_eh+
     599 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 scsi_tm+
     600 root      20   0       0      0      0 S   0.0   0.0   0:00.01 scsi_eh+
     601 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 scsi_tm+
     608 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_he+
     609 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_pa+
     610 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_cm+
-    614 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    616 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
+    614 root       0 -20       0      0      0 I   0.0   0.0   0:00.05 kworker+
+    616 root       0 -20       0      0      0 I   0.0   0.0   0:00.01 kworker+
     643 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_ev+
     644 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_fw+
     645 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_fc
     646 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mlx5_hv+
-    686 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
+    686 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
     689 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kdmflus+
     696 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kdmflus+
     714 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfsalloc
     715 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs_mru+
     716 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-buf+
     717 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-con+
     718 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-rec+
     719 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-blo+
     720 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-ino+
     721 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-log+
     722 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-cil+
-    723 root      20   0       0      0      0 S   0.0   0.0   0:00.10 xfsaild+
-    726 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    753 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    769 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    770 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    789 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-    791 root      20   0   58896  37912  36776 S   0.0   0.1   0:02.75 systemd+
-    804 root      20   0   35400  13720   9188 S   0.0   0.0   0:00.38 systemd+
+    723 root      20   0       0      0      0 S   0.0   0.0   1:35.65 xfsaild+
+    769 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
+    770 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
+    791 root      20   0  287996 164816 163556 S   0.0   0.3  63:29.21 systemd+
+    804 root      20   0   35400  13784   9252 S   0.0   0.0   0:01.97 systemd+
     884 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-buf+
     885 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-con+
     886 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-rec+
     887 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-blo+
     888 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-ino+
     890 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-log+
     891 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-cil+
@@ -224,74 +193,108 @@
     898 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_mcast
     899 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_nl_s+
     900 root      39  19       0      0      0 S   0.0   0.0   0:00.00 kipmi0
     901 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kdmflus+
     902 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_mad1
     903 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_mad2
     904 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mkey_ca+
-    905 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
     908 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi_opfn
     937 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-buf+
     938 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-con+
     939 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-rec+
     940 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-blo+
     941 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-ino+
     944 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-log+
     945 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-cil+
     946 root      20   0       0      0      0 S   0.0   0.0   0:00.00 xfsaild+
     949 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipoib_wq
     950 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rdma_cm
     951 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipoib_wq
     956 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 iscsi_c+
-    959 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
     967 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 irq/196+
     968 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 irq/197+
     969 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 irq/198+
     970 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 target_+
     971 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 target_+
     972 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xcopy_wq
-    973 root      16  -4   18144   4468   1700 S   0.0   0.0   0:00.01 auditd
+    973 root      16  -4   18144   4468   1700 S   0.0   0.0   0:00.65 auditd
    1012 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi1_up+
    1013 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi0_0
    1014 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi_lin+
    1015 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rpciod
    1016 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xprtiod
-   1023 root      20   0  257352  21820  16768 S   0.0   0.0   0:09.05 Network+
-   1028 root      20   0   79360   5400   2872 S   0.0   0.0   0:01.56 irqbala+
-   1030 root      20   0  196632  18192  15860 S   0.0   0.0   0:04.08 rsyslogd
-   1036 root      20   0   20388  11260   8952 S   0.0   0.0   0:00.17 systemd+
-   1038 chrony    20   0   10440   3112   2612 S   0.0   0.0   0:00.03 chronyd
+   1023 root      20   0  257396  21872  16768 S   0.0   0.0  35:53.29 Network+
+   1028 root      20   0   79360   5400   2872 S   0.0   0.0   6:05.96 irqbala+
+   1030 root      20   0  624696  39184  37316 S   0.0   0.1 122:03.62 rsyslogd
+   1036 root      20   0   20388  11436   9028 S   0.0   0.0   0:02.02 systemd+
+   1038 chrony    20   0   10440   3112   2612 S   0.0   0.0   0:02.24 chronyd
    1058 dbus      20   0   10792   4620   3932 S   0.0   0.0   0:00.04 dbus-br+
-   1081 dbus      20   0    5260   2792   2368 S   0.0   0.0   0:00.15 dbus-br+
-   1087 root      20   0   15836   9476   8172 S   0.0   0.0   0:00.03 sshd
-   1094 root      20   0   81052   2216      0 S   0.0   0.0   0:00.00 rhsmcer+
+   1081 dbus      20   0    5260   2792   2368 S   0.0   0.0   0:00.83 dbus-br+
+   1087 root      20   0   15836   9476   8172 S   0.0   0.0   0:00.04 sshd
+   1094 root      20   0   81052   4452   2220 S   0.0   0.0   0:00.07 rhsmcer+
    1096 root      20   0    3044   1096   1008 S   0.0   0.0   0:00.03 agetty
    1097 root      20   0    5612   1100   1008 S   0.0   0.0   0:00.00 agetty
-   1098 root      20   0   22388  13884  10664 S   0.0   0.0   0:00.26 systemd
+   1098 root      20   0   22388  13888  10664 S   0.0   0.0   0:00.51 systemd
    1109 root      20   0   25588   5456      0 S   0.0   0.0   0:00.00 (sd-pam)
    1125 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_mad1
    1126 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipoib_wq
-   1677 root      20   0   18916  11400   9508 S   0.0   0.0   0:00.06 sshd
-   1679 root      20   0    8604   3788   2904 S   0.0   0.0   0:00.02 crond
-   1681 root      20   0  231512  10200   5392 S   0.0   0.0   0:01.48 restrai+
-   1688 root      20   0   19000   7312   5188 S   0.0   0.0   0:00.40 sshd
-   1689 root      20   0    7568   4500   3680 S   0.0   0.0   0:00.12 bash
+   1679 root      20   0    8604   3800   2912 S   0.0   0.0   0:01.69 crond
+   1681 root      20   0  231632  10580   5584 S   0.0   0.0   0:23.25 restrai+
    1716 root      20   0    7276   3808   3444 S   0.0   0.0   0:00.02 10_bash+
-   1742 root      20   0    7308   3736   3320 S   0.0   0.0   0:00.89 runtest+
+   1742 root      20   0    7308   3736   3320 S   0.0   0.0   3:43.81 runtest+
    1975 root      20   0    6464   1548   1312 S   0.0   0.0   0:00.02 rdma-ndd
-   2288 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-   2313 root      20   0       0      0      0 I   0.0   0.0   0:00.05 kworker+
-   2380 root      20   0       0      0      0 I   0.0   0.0   0:00.05 kworker+
-   2874 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-   2881 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-   3457 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
-   3462 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-   3617 root      20   0       0      0      0 I   0.0   0.0   0:00.04 kworker+
    3646 root      20   0   13516   7760   3920 S   0.0   0.0   0:00.13 opafmd
-   3647 root      20   0  912452 266228   8468 S   0.0   0.5   0:01.99 sm
-   3668 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
-   4029 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-   4082 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
-   4280 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
-   4366 root      20   0    5584   1032    940 S   0.0   0.0   0:00.00 sleep
-   4367 root      20   0   35204  30712  10240 S   0.0   0.1   0:01.22 python
-   4408 root      20   0    7120   3284   3028 S   0.0   0.0   0:00.00 sh
+   3647 root      20   0  912452 266956   8704 S   0.0   0.5  45:37.86 sm
+  25010 root      20   0       0      0      0 I   0.0   0.0   0:01.44 kworker+
+  51166 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
+  62138 root      20   0       0      0      0 I   0.0   0.0   0:00.65 kworker+
+  93565 root      20   0       0      0      0 I   0.0   0.0   0:00.56 kworker+
+ 109289 root      20   0       0      0      0 I   0.0   0.0   0:01.09 kworker+
+ 212823 root      20   0       0      0      0 I   0.0   0.0   0:02.10 kworker+
+ 300059 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 331127 root      20   0       0      0      0 I   0.0   0.0   0:00.87 kworker+
+ 331128 root      20   0       0      0      0 I   0.0   0.0   0:00.52 kworker+
+ 335538 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 382588 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+ 392910 root      20   0       0      0      0 I   0.0   0.0   0:00.18 kworker+
+ 398064 root      20   0       0      0      0 I   0.0   0.0   0:00.45 kworker+
+ 413038 root      20   0       0      0      0 I   0.0   0.0   0:00.88 kworker+
+ 424555 root      20   0       0      0      0 I   0.0   0.0   0:03.15 kworker+
+ 456211 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 463740 root      20   0       0      0      0 I   0.0   0.0   0:04.70 kworker+
+ 475216 root      20   0       0      0      0 I   0.0   0.0   0:00.37 kworker+
+ 475997 root      20   0       0      0      0 I   0.0   0.0   0:00.12 kworker+
+ 500947 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 503867 root      20   0       0      0      0 I   0.0   0.0   0:00.06 kworker+
+ 504587 root      20   0       0      0      0 I   0.0   0.0   0:00.31 kworker+
+ 508313 root      20   0       0      0      0 I   0.0   0.0   0:00.18 kworker+
+ 512538 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 513550 root      20   0       0      0      0 I   0.0   0.0   0:00.19 kworker+
+ 515158 root      20   0       0      0      0 I   0.0   0.0   0:00.10 kworker+
+ 515663 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 521024 root      20   0       0      0      0 I   0.0   0.0   0:00.04 kworker+
+ 523135 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 525195 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
+ 527040 root      20   0       0      0      0 I   0.0   0.0   0:00.19 kworker+
+ 527230 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
+ 528097 root      20   0       0      0      0 I   0.0   0.0   0:03.43 kworker+
+ 528959 root      20   0       0      0      0 I   0.0   0.0   0:00.07 kworker+
+ 529090 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+ 530363 root      20   0       0      0      0 I   0.0   0.0   0:00.12 kworker+
+ 530376 root      20   0       0      0      0 I   0.0   0.0   0:00.06 kworker+
+ 531107 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 531258 root      20   0       0      0      0 I   0.0   0.0   0:00.19 kworker+
+ 531583 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+ 531662 root      20   0       0      0      0 I   0.0   0.0   0:00.06 kworker+
+ 532219 root      20   0   18924  11448   9556 S   0.0   0.0   0:00.05 sshd
+ 532230 root      20   0   18784   6472   4584 S   0.0   0.0   0:00.14 sshd
+ 532231 root      20   0    7568   4444   3620 S   0.0   0.0   0:00.06 bash
+ 532232 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 532237 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 532238 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 532262 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+ 532293 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 532294 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+ 532295 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 532437 root      20   0    5584   1032    940 S   0.0   0.0   0:00.00 sleep
+ 532438 root      20   0   35352  30596  10144 S   0.0   0.1   0:01.61 python
+ 532482 root      20   0    7120   3304   3052 S   0.0   0.0   0:00.00 sh
```

### Comparing `python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/log` & `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/log`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/rdmaqe/tests/opa-fm/setup.py` & `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/setup.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/LICENSE` & `python_rdma_qe-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/pyproject.toml` & `python_rdma_qe-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.5/PKG-INFO` & `python_rdma_qe-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rdma-qe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Redhat Kernel RDMA QE Python libs and tests
 Project-URL: Documentation, https://gitlab.com/rh-rdma-qe/python-rdma-qe#README.md
 Project-URL: Issues, https://gitlab.com/rh-rdma-qe/python-rdma-qe/issues
 Project-URL: Source, https://gitlab.com/rh-rdma-qe/python-rdma-qe
 Author-email: Zhaojuan Guo <zguo@redhat.com>
 Maintainer-email: Zhaojuan Guo <zguo@redhat.com>
 License-Expression: GPL-3.0-or-later
```

