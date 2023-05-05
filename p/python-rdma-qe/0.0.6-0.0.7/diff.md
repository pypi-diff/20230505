# Comparing `tmp/python_rdma_qe-0.0.6.tar.gz` & `tmp/python_rdma_qe-0.0.7.tar.gz`

## Comparing `python_rdma_qe-0.0.6.tar` & `python_rdma_qe-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe_test.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/requirements-stable.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdmaqe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/cli.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/file_libs.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/fmf_tools.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/common/tc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/__init__.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/general.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/opa.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/roce.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/abc_sriov.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/.fmf/version
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/__init__.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/functional.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/init_mem.txt
--rw-r--r--   0        0        0    23790 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/init_top.txt
--rw-r--r--   0        0        0    16908 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/log
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/main.fmf
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/rdmaqe/tests/sriov/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/LICENSE
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/README.md
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe_test.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/requirements-stable.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdmaqe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/cli.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/file_libs.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/fmf_tools.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/tc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/__init__.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/general.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/opa.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/roce.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/rxe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/__init__.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/abc_sriov.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/.fmf/version
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/__init__.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/functional.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/init_mem.txt
+-rw-r--r--   0        0        0    23791 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/init_top.txt
+-rw-r--r--   0        0        0    16908 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/log
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/main.fmf
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/sriov/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/LICENSE
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/README.md
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/PKG-INFO
```

### Comparing `python_rdma_qe-0.0.6/rdmaqe_test.py` & `python_rdma_qe-0.0.7/rdmaqe_test.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/requirements-stable.txt` & `python_rdma_qe-0.0.7/requirements-stable.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/common/cli.py` & `python_rdma_qe-0.0.7/rdmaqe/common/cli.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/common/file_libs.py` & `python_rdma_qe-0.0.7/rdmaqe/common/file_libs.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/common/fmf_tools.py` & `python_rdma_qe-0.0.7/rdmaqe/common/fmf_tools.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/common/tc.py` & `python_rdma_qe-0.0.7/rdmaqe/common/tc.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/rdma/general.py` & `python_rdma_qe-0.0.7/rdmaqe/rdma/general.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/rdma/opa.py` & `python_rdma_qe-0.0.7/rdmaqe/rdma/opa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""roce.py: Module to check or configure OPA."""
+"""roce.py: Module to check or configure OPA HCA/fabric."""
 
 __author__ = "Zhaojuan Guo"
 __copyright__ = "Copyright (c) 2023 Red Hat, Inc. All rights reserved."
 
 import libsan.host.linux
 from libsan import _print
 from libsan.host.cmdline import run
```

### Comparing `python_rdma_qe-0.0.6/rdmaqe/rdma/roce.py` & `python_rdma_qe-0.0.7/rdmaqe/rdma/roce.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/abc_sriov.py` & `python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/abc_sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/rdma/sriov/sriov.py` & `python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/1.txt` & `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/1.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/functional.py` & `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/functional.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/init_top.txt` & `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/init_top.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-top - 22:36:55 up 14 days, 13:50,  1 user,  load average: 0.10, 0.03, 0.01
+top - 22:39:09 up 14 days, 13:52,  1 user,  load average: 0.10, 0.04, 0.01
 Tasks: 293 total,   1 running, 292 sleeping,   0 stopped,   0 zombie
 %Cpu(s):  0.3 us,  0.8 sy,  0.0 ni, 98.9 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
-MiB Mem :  47972.4 total,  44628.2 free,   2755.1 used,   2094.2 buff/cache
-MiB Swap:  24180.0 total,  24180.0 free,      0.0 used.  45217.3 avail Mem 
+MiB Mem :  47972.4 total,  44622.8 free,   2760.5 used,   2093.6 buff/cache
+MiB Swap:  24180.0 total,  24180.0 free,      0.0 used.  45212.0 avail Mem 
 
     PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND
- 532483 root      20   0   10700   4204   3392 R   5.6   0.0   0:00.03 top
-      1 root      20   0  173180  19528  10996 S   0.0   0.0   0:25.02 systemd
+ 532729 root      20   0   10700   4204   3396 R   5.9   0.0   0:00.02 top
+      1 root      20   0  173180  19544  10996 S   0.0   0.0   0:25.08 systemd
       2 root      20   0       0      0      0 S   0.0   0.0   0:00.46 kthreadd
       3 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rcu_gp
       4 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rcu_par+
       5 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 slub_fl+
       6 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 netns
       8 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      10 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
      12 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mm_perc+
      14 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
      15 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
      16 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_tas+
      17 root      20   0       0      0      0 S   0.0   0.0   0:00.76 ksoftir+
-     18 root      20   0       0      0      0 I   0.0   0.0   6:30.15 rcu_pre+
+     18 root      20   0       0      0      0 I   0.0   0.0   6:30.21 rcu_pre+
      19 root      rt   0       0      0      0 S   0.0   0.0   0:01.75 migrati+
      21 root      20   0       0      0      0 S   0.0   0.0   0:00.14 cpuhp/0
      22 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/1
      23 root      rt   0       0      0      0 S   0.0   0.0   0:01.93 migrati+
      24 root      20   0       0      0      0 S   0.0   0.0   0:00.18 ksoftir+
      26 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
      27 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/2
@@ -103,15 +103,15 @@
     141 root      20   0       0      0      0 S   0.0   0.0   0:00.01 kauditd
     146 root      20   0       0      0      0 S   0.0   0.0   0:00.31 khungta+
     147 root      20   0       0      0      0 S   0.0   0.0   0:00.00 oom_rea+
     148 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 writeba+
     149 root      20   0       0      0      0 S   0.0   0.0   0:09.59 kcompac+
     150 root      20   0       0      0      0 S   0.0   0.0   0:10.44 kcompac+
     151 root      25   5       0      0      0 S   0.0   0.0   0:00.00 ksmd
-    152 root      39  19       0      0      0 S   0.0   0.0   0:03.18 khugepa+
+    152 root      39  19       0      0      0 S   0.0   0.0   0:03.19 khugepa+
     153 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 cryptd
     154 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kintegr+
     155 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kblockd
     156 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 blkcg_p+
     170 root      20   0       0      0      0 I   0.0   0.0   0:01.47 kworker+
     174 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 tpm_dev+
     175 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 md
@@ -133,15 +133,15 @@
     205 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kstrp
     217 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 zswap-s+
     330 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     331 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     332 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker+
     333 root       0 -20       0      0      0 I   0.0   0.0   0:00.16 kworker+
     371 root       0 -20       0      0      0 I   0.0   0.0   0:00.21 kworker+
-    383 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
+    383 root       0 -20       0      0      0 I   0.0   0.0   0:00.04 kworker+
     391 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
     440 root       0 -20       0      0      0 I   0.0   0.0   0:02.82 kworker+
     483 root       0 -20       0      0      0 I   0.0   0.0   0:00.19 kworker+
     508 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
     538 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
     539 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
     552 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 tls-strp
@@ -170,18 +170,18 @@
     716 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-buf+
     717 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-con+
     718 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-rec+
     719 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-blo+
     720 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-ino+
     721 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-log+
     722 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-cil+
-    723 root      20   0       0      0      0 S   0.0   0.0   1:35.65 xfsaild+
+    723 root      20   0       0      0      0 S   0.0   0.0   1:35.66 xfsaild+
     769 root       0 -20       0      0      0 I   0.0   0.0   0:00.02 kworker+
     770 root       0 -20       0      0      0 I   0.0   0.0   0:00.03 kworker+
-    791 root      20   0  287996 164816 163556 S   0.0   0.3  63:29.21 systemd+
+    791 root      20   0  287996 164816 163556 S   0.0   0.3  63:29.23 systemd+
     804 root      20   0   35400  13784   9252 S   0.0   0.0   0:01.97 systemd+
     884 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-buf+
     885 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-con+
     886 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-rec+
     887 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-blo+
     888 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-ino+
     890 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xfs-log+
@@ -218,83 +218,83 @@
     972 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xcopy_wq
     973 root      16  -4   18144   4468   1700 S   0.0   0.0   0:00.65 auditd
    1012 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi1_up+
    1013 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi0_0
    1014 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 hfi_lin+
    1015 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rpciod
    1016 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 xprtiod
-   1023 root      20   0  257396  21872  16768 S   0.0   0.0  35:53.29 Network+
-   1028 root      20   0   79360   5400   2872 S   0.0   0.0   6:05.96 irqbala+
-   1030 root      20   0  624696  39184  37316 S   0.0   0.1 122:03.62 rsyslogd
-   1036 root      20   0   20388  11436   9028 S   0.0   0.0   0:02.02 systemd+
+   1023 root      20   0  257396  21872  16768 S   0.0   0.0  35:53.50 Network+
+   1028 root      20   0   79360   5400   2872 S   0.0   0.0   6:06.00 irqbala+
+   1030 root      20   0  624696  39184  37316 S   0.0   0.1 122:03.64 rsyslogd
+   1036 root      20   0   20388  11436   9028 S   0.0   0.0   0:02.03 systemd+
    1038 chrony    20   0   10440   3112   2612 S   0.0   0.0   0:02.24 chronyd
    1058 dbus      20   0   10792   4620   3932 S   0.0   0.0   0:00.04 dbus-br+
    1081 dbus      20   0    5260   2792   2368 S   0.0   0.0   0:00.83 dbus-br+
    1087 root      20   0   15836   9476   8172 S   0.0   0.0   0:00.04 sshd
    1094 root      20   0   81052   4452   2220 S   0.0   0.0   0:00.07 rhsmcer+
    1096 root      20   0    3044   1096   1008 S   0.0   0.0   0:00.03 agetty
    1097 root      20   0    5612   1100   1008 S   0.0   0.0   0:00.00 agetty
    1098 root      20   0   22388  13888  10664 S   0.0   0.0   0:00.51 systemd
    1109 root      20   0   25588   5456      0 S   0.0   0.0   0:00.00 (sd-pam)
    1125 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ib_mad1
    1126 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 ipoib_wq
    1679 root      20   0    8604   3800   2912 S   0.0   0.0   0:01.69 crond
    1681 root      20   0  231632  10580   5584 S   0.0   0.0   0:23.25 restrai+
    1716 root      20   0    7276   3808   3444 S   0.0   0.0   0:00.02 10_bash+
-   1742 root      20   0    7308   3736   3320 S   0.0   0.0   3:43.81 runtest+
+   1742 root      20   0    7308   3736   3320 S   0.0   0.0   3:43.84 runtest+
    1975 root      20   0    6464   1548   1312 S   0.0   0.0   0:00.02 rdma-ndd
-   3646 root      20   0   13516   7760   3920 S   0.0   0.0   0:00.13 opafmd
-   3647 root      20   0  912452 266956   8704 S   0.0   0.5  45:37.86 sm
   25010 root      20   0       0      0      0 I   0.0   0.0   0:01.44 kworker+
   51166 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
-  62138 root      20   0       0      0      0 I   0.0   0.0   0:00.65 kworker+
+  62138 root      20   0       0      0      0 I   0.0   0.0   0:00.66 kworker+
   93565 root      20   0       0      0      0 I   0.0   0.0   0:00.56 kworker+
  109289 root      20   0       0      0      0 I   0.0   0.0   0:01.09 kworker+
  212823 root      20   0       0      0      0 I   0.0   0.0   0:02.10 kworker+
  300059 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 331127 root      20   0       0      0      0 I   0.0   0.0   0:00.87 kworker+
+ 331127 root      20   0       0      0      0 I   0.0   0.0   0:00.88 kworker+
  331128 root      20   0       0      0      0 I   0.0   0.0   0:00.52 kworker+
  335538 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
  382588 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
  392910 root      20   0       0      0      0 I   0.0   0.0   0:00.18 kworker+
  398064 root      20   0       0      0      0 I   0.0   0.0   0:00.45 kworker+
- 413038 root      20   0       0      0      0 I   0.0   0.0   0:00.88 kworker+
  424555 root      20   0       0      0      0 I   0.0   0.0   0:03.15 kworker+
- 456211 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 463740 root      20   0       0      0      0 I   0.0   0.0   0:04.70 kworker+
+ 463740 root      20   0       0      0      0 I   0.0   0.0   0:04.71 kworker+
  475216 root      20   0       0      0      0 I   0.0   0.0   0:00.37 kworker+
  475997 root      20   0       0      0      0 I   0.0   0.0   0:00.12 kworker+
  500947 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
  503867 root      20   0       0      0      0 I   0.0   0.0   0:00.06 kworker+
  504587 root      20   0       0      0      0 I   0.0   0.0   0:00.31 kworker+
  508313 root      20   0       0      0      0 I   0.0   0.0   0:00.18 kworker+
- 512538 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 512538 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
  513550 root      20   0       0      0      0 I   0.0   0.0   0:00.19 kworker+
  515158 root      20   0       0      0      0 I   0.0   0.0   0:00.10 kworker+
  515663 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 521024 root      20   0       0      0      0 I   0.0   0.0   0:00.04 kworker+
  523135 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
  525195 root      20   0       0      0      0 I   0.0   0.0   0:00.09 kworker+
- 527040 root      20   0       0      0      0 I   0.0   0.0   0:00.19 kworker+
+ 527040 root      20   0       0      0      0 I   0.0   0.0   0:00.20 kworker+
  527230 root      20   0       0      0      0 I   0.0   0.0   0:00.01 kworker+
- 528097 root      20   0       0      0      0 I   0.0   0.0   0:03.43 kworker+
+ 528097 root      20   0       0      0      0 I   0.0   0.0   0:03.47 kworker+
  528959 root      20   0       0      0      0 I   0.0   0.0   0:00.07 kworker+
  529090 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
  530363 root      20   0       0      0      0 I   0.0   0.0   0:00.12 kworker+
- 530376 root      20   0       0      0      0 I   0.0   0.0   0:00.06 kworker+
+ 530376 root      20   0       0      0      0 I   0.0   0.0   0:00.07 kworker+
  531107 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
  531258 root      20   0       0      0      0 I   0.0   0.0   0:00.19 kworker+
  531583 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
  531662 root      20   0       0      0      0 I   0.0   0.0   0:00.06 kworker+
  532219 root      20   0   18924  11448   9556 S   0.0   0.0   0:00.05 sshd
- 532230 root      20   0   18784   6472   4584 S   0.0   0.0   0:00.14 sshd
- 532231 root      20   0    7568   4444   3620 S   0.0   0.0   0:00.06 bash
+ 532230 root      20   0   18784   6472   4584 S   0.0   0.0   0:00.20 sshd
+ 532231 root      20   0    7568   4444   3620 S   0.0   0.0   0:00.10 bash
  532232 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
  532237 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
  532238 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 532262 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
+ 532262 root      20   0       0      0      0 I   0.0   0.0   0:00.03 kworker+
  532293 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
  532294 root      20   0       0      0      0 I   0.0   0.0   0:00.02 kworker+
  532295 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
- 532437 root      20   0    5584   1032    940 S   0.0   0.0   0:00.00 sleep
- 532438 root      20   0   35352  30596  10144 S   0.0   0.1   0:01.61 python
- 532482 root      20   0    7120   3304   3052 S   0.0   0.0   0:00.00 sh
+ 532539 root      20   0   13516   7724   3888 S   0.0   0.0   0:00.13 opafmd
+ 532552 root      20   0  912452 263904   8548 S   0.0   0.5   0:00.42 sm
+ 532594 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 532611 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 532677 root      20   0    5584   1028    940 S   0.0   0.0   0:00.00 sleep
+ 532678 root      20   0   35352  30684  10228 S   0.0   0.1   0:01.53 python3
+ 532725 root      20   0       0      0      0 I   0.0   0.0   0:00.00 kworker+
+ 532728 root      20   0    7120   3260   3012 S   0.0   0.0   0:00.00 sh
```

### Comparing `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/log` & `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/log`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/rdmaqe/tests/opa-fm/setup.py` & `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/setup.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/LICENSE` & `python_rdma_qe-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/pyproject.toml` & `python_rdma_qe-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.6/PKG-INFO` & `python_rdma_qe-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rdma-qe
-Version: 0.0.6
+Version: 0.0.7
 Summary: Redhat Kernel RDMA QE Python libs and tests
 Project-URL: Documentation, https://gitlab.com/rh-rdma-qe/python-rdma-qe#README.md
 Project-URL: Issues, https://gitlab.com/rh-rdma-qe/python-rdma-qe/issues
 Project-URL: Source, https://gitlab.com/rh-rdma-qe/python-rdma-qe
 Author-email: Zhaojuan Guo <zguo@redhat.com>
 Maintainer-email: Zhaojuan Guo <zguo@redhat.com>
 License-Expression: GPL-3.0-or-later
```

