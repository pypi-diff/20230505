# Comparing `tmp/bmcs_cross_section-0.0.55a0.tar.gz` & `tmp/bmcs_cross_section-0.0.56a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmcs_cross_section-0.0.55a0.tar", last modified: Fri Jan 13 13:58:29 2023, max compression
+gzip compressed data, was "bmcs_cross_section-0.0.56a0.tar", last modified: Fri May  5 05:39:53 2023, max compression
```

## Comparing `bmcs_cross_section-0.0.55a0.tar` & `bmcs_cross_section-0.0.56a0.tar`

### file list

```diff
@@ -1,48 +1,225 @@
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.109125 bmcs_cross_section-0.0.55a0/
--rw-rw-r--   0 rch       (1000) rch       (1000)      684 2023-01-13 13:58:29.105125 bmcs_cross_section-0.0.55a0/PKG-INFO
--rwxrwxr-x   0 rch       (1000) rch       (1000)       21 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/README.md
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.101125 bmcs_cross_section-0.0.55a0/bmcs_cross_section/
--rwxrwxr-x   0 rch       (1000) rch       (1000)       32 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/__init__.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)      664 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/api.py
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.101125 bmcs_cross_section-0.0.55a0/bmcs_cross_section/crack_bridge/
--rwxrwxr-x   0 rch       (1000) rch       (1000)        0 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/crack_bridge/__init__.py
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.105125 bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/
--rwxrwxr-x   0 rch       (1000) rch       (1000)      240 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/__init__.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     2130 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_design.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     2702 2022-12-19 12:42:21.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_layout.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     2892 2022-12-19 12:42:21.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_layout_dict.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     3344 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_reinf_layer.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)    14559 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_shape.py
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.105125 bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/
--rwxrwxr-x   0 rch       (1000) rch       (1000)      177 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/__init__.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)    13791 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/concrete.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)    10438 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/ec2.py
--rw-rw-r--   0 rch       (1000) rch       (1000)     5353 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/ec2_creep_shrinkage.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)      560 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/matmod.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     4840 2022-12-19 13:04:52.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/reinforcement.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     8068 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/sz_advanced.py
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.105125 bmcs_cross_section-0.0.55a0/bmcs_cross_section/mkappa/
--rwxrwxr-x   0 rch       (1000) rch       (1000)       28 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/mkappa/__init__.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)    32742 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/mkappa/mkappa.py
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.105125 bmcs_cross_section-0.0.55a0/bmcs_cross_section/mxn/
--rwxrwxr-x   0 rch       (1000) rch       (1000)        0 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/mxn/__init__.py
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.105125 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/
--rwxrwxr-x   0 rch       (1000) rch       (1000)       99 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/__init__.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)    12432 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pull_out.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)    25241 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pullout2layer_sim.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     3053 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pullout_ELF_RLM.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)    10888 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pullout_analytical_sim.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)    31122 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pullout_sim.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     1626 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_dp_sim.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     1427 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_ep_sim.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     2066 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_fatigue_sim.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)      620 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_frp_sim.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)     7789 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_multilinear_sim.py
--rwxrwxr-x   0 rch       (1000) rch       (1000)       23 2023-01-13 13:58:22.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section/version.py
-drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-01-13 13:58:29.101125 bmcs_cross_section-0.0.55a0/bmcs_cross_section.egg-info/
--rw-rw-r--   0 rch       (1000) rch       (1000)      684 2023-01-13 13:58:29.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section.egg-info/PKG-INFO
--rw-rw-r--   0 rch       (1000) rch       (1000)     1491 2023-01-13 13:58:29.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section.egg-info/SOURCES.txt
--rw-rw-r--   0 rch       (1000) rch       (1000)        1 2023-01-13 13:58:29.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section.egg-info/dependency_links.txt
--rw-rw-r--   0 rch       (1000) rch       (1000)       19 2023-01-13 13:58:29.000000 bmcs_cross_section-0.0.55a0/bmcs_cross_section.egg-info/top_level.txt
--rw-rw-r--   0 rch       (1000) rch       (1000)       38 2023-01-13 13:58:29.109125 bmcs_cross_section-0.0.55a0/setup.cfg
--rwxrwxr-x   0 rch       (1000) rch       (1000)     4334 2023-01-13 13:12:31.000000 bmcs_cross_section-0.0.55a0/setup.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.690487 bmcs_cross_section-0.0.56a0/
+-rw-rw-r--   0 rch       (1000) rch       (1000)      686 2023-05-05 05:39:53.690487 bmcs_cross_section-0.0.56a0/PKG-INFO
+-rwxrwxr-x   0 rch       (1000) rch       (1000)       21 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.56a0/README.md
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.670478 bmcs_cross_section-0.0.56a0/bmcs_cross_section/
+-rwxrwxr-x   0 rch       (1000) rch       (1000)       32 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/__init__.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)      528 2023-01-22 14:20:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/api.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.670478 bmcs_cross_section-0.0.56a0/bmcs_cross_section/crack_bridge/
+-rwxrwxr-x   0 rch       (1000) rch       (1000)        0 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/crack_bridge/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.674480 bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/
+-rwxrwxr-x   0 rch       (1000) rch       (1000)      240 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/__init__.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     1900 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/cs_design.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     3111 2023-01-21 12:01:50.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/cs_layout_dict.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     3534 2023-01-21 10:41:13.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/cs_reinf_layer.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)    14561 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/cs_shape.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.674480 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/
+-rwxrwxr-x   0 rch       (1000) rch       (1000)      181 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.674480 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/
+-rw-rw-r--   0 rch       (1000) rch       (1000)       85 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/__init__.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)     2110 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/concrete_compression_ec2.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)     2225 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/concrete_compression_ec2_plateau.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)     1919 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/concrete_compression_pwl.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)     1940 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/concrete_matmod.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)     1992 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/concrete_tension_pwl.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     2503 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/ec2.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)     3333 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/ec2_concrete_matmod.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)     2623 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/ec2_concrete_matmod_base.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)     3955 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete/ec2_plateau_concrete_matmod.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)    13321 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete_old.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     2623 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/ec2.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)      560 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/matmod.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     4855 2023-01-21 15:38:49.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/reinforcement.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     8068 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/sz_advanced.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.674480 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mkappa/
+-rwxrwxr-x   0 rch       (1000) rch       (1000)      107 2023-01-22 14:19:31.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mkappa/__init__.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)    17332 2023-01-22 14:18:23.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mkappa/mkappa.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)      497 2023-01-22 14:07:22.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mkappa/mkappa_pstudy.py
+-rw-rw-r--   0 rch       (1000) rch       (1000)    11831 2023-01-22 14:18:00.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mkappa/mkappa_rho.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.674480 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      547 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2566 2018-11-14 16:10:12.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/constitutive_law.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     5835 2023-01-23 09:51:49.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/cross_section.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3938 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/cross_section_component.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      644 2023-01-23 09:36:47.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/cross_section_state.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.674480 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/docs/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-07-01 09:20:47.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/docs/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     7966 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/docs/conf.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4844 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/docs/gen_docs.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     6116 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/ecb_calib.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.678481 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/material_types/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      236 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/material_types/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2520 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/material_types/material_type_base.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2086 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/material_types/material_type_handler.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3286 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/material_types/material_type_matrix_mixture.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1878 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/material_types/material_type_reinf_bar.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2880 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/material_types/material_type_reinf_fabric.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.678481 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)       45 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.678481 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      156 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.678481 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2891 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/TT-csv-dat-file-generator.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1447 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/TT-csv-file-generator_W20_hre.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)       63 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    12792 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/__test__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     9959 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/ex_run.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    11103 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/ex_run_table.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    11781 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/ex_run_view.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1592 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/ex_treatment.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    18024 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/ex_type.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4912 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/ex_type_data_analysis_methods.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4383 2016-04-11 12:47:21.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/ex_utils.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      644 2016-01-04 16:21:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/i_ex_run.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      799 2016-01-04 16:21:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/i_ex_type.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3848 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/loadtxt_bending.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1510 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/loadtxt_novalue.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     9091 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/test.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4796 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/exdb/unit_converter.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.678481 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.678481 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/trc/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/trc/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    17478 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/trc/ccs_unit_cell.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    12912 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/trc/composite_cross_section.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     7631 2016-08-24 07:45:56.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/trc/concrete_mixture.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    23618 2016-08-24 07:45:56.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/trc/fabric_layout.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     7858 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/matdb/trc/fabric_layup.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.678481 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/plugins/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/plugins/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1435 2016-01-04 16:21:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/plugins/promod_plugin.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      617 2016-01-04 16:22:31.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/plugins/promod_service.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3396 2016-01-04 16:21:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/plugins/promod_ui_plugin.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.682483 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/simdb/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      124 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/simdb/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2455 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/simdb/sftp_server.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2601 2016-03-30 13:49:53.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/simdb/simdb.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)       46 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/simdb/simdb_add_trait.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    10294 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/simdb/simdb_class.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4139 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/db/simdb/simdb_migrate_class.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.682483 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.682483 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_calib/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_calib/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    44664 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_calib/mats_calib_damage_fn.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.682483 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      207 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1566 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/__test__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1008 2016-01-04 16:21:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/i_sim_array.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1099 2016-01-04 16:21:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/i_sim_model.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    23725 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/sim_array.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    16601 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/sim_array_view.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     5050 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/sim_factor.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3467 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/sim_model.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1379 2016-01-04 16:21:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/sim_output.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    11487 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/sim_pstudy.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1224 2016-01-04 16:22:31.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/sim_todo.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     6025 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matresdev/simiter/sim_pstudy/tutorial.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.682483 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_cross_section/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      293 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_cross_section/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     7386 2023-01-23 09:44:22.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_cross_section/matrix_cross_section.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      524 2014-07-01 09:20:47.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_cross_section/matrix_cross_section_geo.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3658 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_cross_section/matrix_cross_section_geo_I.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1932 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_cross_section/matrix_cross_section_geo_circ.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1686 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_cross_section/matrix_cross_section_geo_rect.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.682483 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_laws/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      323 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_laws/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1323 2018-11-14 16:10:12.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_laws/matrix_law_base.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      929 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_laws/matrix_law_bilinear.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1354 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_laws/matrix_law_block.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1127 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_laws/matrix_law_linear.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1009 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_laws/matrix_law_quad.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1432 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/matrix_laws/matrix_law_quadratic.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.682483 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)       45 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/examples/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/examples/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2480 2016-12-21 08:50:44.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/examples/mfn_line_example.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3786 2016-12-21 08:50:44.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/examples/mfn_multiline_example.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    15466 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/mfn_chaco_editor.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    16748 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/mfn_chaco_multiline_editor.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     5374 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/mfn_line.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4443 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/mfn_matplotlib_editor.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4963 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/mfn_matplotlib_multiline_editor.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      800 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/mfn_multiline.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4458 2016-01-04 16:21:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_line/mfn_plot_adapter.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_ndgrid/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_ndgrid/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     5560 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_ndgrid/mfn_ndgrid.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_polar/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:35.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_polar/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      495 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_polar/__test__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    10291 2016-11-25 15:03:41.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_polar/mfn_polar.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)    29981 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mfn/mfn_polar/mfn_polar_editor.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1793 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mxn_class_extension.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2092 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mxn_class_extension_handler.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     9043 2023-01-23 09:50:46.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mxn_diagram.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1724 2023-01-23 09:37:28.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/mxn_tree_node.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      373 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      648 2016-12-21 08:55:04.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/reinf_law_base.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1134 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/reinf_law_bilinear.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1253 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/reinf_law_cubic.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1195 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/reinf_law_fbm.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1041 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/reinf_law_linear.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1430 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/reinf_law_piecewise_linear.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      960 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_laws/reinf_law_steel.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_layout/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      251 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_layout/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2329 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_layout/reinf_fabric_handler.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1632 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_layout/reinf_layout_component.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3847 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_layout/reinf_layout_component_bar.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     5733 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_layout/reinf_layout_component_tex_layer.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     5547 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/reinf_layout/reinf_layout_component_tex_uniform.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/scripts/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)       46 2016-12-17 23:26:36.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/scripts/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     2254 2016-12-21 14:39:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/scripts/mxnapp.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/simple_script/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2018-11-14 16:10:12.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/simple_script/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     5383 2018-11-14 16:10:12.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/simple_script/mxn_simple_script.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/use_cases/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      274 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/use_cases/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1377 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/use_cases/use_case_container.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      530 2014-08-05 08:32:36.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/use_cases/use_case_database.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     5957 2016-11-24 13:59:05.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/use_cases/use_case_parametric_study.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)       77 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.686485 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:36.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/__init__.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.690487 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/editors/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)       47 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/editors/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      314 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/editors/mpl_figure_editor.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3573 2016-12-21 10:33:47.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/editors/mpl_figure_editor_qt.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3102 2016-11-24 10:59:20.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/editors/mpl_figure_editor_wx.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3003 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/either_type.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.690487 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/ui/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)        0 2014-02-04 13:40:36.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/ui/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     1877 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/extra_traits/ui/item.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      432 2014-08-09 00:03:12.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/file_handler.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     7066 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/utils/keyref.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.690487 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/view/
+-rwxrwxrwx   0 rch       (1000) rch       (1000)      188 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/view/__init__.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     9535 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/view/mxn_tree_customized_nodes.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     4233 2019-06-27 15:47:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/view/mxn_tree_view.py
+-rwxrwxrwx   0 rch       (1000) rch       (1000)     3558 2014-11-07 09:45:06.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/mxn/view/mxn_tree_view_handler.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.690487 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/
+-rwxrwxr-x   0 rch       (1000) rch       (1000)       99 2022-12-15 11:14:16.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/__init__.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)    12438 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pull_out.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)    25259 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pullout2layer_sim.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     3057 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pullout_ELF_RLM.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)    10888 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pullout_analytical_sim.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)    31144 2023-05-05 05:37:23.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pullout_sim.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     1626 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_dp_sim.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     1427 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_ep_sim.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     2066 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_fatigue_sim.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)      620 2022-12-03 13:18:30.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_frp_sim.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     7793 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_multilinear_sim.py
+-rwxrwxr-x   0 rch       (1000) rch       (1000)       23 2023-05-05 05:39:14.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section/version.py
+drwxrwxr-x   0 rch       (1000) rch       (1000)        0 2023-05-05 05:39:53.670478 bmcs_cross_section-0.0.56a0/bmcs_cross_section.egg-info/
+-rw-rw-r--   0 rch       (1000) rch       (1000)      686 2023-05-05 05:39:53.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section.egg-info/PKG-INFO
+-rw-rw-r--   0 rch       (1000) rch       (1000)     9886 2023-05-05 05:39:53.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section.egg-info/SOURCES.txt
+-rw-rw-r--   0 rch       (1000) rch       (1000)        1 2023-05-05 05:39:53.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section.egg-info/dependency_links.txt
+-rw-rw-r--   0 rch       (1000) rch       (1000)       19 2023-05-05 05:39:53.000000 bmcs_cross_section-0.0.56a0/bmcs_cross_section.egg-info/top_level.txt
+-rw-rw-r--   0 rch       (1000) rch       (1000)       38 2023-05-05 05:39:53.690487 bmcs_cross_section-0.0.56a0/setup.cfg
+-rwxrwxr-x   0 rch       (1000) rch       (1000)     4336 2023-01-21 10:08:57.000000 bmcs_cross_section-0.0.56a0/setup.py
```

### Comparing `bmcs_cross_section-0.0.55a0/PKG-INFO` & `bmcs_cross_section-0.0.56a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bmcs_cross_section
-Version: 0.0.55a0
-Summary: Models of brittle-matrix composite cross sections.
+Version: 0.0.56a0
+Summary: Models of brittle-concrete composite cross sections.
 Home-page: https://github.com/bmcs-group/bmcs_cross_section
 Author: BMCS-Group
 Author-email: rostislav.chudoba@rwt-aachen.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/api.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from bmcs_cross_section.mkappa.mkappa import MKappa, MKappaParamsStudy
