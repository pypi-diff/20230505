# Comparing `tmp/cloudshell-shell-core-5.1.1.zip` & `tmp/cloudshell-shell-core-6.0.0.zip`

## zipinfo {}

```diff
@@ -1,71 +1,77 @@
-Zip file size: 31924 bytes, number of entries: 69
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/
--rw-r--r--  2.0 unx       38 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/setup.cfg
--rw-r--r--  2.0 unx      826 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/PKG-INFO
--rw-r--r--  2.0 unx       59 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/test_requirements.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/requirements.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/version.txt
--rw-r--r--  2.0 unx     1477 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/setup.py
--rw-r--r--  2.0 unx       54 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/README.txt
--rw-r--r--  2.0 unx       71 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/dev_requirements.txt
--rw-r--r--  2.0 unx       41 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/MANIFEST.in
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/
--rw-r--r--  2.0 unx       41 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx     2740 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1107 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      107 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip/_vendor/
--rw-r--r--  2.0 unx      476 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip/_vendor/vendor.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1093 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      124 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/interfaces/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/
--rw-r--r--  2.0 unx     1033 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/base_autoload_structure_generator.py
--rw-r--r--  2.0 unx     5452 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/orchestration_save_restore.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/__init__.py
--rw-r--r--  2.0 unx      536 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/driver_utils.py
--rw-r--r--  2.0 unx      227 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/resource_driver_interface.py
--rw-r--r--  2.0 unx      437 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/api_utils.py
--rw-r--r--  2.0 unx    11839 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/driver_context.py
--rw-r--r--  2.0 unx     5213 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/context_utils.py
--rw-r--r--  2.0 unx     2712 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/interfaces/save_restore.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/interfaces/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/__init__.py
--rw-r--r--  2.0 unx     4620 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/logging_session.py
--rw-r--r--  2.0 unx     2853 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/cloudshell_session.py
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/top_level.txt
--rw-r--r--  2.0 unx      826 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     1957 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/requires.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/interfaces/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/session/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/__init__.py
--rw-r--r--  2.0 unx     2486 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/test_orch_save_restore.py
--rw-r--r--  2.0 unx     4611 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/interfaces/test_save_and_restore.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/interfaces/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/utils/__init__.py
--rw-r--r--  2.0 unx      845 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/utils/test_api_utils.py
--rw-r--r--  2.0 unx     2992 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/utils/test_context_utils.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/session/__init__.py
--rw-r--r--  2.0 unx     5816 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/session/test_cloudshell_session.py
--rw-r--r--  2.0 unx    10297 b- defN 23-Mar-08 14:07 cloudshell-shell-core-5.1.1/tests/session/test_logging_session.py
-69 files, 73776 bytes uncompressed, 17794 bytes compressed:  75.9%
+Zip file size: 40513 bytes, number of entries: 75
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/
+-rw-r--r--  2.0 unx       29 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/test_requirements.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/version.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/setup.cfg
+-rw-r--r--  2.0 unx      102 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/requirements.txt
+-rw-r--r--  2.0 unx     1555 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/setup.py
+-rw-r--r--  2.0 unx      224 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/dev_requirements.txt
+-rw-r--r--  2.0 unx     3252 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/README.md
+-rw-r--r--  2.0 unx       41 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx      899 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/
+-rw-r--r--  2.0 unx       76 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/
+-rw-r--r--  2.0 unx       76 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/interfaces/
+-rw-r--r--  2.0 unx      227 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/resource_driver_interface.py
+-rw-r--r--  2.0 unx      437 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/api_utils.py
+-rw-r--r--  2.0 unx     5422 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/orchestration_save_restore.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/__init__.py
+-rw-r--r--  2.0 unx    11823 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/driver_context.py
+-rw-r--r--  2.0 unx     5186 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/context_utils.py
+-rw-r--r--  2.0 unx      528 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/driver_utils.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/base_autoload_structure_generator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/__init__.py
+-rw-r--r--  2.0 unx     2845 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/cloudshell_session.py
+-rw-r--r--  2.0 unx     5606 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/logging_session.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/utils/get_installed_packages.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/utils/__init__.py
+-rw-r--r--  2.0 unx     2680 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/interfaces/save_restore.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell/shell/core/interfaces/__init__.py
+-rw-r--r--  2.0 unx       17 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      102 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/requires.txt
+-rw-r--r--  2.0 unx     2111 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      899 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel/vendored/
+-rw-r--r--  2.0 unx       16 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel/vendored/vendor.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip/_vendor/
+-rw-r--r--  2.0 unx      476 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--  2.0 unx     1107 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      104 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     1093 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      125 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     9953 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       41 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/session/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/interfaces/
+-rw-r--r--  2.0 unx     2266 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/test_orch_save_restore.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/__init__.py
+-rw-r--r--  2.0 unx     5686 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/session/test_cloudshell_session.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/session/__init__.py
+-rw-r--r--  2.0 unx     9409 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/session/test_logging_session.py
+-rw-r--r--  2.0 unx      718 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/utils/test_api_utils.py
+-rw-r--r--  2.0 unx     2858 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/utils/test_context_utils.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/utils/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/interfaces/__init__.py
+-rw-r--r--  2.0 unx     4611 b- defN 23-May-05 07:46 cloudshell-shell-core-6.0.0/tests/interfaces/test_save_and_restore.py
+75 files, 87041 bytes uncompressed, 25035 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,208 +1,226 @@
-Filename: cloudshell-shell-core-5.1.1/
+Filename: cloudshell-shell-core-6.0.0/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/
+Filename: cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/
+Filename: cloudshell-shell-core-6.0.0/.tox/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/
+Filename: cloudshell-shell-core-6.0.0/tests/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/setup.cfg
+Filename: cloudshell-shell-core-6.0.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/PKG-INFO
+Filename: cloudshell-shell-core-6.0.0/version.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/test_requirements.txt
+Filename: cloudshell-shell-core-6.0.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/requirements.txt
+Filename: cloudshell-shell-core-6.0.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/version.txt
+Filename: cloudshell-shell-core-6.0.0/setup.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/setup.py
+Filename: cloudshell-shell-core-6.0.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/README.txt
+Filename: cloudshell-shell-core-6.0.0/README.md
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/dev_requirements.txt
+Filename: cloudshell-shell-core-6.0.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/MANIFEST.in
+Filename: cloudshell-shell-core-6.0.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/utils/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/interfaces/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/resource_driver_interface.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/top_level.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/api_utils.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/entry_points.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/orchestration_save_restore.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/top_level.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/LICENSE.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/driver_context.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/entry_points.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/context_utils.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip/_vendor/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/driver_utils.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip/_vendor/vendor.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/base_autoload_structure_generator.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/top_level.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/LICENSE.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/cloudshell_session.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/entry_points.txt
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/logging_session.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/utils/get_installed_packages.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/__init__.py
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/utils/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/interfaces/save_restore.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-core-6.0.0/cloudshell/shell/core/interfaces/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/interfaces/
+Filename: cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/
+Filename: cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/base_autoload_structure_generator.py
+Filename: cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/orchestration_save_restore.py
+Filename: cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/__init__.py
+Filename: cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/driver_utils.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/resource_driver_interface.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/api_utils.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/driver_context.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/context_utils.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/interfaces/save_restore.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/interfaces/__init__.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/__init__.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/logging_session.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/cloudshell_session.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel/vendored/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/top_level.txt
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel/vendored/vendor.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/PKG-INFO
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip/_vendor/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/dependency_links.txt
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip/_vendor/vendor.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/SOURCES.txt
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/requires.txt
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/interfaces/
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/utils/
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/session/
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/__init__.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/test_orch_save_restore.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/interfaces/test_save_and_restore.py
+Filename: cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/interfaces/__init__.py
+Filename: cloudshell-shell-core-6.0.0/tests/session/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/utils/__init__.py
+Filename: cloudshell-shell-core-6.0.0/tests/utils/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/utils/test_api_utils.py
+Filename: cloudshell-shell-core-6.0.0/tests/interfaces/
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/utils/test_context_utils.py
+Filename: cloudshell-shell-core-6.0.0/tests/test_orch_save_restore.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/session/__init__.py
+Filename: cloudshell-shell-core-6.0.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/session/test_cloudshell_session.py
+Filename: cloudshell-shell-core-6.0.0/tests/session/test_cloudshell_session.py
 Comment: 
 
-Filename: cloudshell-shell-core-5.1.1/tests/session/test_logging_session.py
+Filename: cloudshell-shell-core-6.0.0/tests/session/__init__.py
+Comment: 
+
+Filename: cloudshell-shell-core-6.0.0/tests/session/test_logging_session.py
+Comment: 
+
+Filename: cloudshell-shell-core-6.0.0/tests/utils/test_api_utils.py
+Comment: 
+
+Filename: cloudshell-shell-core-6.0.0/tests/utils/test_context_utils.py
+Comment: 
+
+Filename: cloudshell-shell-core-6.0.0/tests/utils/__init__.py
+Comment: 
+
+Filename: cloudshell-shell-core-6.0.0/tests/interfaces/__init__.py
+Comment: 
+
+Filename: cloudshell-shell-core-6.0.0/tests/interfaces/test_save_and_restore.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-shell-core-5.1.1/PKG-INFO` & `cloudshell-shell-core-6.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: cloudshell-shell-core
-Version: 5.1.1
+Version: 6.0.0
 Summary: Core package for all CloudShell Shells. This package contains the basic driver interfaces and metadata definitions as well as utilities and helpers created specifically for Shells
 Home-page: https://github.com/QualiSystems/cloudshell-shell-core
 Author: Quali
 Author-email: info@quali.com
 License: Apache 2.0
 Keywords: sandbox cloud cmp cloudshell
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: ~=3.7
 
 Core package for all CloudShell Shells. This package contains the basic driver interfaces and metadata definitions as well as utilities and helpers created specifically for Shells
```

