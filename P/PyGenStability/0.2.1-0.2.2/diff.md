# Comparing `tmp/PyGenStability-0.2.1.tar.gz` & `tmp/PyGenStability-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGenStability-0.2.1.tar", last modified: Fri Apr 28 09:25:35 2023, max compression
+gzip compressed data, was "PyGenStability-0.2.2.tar", last modified: Fri May  5 07:04:54 2023, max compression
```

## Comparing `PyGenStability-0.2.1.tar` & `PyGenStability-0.2.2.tar`

### file list

```diff
@@ -1,136 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.661808 PyGenStability-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-04-28 09:25:35.661808 PyGenStability-0.2.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    12183 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.645808 PyGenStability-0.2.1/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.657808 PyGenStability-0.2.1/extra/lemon/
--rw-r--r--   0 runner    (1001) docker     (123)   112976 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/adaptors.h
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/arg_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/assert.h
--rw-r--r--   0 runner    (1001) docker     (123)    38788 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bellman_ford.h
--rw-r--r--   0 runner    (1001) docker     (123)    55605 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bfs.h
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bin_heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/binomial_heap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.657808 PyGenStability-0.2.1/extra/lemon/bits/
--rw-r--r--   0 runner    (1001) docker     (123)    15730 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/alteration_notifier.h
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/array_map.h
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/bezier.h
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/default_map.h
--rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/edge_set_extender.h
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/enable_if.h
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/graph_adaptor_extender.h
--rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/graph_extender.h
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/lock.h
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/map_extender.h
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/path_dump.h
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/solver_bits.h
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/traits.h
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/variant.h
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/vector_map.h
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bits/windows.h
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/bucket_heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    32476 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/capacity_scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/cbc.h
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/christofides_tsp.h
--rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/circulation.h
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/clp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/color.h
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/concept_check.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.657808 PyGenStability-0.2.1/extra/lemon/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)    33103 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/concepts/bpgraph.h
--rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/concepts/digraph.h
--rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/concepts/graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    70657 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/concepts/graph_components.h
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/concepts/heap.h
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/concepts/maps.h
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/concepts/path.h
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/config.h
--rw-r--r--   0 runner    (1001) docker     (123)    51928 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/connectivity.h
--rw-r--r--   0 runner    (1001) docker     (123)    84609 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/core.h
--rw-r--r--   0 runner    (1001) docker     (123)    52740 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/cost_scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/counter.h
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/cplex.h
--rw-r--r--   0 runner    (1001) docker     (123)    41529 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/cycle_canceling.h
--rw-r--r--   0 runner    (1001) docker     (123)    51690 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/dheap.h
--rw-r--r--   0 runner    (1001) docker     (123)    44037 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/dijkstra.h
--rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/dim2.h
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/dimacs.h
--rw-r--r--   0 runner    (1001) docker     (123)    37594 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/edge_set.h
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/edmonds_karp.h
--rw-r--r--   0 runner    (1001) docker     (123)    27039 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/elevator.h
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/error.h
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/euler.h
--rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/fib_heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    64564 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/fractional_matching.h
--rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/full_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/glpk.h
--rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/gomory_hu.h
--rw-r--r--   0 runner    (1001) docker     (123)    38686 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/graph_to_eps.h
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/greedy_tsp.h
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/grid_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    25284 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/grosso_locatelli_pullan_mc.h
--rw-r--r--   0 runner    (1001) docker     (123)    31632 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/hao_orlin.h
--rw-r--r--   0 runner    (1001) docker     (123)    19939 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/hartmann_orlin_mmc.h
--rw-r--r--   0 runner    (1001) docker     (123)    20199 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/howard_mmc.h
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/hypercube_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/insertion_tsp.h
--rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/karp_mmc.h
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/kruskal.h
--rw-r--r--   0 runner    (1001) docker     (123)   119973 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/lgf_reader.h
--rw-r--r--   0 runner    (1001) docker     (123)    84311 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/lgf_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)    71515 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/list_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/lp.h
--rw-r--r--   0 runner    (1001) docker     (123)    64377 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/lp_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/lp_skeleton.h
--rw-r--r--   0 runner    (1001) docker     (123)   119337 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/maps.h
--rw-r--r--   0 runner    (1001) docker     (123)   112822 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/matching.h
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/math.h
--rw-r--r--   0 runner    (1001) docker     (123)    26717 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/max_cardinality_search.h
--rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/min_cost_arborescence.h
--rw-r--r--   0 runner    (1001) docker     (123)    22036 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/nagamochi_ibaraki.h
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/nauty_reader.h
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/nearest_neighbor_tsp.h
--rw-r--r--   0 runner    (1001) docker     (123)    52906 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/network_simplex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/opt2_tsp.h
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/pairing_heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    31339 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/path.h
--rw-r--r--   0 runner    (1001) docker     (123)    86230 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/planarity.h
--rw-r--r--   0 runner    (1001) docker     (123)    31028 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/preflow.h
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/quad_heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/radix_heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/radix_sort.h
--rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/random.h
--rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/smart_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/soplex.h
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/static_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    23880 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/suurballe.h
--rw-r--r--   0 runner    (1001) docker     (123)    15371 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/time_measure.h
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/tolerance.h
--rw-r--r--   0 runner    (1001) docker     (123)    50397 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/extra/lemon/unionfind.h
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:25:35.661808 PyGenStability-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.645808 PyGenStability-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.657808 PyGenStability-0.2.1/src/PyGenStability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-04-28 09:25:35.000000 PyGenStability-0.2.1/src/PyGenStability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-28 09:25:35.000000 PyGenStability-0.2.1/src/PyGenStability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:25:35.000000 PyGenStability-0.2.1/src/PyGenStability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 09:25:35.000000 PyGenStability-0.2.1/src/PyGenStability.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:25:35.000000 PyGenStability-0.2.1/src/PyGenStability.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 09:25:35.000000 PyGenStability-0.2.1/src/PyGenStability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:25:35.000000 PyGenStability-0.2.1/src/PyGenStability.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.661808 PyGenStability-0.2.1/src/pygenstability/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    16324 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.661808 PyGenStability-0.2.1/src/pygenstability/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/contrib/sankey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:25:35.661808 PyGenStability-0.2.1/src/pygenstability/generalized_louvain/
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/generalized_louvain/generalized_louvain.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/optimal_scales.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-04-28 09:25:31.000000 PyGenStability-0.2.1/src/pygenstability/pygenstability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12183 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.815445 PyGenStability-0.2.2/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.827445 PyGenStability-0.2.2/extra/lemon/
+-rw-r--r--   0 runner    (1001) docker     (123)   112976 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/adaptors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/arg_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/assert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38788 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bellman_ford.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55605 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bin_heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/binomial_heap.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.831445 PyGenStability-0.2.2/extra/lemon/bits/
+-rw-r--r--   0 runner    (1001) docker     (123)    15730 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/alteration_notifier.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/array_map.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/bezier.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/default_map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/edge_set_extender.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/enable_if.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/graph_adaptor_extender.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/graph_extender.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/lock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/map_extender.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/path_dump.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/solver_bits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/traits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/variant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/vector_map.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bits/windows.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/bucket_heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32476 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/capacity_scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/cbc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/christofides_tsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/circulation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/clp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/color.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/concept_check.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.831445 PyGenStability-0.2.2/extra/lemon/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)    33103 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/concepts/bpgraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/concepts/digraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/concepts/graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    70657 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/concepts/graph_components.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/concepts/heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/concepts/maps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/concepts/path.h
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51928 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/connectivity.h
+-rw-r--r--   0 runner    (1001) docker     (123)    84609 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52740 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/cost_scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/counter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/cplex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41529 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/cycle_canceling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51690 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/dheap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44037 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/dijkstra.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/dim2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/dimacs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37594 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/edge_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/edmonds_karp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27039 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/elevator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/euler.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/fib_heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64564 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/fractional_matching.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/full_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/glpk.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/gomory_hu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38686 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/graph_to_eps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/greedy_tsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/grid_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25284 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/grosso_locatelli_pullan_mc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31632 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/hao_orlin.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19939 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/hartmann_orlin_mmc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20199 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/howard_mmc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/hypercube_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/insertion_tsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/karp_mmc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/kruskal.h
+-rw-r--r--   0 runner    (1001) docker     (123)   119973 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/lgf_reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    84311 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/lgf_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    71515 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/list_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/lp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64377 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/lp_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/lp_skeleton.h
+-rw-r--r--   0 runner    (1001) docker     (123)   119337 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/maps.h
+-rw-r--r--   0 runner    (1001) docker     (123)   112822 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/matching.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26717 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/max_cardinality_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/min_cost_arborescence.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22036 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/nagamochi_ibaraki.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/nauty_reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/nearest_neighbor_tsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52906 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/network_simplex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/opt2_tsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/pairing_heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31339 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/path.h
+-rw-r--r--   0 runner    (1001) docker     (123)    86230 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/planarity.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31028 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/preflow.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/quad_heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/radix_heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/radix_sort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/smart_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/soplex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/static_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23880 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/suurballe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15371 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/time_measure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/tolerance.h
+-rw-r--r--   0 runner    (1001) docker     (123)    50397 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/extra/lemon/unionfind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/generalizedLouvain/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/.git
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CODE_HISTORY.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.815445 PyGenStability-0.2.2/generalizedLouvain/CPP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/graphhelpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/linearised_internals_comb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/linearised_internals_generic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/linearised_internals_norm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/louvain_gen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/run_gen_louvain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/stability.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/stability_gen.h
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/triangletest.edj
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/triangletest_null.edj
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/CPP/cliques/vector_partition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6522 2023-05-05 07:04:51.000000 PyGenStability-0.2.2/generalizedLouvain/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.815445 PyGenStability-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/src/PyGenStability.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-05-05 07:04:54.000000 PyGenStability-0.2.2/src/PyGenStability.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-05 07:04:54.000000 PyGenStability-0.2.2/src/PyGenStability.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:04:54.000000 PyGenStability-0.2.2/src/PyGenStability.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 07:04:54.000000 PyGenStability-0.2.2/src/PyGenStability.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:04:54.000000 PyGenStability-0.2.2/src/PyGenStability.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 07:04:54.000000 PyGenStability-0.2.2/src/PyGenStability.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 07:04:54.000000 PyGenStability-0.2.2/src/PyGenStability.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/src/pygenstability/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16324 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/src/pygenstability/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/contrib/sankey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:04:54.835446 PyGenStability-0.2.2/src/pygenstability/generalized_louvain/
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/generalized_louvain/generalized_louvain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/optimal_scales.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-05-05 07:04:50.000000 PyGenStability-0.2.2/src/pygenstability/pygenstability.py
```

### Comparing `PyGenStability-0.2.1/LICENSE` & `PyGenStability-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/PKG-INFO` & `PyGenStability-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGenStability
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python binding of generalised Louvain with Markov Stability
 Home-page: https://github.com/ImperialCollegeLondon/PyGenStability
 Author: Alexis Arnaudon
 Author-email: alexis.arnaudon@epfl.ch
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyGenStability-0.2.1/README.md` & `PyGenStability-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/adaptors.h` & `PyGenStability-0.2.2/extra/lemon/adaptors.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/arg_parser.h` & `PyGenStability-0.2.2/extra/lemon/arg_parser.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/assert.h` & `PyGenStability-0.2.2/extra/lemon/assert.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bellman_ford.h` & `PyGenStability-0.2.2/extra/lemon/bellman_ford.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bfs.h` & `PyGenStability-0.2.2/extra/lemon/bfs.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bin_heap.h` & `PyGenStability-0.2.2/extra/lemon/bin_heap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/binomial_heap.h` & `PyGenStability-0.2.2/extra/lemon/binomial_heap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/alteration_notifier.h` & `PyGenStability-0.2.2/extra/lemon/bits/alteration_notifier.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/array_map.h` & `PyGenStability-0.2.2/extra/lemon/bits/array_map.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/bezier.h` & `PyGenStability-0.2.2/extra/lemon/bits/bezier.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/default_map.h` & `PyGenStability-0.2.2/extra/lemon/bits/default_map.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/edge_set_extender.h` & `PyGenStability-0.2.2/extra/lemon/bits/edge_set_extender.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/enable_if.h` & `PyGenStability-0.2.2/extra/lemon/bits/enable_if.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/graph_adaptor_extender.h` & `PyGenStability-0.2.2/extra/lemon/bits/graph_adaptor_extender.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/graph_extender.h` & `PyGenStability-0.2.2/extra/lemon/bits/graph_extender.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/lock.h` & `PyGenStability-0.2.2/extra/lemon/bits/lock.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/map_extender.h` & `PyGenStability-0.2.2/extra/lemon/bits/map_extender.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/path_dump.h` & `PyGenStability-0.2.2/extra/lemon/bits/path_dump.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/solver_bits.h` & `PyGenStability-0.2.2/extra/lemon/bits/solver_bits.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/traits.h` & `PyGenStability-0.2.2/extra/lemon/bits/traits.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/variant.h` & `PyGenStability-0.2.2/extra/lemon/bits/variant.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/vector_map.h` & `PyGenStability-0.2.2/extra/lemon/bits/vector_map.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bits/windows.h` & `PyGenStability-0.2.2/extra/lemon/bits/windows.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/bucket_heap.h` & `PyGenStability-0.2.2/extra/lemon/bucket_heap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/capacity_scaling.h` & `PyGenStability-0.2.2/extra/lemon/capacity_scaling.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/cbc.h` & `PyGenStability-0.2.2/extra/lemon/cbc.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/christofides_tsp.h` & `PyGenStability-0.2.2/extra/lemon/christofides_tsp.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/circulation.h` & `PyGenStability-0.2.2/extra/lemon/circulation.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/clp.h` & `PyGenStability-0.2.2/extra/lemon/clp.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/color.h` & `PyGenStability-0.2.2/extra/lemon/color.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/concept_check.h` & `PyGenStability-0.2.2/extra/lemon/concept_check.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/concepts/bpgraph.h` & `PyGenStability-0.2.2/extra/lemon/concepts/bpgraph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/concepts/digraph.h` & `PyGenStability-0.2.2/extra/lemon/concepts/digraph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/concepts/graph.h` & `PyGenStability-0.2.2/extra/lemon/concepts/graph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/concepts/graph_components.h` & `PyGenStability-0.2.2/extra/lemon/concepts/graph_components.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/concepts/heap.h` & `PyGenStability-0.2.2/extra/lemon/concepts/heap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/concepts/maps.h` & `PyGenStability-0.2.2/extra/lemon/concepts/maps.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/concepts/path.h` & `PyGenStability-0.2.2/extra/lemon/concepts/path.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/connectivity.h` & `PyGenStability-0.2.2/extra/lemon/connectivity.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/core.h` & `PyGenStability-0.2.2/extra/lemon/core.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/cost_scaling.h` & `PyGenStability-0.2.2/extra/lemon/cost_scaling.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/counter.h` & `PyGenStability-0.2.2/extra/lemon/counter.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/cplex.h` & `PyGenStability-0.2.2/extra/lemon/cplex.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/cycle_canceling.h` & `PyGenStability-0.2.2/extra/lemon/cycle_canceling.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/dfs.h` & `PyGenStability-0.2.2/extra/lemon/dfs.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/dheap.h` & `PyGenStability-0.2.2/extra/lemon/dheap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/dijkstra.h` & `PyGenStability-0.2.2/extra/lemon/dijkstra.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/dim2.h` & `PyGenStability-0.2.2/extra/lemon/dim2.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/dimacs.h` & `PyGenStability-0.2.2/extra/lemon/dimacs.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/edge_set.h` & `PyGenStability-0.2.2/extra/lemon/edge_set.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/edmonds_karp.h` & `PyGenStability-0.2.2/extra/lemon/edmonds_karp.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/elevator.h` & `PyGenStability-0.2.2/extra/lemon/elevator.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/error.h` & `PyGenStability-0.2.2/extra/lemon/error.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/euler.h` & `PyGenStability-0.2.2/extra/lemon/euler.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/fib_heap.h` & `PyGenStability-0.2.2/extra/lemon/fib_heap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/fractional_matching.h` & `PyGenStability-0.2.2/extra/lemon/fractional_matching.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/full_graph.h` & `PyGenStability-0.2.2/extra/lemon/full_graph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/glpk.h` & `PyGenStability-0.2.2/extra/lemon/glpk.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/gomory_hu.h` & `PyGenStability-0.2.2/extra/lemon/gomory_hu.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/graph_to_eps.h` & `PyGenStability-0.2.2/extra/lemon/graph_to_eps.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/greedy_tsp.h` & `PyGenStability-0.2.2/extra/lemon/greedy_tsp.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/grid_graph.h` & `PyGenStability-0.2.2/extra/lemon/grid_graph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/grosso_locatelli_pullan_mc.h` & `PyGenStability-0.2.2/extra/lemon/grosso_locatelli_pullan_mc.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/hao_orlin.h` & `PyGenStability-0.2.2/extra/lemon/hao_orlin.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/hartmann_orlin_mmc.h` & `PyGenStability-0.2.2/extra/lemon/hartmann_orlin_mmc.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/howard_mmc.h` & `PyGenStability-0.2.2/extra/lemon/howard_mmc.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/hypercube_graph.h` & `PyGenStability-0.2.2/extra/lemon/hypercube_graph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/insertion_tsp.h` & `PyGenStability-0.2.2/extra/lemon/insertion_tsp.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/karp_mmc.h` & `PyGenStability-0.2.2/extra/lemon/karp_mmc.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/kruskal.h` & `PyGenStability-0.2.2/extra/lemon/kruskal.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/lgf_reader.h` & `PyGenStability-0.2.2/extra/lemon/lgf_reader.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/lgf_writer.h` & `PyGenStability-0.2.2/extra/lemon/lgf_writer.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/list_graph.h` & `PyGenStability-0.2.2/extra/lemon/list_graph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/lp.h` & `PyGenStability-0.2.2/extra/lemon/lp.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/lp_base.h` & `PyGenStability-0.2.2/extra/lemon/lp_base.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/lp_skeleton.h` & `PyGenStability-0.2.2/extra/lemon/lp_skeleton.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/maps.h` & `PyGenStability-0.2.2/extra/lemon/maps.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/matching.h` & `PyGenStability-0.2.2/extra/lemon/matching.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/math.h` & `PyGenStability-0.2.2/extra/lemon/math.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/max_cardinality_search.h` & `PyGenStability-0.2.2/extra/lemon/max_cardinality_search.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/min_cost_arborescence.h` & `PyGenStability-0.2.2/extra/lemon/min_cost_arborescence.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/nagamochi_ibaraki.h` & `PyGenStability-0.2.2/extra/lemon/nagamochi_ibaraki.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/nauty_reader.h` & `PyGenStability-0.2.2/extra/lemon/nauty_reader.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/nearest_neighbor_tsp.h` & `PyGenStability-0.2.2/extra/lemon/nearest_neighbor_tsp.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/network_simplex.h` & `PyGenStability-0.2.2/extra/lemon/network_simplex.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/opt2_tsp.h` & `PyGenStability-0.2.2/extra/lemon/opt2_tsp.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/pairing_heap.h` & `PyGenStability-0.2.2/extra/lemon/pairing_heap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/path.h` & `PyGenStability-0.2.2/extra/lemon/path.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/planarity.h` & `PyGenStability-0.2.2/extra/lemon/planarity.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/preflow.h` & `PyGenStability-0.2.2/extra/lemon/preflow.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/quad_heap.h` & `PyGenStability-0.2.2/extra/lemon/quad_heap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/radix_heap.h` & `PyGenStability-0.2.2/extra/lemon/radix_heap.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/radix_sort.h` & `PyGenStability-0.2.2/extra/lemon/radix_sort.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/random.h` & `PyGenStability-0.2.2/extra/lemon/random.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/smart_graph.h` & `PyGenStability-0.2.2/extra/lemon/smart_graph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/soplex.h` & `PyGenStability-0.2.2/extra/lemon/soplex.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/static_graph.h` & `PyGenStability-0.2.2/extra/lemon/static_graph.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/suurballe.h` & `PyGenStability-0.2.2/extra/lemon/suurballe.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/time_measure.h` & `PyGenStability-0.2.2/extra/lemon/time_measure.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/tolerance.h` & `PyGenStability-0.2.2/extra/lemon/tolerance.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/extra/lemon/unionfind.h` & `PyGenStability-0.2.2/extra/lemon/unionfind.h`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/setup.py` & `PyGenStability-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 from pybind11.setup_helpers import Pybind11Extension
-from setuptools import find_packages
+from setuptools import find_namespace_packages
 from setuptools import setup
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 ext_modules = [
     Pybind11Extension(
         "pygenstability.generalized_louvain",
         ["src/pygenstability/generalized_louvain/generalized_louvain.cpp"],
         include_dirs=["extra", "generalizedLouvain"],
         extra_compile_args=["-std=c++11"],
@@ -53,11 +53,11 @@
     install_requires=install_requires,
     zip_safe=False,
     extras_require={
         "plotly": plotly_require,
         "all": plotly_require + test_require,
     },
     entry_points={"console_scripts": ["pygenstability=pygenstability.app:cli"]},
-    packages=find_packages("src", exclude=["tests"]),
+    packages=find_namespace_packages("src"),
     include_package_data=True,
     package_dir={"": "src"},
 )
```