+from bmcs_cross_section.mkappa import MKappa, MKappaRho, MKappaParamsStudy
 from bmcs_cross_section.matmod import \
-    ConcreteMatMod, EC2PlateauConcreteMatMod, EC2ConcreteMatMod, PWLConcreteMatMod, SteelReinfMatMod, CarbonReinfMatMod
+    ConcreteMatMod, SteelReinfMatMod, CarbonReinfMatMod
 from bmcs_cross_section.matmod.ec2 import EC2
-from bmcs_cross_section.matmod.ec2_creep_shrinkage import EC2CreepShrinkage
 # from bmcs_cross_section.pullout import PullOutModel1D
 # from bmcs_cross_section.pullout.pullout_sim import PullOutModel
 from bmcs_cross_section.cs_design import BarLayer, ReinfLayer, FabricLayer, CrossSectionLayout, \
     CrossSectionDesign, CustomShape, TShape, Rectangle, Circle, ICrossSectionShape, IShape
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_design.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/cs_design.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 # from .cs_layout import CrossSectionLayout
 from .cs_layout_dict import CrossSectionLayout
 from .cs_shape import Rectangle, Circle, TShape, CustomShape, ICrossSectionShape, IShape
 from bmcs_utils.api import Model, Item, View, EitherTypeEditor
 import traits.api as tr
