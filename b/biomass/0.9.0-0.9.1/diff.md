# Comparing `tmp/biomass-0.9.0.tar.gz` & `tmp/biomass-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomass-0.9.0.tar", last modified: Thu Jul 21 10:22:20 2022, max compression
+gzip compressed data, was "biomass-0.9.1.tar", last modified: Wed Jul 27 15:46:39 2022, max compression
```

## Comparing `biomass-0.9.0.tar` & `biomass-0.9.1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:20.003769 biomass-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11391 2022-07-21 10:22:06.000000 biomass-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-07-21 10:22:06.000000 biomass-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4842 2022-07-21 10:22:20.003769 biomass-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3225 2022-07-21 10:22:06.000000 biomass-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.987769 biomass-0.9.0/biomass/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.987769 biomass-0.9.0/biomass/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11835 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/analysis/initial_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)    11550 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/analysis/parameter.py
--rw-r--r--   0 runner    (1001) docker     (121)    13806 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/analysis/reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/analysis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.991769 biomass-0.9.0/biomass/construction/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14010 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/julia_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    60101 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/reaction_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.991769 biomass-0.9.0/biomass/construction/template/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.991769 biomass-0.9.0/biomass/construction/template/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4231 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/template/viz.py
--rw-r--r--   0 runner    (1001) docker     (121)    38232 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/text2model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8810 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/construction/thermodynamic_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (121)    16238 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.991769 biomass-0.9.0/biomass/dynamics/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/dynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7321 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/dynamics/signaling_systems.py
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/dynamics/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)    20535 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/dynamics/temporal_dynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.991769 biomass-0.9.0/biomass/estimation/
--rwxr-xr-x   0 runner    (1001) docker     (121)      116 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/estimation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8911 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/estimation/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/estimation/search_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/exec_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    11866 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.991769 biomass-0.9.0/biomass/models/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.991769 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.995769 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     8952 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     7108 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     9323 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     6871 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     8397 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/viz.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.995769 biomass-0.9.0/biomass/models/circadian_clock/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.995769 biomass-0.9.0/biomass/models/circadian_clock/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     5890 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/circadian_clock/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.995769 biomass-0.9.0/biomass/models/g1s_transition/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.995769 biomass-0.9.0/biomass/models/g1s_transition/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     2707 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/g1s_transition/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.995769 biomass-0.9.0/biomass/models/insulin_signaling/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.995769 biomass-0.9.0/biomass/models/insulin_signaling/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     3410 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     2889 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/insulin_signaling/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.999769 biomass-0.9.0/biomass/models/mapk_cascade/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.999769 biomass-0.9.0/biomass/models/mapk_cascade/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     5035 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/mapk_cascade/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.999769 biomass-0.9.0/biomass/models/nfkb_pathway/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.999769 biomass-0.9.0/biomass/models/nfkb_pathway/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     4866 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/nfkb_pathway/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.999769 biomass-0.9.0/biomass/models/pan_rtk/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.999769 biomass-0.9.0/biomass/models/pan_rtk/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15308 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     6100 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)    28112 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)    39952 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/pan_rtk/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:20.003769 biomass-0.9.0/biomass/models/prolif_quies/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:20.003769 biomass-0.9.0/biomass/models/prolif_quies/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     6095 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/prolif_quies/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:20.003769 biomass-0.9.0/biomass/models/tgfb_smad/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:20.003769 biomass-0.9.0/biomass/models/tgfb_smad/name2idx/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/name2idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/name2idx/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/name2idx/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     7440 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     6265 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/reaction_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/search_param.py
--rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/models/tgfb_smad/viz.py
--rw-r--r--   0 runner    (1001) docker     (121)     4960 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    11294 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/result.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-21 10:22:06.000000 biomass-0.9.0/biomass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.987769 biomass-0.9.0/biomass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4842 2022-07-21 10:22:19.000000 biomass-0.9.0/biomass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5639 2022-07-21 10:22:19.000000 biomass-0.9.0/biomass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 10:22:19.000000 biomass-0.9.0/biomass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-07-21 10:22:19.000000 biomass-0.9.0/biomass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-21 10:22:19.000000 biomass-0.9.0/biomass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-07-21 10:22:06.000000 biomass-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-07-21 10:22:06.000000 biomass-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-21 10:22:20.003769 biomass-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-07-21 10:22:06.000000 biomass-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:19.987769 biomass-0.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:20.003769 biomass-0.9.0/tests/test_text2model/
--rwxr-xr-x   0 runner    (1001) docker     (121)    10303 2022-07-21 10:22:06.000000 biomass-0.9.0/tests/test_text2model/C.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 10:22:06.000000 biomass-0.9.0/tests/test_text2model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-07-21 10:22:06.000000 biomass-0.9.0/tests/test_text2model/test_error_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-07-21 10:22:06.000000 biomass-0.9.0/tests/test_text2model/test_fos_model_from_txt.py
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-07-21 10:22:06.000000 biomass-0.9.0/tests/test_text2model/test_model_construction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-07-21 10:22:06.000000 biomass-0.9.0/tests/test_text2model/test_thermodynamic_restriction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11391 2022-07-27 15:46:32.000000 biomass-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-07-27 15:46:32.000000 biomass-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-07-27 15:46:39.091578 biomass-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3109 2022-07-27 15:46:32.000000 biomass-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass/
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass/analysis/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11835 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/analysis/initial_condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11550 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/analysis/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13806 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/analysis/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/analysis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass/construction/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14010 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/julia_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60101 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/reaction_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass/construction/template/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass/construction/template/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4231 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/template/viz.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38232 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/text2model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8810 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/construction/thermodynamic_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16238 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/core.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7321 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/dynamics/signaling_systems.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/dynamics/solver.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20535 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/dynamics/temporal_dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass/estimation/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      116 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/estimation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8911 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/estimation/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/estimation/search_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/exec_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12048 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass/models/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.083578 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.083578 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8952 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7108 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9323 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6871 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8397 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/viz.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.083578 biomass-0.9.1/biomass/models/circadian_clock/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.083578 biomass-0.9.1/biomass/models/circadian_clock/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5890 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3613 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/circadian_clock/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.083578 biomass-0.9.1/biomass/models/g1s_transition/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.083578 biomass-0.9.1/biomass/models/g1s_transition/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2707 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/g1s_transition/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.087578 biomass-0.9.1/biomass/models/insulin_signaling/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.087578 biomass-0.9.1/biomass/models/insulin_signaling/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      929 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3410 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2889 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/insulin_signaling/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.087578 biomass-0.9.1/biomass/models/mapk_cascade/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.087578 biomass-0.9.1/biomass/models/mapk_cascade/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5035 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/mapk_cascade/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.087578 biomass-0.9.1/biomass/models/nfkb_pathway/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/biomass/models/nfkb_pathway/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4866 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/nfkb_pathway/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/biomass/models/pan_rtk/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/biomass/models/pan_rtk/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15308 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6100 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28112 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39952 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/pan_rtk/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/biomass/models/prolif_quies/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/biomass/models/prolif_quies/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6095 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/prolif_quies/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/biomass/models/tgfb_smad/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/biomass/models/tgfb_smad/name2idx/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/name2idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/name2idx/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/name2idx/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7440 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6265 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/reaction_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/models/tgfb_smad/viz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4960 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11294 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-27 15:46:32.000000 biomass-0.9.1/biomass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.079578 biomass-0.9.1/biomass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-07-27 15:46:39.000000 biomass-0.9.1/biomass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5639 2022-07-27 15:46:39.000000 biomass-0.9.1/biomass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 15:46:39.000000 biomass-0.9.1/biomass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-27 15:46:39.000000 biomass-0.9.1/biomass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-27 15:46:39.000000 biomass-0.9.1/biomass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-07-27 15:46:32.000000 biomass-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-07-27 15:46:32.000000 biomass-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-27 15:46:39.095579 biomass-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-07-27 15:46:32.000000 biomass-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.075578 biomass-0.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:39.091578 biomass-0.9.1/tests/test_text2model/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10303 2022-07-27 15:46:32.000000 biomass-0.9.1/tests/test_text2model/C.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-27 15:46:32.000000 biomass-0.9.1/tests/test_text2model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-07-27 15:46:32.000000 biomass-0.9.1/tests/test_text2model/test_error_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-07-27 15:46:32.000000 biomass-0.9.1/tests/test_text2model/test_fos_model_from_txt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-07-27 15:46:32.000000 biomass-0.9.1/tests/test_text2model/test_model_construction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-07-27 15:46:32.000000 biomass-0.9.1/tests/test_text2model/test_thermodynamic_restriction.py
```

### Comparing `biomass-0.9.0/LICENSE` & `biomass-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/PKG-INFO` & `biomass-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomass
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python Framework for Modeling and Analysis of Signaling Systems
 Home-page: https://github.com/biomass-dev/biomass
 Author: Hiroaki Imoto
 Author-email: himoto@protein.osaka-u.ac.jp
 Maintainer: Hiroaki Imoto
 Maintainer-email: himoto@protein.osaka-u.ac.jp
 License: Apache 2.0