## Comparing `cloudshell-shell-core-5.1.1/setup.py` & `cloudshell-shell-core-6.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     name="cloudshell-shell-core",
     url="https://github.com/QualiSystems/cloudshell-shell-core",
     author="Quali",
     license="Apache 2.0",
     author_email="info@quali.com",
     packages=find_packages(),
     install_requires=required,
+    python_requires="~=3.7",
     tests_require=required_for_tests,
     version=version_from_file,
     description=(
         "Core package for all CloudShell Shells. This package contains the basic "
         "driver interfaces and metadata definitions as well as utilities and helpers "
         "created specifically for Shells"
     ),
@@ -31,12 +32,13 @@
         "driver interfaces and metadata definitions as well as utilities and helpers "
         "created specifically for Shells"
     ),
     include_package_data=True,
     keywords="sandbox cloud cmp cloudshell",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
-        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries",
         "License :: OSI Approved :: Apache Software License",
     ],
 )
```

## Comparing `cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/entry_points.txt` & `cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/LICENSE.txt` & `cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-core-5.1.1/.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/LICENSE.txt` & `cloudshell-shell-core-6.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-core-5.1.1/cloudshell/shell/core/base_autoload_structure_generator.py` & `cloudshell-shell-core-6.0.0/cloudshell/shell/core/base_autoload_structure_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cloudshell.shell.core.driver_context import AutoLoadAttribute, AutoLoadResource
 
 
-class BaseResource(object):
+class BaseResource:
     def __init__(self, resource_model="", name="", relative_address="", unique_id=None):
         self.resource_model = resource_model
         self.name = name
         self.relative_address = relative_address
         self.unique_id = unique_id
         self.attributes = {}