-from bmcs_utils.api import \
-    Float, EitherType, Instance
-from bmcs_cross_section.matmod import \
-    PWLConcreteMatMod, EC2PlateauConcreteMatMod, EC2ConcreteMatMod
+import bmcs_utils.api as bu
+from bmcs_cross_section.matmod import ConcreteMatMod
 
 class CrossSectionDesign(Model):
     name = 'Cross Section Design'
 
-    matrix = EitherType(options=[
-        ('EC2', EC2ConcreteMatMod),
-        ('EC2 with plateau', EC2PlateauConcreteMatMod),
-        ('piecewise linear', PWLConcreteMatMod),
-        # ('EC2 softening tension', ConcreteMaterialModelAdv),
-        ], MAT=True)
+    matrix = bu.Instance(ConcreteMatMod)
+    def _matrix_default(self):
+        return ConcreteMatMod()
+
+    concrete = tr.Property
+    def _get_concrete(self):
+        """Alias attribute for matrix"""
+        return self.matrix
+
+    def _set_concrete(self, value):
+        """Alias attribute for matrix"""
+        self.matrix = value
 
-    cross_section_layout = Instance(CrossSectionLayout)
+    cross_section_layout = bu.Instance(CrossSectionLayout)
 
     def _cross_section_layout_default(self):
         return CrossSectionLayout(cs_design=self)
 
     depends_on = ['matrix', 'cross_section_layout', 'cross_section_shape']
     tree = ['matrix','cross_section_layout','cross_section_shape']
 
     csl = tr.Property()
     def _get_csl(self):
         return self.cross_section_layout
 