@@ -27,14 +27,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: graph
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <br>
 <p align="center">
     <a href="https://biomass-core.readthedocs.io/en/latest">
@@ -69,16 +70,14 @@
 
 ```shell
 $ pip install biomass
 ```
 
 BioMASS supports Python 3.7 or newer.
 
-:ledger: **Note: You will need to manually install [Graphviz](https://www.graphviz.org) (version 2.42 or later).**
-
 ## References
 
 - Imoto, H., Zhang, S. & Okada, M. A Computational Framework for Prediction and Analysis of Cancer Signaling Dynamics from RNA Sequencing Data—Application to the ErbB Receptor Signaling Pathway. _Cancers_ **12**, 2878 (2020). https://doi.org/10.3390/cancers12102878
 
 - Imoto, H., Yamashiro, S. & Okada, M. A text-based computational framework for patient -specific modeling for classification of cancers. _iScience_ **25**, 103944 (2022). https://doi.org/10.1016/j.isci.2022.103944
 
 ## Author
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biomass Version: 0.9.0 Summary: A Python Framework
+Metadata-Version: 2.1 Name: biomass Version: 0.9.1 Summary: A Python Framework
 for Modeling and Analysis of Signaling Systems Home-page: https://github.com/
 biomass-dev/biomass Author: Hiroaki Imoto Author-email: himoto@protein.osaka-
 u.ac.jp Maintainer: Hiroaki Imoto Maintainer-email: himoto@protein.osaka-
 u.ac.jp License: Apache 2.0 Download-URL: https://github.com/biomass-dev/
 biomass/releases Project-URL: Documentation, https://biomass-
 core.readthedocs.io/en/latest/ Project-URL: Source Code, https://github.com/
 biomass-dev/biomass Project-URL: Bug Tracker, https://github.com/biomass-dev/
@@ -15,15 +15,16 @@
 :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Bio-Informatics Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: docs License-File: LICENSE
+text/markdown Provides-Extra: graph Provides-Extra: dev Provides-Extra: docs
+License-File: LICENSE
 [https://raw.githubusercontent.com/biomass-dev/biomass/master/docs/_static/img/
                                biomass-logo.png]
 [![PyPI version](https://img.shields.io/pypi/v/
 biomass.svg?logo=PyPI&logoColor=white)](https://pypi.python.org/pypi/biomass)
 [![Actions Status](https://github.com/biomass-dev/biomass/workflows/Tests/
 badge.svg)](https://github.com/biomass-dev/biomass/actions) [![Documentation
 Status](https://img.shields.io/readthedocs/biomass-core/
@@ -48,18 +49,16 @@
 - **Documentation:** https://biomass-core.rtfd.io - **Source code:** https://
 github.com/biomass-dev/biomass - **Bug reports:** https://github.com/biomass-
 dev/biomass/issues - **Citing in your work:** https://biomass-core.rtfd.io/en/
 latest/citing.html It provides useful tools for numerical simulation, parameter
 estimation, network analysis, and result visualization. ## Installation The
 BioMASS library is available at the [Python Package Index (PyPI)](https://
 pypi.org/project/biomass). ```shell $ pip install biomass ``` BioMASS supports
-Python 3.7 or newer. :ledger: **Note: You will need to manually install
-[Graphviz](https://www.graphviz.org) (version 2.42 or later).** ## References -
-Imoto, H., Zhang, S. & Okada, M. A Computational Framework for Prediction and
-Analysis of Cancer Signaling Dynamics from RNA Sequencing DataâApplication to
-the ErbB Receptor Signaling Pathway. _Cancers_ **12**, 2878 (2020). https://
-doi.org/10.3390/cancers12102878 - Imoto, H., Yamashiro, S. & Okada, M. A text-
-based computational framework for patient -specific modeling for classification
-of cancers. _iScience_ **25**, 103944 (2022). https://doi.org/10.1016/
-j.isci.2022.103944 ## Author [Hiroaki Imoto](https://github.com/himoto) ##
-License [Apache License 2.0](https://github.com/biomass-dev/biomass/blob/
-master/LICENSE)
+Python 3.7 or newer. ## References - Imoto, H., Zhang, S. & Okada, M. A
+Computational Framework for Prediction and Analysis of Cancer Signaling
+Dynamics from RNA Sequencing DataâApplication to the ErbB Receptor Signaling
+Pathway. _Cancers_ **12**, 2878 (2020). https://doi.org/10.3390/cancers12102878
+- Imoto, H., Yamashiro, S. & Okada, M. A text-based computational framework for
+patient -specific modeling for classification of cancers. _iScience_ **25**,
+103944 (2022). https://doi.org/10.1016/j.isci.2022.103944 ## Author [Hiroaki
+Imoto](https://github.com/himoto) ## License [Apache License 2.0](https://
+github.com/biomass-dev/biomass/blob/master/LICENSE)
```

### Comparing `biomass-0.9.0/README.md` & `biomass-0.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 
 ```shell
 $ pip install biomass
 ```
 
 BioMASS supports Python 3.7 or newer.
 
-:ledger: **Note: You will need to manually install [Graphviz](https://www.graphviz.org) (version 2.42 or later).**
-
 ## References
 
 - Imoto, H., Zhang, S. & Okada, M. A Computational Framework for Prediction and Analysis of Cancer Signaling Dynamics from RNA Sequencing Data—Application to the ErbB Receptor Signaling Pathway. _Cancers_ **12**, 2878 (2020). https://doi.org/10.3390/cancers12102878
 
 - Imoto, H., Yamashiro, S. & Okada, M. A text-based computational framework for patient -specific modeling for classification of cancers. _iScience_ **25**, 103944 (2022). https://doi.org/10.1016/j.isci.2022.103944
 
 ## Author
```

#### html2text {}

```diff
@@ -27,18 +27,16 @@
 - **Documentation:** https://biomass-core.rtfd.io - **Source code:** https://
 github.com/biomass-dev/biomass - **Bug reports:** https://github.com/biomass-
 dev/biomass/issues - **Citing in your work:** https://biomass-core.rtfd.io/en/
 latest/citing.html It provides useful tools for numerical simulation, parameter
 estimation, network analysis, and result visualization. ## Installation The
 BioMASS library is available at the [Python Package Index (PyPI)](https://
 pypi.org/project/biomass). ```shell $ pip install biomass ``` BioMASS supports
-Python 3.7 or newer. :ledger: **Note: You will need to manually install
-[Graphviz](https://www.graphviz.org) (version 2.42 or later).** ## References -
-Imoto, H., Zhang, S. & Okada, M. A Computational Framework for Prediction and
-Analysis of Cancer Signaling Dynamics from RNA Sequencing DataâApplication to
-the ErbB Receptor Signaling Pathway. _Cancers_ **12**, 2878 (2020). https://
-doi.org/10.3390/cancers12102878 - Imoto, H., Yamashiro, S. & Okada, M. A text-
-based computational framework for patient -specific modeling for classification
-of cancers. _iScience_ **25**, 103944 (2022). https://doi.org/10.1016/
-j.isci.2022.103944 ## Author [Hiroaki Imoto](https://github.com/himoto) ##
-License [Apache License 2.0](https://github.com/biomass-dev/biomass/blob/
-master/LICENSE)
+Python 3.7 or newer. ## References - Imoto, H., Zhang, S. & Okada, M. A
+Computational Framework for Prediction and Analysis of Cancer Signaling
+Dynamics from RNA Sequencing DataâApplication to the ErbB Receptor Signaling
+Pathway. _Cancers_ **12**, 2878 (2020). https://doi.org/10.3390/cancers12102878
+- Imoto, H., Yamashiro, S. & Okada, M. A text-based computational framework for
+patient -specific modeling for classification of cancers. _iScience_ **25**,
+103944 (2022). https://doi.org/10.1016/j.isci.2022.103944 ## Author [Hiroaki
+Imoto](https://github.com/himoto) ## License [Apache License 2.0](https://
+github.com/biomass-dev/biomass/blob/master/LICENSE)
```

### Comparing `biomass-0.9.0/biomass/analysis/initial_condition.py` & `biomass-0.9.1/biomass/analysis/initial_condition.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/analysis/parameter.py` & `biomass-0.9.1/biomass/analysis/parameter.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/analysis/reaction.py` & `biomass-0.9.1/biomass/analysis/reaction.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/analysis/util.py` & `biomass-0.9.1/biomass/analysis/util.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/julia_template.py` & `biomass-0.9.1/biomass/construction/julia_template.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/reaction_rules.py` & `biomass-0.9.1/biomass/construction/reaction_rules.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/template/observable.py` & `biomass-0.9.1/biomass/construction/template/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/template/ode.py` & `biomass-0.9.1/biomass/construction/template/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/template/problem.py` & `biomass-0.9.1/biomass/construction/template/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/template/reaction_network.py` & `biomass-0.9.1/biomass/construction/template/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/template/search_param.py` & `biomass-0.9.1/biomass/construction/template/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/template/viz.py` & `biomass-0.9.1/biomass/construction/template/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/text2model.py` & `biomass-0.9.1/biomass/construction/text2model.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/construction/thermodynamic_restrictions.py` & `biomass-0.9.1/biomass/construction/thermodynamic_restrictions.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/core.py` & `biomass-0.9.1/biomass/core.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/dynamics/signaling_systems.py` & `biomass-0.9.1/biomass/dynamics/signaling_systems.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/dynamics/solver.py` & `biomass-0.9.1/biomass/dynamics/solver.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/dynamics/temporal_dynamics.py` & `biomass-0.9.1/biomass/dynamics/temporal_dynamics.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/estimation/optimizer.py` & `biomass-0.9.1/biomass/estimation/optimizer.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/estimation/search_util.py` & `biomass-0.9.1/biomass/estimation/search_util.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/exec_model.py` & `biomass-0.9.1/biomass/exec_model.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/graph.py` & `biomass-0.9.1/biomass/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
 import re
 import warnings
 from collections import defaultdict
 from types import ModuleType
 from typing import List, Literal, Optional
 
-import pygraphviz as pgv
-from pyvis.network import Network
-
 
 class NetworkGraph(object):
     """
     Visualization of the biological network as a graph.
 
     Parameters
     ----------
@@ -48,14 +45,16 @@
         self._species = biomass_model.V.NAMES
         self.pval = biomass_model.param_values
         self.ival = biomass_model.initial_values
         self.problem = biomass_model.OptimizationProblem()
         self.viz = biomass_model.Visualization()
         self.rxn = biomass_model.ReactionNetwork()
 
+        self.graph = None
+
     @property
     def path(self) -> str:
         return self._path
 
     @property
     def parameters(self) -> List[str]:
         return self._parameters
@@ -125,26 +124,31 @@
                         was_warned = True
         return data
 
     def to_graph(self) -> None:
         """Constructs a directed graph of the model.
         Using the pygraphviz library a directed graph of the model is constructed by parsing the equations from
         ode.py/reaction_network.py. Equations will be split at the equal sign and an edge is added between the species on the
-        lefthand side to all species on the righthand side. Self references will not be considered.
+        lefthand side to all species on the right hand side. Self references will not be considered.
 
         Raises
         ------
         AssertionError
             If more species are part of the model, than are detected from ode.py/reaction_network.py or vice versa.
 
         Warns
         -----
         UserWarning
             If species equations are detected outside of the ODE section.
         """
+        try:
+            import pygraphviz as pgv
+        except ImportError:
+            print("pygraphviz is required to run this function.")
+
         use_flux = False
         try:
             if len(self.rxn.flux(0, self.ival(), self.pval())) > 0:
                 use_flux = True
             else:
                 use_flux = False
         except AttributeError:
@@ -214,17 +218,15 @@
         --------
         >>> model.static_plot("path/to/", "graph.png")
         Creates graph with dot layout and default options.
         >>> model.static_plot("path/to/", "graph.pdf", gviz_prog="-Nshape=box -Nstyle=filled -Nfillcolor="#ffe4c4" -Edir=none")
         Creates graph with dot layout in pdf file format. Nodes will be rectangular and colored bisque, edges will have no arrows indicating direction.
 
         """
-        try:
-            _ = self.graph
-        except AttributeError:
+        if self.graph is None:
             self.to_graph()
         if gviz_prog not in (available_layout := ["neato", "dot", "twopi", "circo", "fdp", "nop"]):
             raise ValueError(
                 f"gviz_prog must be one of [{', '.join(available_layout)}], got {gviz_prog}."
             )
         if not save_dir:
             save_dir = self.path
@@ -263,16 +265,19 @@
         --------
         >>> model.dynamic_plot("path/to/", "graph.html")
         Creates graph and shows interactive graph with default options.
         >>> model.dynamic_plot("path/to/", "graph.html", show=False, show_controls=True, which_controls=["physics", "manipulation", "interaction"])
         Creates interactive graph. Controls for physics, manipulation and interaction will be available.
         """
         try:
-            _ = self.graph
-        except AttributeError:
+            from pyvis.network import Network
+        except ImportError:
+            print("pyvis is required to run this function.")
+
+        if self.graph is None:
             self.to_graph()
         if os.path.splitext(file_name)[1] != ".html":
             file_name = file_name + ".html"
         if not save_dir:
             save_dir = self.path
         network = Network(directed=True)
         network.add_nodes(self.graph.nodes())
```

### Comparing `biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/name2idx/species.py` & `biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/name2idx/species.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/observable.py` & `biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/ode.py` & `biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/problem.py` & `biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/reaction_network.py` & `biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/search_param.py` & `biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/Nakakuki_Cell_2010/viz.py` & `biomass-0.9.1/biomass/models/Nakakuki_Cell_2010/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/circadian_clock/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/circadian_clock/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/circadian_clock/name2idx/species.py` & `biomass-0.9.1/biomass/models/circadian_clock/name2idx/species.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/circadian_clock/observable.py` & `biomass-0.9.1/biomass/models/circadian_clock/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/circadian_clock/ode.py` & `biomass-0.9.1/biomass/models/circadian_clock/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/circadian_clock/problem.py` & `biomass-0.9.1/biomass/models/circadian_clock/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/circadian_clock/reaction_network.py` & `biomass-0.9.1/biomass/models/circadian_clock/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/circadian_clock/search_param.py` & `biomass-0.9.1/biomass/models/circadian_clock/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/circadian_clock/viz.py` & `biomass-0.9.1/biomass/models/circadian_clock/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/g1s_transition/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/g1s_transition/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/g1s_transition/observable.py` & `biomass-0.9.1/biomass/models/g1s_transition/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/g1s_transition/ode.py` & `biomass-0.9.1/biomass/models/g1s_transition/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/g1s_transition/problem.py` & `biomass-0.9.1/biomass/models/g1s_transition/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/g1s_transition/reaction_network.py` & `biomass-0.9.1/biomass/models/g1s_transition/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/g1s_transition/search_param.py` & `biomass-0.9.1/biomass/models/g1s_transition/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/g1s_transition/viz.py` & `biomass-0.9.1/biomass/models/g1s_transition/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/insulin_signaling/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/insulin_signaling/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/insulin_signaling/name2idx/species.py` & `biomass-0.9.1/biomass/models/insulin_signaling/name2idx/species.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/insulin_signaling/observable.py` & `biomass-0.9.1/biomass/models/insulin_signaling/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/insulin_signaling/ode.py` & `biomass-0.9.1/biomass/models/insulin_signaling/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/insulin_signaling/problem.py` & `biomass-0.9.1/biomass/models/insulin_signaling/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/insulin_signaling/reaction_network.py` & `biomass-0.9.1/biomass/models/insulin_signaling/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/insulin_signaling/search_param.py` & `biomass-0.9.1/biomass/models/insulin_signaling/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/insulin_signaling/viz.py` & `biomass-0.9.1/biomass/models/insulin_signaling/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/mapk_cascade/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/mapk_cascade/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/mapk_cascade/observable.py` & `biomass-0.9.1/biomass/models/mapk_cascade/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/mapk_cascade/ode.py` & `biomass-0.9.1/biomass/models/mapk_cascade/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/mapk_cascade/problem.py` & `biomass-0.9.1/biomass/models/mapk_cascade/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/mapk_cascade/reaction_network.py` & `biomass-0.9.1/biomass/models/mapk_cascade/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/mapk_cascade/search_param.py` & `biomass-0.9.1/biomass/models/mapk_cascade/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/mapk_cascade/viz.py` & `biomass-0.9.1/biomass/models/mapk_cascade/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/nfkb_pathway/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/nfkb_pathway/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/nfkb_pathway/name2idx/species.py` & `biomass-0.9.1/biomass/models/nfkb_pathway/name2idx/species.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/nfkb_pathway/observable.py` & `biomass-0.9.1/biomass/models/nfkb_pathway/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/nfkb_pathway/ode.py` & `biomass-0.9.1/biomass/models/nfkb_pathway/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/nfkb_pathway/problem.py` & `biomass-0.9.1/biomass/models/nfkb_pathway/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/nfkb_pathway/reaction_network.py` & `biomass-0.9.1/biomass/models/nfkb_pathway/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/nfkb_pathway/search_param.py` & `biomass-0.9.1/biomass/models/nfkb_pathway/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/nfkb_pathway/viz.py` & `biomass-0.9.1/biomass/models/nfkb_pathway/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/pan_rtk/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/pan_rtk/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/pan_rtk/name2idx/species.py` & `biomass-0.9.1/biomass/models/pan_rtk/name2idx/species.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/pan_rtk/observable.py` & `biomass-0.9.1/biomass/models/pan_rtk/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/pan_rtk/ode.py` & `biomass-0.9.1/biomass/models/pan_rtk/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/pan_rtk/problem.py` & `biomass-0.9.1/biomass/models/pan_rtk/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/pan_rtk/reaction_network.py` & `biomass-0.9.1/biomass/models/pan_rtk/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/pan_rtk/search_param.py` & `biomass-0.9.1/biomass/models/pan_rtk/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/pan_rtk/viz.py` & `biomass-0.9.1/biomass/models/pan_rtk/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/prolif_quies/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/prolif_quies/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/prolif_quies/name2idx/species.py` & `biomass-0.9.1/biomass/models/prolif_quies/name2idx/species.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/prolif_quies/observable.py` & `biomass-0.9.1/biomass/models/prolif_quies/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/prolif_quies/ode.py` & `biomass-0.9.1/biomass/models/prolif_quies/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/prolif_quies/problem.py` & `biomass-0.9.1/biomass/models/prolif_quies/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/prolif_quies/reaction_network.py` & `biomass-0.9.1/biomass/models/prolif_quies/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/prolif_quies/search_param.py` & `biomass-0.9.1/biomass/models/prolif_quies/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/prolif_quies/viz.py` & `biomass-0.9.1/biomass/models/prolif_quies/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/tgfb_smad/name2idx/parameters.py` & `biomass-0.9.1/biomass/models/tgfb_smad/name2idx/parameters.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/tgfb_smad/name2idx/species.py` & `biomass-0.9.1/biomass/models/tgfb_smad/name2idx/species.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/tgfb_smad/observable.py` & `biomass-0.9.1/biomass/models/tgfb_smad/observable.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/tgfb_smad/ode.py` & `biomass-0.9.1/biomass/models/tgfb_smad/ode.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/tgfb_smad/problem.py` & `biomass-0.9.1/biomass/models/tgfb_smad/problem.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/tgfb_smad/reaction_network.py` & `biomass-0.9.1/biomass/models/tgfb_smad/reaction_network.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/tgfb_smad/search_param.py` & `biomass-0.9.1/biomass/models/tgfb_smad/search_param.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/models/tgfb_smad/viz.py` & `biomass-0.9.1/biomass/models/tgfb_smad/viz.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/plotting.py` & `biomass-0.9.1/biomass/plotting.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass/result.py` & `biomass-0.9.1/biomass/result.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/biomass.egg-info/PKG-INFO` & `biomass-0.9.1/biomass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomass
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python Framework for Modeling and Analysis of Signaling Systems
 Home-page: https://github.com/biomass-dev/biomass
 Author: Hiroaki Imoto
 Author-email: himoto@protein.osaka-u.ac.jp
 Maintainer: Hiroaki Imoto
 Maintainer-email: himoto@protein.osaka-u.ac.jp
 License: Apache 2.0
@@ -27,14 +27,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: graph
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <br>
 <p align="center">
     <a href="https://biomass-core.readthedocs.io/en/latest">
@@ -69,16 +70,14 @@
 
 ```shell
 $ pip install biomass
 ```
 
 BioMASS supports Python 3.7 or newer.
 
-:ledger: **Note: You will need to manually install [Graphviz](https://www.graphviz.org) (version 2.42 or later).**
-
 ## References
 
 - Imoto, H., Zhang, S. & Okada, M. A Computational Framework for Prediction and Analysis of Cancer Signaling Dynamics from RNA Sequencing Data—Application to the ErbB Receptor Signaling Pathway. _Cancers_ **12**, 2878 (2020). https://doi.org/10.3390/cancers12102878
 
 - Imoto, H., Yamashiro, S. & Okada, M. A text-based computational framework for patient -specific modeling for classification of cancers. _iScience_ **25**, 103944 (2022). https://doi.org/10.1016/j.isci.2022.103944
 
 ## Author
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biomass Version: 0.9.0 Summary: A Python Framework
+Metadata-Version: 2.1 Name: biomass Version: 0.9.1 Summary: A Python Framework
 for Modeling and Analysis of Signaling Systems Home-page: https://github.com/
 biomass-dev/biomass Author: Hiroaki Imoto Author-email: himoto@protein.osaka-
 u.ac.jp Maintainer: Hiroaki Imoto Maintainer-email: himoto@protein.osaka-
 u.ac.jp License: Apache 2.0 Download-URL: https://github.com/biomass-dev/
 biomass/releases Project-URL: Documentation, https://biomass-
 core.readthedocs.io/en/latest/ Project-URL: Source Code, https://github.com/
 biomass-dev/biomass Project-URL: Bug Tracker, https://github.com/biomass-dev/
@@ -15,15 +15,16 @@
 :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Bio-Informatics Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: docs License-File: LICENSE
+text/markdown Provides-Extra: graph Provides-Extra: dev Provides-Extra: docs
+License-File: LICENSE
 [https://raw.githubusercontent.com/biomass-dev/biomass/master/docs/_static/img/
                                biomass-logo.png]
 [![PyPI version](https://img.shields.io/pypi/v/
 biomass.svg?logo=PyPI&logoColor=white)](https://pypi.python.org/pypi/biomass)
 [![Actions Status](https://github.com/biomass-dev/biomass/workflows/Tests/
 badge.svg)](https://github.com/biomass-dev/biomass/actions) [![Documentation
 Status](https://img.shields.io/readthedocs/biomass-core/
@@ -48,18 +49,16 @@
 - **Documentation:** https://biomass-core.rtfd.io - **Source code:** https://
 github.com/biomass-dev/biomass - **Bug reports:** https://github.com/biomass-
 dev/biomass/issues - **Citing in your work:** https://biomass-core.rtfd.io/en/
 latest/citing.html It provides useful tools for numerical simulation, parameter
 estimation, network analysis, and result visualization. ## Installation The
 BioMASS library is available at the [Python Package Index (PyPI)](https://
 pypi.org/project/biomass). ```shell $ pip install biomass ``` BioMASS supports
-Python 3.7 or newer. :ledger: **Note: You will need to manually install
-[Graphviz](https://www.graphviz.org) (version 2.42 or later).** ## References -
-Imoto, H., Zhang, S. & Okada, M. A Computational Framework for Prediction and
-Analysis of Cancer Signaling Dynamics from RNA Sequencing DataâApplication to
-the ErbB Receptor Signaling Pathway. _Cancers_ **12**, 2878 (2020). https://
-doi.org/10.3390/cancers12102878 - Imoto, H., Yamashiro, S. & Okada, M. A text-
-based computational framework for patient -specific modeling for classification
-of cancers. _iScience_ **25**, 103944 (2022). https://doi.org/10.1016/
-j.isci.2022.103944 ## Author [Hiroaki Imoto](https://github.com/himoto) ##
-License [Apache License 2.0](https://github.com/biomass-dev/biomass/blob/
-master/LICENSE)
+Python 3.7 or newer. ## References - Imoto, H., Zhang, S. & Okada, M. A
+Computational Framework for Prediction and Analysis of Cancer Signaling
+Dynamics from RNA Sequencing DataâApplication to the ErbB Receptor Signaling
+Pathway. _Cancers_ **12**, 2878 (2020). https://doi.org/10.3390/cancers12102878
+- Imoto, H., Yamashiro, S. & Okada, M. A text-based computational framework for
+patient -specific modeling for classification of cancers. _iScience_ **25**,
+103944 (2022). https://doi.org/10.1016/j.isci.2022.103944 ## Author [Hiroaki
+Imoto](https://github.com/himoto) ## License [Apache License 2.0](https://
+github.com/biomass-dev/biomass/blob/master/LICENSE)
```

### Comparing `biomass-0.9.0/biomass.egg-info/SOURCES.txt` & `biomass-0.9.1/biomass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/setup.py` & `biomass-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,18 @@
             "Documentation": "https://biomass-core.readthedocs.io/en/latest/",
             "Source Code": "https://github.com/biomass-dev/biomass",
             "Bug Tracker": "https://github.com/biomass-dev/biomass/issues",
         },
         packages=find_packages(exclude=["tests", "docs"]),
         install_requires=get_install_requires(),
         extras_require={
+            "graph": [
+                "pygraphviz>=1.9",
+                "pyvis>=0.2.1",
+            ],
             "dev": [
                 "black>=20.8b1",
                 "flake8",
                 "isort",
                 "pre-commit",
                 "pytest",
             ],
```

### Comparing `biomass-0.9.0/tests/test_text2model/C.py` & `biomass-0.9.1/tests/test_text2model/C.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/tests/test_text2model/test_error_message.py` & `biomass-0.9.1/tests/test_text2model/test_error_message.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/tests/test_text2model/test_fos_model_from_txt.py` & `biomass-0.9.1/tests/test_text2model/test_fos_model_from_txt.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/tests/test_text2model/test_model_construction.py` & `biomass-0.9.1/tests/test_text2model/test_model_construction.py`

 * *Files identical despite different names*

### Comparing `biomass-0.9.0/tests/test_text2model/test_thermodynamic_restriction.py` & `biomass-0.9.1/tests/test_text2model/test_thermodynamic_restriction.py`

 * *Files identical despite different names*

