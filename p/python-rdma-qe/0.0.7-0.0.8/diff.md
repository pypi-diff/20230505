# Comparing `tmp/python_rdma_qe-0.0.7.tar.gz` & `tmp/python_rdma_qe-0.0.8.tar.gz`

## Comparing `python_rdma_qe-0.0.7.tar` & `python_rdma_qe-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe_test.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/requirements-stable.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdmaqe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/cli.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/file_libs.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/fmf_tools.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/common/tc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/__init__.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/general.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/opa.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/roce.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/rxe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/abc_sriov.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/.fmf/version
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/__init__.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/functional.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/init_mem.txt
--rw-r--r--   0        0        0    23791 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/init_top.txt
--rw-r--r--   0        0        0    16908 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/log
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/main.fmf
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/rdmaqe/tests/sriov/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/LICENSE
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/README.md
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe_test.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/requirements-stable.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdmaqe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/common/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/common/cli.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/common/file_libs.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/common/fmf_tools.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/common/tc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/__init__.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/general.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/opa.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/roce.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/rxe.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/siw.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/sriov/__init__.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/sriov/abc_sriov.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/rdma/sriov/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/.fmf/version
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/__init__.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/functional.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/init_mem.txt
+-rw-r--r--   0        0        0    23791 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/init_top.txt
+-rw-r--r--   0        0        0    16908 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/log
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/main.fmf
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/rdmaqe/tests/sriov/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/LICENSE
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/README.md
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.8/PKG-INFO
```

### Comparing `python_rdma_qe-0.0.7/rdmaqe_test.py` & `python_rdma_qe-0.0.8/rdmaqe_test.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/requirements-stable.txt` & `python_rdma_qe-0.0.8/requirements-stable.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/common/cli.py` & `python_rdma_qe-0.0.8/rdmaqe/common/cli.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/common/file_libs.py` & `python_rdma_qe-0.0.8/rdmaqe/common/file_libs.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/common/fmf_tools.py` & `python_rdma_qe-0.0.8/rdmaqe/common/fmf_tools.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/common/tc.py` & `python_rdma_qe-0.0.8/rdmaqe/common/tc.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/rdma/general.py` & `python_rdma_qe-0.0.8/rdmaqe/rdma/general.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/rdma/opa.py` & `python_rdma_qe-0.0.8/rdmaqe/rdma/opa.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/rdma/roce.py` & `python_rdma_qe-0.0.8/rdmaqe/rdma/roce.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/rdma/rxe.py` & `python_rdma_qe-0.0.8/rdmaqe/rdma/rxe.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/abc_sriov.py` & `python_rdma_qe-0.0.8/rdmaqe/rdma/sriov/abc_sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/rdma/sriov/sriov.py` & `python_rdma_qe-0.0.8/rdmaqe/rdma/sriov/sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/1.txt` & `python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/1.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/functional.py` & `python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/functional.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/init_top.txt` & `python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/init_top.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/log` & `python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/log`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/rdmaqe/tests/opa-fm/setup.py` & `python_rdma_qe-0.0.8/rdmaqe/tests/opa-fm/setup.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/LICENSE` & `python_rdma_qe-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/pyproject.toml` & `python_rdma_qe-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.7/PKG-INFO` & `python_rdma_qe-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rdma-qe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Redhat Kernel RDMA QE Python libs and tests
 Project-URL: Documentation, https://gitlab.com/rh-rdma-qe/python-rdma-qe#README.md
 Project-URL: Issues, https://gitlab.com/rh-rdma-qe/python-rdma-qe/issues
 Project-URL: Source, https://gitlab.com/rh-rdma-qe/python-rdma-qe
 Author-email: Zhaojuan Guo <zguo@redhat.com>
 Maintainer-email: Zhaojuan Guo <zguo@redhat.com>
 License-Expression: GPL-3.0-or-later
```