-    H = tr.Property(Float)
+    H = tr.Property(bu.Float)
     def _get_H(self):
         return self.cross_section_shape_.H
     def _set_H(self,value):
         self.cross_section_shape_.H = value
 
-    cross_section_shape = EitherType(
-                          options=[('rectangle', Rectangle),
-                                    # ('circle', Circle),
-                                   ('I-shape', IShape),
-                                    ('T-shape', TShape),
-                                   ('custom', CustomShape)],
-                          CS=True, tree=True)
+    cross_section_shape = bu.EitherType(options=[
+        ('rectangle', Rectangle),
+        ('I-shape', IShape),
+        ('T-shape', TShape),
+        ('custom', CustomShape)],
+    CS=True, tree=True)
 
     ipw_view = View(
-        Item('matrix', latex=r'\mathrm{Conc.~law}', editor=EitherTypeEditor(show_properties=False)),
+        Item('matrix', latex=r'\mathrm{Conc.~law}'),
         Item('cross_section_shape', latex=r'\mathrm{CS~shape}', editor=EitherTypeEditor(show_properties=False)),
     )
 
     def subplots(self, fig):
         return fig.subplots(1, 1)
 
     def update_plot(self, ax):
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_layout.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/cs_layout_dict.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,96 @@
 import numpy as np
 import traits.api as tr
 from bmcs_utils.api import \
-    InteractiveModel, View, Item, EitherType, ModelList, List, Button, ButtonEditor, Int
+    ModelDict, View, Item, EitherType, ModelList, List, Button, ButtonEditor, Int, Str
 from .cs_reinf_layer import ReinfLayer
 
-class CrossSectionLayout(ModelList):
-    name = 'Cross Section Layout'
 
-    items = List(ReinfLayer, [])
+class CrossSectionLayout(ModelDict):
+    name = 'Cross Section Layout'
 
     cs_design = tr.WeakRef
     add_reinf_layer_btn = Button()
     remove_reinf_layer_btn = Button()
-    reinf_layer_name = Str()
+    reinf_layer_name = Str('Layer 1')
 
     @tr.observe('add_reinf_layer_btn')
     def add_reinf_layer_btn_click(self, event=None):
-        self.add_layer(ReinfLayer(name=self.reinf_layer_name))
+        if self.reinf_layer_name in self.items:
+            print('Layer "' + self.reinf_layer_name + '" is already added!')
+        else:
+            self.add_layer(ReinfLayer(name=self.reinf_layer_name))
 
     @tr.observe('remove_reinf_layer_btn')
     def remove_reinf_layer_btn_click(self, event=None):
         name = self.reinf_layer_name
         if name in self.items:
-            self.items.pop(name)
+            self.__delitem__(name)
             print('Reinf layer "' + name + '" is removed!')
         else:
             print('Reinf layer "' + name + '" doesn\'t exist to remove!')
 
     def add_layer(self, rl):
+        self.__setitem__(rl.name, rl)
         rl.cs_layout = self
-        self.items.append(rl)
 
     z_j = tr.Property
+
     def _get_z_j(self):
-        return np.array([r.z for r in self.items], dtype=np.float_)
+        return np.array([r.z for r in self.items.values()], dtype=np.float_)
 
     p_j = tr.Property
     '''
     Get the perimeter
     '''
+
     def _get_p_j(self):
-        return np.array([r.p for r in self.items], dtype=np.float_)
+        return np.array([r.p for r in self.items.values()], dtype=np.float_)
 
     A_j = tr.Property
+
     def _get_A_j(self):
-        return np.array([r.A for r in self.items], dtype=np.float_)
+        return np.array([r.A for r in self.items.values()], dtype=np.float_)
+
+    eps_0_j = tr.Property
+    """Prestressing strain
+    """
+    def _get_eps_0_j(self):
+        return np.array([r.eps_0 for r in self.items.values()], dtype=np.float_)
+
 
     def get_N_tj(self, eps_tj):
+        eps_tot_tj = self.eps_0_j + eps_tj
         return np.array([r.get_N(eps_t)
-                         for r, eps_t in zip(self.items, eps_tj.T)],
-                         dtype=np.float_).T
+                         for r, eps_t in zip(self.items.values(), eps_tot_tj.T)],
+                        dtype=np.float_).T
 
     ipw_view = View(
         Item('add_reinf_layer_btn', editor=ButtonEditor(icon='plus', label='Add reinf. layer')),
         Item('remove_reinf_layer_btn', editor=ButtonEditor(icon='minus', label='Remove reinf. layer')),
         Item('reinf_layer_name', latex='\mathrm{Layer~name}'),
     )
 
     def subplots(self, fig):
         return fig.subplots(1, 1)
 
     def plot_csl(self, ax):
         self.cs_design.cross_section_shape_.update_plot(ax)
 
         H = int(self.cs_design.cross_section_shape_.H)
-
-        maxA = 0
-        for layer in self.items:
-            A = layer.A
-            maxA = max(A, maxA)
-
-        for layer in self.items:
+        max_A = 1
+        if len(self.items) > 0:
+            max_A = max(layer.A for layer in self.items.values())
+        for layer in self.items.values():
             z = layer.z
             A = layer.A
             b = self.cs_design.cross_section_shape_.get_b([z])
-            ax.plot([-0.9 * b/2, 0.9 * b/2], [z, z], color='r',
-                    linewidth=5 * A/maxA)
+            ax.plot([-0.9 * b / 2, 0.9 * b / 2], [z, z], color='r',
+                    linewidth=5 * A / max_A)
 
         # ax.annotate(
         #     'E_composite = {} GPa'.format(np.round(self.get_comp_E() / 1000), 0),
         #     xy=(-H / 2 * 0.8, (H / 2 + H / 2) * 0.8), color='blue'
         # )
 
     def update_plot(self, ax):
-        self.plot_csl(ax)
+        self.plot_csl(ax)
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_reinf_layer.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/cs_reinf_layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import traits.api as tr
 from bmcs_utils.api import \
-    InteractiveModel, Item, View, Float, Int, FloatEditor, EitherType, EitherTypeEditor
+    Model, Item, View, Float, Int, EitherType, EitherTypeEditor
 from bmcs_cross_section.matmod import ReinfMatMod, SteelReinfMatMod, CarbonReinfMatMod
 
 