### Comparing `PyGenStability-0.2.1/src/PyGenStability.egg-info/PKG-INFO` & `PyGenStability-0.2.2/src/PyGenStability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGenStability
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python binding of generalised Louvain with Markov Stability
 Home-page: https://github.com/ImperialCollegeLondon/PyGenStability
 Author: Alexis Arnaudon
 Author-email: alexis.arnaudon@epfl.ch
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyGenStability-0.2.1/src/PyGenStability.egg-info/SOURCES.txt` & `PyGenStability-0.2.2/src/PyGenStability.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -101,14 +101,31 @@
 extra/lemon/concepts/bpgraph.h
 extra/lemon/concepts/digraph.h
 extra/lemon/concepts/graph.h
 extra/lemon/concepts/graph_components.h
 extra/lemon/concepts/heap.h
 extra/lemon/concepts/maps.h
 extra/lemon/concepts/path.h
+generalizedLouvain/.git
+generalizedLouvain/CODE_HISTORY.txt
+generalizedLouvain/LICENSE
+generalizedLouvain/README.md
+generalizedLouvain/CPP/cliques/Makefile
+generalizedLouvain/CPP/cliques/graphhelpers.h
+generalizedLouvain/CPP/cliques/io.h
+generalizedLouvain/CPP/cliques/linearised_internals_comb.h
+generalizedLouvain/CPP/cliques/linearised_internals_generic.h
+generalizedLouvain/CPP/cliques/linearised_internals_norm.h
+generalizedLouvain/CPP/cliques/louvain_gen.h
+generalizedLouvain/CPP/cliques/run_gen_louvain.cpp
+generalizedLouvain/CPP/cliques/stability.h
+generalizedLouvain/CPP/cliques/stability_gen.h
+generalizedLouvain/CPP/cliques/triangletest.edj
+generalizedLouvain/CPP/cliques/triangletest_null.edj
+generalizedLouvain/CPP/cliques/vector_partition.h
 src/PyGenStability.egg-info/PKG-INFO
 src/PyGenStability.egg-info/SOURCES.txt
 src/PyGenStability.egg-info/dependency_links.txt
 src/PyGenStability.egg-info/entry_points.txt
 src/PyGenStability.egg-info/not-zip-safe
 src/PyGenStability.egg-info/requires.txt
 src/PyGenStability.egg-info/top_level.txt
```

### Comparing `PyGenStability-0.2.1/src/pygenstability/app.py` & `PyGenStability-0.2.2/src/pygenstability/app.py`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/src/pygenstability/constructors.py` & `PyGenStability-0.2.2/src/pygenstability/constructors.py`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/src/pygenstability/contrib/sankey.py` & `PyGenStability-0.2.2/src/pygenstability/contrib/sankey.py`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/src/pygenstability/generalized_louvain/generalized_louvain.cpp` & `PyGenStability-0.2.2/src/pygenstability/generalized_louvain/generalized_louvain.cpp`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/src/pygenstability/optimal_scales.py` & `PyGenStability-0.2.2/src/pygenstability/optimal_scales.py`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/src/pygenstability/plotting.py` & `PyGenStability-0.2.2/src/pygenstability/plotting.py`

 * *Files identical despite different names*

### Comparing `PyGenStability-0.2.1/src/pygenstability/pygenstability.py` & `PyGenStability-0.2.2/src/pygenstability/pygenstability.py`

 * *Files identical despite different names*