```

## Comparing `cloudshell-shell-core-5.1.1/cloudshell/shell/core/orchestration_save_restore.py` & `cloudshell-shell-core-6.0.0/cloudshell/shell/core/orchestration_save_restore.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import datetime
+import logging
 
 import jsonpickle
 
 from cloudshell.shell.core.interfaces.save_restore import (
     OrchestrationRestoreRules,
     OrchestrationSavedArtifact,
     OrchestrationSavedArtifactInfo,
     OrchestrationSaveResult,
 )
 
+logger = logging.getLogger(__name__)
 
-class OrchestrationSaveRestore(object):
+
+class OrchestrationSaveRestore:
     REQUIRED_SAVE_ATTRIBUTES_LIST = [
         "resource_name",
         ("saved_artifact", "identifier"),
         ("saved_artifact", "artifact_type"),
         ("restore_rules", "requires_same_resource"),
     ]
 
-    def __init__(self, logger, resource_name):
+    def __init__(self, resource_name: str):
         self._resource_name = resource_name
-        self._logger = logger
 
     def prepare_orchestration_save_result(self, saved_file_path):
         artifact_type = saved_file_path.split(":")[0]
-        identifier = saved_file_path.replace("{0}:".format(artifact_type), "")
+        identifier = saved_file_path.replace(f"{artifact_type}:", "")
         saved_artifact = OrchestrationSavedArtifact(
             identifier=identifier, artifact_type=artifact_type
         )
         saved_artifact_info = OrchestrationSavedArtifactInfo(
             resource_name=self._resource_name,
             created_date=datetime.datetime.now(),
             restore_rules=self._get_restore_rules(),
@@ -61,23 +63,23 @@
         if (
             saved_config.get("restore_rules", {}).get("requires_same_resource")
             and saved_config.get("resource_name", "").lower()
             != self._resource_name.lower()
         ):
             raise Exception(
                 "ConfigurationOperations",
-                "Incompatible resource, expected {}".format(self._resource_name),
+                f"Incompatible resource, expected {self._resource_name}",
             )
 
         saved_artifact_dict = saved_config.get("saved_artifact", {})
         if not saved_artifact_dict:
             raise Exception()
         scheme = saved_artifact_dict.get("artifact_type")
         url_path = saved_artifact_dict.get("identifier")
-        path = "{}:{}".format(scheme, url_path)
+        path = f"{scheme}:{url_path}"
         restore_params = {
             "configuration_type": "running",
             "restore_method": "override",
             "vrf_management_name": None,
             "path": path,
         }
 
@@ -120,24 +122,24 @@
                 if not hasattr(saved_config, class_attribute):
                     is_fail = True
                     fail_attribute = class_attribute
 
         if is_fail:
             raise Exception(
                 "ConfigurationOperations",
-                "Mandatory field {0} is missing in Saved Artifact Info "
-                "request json".format(fail_attribute),
+                f"Mandatory field {fail_attribute} is missing in Saved Artifact Info "
+                "request json",
             )
 
     def _validate_custom_params(self, custom_params):
         if not custom_params.get("custom_params"):
             raise Exception(
                 "ConfigurationOperations", "custom_params attribute is empty"
             )
 
     def _get_restore_rules(self):
         """Populate required restore rules.
 
         :return OrchestrationRestoreRules: response
         """
-        self._logger.info("Creating Restore Rules")
+        logger.info("Creating Restore Rules")
         return OrchestrationRestoreRules(True)
```

## Comparing `cloudshell-shell-core-5.1.1/cloudshell/shell/core/driver_utils.py` & `cloudshell-shell-core-6.0.0/cloudshell/shell/core/driver_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import wraps
 from threading import Event, Lock
 
 
-class GlobalLock(object):
+class GlobalLock:
     _event = Event()
     _event.set()
     _lock = Lock()
 
     @staticmethod
     def lock(func):
         @wraps(func)
```

## Comparing `cloudshell-shell-core-5.1.1/cloudshell/shell/core/driver_context.py` & `cloudshell-shell-core-6.0.0/cloudshell/shell/core/driver_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,15 @@
     def __init__(self, connectivity, resource, remote_reservation, remote_endpoints):
         self.connectivity = connectivity
         self.resource = resource
         self.remote_reservation = remote_reservation
         self.remote_endpoints = remote_endpoints
 
 
-class ApiVmDetails(object):
+class ApiVmDetails:
     """API VM details.
 
     :param CloudProviderName: The name of the cloud provider
     :type CloudProviderName: str
 
     :param UID: UUID of the created VM
     :type UID: str
@@ -420,15 +420,15 @@
 
     def __init__(self, cloud_provider_name="", uid="", vm_custom_params=None):
         self.CloudProviderName = cloud_provider_name
         self.UID = uid
         self.VmCustomParams = vm_custom_params or []
 
 
-class ApiVmCustomParam(object):
+class ApiVmCustomParam:
     """API VM custom param.
 
     :type Name: str
     :type Value: str
     """
 
     def __init__(self, name="", value=""):
```

## Comparing `cloudshell-shell-core-5.1.1/cloudshell/shell/core/context_utils.py` & `cloudshell-shell-core-6.0.0/cloudshell/shell/core/context_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         _CONTEXT_CONTAINER.get(currentThread(), None)
     resource = get_resource_context_details(context)
     if resource and hasattr(resource, attribute):
         return getattr(resource, attribute)
     else:
         raise Exception(
             "get_resource_context_attribute",
-            "Resource context does not have attribute {0}".format(attribute),
+            f"Resource context does not have attribute {attribute}",
         )
 
 
 def get_attribute_by_name(attribute_name, context=None):
     """Return attribute from attributes or resource context."""
     attributes = get_resource_context_attribute(context=context, attribute="attributes")
     resolved_attribute = None
@@ -127,15 +127,15 @@
     """Helps to get reservation context attribute."""
     reservation = get_reservation_context_details(context)
     if reservation and hasattr(reservation, attribute):
         return getattr(reservation, attribute)
     else:
         raise Exception(
             "get_reservation_context_attribute",
-            "Reservation context does not have attribute {0}".format(attribute),
+            f"Reservation context does not have attribute {attribute}",
         )
 
 
 def get_connectivity_context_details(context=None):
     """Helps to get connectivity context details."""
     if not context:
         _CONTEXT_CONTAINER.get(currentThread(), None)
@@ -152,9 +152,9 @@
     """Helps to get connectivity context attribute."""
     connectivity = get_connectivity_context_details(context)
     if connectivity and hasattr(connectivity, attribute):
         return getattr(connectivity, attribute)
     else:
         raise Exception(
             "get_connectivity_context_attribute",
-            "Connectivity context does not have attribute {0}".format(attribute),
+            f"Connectivity context does not have attribute {attribute}",
         )
```

## Comparing `cloudshell-shell-core-5.1.1/cloudshell/shell/core/interfaces/save_restore.py` & `cloudshell-shell-core-6.0.0/cloudshell/shell/core/interfaces/save_restore.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class OrchestrationSavedArtifact(object):
+class OrchestrationSavedArtifact:
     def __init__(self, artifact_type, identifier):
         """Represents a saved artifact according to the save and restore standard.
 
         This is a base class which can be extended with additional attributes
         required to later restore the artifact such as location or credentials.
 
         :param artifact_type: Describes the type of saved artifact
@@ -13,39 +13,39 @@
         (e.g the image url, a file full path)
         :type identifier: str
         """
         self.artifact_type = artifact_type
         self.identifier = identifier
 
 
-class OrchestrationSaveResult(object):
+class OrchestrationSaveResult:
     def __init__(self, saved_artifacts_info):
         """Container class for the orchestration_save result.
 
         :param saved_artifacts_info: An object describing the artifacts saved by
          this operation
         :type saved_artifacts_info: OrchestrationSavedArtifactInfo
         """
         self.saved_artifacts_info = saved_artifacts_info
 
 
-class OrchestrationRestoreRules(object):
+class OrchestrationRestoreRules:
     def __init__(self, requires_same_resource, additional_rules=None):
         """Container class for the orchestration_save result.
 
         :type additional_rules: dict
         """
         if not additional_rules:
             additional_rules = {}
         self.requires_same_resource = requires_same_resource
         for rule in additional_rules:
             setattr(self, rule, additional_rules[rule])
 
 
-class OrchestrationSavedArtifactInfo(object):
+class OrchestrationSavedArtifactInfo:
     def __init__(self, resource_name, created_date, restore_rules, saved_artifact):
         """This object describes the saved artifacts from a specific save operation.
 
         This information is stored and may later be sent to the Shell as a part of
         a restore operation.
 
         :param resource_name: The name of the resource on which the save operation
```

## Comparing `cloudshell-shell-core-5.1.1/cloudshell/shell/core/session/cloudshell_session.py` & `cloudshell-shell-core-6.0.0/cloudshell/shell/core/session/cloudshell_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cloudshell.api.cloudshell_api import CloudShellAPISession
 
 
-class CloudShellSessionContext(object):
+class CloudShellSessionContext:
     DEFAULT_DOMAIN = "Global"
     DEFAULT_API_SCHEME = "http"
 
     def __init__(self, context):
         """Initializes an instance of CloudShellSessionContext.
 
         :param context: Command context
```

## Comparing `cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/PKG-INFO` & `cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: cloudshell-shell-core
-Version: 5.1.1
+Version: 6.0.0
 Summary: Core package for all CloudShell Shells. This package contains the basic driver interfaces and metadata definitions as well as utilities and helpers created specifically for Shells
 Home-page: https://github.com/QualiSystems/cloudshell-shell-core
 Author: Quali
 Author-email: info@quali.com
 License: Apache 2.0
 Keywords: sandbox cloud cmp cloudshell
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: ~=3.7
 
 Core package for all CloudShell Shells. This package contains the basic driver interfaces and metadata definitions as well as utilities and helpers created specifically for Shells
```

## Comparing `cloudshell-shell-core-5.1.1/cloudshell_shell_core.egg-info/SOURCES.txt` & `cloudshell-shell-core-6.0.0/cloudshell_shell_core.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 MANIFEST.in
-README.txt
+README.md
 dev_requirements.txt
 requirements.txt
 setup.py
 test_requirements.txt
 version.txt
-.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/LICENSE.txt
-.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/entry_points.txt
-.tox/build/lib/python3.7/site-packages/pip-23.0.1.dist-info/top_level.txt
-.tox/build/lib/python3.7/site-packages/pip/_vendor/vendor.txt
-.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/entry_points.txt
-.tox/build/lib/python3.7/site-packages/setuptools-67.4.0.dist-info/top_level.txt
-.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/LICENSE.txt
-.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/entry_points.txt
-.tox/build/lib/python3.7/site-packages/wheel-0.38.4.dist-info/top_level.txt
+.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/entry_points.txt
+.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/top_level.txt
+.tox/build/lib/python3.9/site-packages/pip/_vendor/vendor.txt
+.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/entry_points.txt
+.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/top_level.txt
+.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
+.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/entry_points.txt
+.tox/build/lib/python3.9/site-packages/wheel/vendored/vendor.txt
 cloudshell/__init__.py
 cloudshell/shell/__init__.py
 cloudshell/shell/core/__init__.py
 cloudshell/shell/core/api_utils.py
 cloudshell/shell/core/base_autoload_structure_generator.py
 cloudshell/shell/core/context_utils.py
 cloudshell/shell/core/driver_context.py
@@ -25,14 +26,16 @@
 cloudshell/shell/core/orchestration_save_restore.py
 cloudshell/shell/core/resource_driver_interface.py
 cloudshell/shell/core/interfaces/__init__.py
 cloudshell/shell/core/interfaces/save_restore.py
 cloudshell/shell/core/session/__init__.py
 cloudshell/shell/core/session/cloudshell_session.py
 cloudshell/shell/core/session/logging_session.py
+cloudshell/shell/core/utils/__init__.py
+cloudshell/shell/core/utils/get_installed_packages.py
 cloudshell_shell_core.egg-info/PKG-INFO
 cloudshell_shell_core.egg-info/SOURCES.txt
 cloudshell_shell_core.egg-info/dependency_links.txt
 cloudshell_shell_core.egg-info/requires.txt
 cloudshell_shell_core.egg-info/top_level.txt
 tests/__init__.py
 tests/test_orch_save_restore.py
```

## Comparing `cloudshell-shell-core-5.1.1/tests/test_orch_save_restore.py` & `cloudshell-shell-core-6.0.0/tests/test_orch_save_restore.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,31 @@
-import sys
 from unittest import TestCase
 
 import jsonpickle
 from jsonschema import validate
 
 from cloudshell.shell.core.orchestration_save_restore import OrchestrationSaveRestore
 
 from tests.interfaces.test_save_and_restore import get_schema
 
-if sys.version_info >= (3, 0):
-    from unittest.mock import MagicMock
-else:
-    from mock import MagicMock
-
 
 class TestOrchestrationSaveRestore(TestCase):
     def setUp(self):
-        logger = MagicMock()
         resource_name = "Test"
-        self._orch_obj = OrchestrationSaveRestore(
-            logger=logger, resource_name=resource_name
-        )
+        self._orch_obj = OrchestrationSaveRestore(resource_name)
 
     def test_prepare_orchestration_save_result(self):
         file_path = "tftp://127.0.0.1/Test Folder/file.name"
         response = self._orch_obj.prepare_orchestration_save_result(file_path)
         validate(jsonpickle.loads(response), schema=get_schema())
 
     def test_parse_orch_save_result_no_custom_params(self):
         scheme = "tftp"
         folder_path = "//127.0.0.1/Test Folder/file.name"
-        file_path = "{}:{}".format(scheme, folder_path)
+        file_path = f"{scheme}:{folder_path}"
         saved_artifact_info = self._orch_obj.prepare_orchestration_save_result(
             file_path
         )
         custom_params = None
         response = self._orch_obj.parse_orchestration_save_result(
             saved_artifact_info, custom_params
         )
@@ -48,15 +39,15 @@
                 {
                 "custom_params": {
                         "vrf_management_name": "network-1"
                         }
                 }"""
         scheme = "tftp"
         folder_path = "//127.0.0.1/Test Folder/file.name"
-        file_path = "{}:{}".format(scheme, folder_path)
+        file_path = f"{scheme}:{folder_path}"
         saved_artifact_info = self._orch_obj.prepare_orchestration_save_result(
             file_path
         )
         response = self._orch_obj.parse_orchestration_save_result(
             saved_artifact_info, custom_params
         )
         self.assertEqual(response.get("configuration_type"), "running")
```

## Comparing `cloudshell-shell-core-5.1.1/tests/interfaces/test_save_and_restore.py` & `cloudshell-shell-core-6.0.0/tests/interfaces/test_save_and_restore.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-core-5.1.1/tests/utils/test_api_utils.py` & `cloudshell-shell-core-6.0.0/tests/utils/test_api_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,12 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
-import sys
 from unittest import TestCase
+from unittest.mock import MagicMock
 
 from cloudshell.shell.core.api_utils import decrypt_password_from_attribute
 
-if sys.version_info >= (3, 0):
-    from unittest.mock import MagicMock
-else:
-    from mock import MagicMock
-
 
 class TestApiUtils(TestCase):
     def setUp(self):
         self.context = MagicMock()
 
     def test_decrypt_password_by_attribute_name(self):
         password = "test_password"
```

## Comparing `cloudshell-shell-core-5.1.1/tests/utils/test_context_utils.py` & `cloudshell-shell-core-6.0.0/tests/utils/test_context_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
-import sys
 from unittest import TestCase
+from unittest.mock import MagicMock, patch
 
 from cloudshell.shell.core.context_utils import (
     get_attribute_by_name,
     get_connectivity_context_attribute,
     get_context,
     get_reservation_context_attribute,
     get_resource_address,
     get_resource_name,
     put_context,
 )
 
-if sys.version_info >= (3, 0):
-    from unittest.mock import MagicMock, patch
-else:
-    from mock import MagicMock, patch
-
 
 class TestContextUtils(TestCase):
     def setUp(self):
         self.context = MagicMock()
 
     def test_put_and_get_context(self):
         put_context(self.context)
```

## Comparing `cloudshell-shell-core-5.1.1/tests/session/test_cloudshell_session.py` & `cloudshell-shell-core-6.0.0/tests/session/test_cloudshell_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-import sys
-from unittest import TestCase
+from unittest import TestCase, mock
+from unittest.mock import MagicMock, Mock
 
 from cloudshell.shell.core.driver_context import (
     ConnectivityContext,
     ReservationContextDetails,
     ResourceCommandContext,
     ResourceContextDetails,
     ResourceRemoteCommandContext,
 )
 from cloudshell.shell.core.session.cloudshell_session import CloudShellSessionContext
 
-if sys.version_info >= (3, 0):
-    from unittest import mock
-    from unittest.mock import MagicMock, Mock
-else:
-    import mock
-    from mock import MagicMock, Mock
-
 
 class TestCloudShellSessionContext(TestCase):
     def test_cloudshell_session_context_proper_initialized(self):
         # Arrange
         context = mock.create_autospec(ResourceCommandContext)
         context.connectivity = mock.create_autospec(ConnectivityContext)
         context.connectivity.server_address = "localhost"
```

## Comparing `cloudshell-shell-core-5.1.1/tests/session/test_logging_session.py` & `cloudshell-shell-core-6.0.0/tests/session/test_logging_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-import sys
-from unittest import TestCase
+import platform
+from unittest import TestCase, mock
 
 from cloudshell.logging.qs_logger import _LOGGER_CONTAINER
 
 from cloudshell.shell.core.driver_context import (
     AutoLoadCommandContext,
     ReservationContextDetails,
     ResourceCommandContext,
@@ -12,105 +12,89 @@
     ResourceRemoteCommandContext,
 )
 from cloudshell.shell.core.session.logging_session import (
     INVENTORY,
     LoggingSessionContext,
 )
 
-if sys.version_info >= (3, 0):
-    from unittest import mock
-else:
-    import mock
-
 
 class TestLoggingSessionContext(TestCase):
     def setUp(self):
         # Clear loggers between tests
         _LOGGER_CONTAINER.clear()
 
     @mock.patch("cloudshell.shell.core.session.logging_session.get_qs_logger")
-    @mock.patch("cloudshell.shell.core.session.logging_session.log_execution_info")
     @mock.patch(
         "cloudshell.shell.core.session.logging_session.LoggingSessionContext"
         ".get_execution_info"
     )
     def test_logger_initialized_for_autoload_context(
-        self, get_execution_info, log_execution_info, get_qs_logger
+        self, get_execution_info, get_qs_logger
     ):
         # Arrange
         auto_load_context = mock.create_autospec(AutoLoadCommandContext)
         auto_load_context.resource = mock.create_autospec(ResourceContextDetails)
         auto_load_context.resource.name = "my_device"
 
         execution_info = mock.Mock()
         get_execution_info.return_value = execution_info
 
         qs_logger = mock.Mock()
-        child_logger = mock.Mock()
-        qs_logger.getChild.return_value = child_logger
-        qs_logger.handlers = [mock.Mock()]
-        qs_logger.filters = [mock.Mock()]
         get_qs_logger.return_value = qs_logger
 
         # Act
         with LoggingSessionContext(auto_load_context) as logger:
             get_execution_info.assert_called_once_with(auto_load_context)
             get_qs_logger.assert_called_once_with(
                 log_group=INVENTORY,
-                log_category="QS",
+                log_category="cloudshell",
                 log_file_prefix=auto_load_context.resource.name,
+                exec_info=execution_info,
             )
-            log_execution_info.assert_called_once_with(qs_logger, execution_info)
-            self.assertEqual(child_logger, logger)
+            assert logger == qs_logger
 
     @mock.patch("cloudshell.shell.core.session.logging_session.get_qs_logger")
-    @mock.patch("cloudshell.shell.core.session.logging_session.log_execution_info")
     @mock.patch(
         "cloudshell.shell.core.session.logging_session.LoggingSessionContext"
         ".get_execution_info"
     )
     def test_logger_initialized_for_resource_context_without_reservation(
-        self, get_execution_info, log_execution_info, get_qs_logger
+        self, get_execution_info, get_qs_logger
     ):
         # Arrange
         resource_command_context = mock.create_autospec(ResourceCommandContext)
         resource_command_context.resource = mock.create_autospec(ResourceContextDetails)
         resource_command_context.resource.name = "my_device"
         resource_command_context.reservation = None
 
         execution_info = mock.Mock()
         get_execution_info.return_value = execution_info
 
         qs_logger = mock.Mock()
-        child_logger = mock.Mock()
-        qs_logger.getChild.return_value = child_logger
-        qs_logger.handlers = [mock.Mock()]
-        qs_logger.filters = [mock.Mock()]
         get_qs_logger.return_value = qs_logger
 
         # Act
         with LoggingSessionContext(resource_command_context) as logger:
             # Assert
             get_execution_info.assert_called_once_with(resource_command_context)
             get_qs_logger.assert_called_once_with(
                 log_group=INVENTORY,
-                log_category="QS",
+                log_category="cloudshell",
                 log_file_prefix=resource_command_context.resource.name,
+                exec_info=execution_info,
             )
-            log_execution_info.assert_called_once_with(qs_logger, execution_info)
-            self.assertEqual(child_logger, logger)
+            assert logger == qs_logger
 
     @mock.patch("cloudshell.shell.core.session.logging_session.get_qs_logger")
-    @mock.patch("cloudshell.shell.core.session.logging_session.log_execution_info")
     @mock.patch(
         "cloudshell.shell.core.session.logging_session.LoggingSessionContext"
         ".get_execution_info"
     )
     def test_logger_initialized_for_resource_context_with_reservation(
-        self, get_execution_info, log_execution_info, get_qs_logger
+        self, get_execution_info, get_qs_logger
     ):
         # Arrange
         resource_command_context = mock.create_autospec(ResourceCommandContext)
         resource_command_context.resource = mock.create_autospec(ResourceContextDetails)
         resource_command_context.resource.name = "my_device"
         resource_command_context.reservation = mock.create_autospec(
             ReservationContextDetails
@@ -120,80 +104,70 @@
         reservation_id = mock.Mock()
         resource_command_context.reservation.reservation_id = reservation_id
 
         execution_info = mock.Mock()
         get_execution_info.return_value = execution_info
 
         qs_logger = mock.Mock()
-        child_logger = mock.Mock()
-        qs_logger.getChild.return_value = child_logger
-        qs_logger.handlers = [mock.Mock()]
-        qs_logger.filters = [mock.Mock()]
         get_qs_logger.return_value = qs_logger
 
         # Act
         with LoggingSessionContext(resource_command_context) as logger:
             # Assert
             get_execution_info.assert_called_once_with(resource_command_context)
             get_qs_logger.assert_called_once_with(
                 log_group=reservation_id,
-                log_category="QS",
+                log_category="cloudshell",
                 log_file_prefix=resource_command_context.resource.name,
+                exec_info=execution_info,
             )
-            log_execution_info.assert_called_once_with(qs_logger, execution_info)
-            self.assertEqual(child_logger, logger)
+            assert logger == qs_logger
 
     @mock.patch("cloudshell.shell.core.session.logging_session.get_qs_logger")
-    @mock.patch("cloudshell.shell.core.session.logging_session.log_execution_info")
     @mock.patch(
         "cloudshell.shell.core.session.logging_session.LoggingSessionContext"
         ".get_execution_info"
     )
     def test_logger_initialized_for_remote_context_without_reservation(
-        self, get_execution_info, log_execution_info, get_qs_logger
+        self, get_execution_info, get_qs_logger
     ):
         # Arrange
         remote_command_context = mock.create_autospec(ResourceRemoteCommandContext)
         remote_command_context.resource = mock.create_autospec(ResourceContextDetails)
         remote_command_context.resource.name = "my_device"
         remote_command_context.remote_reservation = None
         remote_endpoint = mock.create_autospec(ResourceContextDetails)
         remote_endpoint.name = "connected_device"
         remote_command_context.remote_endpoints = [remote_endpoint]
 
         execution_info = mock.Mock()
         get_execution_info.return_value = execution_info
 
         qs_logger = mock.Mock()
-        child_logger = mock.Mock()
-        qs_logger.getChild.return_value = child_logger
-        qs_logger.handlers = [mock.Mock()]
-        qs_logger.filters = [mock.Mock()]
         get_qs_logger.return_value = qs_logger
 
         # Act
         with LoggingSessionContext(remote_command_context) as logger:
             # Assert
             get_execution_info.assert_called_once_with(remote_command_context)
             get_qs_logger.assert_called_once_with(
                 log_group=INVENTORY,
-                log_category="QS",
-                log_file_prefix=remote_endpoint.name,
+                log_category="cloudshell",
+                log_file_prefix=remote_command_context.resource.name,
+                exec_info=execution_info,
             )
-            log_execution_info.assert_called_once_with(qs_logger, execution_info)
-            self.assertEqual(child_logger, logger)
+            assert logger == qs_logger
 
     @mock.patch("cloudshell.shell.core.session.logging_session.get_qs_logger")
-    @mock.patch("cloudshell.shell.core.session.logging_session.log_execution_info")
     @mock.patch(
         "cloudshell.shell.core.session.logging_session.LoggingSessionContext"
         ".get_execution_info"
     )
     def test_logger_initialized_for_remote_context_with_reservation(
-        self, get_execution_info, log_execution_info, get_qs_logger
+        self, get_execution_info, get_qs_logger
     ):
         # Arrange
         remote_command_context = mock.create_autospec(ResourceRemoteCommandContext)
         remote_command_context.resource = mock.create_autospec(ResourceContextDetails)
         remote_command_context.resource.name = "my_device"
         remote_command_context.remote_reservation = mock.create_autospec(
             ReservationContextDetails
@@ -203,47 +177,65 @@
         remote_endpoint.name = "connected_device"
         remote_command_context.remote_endpoints = [remote_endpoint]
 
         execution_info = mock.Mock()
         get_execution_info.return_value = execution_info
 
         qs_logger = mock.Mock()
-        child_logger = mock.Mock()
-        qs_logger.getChild.return_value = child_logger
-        qs_logger.handlers = [mock.Mock()]
-        qs_logger.filters = [mock.Mock()]
         get_qs_logger.return_value = qs_logger
 
         # Act
         with LoggingSessionContext(remote_command_context) as logger:
             # Assert
             get_execution_info.assert_called_once_with(remote_command_context)
             get_qs_logger.assert_called_once_with(
                 log_group=remote_command_context.remote_reservation.reservation_id,
-                log_category="QS",
-                log_file_prefix=remote_endpoint.name,
+                log_category="cloudshell",
+                log_file_prefix=remote_command_context.resource.name,
+                exec_info=execution_info,
             )
-            log_execution_info.assert_called_once_with(qs_logger, execution_info)
-            self.assertEqual(child_logger, logger)
+            assert logger == qs_logger
 
     @mock.patch("cloudshell.shell.core.session.logging_session.socket.gethostbyname")
     def test_get_execution_info_handles_gethostbyname_exception(
         self, get_host_by_name_mock
     ):
         # Arrange
         auto_load_context = mock.create_autospec(AutoLoadCommandContext)
         auto_load_context.resource = mock.create_autospec(ResourceContextDetails)
         auto_load_context.resource.name = "my_device"
         get_host_by_name_mock.side_effect = Exception("error")
 
         # Act
         result = LoggingSessionContext.get_execution_info(auto_load_context)
 
-        self.assertEqual(result["IP"], "n/a")
+        assert result["INFO"]["IP"] == "n/a"
 
     @staticmethod
     def _get_directory_name(base_filename):
         return os.path.split(os.path.dirname(base_filename))[-1]
 
     @staticmethod
     def _get_filename(base_filename):
         return os.path.basename(base_filename).split("--")[0]
+
+
+def test_get_exec_info():
+    context = mock.Mock()
+
+    exec_info = LoggingSessionContext.get_execution_info(context)
+
+    info_data = exec_info["INFO"]
+    debug_data = exec_info["DEBUG"]
+
+    assert info_data["Python Version"] == platform.python_version()
+    assert info_data["Platform"] == platform.system()
+    assert info_data["Reservation ID"] == context.reservation.reservation_id
+    assert info_data["Description"] == context.reservation.description
+    assert info_data["Username"] == context.reservation.owner_user
+
+    packages = debug_data["Installed Packages"]
+    assert isinstance(packages, tuple)
+    assert len(packages) > 0
+
+    packages_names = [package.split(" ==")[0] for package in packages]
+    assert "cloudshell-logging" in packages_names
```