-class ReinfLayer(InteractiveModel):
+class ReinfLayer(Model):
     # TODO: changes in the ipw interactive window doesn't reflect on mkappa
     #  (maybe because these are lists and changing the elements doesn't notify)
     name = 'Reinf layer'
 
     cs_layout = tr.WeakRef
 
     z = Float(50, CS=True)
@@ -17,21 +17,25 @@
 
     P = Float(100, CS=True)
     """Perimeter"""
 
     A = Float(100, CS=True)
     """Cross sectional area"""
 
+    eps_0 = Float(0, CS=True)
+    """Prestressing strain"""
+
     matmod = EitherType(options=[('steel', SteelReinfMatMod),
                                  ('carbon', CarbonReinfMatMod)])
 
     ipw_view = View(
         Item('matmod', latex=r'\mathrm{behavior}', editor=EitherTypeEditor(show_properties=False)),
         Item('z', latex='z \mathrm{[mm]}'),
         Item('A', latex='A \mathrm{[mm^2]}'),
+        Item('eps_0', label='\varepsilon_0 [-]')
     )
 
     depends_on = ['matmod']
     tree = ['matmod']
 
     def get_N(self, eps):
         return self.A * self.matmod_.get_sig(eps)
@@ -70,14 +74,15 @@
 
     ipw_view = View(
         Item('matmod', latex=r'\mathrm{behavior}'),
         Item('z', latex='z \mathrm{[mm]}'),
         Item('width', latex='\mathrm{fabric~width} \mathrm{[mm]}'),
         Item('spacing', latex='\mathrm{rov~spacing} \mathrm{[mm]}'),
         Item('A_roving', latex='A_r \mathrm{[mm^2]}'),
+        Item('eps_0', label='\varepsilon_0 [-]'),
         Item('A', latex=r'A [mm^2]', readonly=True),
     )
 
 
 class BarLayer(ReinfLayer):
     """"Layer consisting of discrete bar reinforcement"""
     name = 'Bar layer'
@@ -100,9 +105,10 @@
         return 'steel'
 
     ipw_view = View(
         Item('matmod', latex=r'\mathrm{behavior}'),
         Item('z', latex=r'z \mathrm{[mm]}'),
         Item('ds', latex=r'ds \mathrm{[mm]}'),
         Item('count', latex='count'),
-        Item('A', latex=r'A [mm^2]'),
+        Item('eps_0', label='\varepsilon_0 [-]'),
+        Item('A', latex=r'A [mm^2]', readonly=True),
     )
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/cs_design/cs_shape.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/cs_design/cs_shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 
     ipw_view = View(
         Item('cs_points_str', latex=r'\mathrm{Points}', editor=TextAreaEditor()),
         # Item('apply_points_btn', editor=ButtonEditor(label='Apply points', icon='refresh')),
     )
 
     _eps_tu = None
-    eps_tu = tr.Property(desc='Ultimate matrix tensile strain', MAT=True)
+    eps_tu = tr.Property(desc='Ultimate concrete tensile strain', MAT=True)
     def _set_eps_tu(self, value):
         self._eps_tu = value
     def _get_eps_tu(self):
         if self._eps_tu is not None:
             return self._eps_tu
         else:
             return self.eps_cr
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/concrete.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/concrete_old.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,34 +63,34 @@
 
 
 class PWLConcreteMatMod(ConcreteMatMod, bu.InjectSymbExpr):
     name = 'Concrete PWL'
 
     symb_class = PWLConcreteMatModSymbExpr
 
-    E_ct = bu.Float(24000, MAT=True, desc='E modulus of matrix on tension')
-    E_cc = bu.Float(25000, MAT=True, desc='E modulus of matrix on compression')
+    E_ct = bu.Float(24000, MAT=True, desc='E modulus of concrete on tension')
+    E_cc = bu.Float(25000, MAT=True, desc='E modulus of concrete on compression')
     eps_cr = bu.Float(0.00015, MAT=True, desc='Matrix cracking strain')
     _eps_cy = bu.Float(-0.003, MAT=True)
     _eps_cu = bu.Float(-0.01, MAT=True)
 
     # Enforcing negative values for eps_cu and eps_cy
     eps_cy = tr.Property(desc='Matrix compressive yield strain')
     def _set_eps_cy(self, value):
         self._eps_cy = value
     def _get_eps_cy(self):
         return -np.fabs(self._eps_cy)
 
-    eps_cu = tr.Property(desc='Ultimate matrix compressive strain')
+    eps_cu = tr.Property(desc='Ultimate concrete compressive strain')
     def _set_eps_cu(self, value):
         self._eps_cu = value
     def _get_eps_cu(self):
         return -np.fabs(self._eps_cu)
 
-    eps_tu = bu.Float(0.0004, MAT=True, desc='Ultimate matrix tensile strain')
+    eps_tu = bu.Float(0.0004, MAT=True, desc='Ultimate concrete tensile strain')
 
     mu = bu.Float(0.33, MAT=True,
                   desc='Post crack tensile strength ratio (represents how much strength is left after \
                         the crack because of short steel fibers in the mixture)')
 
     ipw_view = bu.View(
         bu.Item('factor'),
@@ -120,58 +120,45 @@
     eps_cr = tr.Property(desc='Matrix cracking strain', MAT=True)
     def _set_eps_cr(self, value):
         self._eps_cr = value
     def _get_eps_cr(self):
         if self._eps_cr is not None:
             return self._eps_cr
         else:
-            if self.factor == 1:
-                return EC2.get_f_ctm(self.f_ck) / self.E_ct
-            else:
-                f_ctk = EC2.get_f_ctk_0_05(self.f_ck)
-                E_k = self.f_ck / EC2.get_eps_c3(self.f_ck)
-                return f_ctk / E_k
+            return EC2.get_f_ctm(self.f_ck) / self.E_ct
 
     _eps_tu = None
-    eps_tu = tr.Property(desc='Ultimate matrix tensile strain', MAT=True)
+    eps_tu = tr.Property(desc='Ultimate concrete tensile strain', MAT=True)
     def _set_eps_tu(self, value):
         self._eps_tu = value
     def _get_eps_tu(self):
         if self._eps_tu is not None:
             return self._eps_tu
         else:
             return self.eps_cr
 
     _E_cc = None
-    E_cc = tr.Property(desc='E modulus of matrix on compression', MAT=True)
+    E_cc = tr.Property(desc='E modulus of concrete on compression', MAT=True)
     def _set_E_cc(self, value):
         self._E_cc = value
     def _get_E_cc(self):
         if self._E_cc is not None:
             return self._E_cc
         else:
-            if self.factor == 1:
-                return EC2.get_E_cm(self.f_ck)
-            else:
-                E_k = self.f_ck / EC2.get_eps_c3(self.f_ck)
-                return E_k
+            return EC2.get_E_cm(self.f_ck)
 
     _E_ct = None
-    E_ct = tr.Property(desc='E modulus of matrix on tension', MAT=True)
+    E_ct = tr.Property(desc='E modulus of concrete on tension', MAT=True)
     def _set_E_ct(self, value):
         self._E_ct = value
     def _get_E_ct(self):
         if self._E_ct is not None:
             return self._E_ct
         else:
-            if self.factor == 1:
-                return EC2.get_E_cm(self.f_ck)
-            else:
-                E_k = self.f_ck / EC2.get_eps_c3(self.f_ck)
-                return E_k
+            return EC2.get_E_cm(self.f_ck)
 
 
     _f_ctm = None
     f_ctm = tr.Property(desc='Axial tensile strength of concrete', MAT=True)
     def _set_f_ctm(self, value):
         self._f_ctm = value
 
@@ -293,15 +280,15 @@
     def _get_n(self):
         return EC2.get_n(self.f_ck)
 
     eps_cy = tr.Property(desc='Matrix compressive yield strain', MAT=True)
     def _get_eps_cy(self):
         return -EC2.get_eps_c2(self.f_ck)
 
-    eps_cu = tr.Property(desc='Ultimate matrix compressive strain', MAT=True)
+    eps_cu = tr.Property(desc='Ultimate concrete compressive strain', MAT=True)
     def _get_eps_cu(self):
         return -EC2.get_eps_cu2(self.f_ck)
 
     def get_sig(self, eps):
         sig = self.symb.get_sig(eps)
         # Compression branch is scaled when defining f_cd
         sig_with_scaled_tension_branch = np.where(sig > 0, self.factor * sig, sig)
@@ -384,15 +371,15 @@
     def _get_f_ck(self):
         return EC2.get_f_ck_from_f_cm(self.f_cm)
 
     eps_cy = tr.Property(desc='Matrix compressive yield strain', MAT=True)
     def _get_eps_cy(self):
         return -EC2.get_eps_c1(self.f_ck)
 
-    eps_cu = tr.Property(desc='Ultimate matrix compressive strain', MAT=True)
+    eps_cu = tr.Property(desc='Ultimate concrete compressive strain', MAT=True)
     def _get_eps_cu(self):
         return -EC2.get_eps_cu1(self.f_ck)
 
     ipw_view = bu.View(
         *EC2ConcreteMatModBase.ipw_view.content,
     )
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/matmod.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/matmod.py`

 * *Files identical despite different names*

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/reinforcement.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/reinforcement.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     def _get_eps_cr(self):
         return self.f_t / self.E
 
     ipw_view = bu.View(
         bu.Item('factor'),
         bu.Item('E', latex=r'E \mathrm{[N/mm^{2}]}'),
         bu.Item('f_t', latex=r'f_\mathrm{t} \mathrm{[N/mm^{2}]}'),
-        bu.Item('eps_cr', latex=r'\varepsilon_\mathrm{cr} \mathrm{[-]}'),
+        bu.Item('eps_cr', latex=r'\varepsilon_\mathrm{cr} \mathrm{[-]}', readonly=True),
     )
 
     def get_eps_plot_range(self):
         return np.linspace(- 0.1*self.eps_cr, 1.1*self.eps_cr,300)
 
     f_t_scaled = tr.Property
     def _get_f_t_scaled(self):
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/matmod/sz_advanced.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/matmod/sz_advanced.py`

 * *Files identical despite different names*

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pull_out.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pull_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import bmcs_utils.api as bu
 import numpy as np
 import sympy as sp
 import traits.api as tr
 
 class PO_ELF_RLM_Symb(bu.SymbExpr):
-    """Pullout of elastic Long fiber, fromm rigid long matrix
+    """Pullout of elastic Long fiber, fromm rigid long concrete
     """
     E_f, A_f = sp.symbols(r'E_\mathrm{f}, A_\mathrm{f}', positive=True)
     E_m, A_m = sp.symbols(r'E_\mathrm{m}, A_\mathrm{m}', positive=True)
     tau, p = sp.symbols(r'\bar{\tau}, p', positive=True)
     C, D = sp.symbols(r'C, D')
     P, w = sp.symbols(r'P, w', positive=True)
     x, a, L_b = sp.symbols(r'x, a, L_b')
@@ -72,15 +72,15 @@
         ('u_ma_x', ('x','P',)),
         ('w_L_b', ('w',)),
         ('aw_pull', ('w',)),
         ('Pw_pull', ('w',)),
     ]
 
 class PO_ELF_ELM_Symb(bu.SymbExpr):
-    """Pullout of elastic Long fiber, fromm elastic long matrix
+    """Pullout of elastic Long fiber, fromm elastic long concrete
     """
     E_m, A_m = sp.symbols(r'E_\mathrm{m}, A_\mathrm{m}', nonnegative=True)
     E_f, A_f = sp.symbols(r'E_\mathrm{f}, A_\mathrm{f}', nonnegative=True)
     tau, p = sp.symbols(r'\bar{\tau}, p', nonnegative=True)
     C, D, E, F = sp.symbols('C, D, E, F')
     P, w = sp.symbols('P, w')
     x, a, L_b = sp.symbols('x, a, L_b')
@@ -250,15 +250,15 @@
         ('aw_pull', ('w',)),
         ('Pw_pull', ('w',)),
     ]
 
 
 class PullOutAModel(bu.Model, bu.InjectSymbExpr):
     """
-    Pullout elastic long fiber and rigid long matrix
+    Pullout elastic long fiber and rigid long concrete
     """
     symb_class = PO_ESF_RLM_Symb
 
     name = "Pull-Out"
 
     E_f = bu.Float(210000, MAT=True)
     E_m = bu.Float(28000, MAT=True)
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pullout2layer_sim.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pullout2layer_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
 
     A_m = Float(15240,
                 CS=True,
                 input=True,
                 unit=r'$\mathrm{mm}^2$',
                 symbol=r'A_\mathrm{m}',
                 auto_set=False, enter_set=True,
-                desc='matrix area')
+                desc='concrete area')
     A_f = Float(153.9,
                 CS=True,
                 input=True,
                 unit='$\\mathrm{mm}^2$',
                 symbol='A_\mathrm{f}',
                 auto_set=False, enter_set=True,
                 desc='reinforcement area')
@@ -493,30 +493,30 @@
     @cached_property
     def _get_u_f0_max(self):
         return self.w_max
 
     def _set_u_f0_max(self, value):
         self.w_max = value
 
-    fixed_boundary = Enum('non-loaded end (matrix)',
-                          'loaded end (matrix)',
+    fixed_boundary = Enum('non-loaded end (concrete)',
+                          'loaded end (concrete)',
                           'non-loaded end (reinf)',
                           'clamped left',
                           BC=True,
-                          desc='which side of the specimen is fixed [non-loaded end [matrix], loaded end [matrix], non-loaded end [reinf]]')
+                          desc='which side of the specimen is fixed [non-loaded end [concrete], loaded end [concrete], non-loaded end [reinf]]')
 
     fixed_dofs = Property(depends_on=itags_str)
 
     @cached_property
     def _get_fixed_dofs(self):
-        if self.fixed_boundary == 'non-loaded end (matrix)':
+        if self.fixed_boundary == 'non-loaded end (concrete)':
             return [0]
         elif self.fixed_boundary == 'non-loaded end (reinf)':
             return [1]
-        elif self.fixed_boundary == 'loaded end (matrix)':
+        elif self.fixed_boundary == 'loaded end (concrete)':
             return [self.controlled_dof - 1]
         elif self.fixed_boundary == 'clamped left':
             return [0, 1]
 
     controlled_dof = Property(depends_on=itags_str)
 
     @cached_property
@@ -654,30 +654,30 @@
         w_0 = U_ti[:, f_dof]
         return P, w_0, w_L
 
     #=========================================================================
     # Plot functions
     #=========================================================================
     def plot_u_p(self, ax, vot,
-                 label_m='matrix', label_f='reinf'):
+                 label_m='concrete', label_f='reinf'):
         X_M = self.X_M
         L = self.geometry.L_x
         u_p = self.get_u_p(vot).T
         ax.plot(X_M, u_p[0], linewidth=2, color='blue', label=label_m)
         ax.fill_between(X_M, 0, u_p[0], facecolor='blue', alpha=0.2)
         ax.plot(X_M, u_p[1], linewidth=2, color='orange', label=label_f)
         ax.fill_between(X_M, 0, u_p[1], facecolor='orange', alpha=0.2)
         ax.plot([0, L], [0, 0], color='black')
         ax.set_ylabel('displacement')
         ax.set_xlabel('bond length')
         ax.legend(loc=2)
         return np.min(u_p), np.max(u_p)
 
     def plot_eps_p(self, ax, vot,
-                   label_m='matrix', label_f='reinf'):
+                   label_m='concrete', label_f='reinf'):
         X_M = self.X_M
         L = self.geometry.L_x
         eps_p = self.get_eps_p(vot).T
         ax.plot(X_M, eps_p[0], linewidth=2, color='blue', label=label_m)
         ax.fill_between(X_M, 0, eps_p[0], facecolor='blue', alpha=0.2)
         ax.plot(X_M, eps_p[1], linewidth=2, color='orange', label=label_f)
         ax.fill_between(X_M, 0, eps_p[1], facecolor='orange', alpha=0.2)
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pullout_ELF_RLM.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pullout_ELF_RLM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import bmcs_utils.api as bu
 import numpy as np
 import sympy as sp
 import traits.api as tr
 
 class PO_ELF_RLM_Symb(bu.SymbExpr):
-    """Pullout of elastic Long fiber, fromm rigid long matrix
+    """Pullout of elastic Long fiber, fromm rigid long concrete
     """
     E_f, A_f = sp.symbols(r'E_\mathrm{f}, A_\mathrm{f}', positive=True)
     E_m, A_m = sp.symbols(r'E_\mathrm{m}, A_\mathrm{m}', positive=True)
     tau, p = sp.symbols(r'\bar{\tau}, p', positive=True)
     C, D = sp.symbols(r'C, D')
     P, w = sp.symbols(r'P, w', positive=True)
     x, a, L_b = sp.symbols(r'x, a, L_b')
@@ -66,15 +66,15 @@
         ('w_L_b', ('w',)),
         ('aw_pull', ('w',)),
         ('Pw_pull', ('w',)),
     ]
 
 class PO_ELF_RLM(bu.Model, bu.InjectSymbExpr):
     """
-    Pullout elastic long fiber and rigid long matrix
+    Pullout elastic long fiber and rigid long concrete
     """
     symb_class = PO_ELF_RLM_Symb
 
     name = "PO-ELF-RLM"
 
     E_f = bu.Float(210000, MAT=True)
     tau = bu.Float(8, MAT=True)
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pullout_analytical_sim.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pullout_analytical_sim.py`

 * *Files identical despite different names*

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/pullout_sim.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/pullout_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,29 +300,29 @@
                         [w, f_top], [-L_b + w_L_b, f_top]], dtype=np.float_)
         line_F.set_xy(x_F)
         x_F0 = np.array([[-L_b, f_bot], [-L_b + w_L_b, f_bot],
                          [-L_b + w_L_b, f_top], [-L_b, f_top]], dtype=np.float_)
         line_F0, = ax.fill([], [], color='white', alpha=1)
         line_F0.set_xy(x_F0)
 
-    def plot_u_p(self, ax, label_m='matrix', label_f='reinf'):
+    def plot_u_p(self, ax, label_m='concrete', label_f='reinf'):
         X_M = self.tstep_source.X_M
         L = self.tstep_source.geometry.L_x
         u_p = self.get_u_p().T
         ax.plot(X_M, u_p[0], linewidth=2, color='blue', label=label_m)
         ax.fill_between(X_M, u_p[0], 0, facecolor='blue', alpha=0.2)
         ax.plot(X_M, u_p[1], linewidth=2, color='orange', label=label_f)
         ax.fill_between(X_M, u_p[1], 0, facecolor='orange', alpha=0.2)
         ax.plot([0, L], [0, 0], color='black')
         ax.set_ylabel('displacement')
         ax.set_xlabel('bond length')
         ax.legend(loc=2)
         return np.min(u_p), np.max(u_p)
 
-    def plot_eps_p(self, ax, label_m='matrix', label_f='reinf'):
+    def plot_eps_p(self, ax, label_m='concrete', label_f='reinf'):
         X_M = self.tstep_source.X_M
         L = self.tstep_source.geometry.L_x
         eps_p = self.get_eps_p().T
         ax.plot(X_M, eps_p[0], linewidth=2, color='blue', label=label_m)
         ax.fill_between(X_M, 0, eps_p[0], facecolor='blue', alpha=0.2)
         ax.plot(X_M, eps_p[1], linewidth=2, color='orange', label=label_f)
         ax.fill_between(X_M, 0, eps_p[1], facecolor='orange', alpha=0.2)
@@ -543,15 +543,15 @@
 
     A_m = bu.Float(15240,
                    CS=True,
                    input=True,
                    unit=r'$\mathrm{mm}^2$',
                    symbol=r'A_\mathrm{m}',
                    auto_set=False, enter_set=True,
-                   desc='matrix area')
+                   desc='concrete area')
     A_f = bu.Float(153.9,
                    CS=True,
                    input=True,
                    unit='$\\mathrm{mm}^2$',
                    symbol='A_\mathrm{f}',
                    auto_set=False, enter_set=True,
                    desc='reinforcement area')
@@ -603,17 +603,18 @@
 
     depends_on = ['cross_section', 'geometry',
                   'material_model',
                   'loading_scenario',
                   'history'
                   ]
     tree = [
-        # 'time_line', 'cross_section',
-        # 'geometry', 'material_model',
-        # 'loading_scenario',
+        # 'time_line',
+        'cross_section',
+        'geometry', 'material_model',
+        'loading_scenario',
         'history'
     ]
 
     def run(self):
         self.sim.run()
 
     def reset(self):
@@ -800,31 +801,31 @@
     def _get_u_f0_max(self):
         return self.w_max
 
     def _set_u_f0_max(self, value):
         self.w_max = value
 
     fixed_boundary = bu.Enum(
-        options=['non-loaded end (matrix)',
-                 'loaded end (matrix)',
+        options=['non-loaded end (concrete)',
+                 'loaded end (concrete)',
                  'non-loaded end (reinf)',
                  'clamped left'],
         BC=True,
-        desc='which side of the specimen is fixed [non-loaded end [matrix], loaded end [matrix], non-loaded end [reinf]]'
+        desc='which side of the specimen is fixed [non-loaded end [concrete], loaded end [concrete], non-loaded end [reinf]]'
     )
 
     fixed_dofs = Property(depends_on="state_changed")
 
     @cached_property
     def _get_fixed_dofs(self):
-        if self.fixed_boundary == 'non-loaded end (matrix)':
+        if self.fixed_boundary == 'non-loaded end (concrete)':
             return [0]
         elif self.fixed_boundary == 'non-loaded end (reinf)':
             return [1]
-        elif self.fixed_boundary == 'loaded end (matrix)':
+        elif self.fixed_boundary == 'loaded end (concrete)':
             return [self.controlled_dof - 1]
         elif self.fixed_boundary == 'clamped left':
             return [0, 1]
 
     controlled_dof = Property(depends_on="state_changed")
 
     @cached_property
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_dp_sim.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_dp_sim.py`

 * *Files identical despite different names*

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_ep_sim.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_ep_sim.py`

 * *Files identical despite different names*

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_fatigue_sim.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_fatigue_sim.py`

 * *Files identical despite different names*

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_frp_sim.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_frp_sim.py`

 * *Files identical despite different names*

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section/pullout/run_pullout_multilinear_sim.py` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section/pullout/run_pullout_multilinear_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     w.configure_traits(*args, **kw)
 
 
 def run_cb_multi(*args, **kw):
     po = PullOutModel(n_e_x=100, k_max=1000, w_max=2.0)
     po.fixed_boundary = 'clamped left'
-    #po.fixed_boundary = 'loaded end (matrix)'
+    #po.fixed_boundary = 'loaded end (concrete)'
     po.sim.tline.step = 0.02
     po.geometry.L_x = 300.0
     po.loading_scenario.trait_set(loading_type='monotonic')
     po.cross_section.trait_set(A_f=16.67 / 9.0, P_b=1.0, A_m=1540.0)
     po.mats_eval.trait_set(s_data='0, 0.1, 0.4, 4.0',
                            tau_data='0, 70.0, 80, 90')
     po.mats_eval.trait_set(s_data='0, 0.1, 0.4, 4.0',
@@ -175,15 +175,15 @@
     w.run()
     w.configure_traits()
 
 
 def run_two_steps():
     po = PullOutModel(n_e_x=60, k_max=5, w_max=1.0)
     po.sim.tline.step = 0.05
-    po.fixed_boundary = 'loaded end (matrix)'
+    po.fixed_boundary = 'loaded end (concrete)'
     po.loading_scenario.trait_set(loading_type='cyclic',
                                   amplitude_type='constant',
                                   loading_range='non-symmetric'
                                   )
     po.loading_scenario.trait_set(number_of_cycles=1,
                                   unloading_ratio=0.98,
                                   )
```

### Comparing `bmcs_cross_section-0.0.55a0/bmcs_cross_section.egg-info/PKG-INFO` & `bmcs_cross_section-0.0.56a0/bmcs_cross_section.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bmcs-cross-section
-Version: 0.0.55a0
-Summary: Models of brittle-matrix composite cross sections.
+Version: 0.0.56a0
+Summary: Models of brittle-concrete composite cross sections.
 Home-page: https://github.com/bmcs-group/bmcs_cross_section
 Author: BMCS-Group
 Author-email: rostislav.chudoba@rwt-aachen.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bmcs_cross_section-0.0.55a0/setup.py` & `bmcs_cross_section-0.0.56a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'bmcs_cross_section'
-DESCRIPTION = "Models of brittle-matrix composite cross sections."
+DESCRIPTION = "Models of brittle-concrete composite cross sections."
 URL = 'https://github.com/bmcs-group/bmcs_cross_section'
 EMAIL = 'rostislav.chudoba@rwt-aachen.de'
 AUTHOR = 'BMCS-Group'
 REQUIRES_PYTHON = '>=3.6.0'
 from bmcs_cross_section.version import __version__
 VERSION = __version__
```

