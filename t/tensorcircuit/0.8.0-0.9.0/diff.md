# Comparing `tmp/tensorcircuit-0.8.0.tar.gz` & `tmp/tensorcircuit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensorcircuit-0.8.0.tar", last modified: Tue Mar 28 04:19:06 2023, max compression
+gzip compressed data, was "dist/tensorcircuit-0.9.0.tar", last modified: Fri May  5 09:12:51 2023, max compression
```

## Comparing `tensorcircuit-0.8.0.tar` & `tensorcircuit-0.9.0.tar`

### file list

```diff
@@ -1,157 +1,169 @@
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.687289 tensorcircuit-0.8.0/
--rw-r--r--   0 shixin     (501) staff       (20)    22586 2023-03-28 04:13:56.000000 tensorcircuit-0.8.0/CHANGELOG.md
--rw-r--r--   0 shixin     (501) staff       (20)     1023 2023-01-31 08:54:48.000000 tensorcircuit-0.8.0/HISTORY.md
--rw-r--r--   0 shixin     (501) staff       (20)    11358 2021-12-08 02:25:17.000000 tensorcircuit-0.8.0/LICENSE
--rw-r--r--   0 shixin     (501) staff       (20)      132 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/MANIFEST.in
--rw-r--r--   0 shixin     (501) staff       (20)    17814 2023-03-28 04:19:06.686699 tensorcircuit-0.8.0/PKG-INFO
--rw-r--r--   0 shixin     (501) staff       (20)    17287 2023-03-07 02:17:54.000000 tensorcircuit-0.8.0/README.md
--rw-r--r--   0 shixin     (501) staff       (20)     5352 2023-03-07 02:17:54.000000 tensorcircuit-0.8.0/README_cn.md
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.379864 tensorcircuit-0.8.0/docs/
--rw-r--r--   0 shixin     (501) staff       (20)      614 2020-04-19 06:32:37.000000 tensorcircuit-0.8.0/docs/Makefile
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.506616 tensorcircuit-0.8.0/docs/source/
--rw-r--r--   0 shixin     (501) staff       (20)     6148 2022-06-10 06:25:56.000000 tensorcircuit-0.8.0/docs/source/.DS_Store
--rw-r--r--   0 shixin     (501) staff       (20)     6332 2022-11-10 08:49:43.000000 tensorcircuit-0.8.0/docs/source/advance.rst
--rw-r--r--   0 shixin     (501) staff       (20)     6308 2023-02-02 06:28:30.000000 tensorcircuit-0.8.0/docs/source/cnconf.py
--rw-r--r--   0 shixin     (501) staff       (20)     6367 2023-02-02 06:28:30.000000 tensorcircuit-0.8.0/docs/source/conf.py
--rw-r--r--   0 shixin     (501) staff       (20)     8192 2022-09-15 11:59:08.000000 tensorcircuit-0.8.0/docs/source/contribution.rst
--rw-r--r--   0 shixin     (501) staff       (20)    10971 2022-09-15 11:59:08.000000 tensorcircuit-0.8.0/docs/source/faq.rst
--rw-r--r--   0 shixin     (501) staff       (20)     3677 2023-02-09 09:31:26.000000 tensorcircuit-0.8.0/docs/source/generate_rst.py
--rw-r--r--   0 shixin     (501) staff       (20)     2551 2023-02-03 06:22:37.000000 tensorcircuit-0.8.0/docs/source/index.rst
--rw-r--r--   0 shixin     (501) staff       (20)      374 2022-05-17 08:27:32.000000 tensorcircuit-0.8.0/docs/source/index_cn.rst.disable
--rw-r--r--   0 shixin     (501) staff       (20)     8413 2023-01-03 14:10:58.000000 tensorcircuit-0.8.0/docs/source/infras.rst
--rw-r--r--   0 shixin     (501) staff       (20)      640 2023-03-07 02:17:54.000000 tensorcircuit-0.8.0/docs/source/modules.rst
--rw-r--r--   0 shixin     (501) staff       (20)     4334 2022-04-13 08:43:33.000000 tensorcircuit-0.8.0/docs/source/modules.rst.backup
--rw-r--r--   0 shixin     (501) staff       (20)    26892 2023-02-02 06:28:30.000000 tensorcircuit-0.8.0/docs/source/quickstart.rst
--rw-r--r--   0 shixin     (501) staff       (20)     6229 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/docs/source/sharpbits.rst
--rw-r--r--   0 shixin     (501) staff       (20)      226 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/docs/source/textbooktoc.rst
--rw-r--r--   0 shixin     (501) staff       (20)      626 2022-12-06 06:08:27.000000 tensorcircuit-0.8.0/docs/source/tutorial.rst
--rw-r--r--   0 shixin     (501) staff       (20)      669 2022-12-06 06:08:27.000000 tensorcircuit-0.8.0/docs/source/tutorial_cn.rst
--rw-r--r--   0 shixin     (501) staff       (20)      509 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/docs/source/whitepapertoc.rst
--rw-r--r--   0 shixin     (501) staff       (20)      531 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/docs/source/whitepapertoc_cn.rst
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.572713 tensorcircuit-0.8.0/examples/
--rw-r--r--   0 shixin     (501) staff       (20)     2172 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/GHZ_DQAS.py
--rw-r--r--   0 shixin     (501) staff       (20)    61992 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/H6_hamiltonian.npy
--rw-r--r--   0 shixin     (501) staff       (20)     3984 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/QAOA_DQAS.py
--rw-r--r--   0 shixin     (501) staff       (20)     1303 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/QEM_DQAS.py
--rw-r--r--   0 shixin     (501) staff       (20)     3345 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/adiabatic_vqnhe.py
--rw-r--r--   0 shixin     (501) staff       (20)     2573 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/chaotic_behavior.py
--rw-r--r--   0 shixin     (501) staff       (20)     2760 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/checkpoint_memsave.py
--rw-r--r--   0 shixin     (501) staff       (20)     6713 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/gradient_benchmark.py
--rw-r--r--   0 shixin     (501) staff       (20)      949 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/hamiltonian_building.py
--rw-r--r--   0 shixin     (501) staff       (20)     1729 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/hchainhamiltonian.py
--rw-r--r--   0 shixin     (501) staff       (20)     1884 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/incremental_twoqubit.py
--rw-r--r--   0 shixin     (501) staff       (20)     2593 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/mcnoise_boost.py
--rw-r--r--   0 shixin     (501) staff       (20)     1675 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/mcnoise_check.py
--rw-r--r--   0 shixin     (501) staff       (20)     2398 2022-11-02 01:16:04.000000 tensorcircuit-0.8.0/examples/mpsvsexact.py
--rw-r--r--   0 shixin     (501) staff       (20)     5217 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/noisy_qml.py
--rw-r--r--   0 shixin     (501) staff       (20)     2289 2023-02-09 09:31:26.000000 tensorcircuit-0.8.0/examples/optperformance_comparison.py
--rw-r--r--   0 shixin     (501) staff       (20)      971 2021-11-17 07:46:30.000000 tensorcircuit-0.8.0/examples/qaoa_block.result
--rw-r--r--   0 shixin     (501) staff       (20)      736 2022-02-17 02:39:55.000000 tensorcircuit-0.8.0/examples/qaoa_graph.py.outdated
--rw-r--r--   0 shixin     (501) staff       (20)     1145 2022-02-17 02:39:48.000000 tensorcircuit-0.8.0/examples/qaoa_micro.py.outdated
--rw-r--r--   0 shixin     (501) staff       (20)      724 2022-04-13 08:43:33.000000 tensorcircuit-0.8.0/examples/qaoa_parallel_opt.py
--rw-r--r--   0 shixin     (501) staff       (20)     2523 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/quantumng.py
--rw-r--r--   0 shixin     (501) staff       (20)     2200 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/simple_qaoa.py
--rw-r--r--   0 shixin     (501) staff       (20)     2628 2023-02-09 09:31:26.000000 tensorcircuit-0.8.0/examples/universal_lr.py
--rw-r--r--   0 shixin     (501) staff       (20)     3412 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/variational_dynamics.py
--rw-r--r--   0 shixin     (501) staff       (20)     3533 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/vqe_extra.py
--rw-r--r--   0 shixin     (501) staff       (20)     3989 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/vqe_extra_mpo.py
--rw-r--r--   0 shixin     (501) staff       (20)     4094 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/vqe_extra_mpo_spopt.py
--rw-r--r--   0 shixin     (501) staff       (20)     4004 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/vqeh2o_benchmark.py
--rw-r--r--   0 shixin     (501) staff       (20)     1005 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/examples/vqnhe_h6.py
--rw-r--r--   0 shixin     (501) staff       (20)       38 2023-03-28 04:19:06.687598 tensorcircuit-0.8.0/setup.cfg
--rw-r--r--   0 shixin     (501) staff       (20)      929 2023-03-28 04:12:04.000000 tensorcircuit-0.8.0/setup.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.609715 tensorcircuit-0.8.0/tensorcircuit/
--rw-r--r--   0 shixin     (501) staff       (20)     1313 2023-03-28 04:14:19.000000 tensorcircuit-0.8.0/tensorcircuit/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)    39188 2023-02-24 11:07:51.000000 tensorcircuit-0.8.0/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.629792 tensorcircuit-0.8.0/tensorcircuit/applications/
--rw-r--r--   0 shixin     (501) staff       (20)      234 2021-12-08 02:25:17.000000 tensorcircuit-0.8.0/tensorcircuit/applications/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)    34460 2023-02-09 09:31:26.000000 tensorcircuit-0.8.0/tensorcircuit/applications/dqas.py
--rw-r--r--   0 shixin     (501) staff       (20)    15348 2023-01-12 02:43:07.000000 tensorcircuit-0.8.0/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 shixin     (501) staff       (20)    18124 2023-01-12 02:43:07.000000 tensorcircuit-0.8.0/tensorcircuit/applications/layers.py
--rw-r--r--   0 shixin     (501) staff       (20)    14032 2022-10-24 07:13:36.000000 tensorcircuit-0.8.0/tensorcircuit/applications/utils.py
--rw-r--r--   0 shixin     (501) staff       (20)    36391 2023-02-09 09:31:26.000000 tensorcircuit-0.8.0/tensorcircuit/applications/vags.py
--rw-r--r--   0 shixin     (501) staff       (20)    15117 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/tensorcircuit/applications/van.py
--rw-r--r--   0 shixin     (501) staff       (20)    23156 2023-02-09 09:31:26.000000 tensorcircuit-0.8.0/tensorcircuit/applications/vqes.py
--rw-r--r--   0 shixin     (501) staff       (20)     8235 2023-01-12 02:43:07.000000 tensorcircuit-0.8.0/tensorcircuit/asciiart.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.643775 tensorcircuit-0.8.0/tensorcircuit/backends/
--rw-r--r--   0 shixin     (501) staff       (20)       80 2022-09-15 11:59:08.000000 tensorcircuit-0.8.0/tensorcircuit/backends/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)    56979 2022-11-23 06:09:06.000000 tensorcircuit-0.8.0/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)     1713 2023-03-15 12:33:25.000000 tensorcircuit-0.8.0/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 shixin     (501) staff       (20)    14540 2023-03-15 12:33:25.000000 tensorcircuit-0.8.0/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)    24612 2023-01-12 02:43:07.000000 tensorcircuit-0.8.0/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)     4024 2022-10-14 04:00:52.000000 tensorcircuit-0.8.0/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 shixin     (501) staff       (20)    13794 2023-01-12 02:43:07.000000 tensorcircuit-0.8.0/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)    21968 2023-01-09 04:05:15.000000 tensorcircuit-0.8.0/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)     3198 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 shixin     (501) staff       (20)    30653 2023-03-02 11:06:11.000000 tensorcircuit-0.8.0/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)     3377 2022-10-14 04:00:52.000000 tensorcircuit-0.8.0/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 shixin     (501) staff       (20)    34020 2023-01-06 02:47:27.000000 tensorcircuit-0.8.0/tensorcircuit/basecircuit.py
--rw-r--r--   0 shixin     (501) staff       (20)    28637 2023-02-16 11:05:26.000000 tensorcircuit-0.8.0/tensorcircuit/channels.py
--rw-r--r--   0 shixin     (501) staff       (20)    36236 2023-03-08 05:54:05.000000 tensorcircuit-0.8.0/tensorcircuit/circuit.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.646735 tensorcircuit-0.8.0/tensorcircuit/compiler/
--rw-r--r--   0 shixin     (501) staff       (20)      165 2023-02-16 12:22:32.000000 tensorcircuit-0.8.0/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     1490 2023-02-16 12:22:32.000000 tensorcircuit-0.8.0/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 shixin     (501) staff       (20)     5215 2023-02-08 08:23:22.000000 tensorcircuit-0.8.0/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 shixin     (501) staff       (20)    28754 2023-02-07 06:55:30.000000 tensorcircuit-0.8.0/tensorcircuit/cons.py
--rw-r--r--   0 shixin     (501) staff       (20)    13806 2023-01-12 06:00:13.000000 tensorcircuit-0.8.0/tensorcircuit/densitymatrix.py
--rw-r--r--   0 shixin     (501) staff       (20)    15210 2023-03-02 11:06:11.000000 tensorcircuit-0.8.0/tensorcircuit/experimental.py
--rw-r--r--   0 shixin     (501) staff       (20)    29143 2023-01-21 00:54:58.000000 tensorcircuit-0.8.0/tensorcircuit/gates.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.652904 tensorcircuit-0.8.0/tensorcircuit/interfaces/
--rw-r--r--   0 shixin     (501) staff       (20)      448 2022-09-15 11:59:08.000000 tensorcircuit-0.8.0/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     1439 2022-09-15 02:01:16.000000 tensorcircuit-0.8.0/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 shixin     (501) staff       (20)     3402 2023-02-24 11:07:51.000000 tensorcircuit-0.8.0/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 shixin     (501) staff       (20)     3355 2023-01-03 14:10:36.000000 tensorcircuit-0.8.0/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 shixin     (501) staff       (20)     9942 2023-01-03 14:10:36.000000 tensorcircuit-0.8.0/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 shixin     (501) staff       (20)     3580 2023-01-03 13:47:26.000000 tensorcircuit-0.8.0/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 shixin     (501) staff       (20)     9975 2023-02-24 11:07:51.000000 tensorcircuit-0.8.0/tensorcircuit/keras.py
--rw-r--r--   0 shixin     (501) staff       (20)    15270 2023-02-09 09:31:26.000000 tensorcircuit-0.8.0/tensorcircuit/mps_base.py
--rw-r--r--   0 shixin     (501) staff       (20)    34398 2022-12-30 04:36:58.000000 tensorcircuit-0.8.0/tensorcircuit/mpscircuit.py
--rw-r--r--   0 shixin     (501) staff       (20)    11878 2023-02-24 11:07:51.000000 tensorcircuit-0.8.0/tensorcircuit/noisemodel.py
--rw-r--r--   0 shixin     (501) staff       (20)    82850 2023-03-17 08:18:25.000000 tensorcircuit-0.8.0/tensorcircuit/quantum.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.654877 tensorcircuit-0.8.0/tensorcircuit/results/
--rw-r--r--   0 shixin     (501) staff       (20)       89 2023-01-03 14:10:36.000000 tensorcircuit-0.8.0/tensorcircuit/results/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     3366 2023-02-16 12:22:32.000000 tensorcircuit-0.8.0/tensorcircuit/results/counts.py
--rw-r--r--   0 shixin     (501) staff       (20)    31378 2023-02-15 14:20:24.000000 tensorcircuit-0.8.0/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 shixin     (501) staff       (20)     9413 2022-09-15 02:01:16.000000 tensorcircuit-0.8.0/tensorcircuit/simplify.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.663430 tensorcircuit-0.8.0/tensorcircuit/templates/
--rw-r--r--   0 shixin     (501) staff       (20)      111 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/tensorcircuit/templates/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     6158 2023-01-31 08:54:48.000000 tensorcircuit-0.8.0/tensorcircuit/templates/blocks.py
--rw-r--r--   0 shixin     (501) staff       (20)     1061 2022-09-15 02:01:16.000000 tensorcircuit-0.8.0/tensorcircuit/templates/chems.py
--rw-r--r--   0 shixin     (501) staff       (20)     1933 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/tensorcircuit/templates/dataset.py
--rw-r--r--   0 shixin     (501) staff       (20)     5811 2023-02-27 05:00:14.000000 tensorcircuit-0.8.0/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 shixin     (501) staff       (20)     3934 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/tensorcircuit/templates/graphs.py
--rw-r--r--   0 shixin     (501) staff       (20)    10942 2023-01-12 02:43:07.000000 tensorcircuit-0.8.0/tensorcircuit/templates/measurements.py
--rw-r--r--   0 shixin     (501) staff       (20)     3552 2022-10-14 04:00:52.000000 tensorcircuit-0.8.0/tensorcircuit/torchnn.py
--rw-r--r--   0 shixin     (501) staff       (20)    27351 2023-02-24 11:07:51.000000 tensorcircuit-0.8.0/tensorcircuit/translation.py
--rw-r--r--   0 shixin     (501) staff       (20)     6603 2023-01-12 02:43:07.000000 tensorcircuit-0.8.0/tensorcircuit/utils.py
--rw-r--r--   0 shixin     (501) staff       (20)    12195 2023-02-16 11:17:41.000000 tensorcircuit-0.8.0/tensorcircuit/vis.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.614060 tensorcircuit-0.8.0/tensorcircuit.egg-info/
--rw-r--r--   0 shixin     (501) staff       (20)    17814 2023-03-28 04:19:06.000000 tensorcircuit-0.8.0/tensorcircuit.egg-info/PKG-INFO
--rw-r--r--   0 shixin     (501) staff       (20)     4041 2023-03-28 04:19:06.000000 tensorcircuit-0.8.0/tensorcircuit.egg-info/SOURCES.txt
--rw-r--r--   0 shixin     (501) staff       (20)        1 2023-03-28 04:19:06.000000 tensorcircuit-0.8.0/tensorcircuit.egg-info/dependency_links.txt
--rw-r--r--   0 shixin     (501) staff       (20)      110 2023-03-28 04:19:06.000000 tensorcircuit-0.8.0/tensorcircuit.egg-info/requires.txt
--rw-r--r--   0 shixin     (501) staff       (20)       20 2023-03-28 04:19:06.000000 tensorcircuit-0.8.0/tensorcircuit.egg-info/top_level.txt
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-03-28 04:19:06.684970 tensorcircuit-0.8.0/tests/
--rw-r--r--   0 shixin     (501) staff       (20)        0 2021-12-08 02:25:17.000000 tensorcircuit-0.8.0/tests/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     1166 2022-07-06 06:14:53.000000 tensorcircuit-0.8.0/tests/conftest.py
--rw-r--r--   0 shixin     (501) staff       (20)    33227 2023-01-09 05:03:09.000000 tensorcircuit-0.8.0/tests/test_backends.py
--rw-r--r--   0 shixin     (501) staff       (20)     3805 2023-02-09 09:31:26.000000 tensorcircuit-0.8.0/tests/test_calibrating.py
--rw-r--r--   0 shixin     (501) staff       (20)    11237 2023-02-16 11:05:26.000000 tensorcircuit-0.8.0/tests/test_channels.py
--rw-r--r--   0 shixin     (501) staff       (20)    45002 2023-02-24 11:07:51.000000 tensorcircuit-0.8.0/tests/test_circuit.py
--rw-r--r--   0 shixin     (501) staff       (20)     2518 2023-02-16 12:22:32.000000 tensorcircuit-0.8.0/tests/test_compiler.py
--rw-r--r--   0 shixin     (501) staff       (20)    17232 2022-10-09 02:02:12.000000 tensorcircuit-0.8.0/tests/test_dmcircuit.py
--rw-r--r--   0 shixin     (501) staff       (20)     1974 2023-02-27 05:00:14.000000 tensorcircuit-0.8.0/tests/test_ensemble.py
--rw-r--r--   0 shixin     (501) staff       (20)     4593 2022-09-16 11:37:21.000000 tensorcircuit-0.8.0/tests/test_gates.py
--rw-r--r--   0 shixin     (501) staff       (20)    11288 2022-09-15 11:59:08.000000 tensorcircuit-0.8.0/tests/test_interfaces.py
--rw-r--r--   0 shixin     (501) staff       (20)     4656 2023-02-09 05:01:38.000000 tensorcircuit-0.8.0/tests/test_keras.py
--rw-r--r--   0 shixin     (501) staff       (20)     6597 2023-03-02 11:06:11.000000 tensorcircuit-0.8.0/tests/test_miscs.py
--rw-r--r--   0 shixin     (501) staff       (20)    10552 2022-11-02 01:16:04.000000 tensorcircuit-0.8.0/tests/test_mpscircuit.py
--rw-r--r--   0 shixin     (501) staff       (20)     5637 2023-02-24 11:07:51.000000 tensorcircuit-0.8.0/tests/test_noisemodel.py
--rw-r--r--   0 shixin     (501) staff       (20)      753 2022-09-15 11:59:08.000000 tensorcircuit-0.8.0/tests/test_qaoa.py
--rw-r--r--   0 shixin     (501) staff       (20)    16823 2023-02-15 14:20:24.000000 tensorcircuit-0.8.0/tests/test_quantum.py
--rw-r--r--   0 shixin     (501) staff       (20)     1245 2022-09-15 11:59:08.000000 tensorcircuit-0.8.0/tests/test_quantum_attr.py
--rw-r--r--   0 shixin     (501) staff       (20)    11050 2023-02-16 12:22:32.000000 tensorcircuit-0.8.0/tests/test_results.py
--rw-r--r--   0 shixin     (501) staff       (20)     1175 2021-12-08 02:25:17.000000 tensorcircuit-0.8.0/tests/test_simplify.py
--rw-r--r--   0 shixin     (501) staff       (20)     5962 2023-01-31 08:54:48.000000 tensorcircuit-0.8.0/tests/test_templates.py
--rw-r--r--   0 shixin     (501) staff       (20)     2039 2023-02-09 09:31:27.000000 tensorcircuit-0.8.0/tests/test_torchnn.py
--rw-r--r--   0 shixin     (501) staff       (20)     3163 2022-09-15 11:59:08.000000 tensorcircuit-0.8.0/tests/test_van.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.252808 tensorcircuit-0.9.0/
+-rw-r--r--   0 shixin     (501) staff       (20)    23650 2023-05-05 09:07:43.000000 tensorcircuit-0.9.0/CHANGELOG.md
+-rw-r--r--   0 shixin     (501) staff       (20)     1023 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/HISTORY.md
+-rw-r--r--   0 shixin     (501) staff       (20)    11358 2021-12-08 02:25:17.000000 tensorcircuit-0.9.0/LICENSE
+-rw-r--r--   0 shixin     (501) staff       (20)      132 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/MANIFEST.in
+-rw-r--r--   0 shixin     (501) staff       (20)    18126 2023-05-05 09:12:51.252232 tensorcircuit-0.9.0/PKG-INFO
+-rw-r--r--   0 shixin     (501) staff       (20)    17577 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/README.md
+-rw-r--r--   0 shixin     (501) staff       (20)     5352 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/README_cn.md
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:50.834058 tensorcircuit-0.9.0/docs/
+-rw-r--r--   0 shixin     (501) staff       (20)      614 2020-04-19 06:32:37.000000 tensorcircuit-0.9.0/docs/Makefile
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:50.876685 tensorcircuit-0.9.0/docs/source/
+-rw-r--r--   0 shixin     (501) staff       (20)     6148 2022-06-10 06:25:56.000000 tensorcircuit-0.9.0/docs/source/.DS_Store
+-rw-r--r--   0 shixin     (501) staff       (20)     6332 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/advance.rst
+-rw-r--r--   0 shixin     (501) staff       (20)     6308 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/cnconf.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6367 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/conf.py
+-rw-r--r--   0 shixin     (501) staff       (20)     8192 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/contribution.rst
+-rw-r--r--   0 shixin     (501) staff       (20)    10971 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/faq.rst
+-rw-r--r--   0 shixin     (501) staff       (20)     3677 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/generate_rst.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2551 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/index.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      374 2022-05-17 08:27:32.000000 tensorcircuit-0.9.0/docs/source/index_cn.rst.disable
+-rw-r--r--   0 shixin     (501) staff       (20)     8413 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/infras.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      660 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/docs/source/modules.rst
+-rw-r--r--   0 shixin     (501) staff       (20)     4334 2022-04-13 08:43:33.000000 tensorcircuit-0.9.0/docs/source/modules.rst.backup
+-rw-r--r--   0 shixin     (501) staff       (20)    27390 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/docs/source/quickstart.rst
+-rw-r--r--   0 shixin     (501) staff       (20)     8223 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/docs/source/sharpbits.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      226 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/docs/source/textbooktoc.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      674 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/docs/source/tutorial.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      669 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/tutorial_cn.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      509 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/docs/source/whitepapertoc.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      531 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/docs/source/whitepapertoc_cn.rst
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.003783 tensorcircuit-0.9.0/examples/
+-rw-r--r--   0 shixin     (501) staff       (20)     2173 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/GHZ_DQAS.py
+-rw-r--r--   0 shixin     (501) staff       (20)    61992 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/H6_hamiltonian.npy
+-rw-r--r--   0 shixin     (501) staff       (20)     3984 2023-04-21 04:22:17.000000 tensorcircuit-0.9.0/examples/QAOA_DQAS.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1304 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/QEM_DQAS.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3346 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/adiabatic_vqnhe.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2574 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/chaotic_behavior.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2760 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/checkpoint_memsave.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6713 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/gradient_benchmark.py
+-rw-r--r--   0 shixin     (501) staff       (20)      950 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/hamiltonian_building.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1729 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/hchainhamiltonian.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1885 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/incremental_twoqubit.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2593 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/mcnoise_boost.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1676 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/mcnoise_check.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2399 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/mpsvsexact.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5217 2023-04-21 04:23:12.000000 tensorcircuit-0.9.0/examples/noisy_qml.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2290 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/optperformance_comparison.py
+-rw-r--r--   0 shixin     (501) staff       (20)      971 2021-11-17 07:46:30.000000 tensorcircuit-0.9.0/examples/qaoa_block.result
+-rw-r--r--   0 shixin     (501) staff       (20)      736 2022-02-17 02:39:55.000000 tensorcircuit-0.9.0/examples/qaoa_graph.py.outdated
+-rw-r--r--   0 shixin     (501) staff       (20)     1145 2022-02-17 02:39:48.000000 tensorcircuit-0.9.0/examples/qaoa_micro.py.outdated
+-rw-r--r--   0 shixin     (501) staff       (20)      814 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/qaoa_parallel_opt.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2523 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/quantumng.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2201 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/simple_qaoa.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2628 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/examples/universal_lr.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3412 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/variational_dynamics.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3533 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/vqe_extra.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3989 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/vqe_extra_mpo.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4094 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/vqe_extra_mpo_spopt.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4004 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/vqeh2o_benchmark.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1006 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/vqnhe_h6.py
+-rw-r--r--   0 shixin     (501) staff       (20)       38 2023-05-05 09:12:51.253770 tensorcircuit-0.9.0/setup.cfg
+-rw-r--r--   0 shixin     (501) staff       (20)      968 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/setup.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.116136 tensorcircuit-0.9.0/tensorcircuit/
+-rw-r--r--   0 shixin     (501) staff       (20)     1395 2023-05-05 09:07:31.000000 tensorcircuit-0.9.0/tensorcircuit/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2901 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tensorcircuit/about.py
+-rw-r--r--   0 shixin     (501) staff       (20)    39188 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.132756 tensorcircuit-0.9.0/tensorcircuit/applications/
+-rw-r--r--   0 shixin     (501) staff       (20)      234 2021-12-08 02:25:17.000000 tensorcircuit-0.9.0/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)    34460 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 shixin     (501) staff       (20)    15348 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 shixin     (501) staff       (20)    18124 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/layers.py
+-rw-r--r--   0 shixin     (501) staff       (20)    14032 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/utils.py
+-rw-r--r--   0 shixin     (501) staff       (20)    36391 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/vags.py
+-rw-r--r--   0 shixin     (501) staff       (20)    15117 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/van.py
+-rw-r--r--   0 shixin     (501) staff       (20)    23156 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 shixin     (501) staff       (20)     8235 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/asciiart.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.160683 tensorcircuit-0.9.0/tensorcircuit/backends/
+-rw-r--r--   0 shixin     (501) staff       (20)       80 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)    57621 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1713 2023-04-11 04:16:09.000000 tensorcircuit-0.9.0/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 shixin     (501) staff       (20)    14928 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)    24925 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4008 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 shixin     (501) staff       (20)    13813 2023-04-21 07:14:14.000000 tensorcircuit-0.9.0/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)    24148 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3825 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 shixin     (501) staff       (20)    31112 2023-05-05 08:09:14.000000 tensorcircuit-0.9.0/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3377 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 shixin     (501) staff       (20)    34020 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/basecircuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)    28637 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/channels.py
+-rw-r--r--   0 shixin     (501) staff       (20)    36220 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/circuit.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.177968 tensorcircuit-0.9.0/tensorcircuit/cloud/
+-rw-r--r--   0 shixin     (501) staff       (20)        0 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)    14582 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 shixin     (501) staff       (20)    17577 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 shixin     (501) staff       (20)       60 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/config.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2252 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/local.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2238 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 shixin     (501) staff       (20)    14212 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3622 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5764 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.181850 tensorcircuit-0.9.0/tensorcircuit/compiler/
+-rw-r--r--   0 shixin     (501) staff       (20)      165 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1490 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5215 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 shixin     (501) staff       (20)    28754 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/cons.py
+-rw-r--r--   0 shixin     (501) staff       (20)    13806 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 shixin     (501) staff       (20)    15210 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/experimental.py
+-rw-r--r--   0 shixin     (501) staff       (20)    29016 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/gates.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.189430 tensorcircuit-0.9.0/tensorcircuit/interfaces/
+-rw-r--r--   0 shixin     (501) staff       (20)      469 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1439 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3402 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3355 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 shixin     (501) staff       (20)    10364 2023-04-27 04:12:44.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5030 2023-04-27 04:52:54.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 shixin     (501) staff       (20)     9959 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/keras.py
+-rw-r--r--   0 shixin     (501) staff       (20)    15270 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/mps_base.py
+-rw-r--r--   0 shixin     (501) staff       (20)    34350 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)    11861 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/noisemodel.py
+-rw-r--r--   0 shixin     (501) staff       (20)    82850 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tensorcircuit/quantum.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.193887 tensorcircuit-0.9.0/tensorcircuit/results/
+-rw-r--r--   0 shixin     (501) staff       (20)       89 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/results/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3366 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/results/counts.py
+-rw-r--r--   0 shixin     (501) staff       (20)    31362 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 shixin     (501) staff       (20)     9413 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/simplify.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.203609 tensorcircuit-0.9.0/tensorcircuit/templates/
+-rw-r--r--   0 shixin     (501) staff       (20)      111 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6158 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1061 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/templates/chems.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1933 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5811 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3934 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 shixin     (501) staff       (20)    10942 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3552 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/torchnn.py
+-rw-r--r--   0 shixin     (501) staff       (20)    27335 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/translation.py
+-rw-r--r--   0 shixin     (501) staff       (20)     7060 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/utils.py
+-rw-r--r--   0 shixin     (501) staff       (20)    12195 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/vis.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.120831 tensorcircuit-0.9.0/tensorcircuit.egg-info/
+-rw-r--r--   0 shixin     (501) staff       (20)    18126 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/PKG-INFO
+-rw-r--r--   0 shixin     (501) staff       (20)     4367 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/SOURCES.txt
+-rw-r--r--   0 shixin     (501) staff       (20)        1 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/dependency_links.txt
+-rw-r--r--   0 shixin     (501) staff       (20)      133 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/requires.txt
+-rw-r--r--   0 shixin     (501) staff       (20)       20 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/top_level.txt
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.251106 tensorcircuit-0.9.0/tests/
+-rw-r--r--   0 shixin     (501) staff       (20)        0 2021-12-08 02:25:17.000000 tensorcircuit-0.9.0/tests/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1457 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tests/conftest.py
+-rw-r--r--   0 shixin     (501) staff       (20)    33394 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tests/test_backends.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3805 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_calibrating.py
+-rw-r--r--   0 shixin     (501) staff       (20)    11237 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_channels.py
+-rw-r--r--   0 shixin     (501) staff       (20)    46467 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tests/test_circuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4204 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tests/test_cloud.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2518 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_compiler.py
+-rw-r--r--   0 shixin     (501) staff       (20)    17232 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_dmcircuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1974 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_ensemble.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4593 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_gates.py
+-rw-r--r--   0 shixin     (501) staff       (20)    13220 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tests/test_interfaces.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4656 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_keras.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6639 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tests/test_miscs.py
+-rw-r--r--   0 shixin     (501) staff       (20)    10552 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_mpscircuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5637 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_noisemodel.py
+-rw-r--r--   0 shixin     (501) staff       (20)      753 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_qaoa.py
+-rw-r--r--   0 shixin     (501) staff       (20)    16823 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_quantum.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1245 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_quantum_attr.py
+-rw-r--r--   0 shixin     (501) staff       (20)    11050 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_results.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1175 2021-12-08 02:25:17.000000 tensorcircuit-0.9.0/tests/test_simplify.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5962 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_templates.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2039 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_torchnn.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3163 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_van.py
```

### Comparing `tensorcircuit-0.8.0/CHANGELOG.md` & `tensorcircuit-0.9.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,41 @@
 # Change Log
 
 ## Unreleased
 
+## 0.9.0
+
+### Added
+
+- Cloud module for Tencent QCloud is now merged into the master branch and ready to release
+
+- Add `tc.about()` to print related software versions and configs
+
+- Torch support is upgraded to 2.0, and now support native vmap and native functional grad, and thus `vvag`. Still jit support is conflict with these functional transformations and be turned off by default
+
+- Add `torch_interfaces_kws` that support static keyword arguments when wrapping with the interface
+
+- Add `gpu_memory_share` function and enable it by default
+
+- Add `scan` methods for backends
+
+- Add example demontrating how jax compiling time can be accelerated by `jax.lax.scan`
+
+### Fixed
+
+- Add tests and fixed some missing methods for cupy backend, cupy backend is now ready to use (though still not guaranteed)
+
+- Fix adjoint gate numpy conversion for fixed gate case
+
+- Sometime, tf just return IndexedSlice instead of tensor from gradient API, partially fix this in tc backend methods
+
+### Changed
+
+- Upgraded black and mypy==1.2.0 (breaking change for developers)
+
 ## 0.8.0
 
 ### Added
 
 - Add `initial_mapping` circuit method to return a new circuit with given `logical_physical_mapping`
 
 - Add `get_positional_logical_mapping` circuit method to return the mapping when only part of the qubits are measured
```

### Comparing `tensorcircuit-0.8.0/HISTORY.md` & `tensorcircuit-0.9.0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/LICENSE` & `tensorcircuit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/PKG-INFO` & `tensorcircuit-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: tensorcircuit
-Version: 0.8.0
+Version: 0.9.0
 Summary: Quantum circuits on top of tensor network
 Home-page: https://github.com/tencent-quantum-lab/tensorcircuit
 Author: TensorCircuit Authors
 Author-email: shixinzhang@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: jax
 Provides-Extra: torch
 Provides-Extra: qiskit
+Provides-Extra: cloud
 License-File: LICENSE
 
 <p align="center">
   <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
     <img width=90% src="docs/source/statics/logov2.jpg">
   </a>
 </p>
@@ -186,14 +187,15 @@
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/buwantaiji"><img src="https://avatars.githubusercontent.com/u/25216189?v=4?s=100" width="100px;" alt="Hao Xie"/><br /><sub><b>Hao Xie</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=buwantaiji" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/pramitsingh0"><img src="https://avatars.githubusercontent.com/u/52959209?v=4?s=100" width="100px;" alt="Pramit Singh"/><br /><sub><b>Pramit Singh</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=pramitsingh0" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/JAllcock"><img src="https://avatars.githubusercontent.com/u/26302022?v=4?s=100" width="100px;" alt="Jonathan Allcock"/><br /><sub><b>Jonathan Allcock</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=JAllcock" title="Documentation">📖</a> <a href="#ideas-JAllcock" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-JAllcock" title="Talks">📢</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/nealchen2003"><img src="https://avatars.githubusercontent.com/u/45502551?v=4?s=100" width="100px;" alt="nealchen2003"/><br /><sub><b>nealchen2003</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=nealchen2003" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/eurethia"><img src="https://avatars.githubusercontent.com/u/84611606?v=4?s=100" width="100px;" alt="隐公观鱼"/><br /><sub><b>隐公观鱼</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/WiuYuan"><img src="https://avatars.githubusercontent.com/u/108848998?v=4?s=100" width="100px;" alt="WiuYuan"/><br /><sub><b>WiuYuan</b></sub></a><br /><a href="#example-WiuYuan" title="Examples">💡</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `tensorcircuit-0.8.0/README.md` & `tensorcircuit-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,15 @@
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/buwantaiji"><img src="https://avatars.githubusercontent.com/u/25216189?v=4?s=100" width="100px;" alt="Hao Xie"/><br /><sub><b>Hao Xie</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=buwantaiji" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/pramitsingh0"><img src="https://avatars.githubusercontent.com/u/52959209?v=4?s=100" width="100px;" alt="Pramit Singh"/><br /><sub><b>Pramit Singh</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=pramitsingh0" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/JAllcock"><img src="https://avatars.githubusercontent.com/u/26302022?v=4?s=100" width="100px;" alt="Jonathan Allcock"/><br /><sub><b>Jonathan Allcock</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=JAllcock" title="Documentation">📖</a> <a href="#ideas-JAllcock" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-JAllcock" title="Talks">📢</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/nealchen2003"><img src="https://avatars.githubusercontent.com/u/45502551?v=4?s=100" width="100px;" alt="nealchen2003"/><br /><sub><b>nealchen2003</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=nealchen2003" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/eurethia"><img src="https://avatars.githubusercontent.com/u/84611606?v=4?s=100" width="100px;" alt="隐公观鱼"/><br /><sub><b>隐公观鱼</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/WiuYuan"><img src="https://avatars.githubusercontent.com/u/108848998?v=4?s=100" width="100px;" alt="WiuYuan"/><br /><sub><b>WiuYuan</b></sub></a><br /><a href="#example-WiuYuan" title="Examples">💡</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `tensorcircuit-0.8.0/README_cn.md` & `tensorcircuit-0.9.0/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/Makefile` & `tensorcircuit-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/.DS_Store` & `tensorcircuit-0.9.0/docs/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/advance.rst` & `tensorcircuit-0.9.0/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/cnconf.py` & `tensorcircuit-0.9.0/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/conf.py` & `tensorcircuit-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/contribution.rst` & `tensorcircuit-0.9.0/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/faq.rst` & `tensorcircuit-0.9.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/generate_rst.py` & `tensorcircuit-0.9.0/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/index.rst` & `tensorcircuit-0.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/infras.rst` & `tensorcircuit-0.9.0/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/modules.rst` & `tensorcircuit-0.9.0/docs/source/modules.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 tensorcircuit
 ==================================================
 .. toctree::
+    ./api/about.rst
     ./api/abstractcircuit.rst
     ./api/applications.rst
     ./api/backends.rst
     ./api/basecircuit.rst
     ./api/channels.rst
     ./api/circuit.rst
     ./api/compiler.rst
```

### Comparing `tensorcircuit-0.8.0/docs/source/modules.rst.backup` & `tensorcircuit-0.9.0/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/quickstart.rst` & `tensorcircuit-0.9.0/docs/source/quickstart.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 - For Windows, due to the lack of support for Jax, we recommend to use docker or WSL, please refer to `TC via windows docker <contribs/development_windows.html>`_ or `TC via WSL <contribs/development_wsl2.html>`_.
 
 - For Mac with M series chips (arm architecture), please refer to `TC on Mac M series <contribs/development_MacARM.html>`_.
 
 Overall, the installation of TensorCircuit is simple, since it is purely in Python and hence very portable. 
 As long as the users can take care of the installation of ML frameworks on the corresponding system, TensorCircuit will work as expected.
 
+To debug the installation issue or report bugs, please check the environment information by ``tc.about()``.
+
 .. Note::
     We also provide a nightly build of tensorcircuit via PyPI which can be accessed by
     ``pip uninstall tensorcircuit``, then
     ``pip install tensorcircuit-nightly``
 
 
 Circuit Object
@@ -312,14 +314,15 @@
     'eigvalsh',
     'einsum',
     'eps',
     'exp',
     'expm',
     'eye',
     'from_dlpack',
+    'g',
     'gather1d',
     'get_random_state',
     'gmres',
     'grad',
     'hessian',
     'i',
     'imag',
@@ -339,22 +342,24 @@
     'kron',
     'left_shift',
     'log',
     'matmul',
     'max',
     'mean',
     'min',
+    'minor',
     'mod',
     'multiply',
     'name',
     'norm',
     'numpy',
     'one_hot',
     'onehot',
     'ones',
+    'optimizer',
     'outer_product',
     'pivot',
     'power',
     'probability_sample',
     'qr',
     'randn',
     'random_split',
@@ -413,14 +418,15 @@
     'value_and_grad',
     'vectorized_value_and_grad',
     'vjp',
     'vmap',
     'vvag',
     'zeros']
 
+​
 
 Switch the Dtype
 --------------------
 
 TensorCircuit supports simulation using 32/64 bit precession. The default dtype is 32-bit as "complex64".
 Change this by ``tc.set_dtype("complex128")``.
 
@@ -681,14 +687,28 @@
     c = b ** 2
     c.backward()
 
     print(a.grad)
 
 For a GPU/CPU, torch/tensorflow, quantum/classical hybrid machine learning pipeline enabled by tensorcircuit, see `example script <https://github.com/tencent-quantum-lab/tensorcircuit/blob/master/examples/hybrid_gpu_pipeline.py>`__.
 
+There is also a more flexible torch interface that support static non-tensor inputs as keyword arguments, which can be utilized as below:
+
+.. code-block:: python
+
+    def f(a, i):
+        s = 0.
+        for _ in range(i):
+            s += a
+        return s
+
+    f_torch = tc.interfaces.torch_interface_kws(f)
+    f_torch(torch.ones([2]), i=3)
+
+
 We also provider wrapper of quantum function for torch module as :py:meth:`tensorcircuit.TorchLayer` alias to :py:meth:`tensorcircuit.torchnn.QuantumNet`.
 
 For ``TorchLayer``, ``use_interface=True`` is by default, which natively allow the quantum function defined on other tensorcircuit backends, such as jax or tf for speed consideration.
 
 ``TorchLayer`` can process multiple input arguments as multiple function inputs, following torch practice.
 
 .. code-block:: python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tensorcircuit-0.8.0/docs/source/sharpbits.rst` & `tensorcircuit-0.9.0/docs/source/sharpbits.rst`

 * *Files 19% similar despite different names*

```diff
@@ -137,14 +137,61 @@
         c.conditional_gate(a, [tc.gates.z(), tc.gates.x()], 0)
         return c.state()
 
     f()
     # <tf.Tensor: shape=(2,), dtype=complex64, numpy=array([0.99999994+0.j, 0.        +0.j], dtype=complex64)>
 
 
+Tensor variables consistency
+-------------------------------------------------------
+
+
+All tensor variables' backend (tf vs jax vs ..), dtype (float vs complex), shape and device (cpu vs gpu) must be compatible/consistent.
+
+Inspect the backend, dtype, shape and device using the following codes.
+
+.. code-block:: python
+
+    for backend in ["numpy", "tensorflow", "jax", "pytorch"]:
+        with tc.runtime_backend(backend):
+            a = tc.backend.ones([2, 3])
+            print("tensor backend:", tc.interfaces.which_backend(a))
+            print("tensor dtype:", tc.backend.dtype(a))
+            print("tensor shape:", tc.backend.shape_tuple(a))
+            print("tensor device:", tc.backend.device(a))
+
+If the backend is inconsistent, one can convert the tensor backend via :py:meth:`tensorcircuit.interfaces.tensortrans.general_args_to_backend`.
+
+.. code-block:: python
+
+    for backend in ["numpy", "tensorflow", "jax", "pytorch"]:
+        with tc.runtime_backend(backend):
+            a = tc.backend.ones([2, 3])
+            print("tensor backend:", tc.interfaces.which_backend(a))
+            b = tc.interfaces.general_args_to_backend(a, target_backend="jax", enable_dlpack=False)
+            print("tensor backend:", tc.interfaces.which_backend(b))
+
+If the dtype is inconsistent, one can convert the tensor dtype using ``tc.backend.cast``.
+
+.. code-block:: python
+
+    for backend in ["numpy", "tensorflow", "jax", "pytorch"]:
+        with tc.runtime_backend(backend):
+            a = tc.backend.ones([2, 3])
+            print("tensor dtype:", tc.backend.dtype(a))
+            b = tc.backend.cast(a, dtype="float64")
+            print("tensor dtype:", tc.backend.dtype(b))
+
+Also note the jax issue on float64/complex128, see `jax gotcha <https://github.com/google/jax#current-gotchas>`_.
+
+If the shape is not consistent, one can convert the shape by ``tc.backend.reshape``.
+
+If the device is not consistent, one can move the tensor between devices by ``tc.backend.device_move``.
+
+
 AD Consistency
 ---------------------
 
 TF and JAX backend manage the differentiation rules differently for complex-valued function (actually up to a complex conjuagte). See issue discussion `tensorflow issue <https://github.com/tensorflow/tensorflow/issues/3348>`_.
 
 In TensorCircuit, currently we make the difference in AD transparent, namely, when switching the backend, the AD behavior and result for complex valued function can be different and determined by the nature behavior of the corresponding backend framework.
 All AD relevant ops such as ``grad`` or ``jacrev`` may be affected. Therefore, the user must be careful when dealing with AD on complex valued function in a backend agnostic way in TensorCircuit.
```

### Comparing `tensorcircuit-0.8.0/docs/source/tutorial.rst` & `tensorcircuit-0.9.0/docs/source/tutorial.rst`

 * *Files 18% similar despite different names*

```diff
@@ -15,8 +15,9 @@
     tutorials/mera.ipynb
     tutorials/gradient_benchmark.ipynb
     tutorials/contractors.ipynb
     tutorials/operator_spreading.ipynb
     tutorials/optimization_and_expressibility.ipynb
     tutorials/vqex_mbl.ipynb
     tutorials/dqas.ipynb
-    tutorials/barren_plateaus.ipynb
+    tutorials/barren_plateaus.ipynb
+    tutorials/qaoa_portfolio_optimization.ipynb
```

### Comparing `tensorcircuit-0.8.0/docs/source/tutorial_cn.rst` & `tensorcircuit-0.9.0/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-0.9.0/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/GHZ_DQAS.py` & `tensorcircuit-0.9.0/examples/GHZ_DQAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 DQAS for GHZ state preparation circuit, deprecated DQAS implementation
 """
+
 import sys
 
 sys.path.insert(0, "../")
 import numpy as np
 import tensorflow as tf
 import cirq
```

### Comparing `tensorcircuit-0.8.0/examples/H6_hamiltonian.npy` & `tensorcircuit-0.9.0/examples/H6_hamiltonian.npy`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/QAOA_DQAS.py` & `tensorcircuit-0.9.0/examples/QAOA_DQAS.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/QEM_DQAS.py` & `tensorcircuit-0.9.0/examples/QEM_DQAS.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 DQAS for QFT QEM circuit design, deprecated DQAS implementation
 """
+
 import sys
 
 sys.path.insert(0, "../")
 
 from functools import partial
 import cirq
 import numpy as np
```

### Comparing `tensorcircuit-0.8.0/examples/adiabatic_vqnhe.py` & `tensorcircuit-0.9.0/examples/adiabatic_vqnhe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Calculate the molecule dissociation curve using VQNHE.
 """
+
 from functools import partial
 import sys
 
 sys.path.insert(0, "../")
 
 import numpy as np
 import tensorflow as tf
```

### Comparing `tensorcircuit-0.8.0/examples/chaotic_behavior.py` & `tensorcircuit-0.9.0/examples/chaotic_behavior.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Some chaotic properties calculations from the circuit state.
 """
+
 from functools import partial
 import sys
 
 sys.path.insert(0, "../")
 import tensorflow as tf
 import tensorcircuit as tc
```

### Comparing `tensorcircuit-0.8.0/examples/checkpoint_memsave.py` & `tensorcircuit-0.9.0/examples/checkpoint_memsave.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/gradient_benchmark.py` & `tensorcircuit-0.9.0/examples/gradient_benchmark.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/hamiltonian_building.py` & `tensorcircuit-0.9.0/examples/hamiltonian_building.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 benchmark sparse hamiltonian building
 """
+
 import time
 import numpy as np
 import quimb
 import tensorcircuit as tc
 
 
 nwires = 20
```

### Comparing `tensorcircuit-0.8.0/examples/hchainhamiltonian.py` & `tensorcircuit-0.9.0/examples/hchainhamiltonian.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/incremental_twoqubit.py` & `tensorcircuit-0.9.0/examples/incremental_twoqubit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Optimizing the parameterized circuit with progressively dense two-qubit gates,
 as a potential approach to alleviate barren plateau.
 """
+
 import sys
 
 sys.path.insert(0, "../")
 import tensorflow as tf
 import numpy as np
 import tensorcircuit as tc
```

### Comparing `tensorcircuit-0.8.0/examples/mcnoise_boost.py` & `tensorcircuit-0.9.0/examples/mcnoise_boost.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/mcnoise_check.py` & `tensorcircuit-0.9.0/examples/mcnoise_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Cross check the correctness of the density matrix simulator and the Monte Carlo trajectory state simulator.
 """
+
 import os
 
 os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
 # cpu is fast for small scale circuit simulation
 import sys
 
 sys.path.insert(0, "../")
```

### Comparing `tensorcircuit-0.8.0/examples/mpsvsexact.py` & `tensorcircuit-0.9.0/examples/mpsvsexact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A simple script to benchmark the approximation power of the MPS simulator.
 """
+
 import sys
 
 sys.path.insert(0, "../")
 
 import tensorcircuit as tc
 
 tc.set_backend("tensorflow")
```

### Comparing `tensorcircuit-0.8.0/examples/noisy_qml.py` & `tensorcircuit-0.9.0/examples/noisy_qml.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/optperformance_comparison.py` & `tensorcircuit-0.9.0/examples/optperformance_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Optimization for performance comparison for different densities of two-qubit gates
 (random layouts averaged).
 """
+
 import sys
 
 sys.path.insert(0, "../")
 import tensorflow as tf
 import numpy as np
 import cotengra as ctg
 import tensorcircuit as tc
```

### Comparing `tensorcircuit-0.8.0/examples/qaoa_block.result` & `tensorcircuit-0.9.0/examples/qaoa_block.result`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/qaoa_graph.py.outdated` & `tensorcircuit-0.9.0/examples/qaoa_graph.py.outdated`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/qaoa_micro.py.outdated` & `tensorcircuit-0.9.0/examples/qaoa_micro.py.outdated`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/qaoa_parallel_opt.py` & `tensorcircuit-0.9.0/examples/qaoa_parallel_opt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Depracated, using ``vectorized_value_and_grad`` instead for batched optimization
+"""
+
 import sys
 
 sys.path.insert(0, "../")
 
 import tensorcircuit as tc
 from tensorcircuit.applications.dqas import (
     parallel_qaoa_train,
```

### Comparing `tensorcircuit-0.8.0/examples/quantumng.py` & `tensorcircuit-0.9.0/examples/quantumng.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/simple_qaoa.py` & `tensorcircuit-0.9.0/examples/simple_qaoa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A plain QAOA optimization example with given graphs using networkx.
 """
+
 import sys
 
 sys.path.insert(0, "../")
 import networkx as nx
 import tensorflow as tf
 import tensorcircuit as tc
```

### Comparing `tensorcircuit-0.8.0/examples/universal_lr.py` & `tensorcircuit-0.9.0/examples/universal_lr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/variational_dynamics.py` & `tensorcircuit-0.9.0/examples/variational_dynamics.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/vqe_extra.py` & `tensorcircuit-0.9.0/examples/vqe_extra.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/vqe_extra_mpo.py` & `tensorcircuit-0.9.0/examples/vqe_extra_mpo.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/vqe_extra_mpo_spopt.py` & `tensorcircuit-0.9.0/examples/vqe_extra_mpo_spopt.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/vqeh2o_benchmark.py` & `tensorcircuit-0.9.0/examples/vqeh2o_benchmark.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/examples/vqnhe_h6.py` & `tensorcircuit-0.9.0/examples/vqnhe_h6.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 H6 molecule VQNHE with code from tc.application
 """
+
 import sys
 
 sys.path.insert(0, "../")
 import numpy as np
 import tensorcircuit as tc
 from tensorcircuit.applications.vqes import VQNHE, JointSchedule, construct_matrix_v3
```

### Comparing `tensorcircuit-0.8.0/setup.py` & `tensorcircuit-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,13 +19,14 @@
     include_package_data=True,
     install_requires=["numpy", "scipy", "tensornetwork", "networkx"],
     extras_require={
         "tensorflow": ["tensorflow"],
         "jax": ["jax", "jaxlib"],
         "torch": ["torch"],
         "qiskit": ["qiskit"],
+        "cloud": ["qiskit", "mthree"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/__init__.py` & `tensorcircuit-0.9.0/tensorcircuit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
+from .utils import gpu_memory_share
+
+gpu_memory_share()
+
+from .about import about
 from .cons import (
     backend,
     set_backend,
     set_dtype,
     set_contractor,
     get_backend,
     get_dtype,
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/abstractcircuit.py` & `tensorcircuit-0.9.0/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/applications/dqas.py` & `tensorcircuit-0.9.0/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/applications/graphdata.py` & `tensorcircuit-0.9.0/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/applications/layers.py` & `tensorcircuit-0.9.0/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/applications/utils.py` & `tensorcircuit-0.9.0/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/applications/vags.py` & `tensorcircuit-0.9.0/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/applications/van.py` & `tensorcircuit-0.9.0/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/applications/vqes.py` & `tensorcircuit-0.9.0/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/asciiart.py` & `tensorcircuit-0.9.0/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/abstract_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1330,14 +1330,36 @@
         :return: [description]
         :rtype: Tensor
         """
         raise NotImplementedError(
             "Backend '{}' has not implemented `switch`.".format(self.name)
         )
 
+    def scan(
+        self: Any, f: Callable[[Tensor, Tensor], Tensor], xs: Tensor, init: Tensor
+    ) -> Tensor:
+        # use restricted f as tensorflow
+        """
+        This API follows ``tf.scan`` covention,
+        i.e. no ys supported as jax
+
+        :param f: _description_
+        :type f: Callable[Tuple[Tensor, Tensor], Tensor]
+        :param xs: _description_
+        :type xs: Tensor
+        :param init: _description_
+        :type init: Tensor
+        :return: _description_
+        :rtype: Tensor
+        """
+        carry = init
+        for x in xs:
+            carry = f(carry, x)
+        return carry
+
     def stop_gradient(self: Any, a: Tensor) -> Tensor:
         """
         Stop backpropagation from ``a``.
 
         :param a: [description]
         :type a: Tensor
         :return: [description]
@@ -1602,14 +1624,15 @@
         return self.jacfwd(self.jacrev(f, argnums=argnums), argnums=argnums)
 
     def jit(
         self: Any,
         f: Callable[..., Any],
         static_argnums: Optional[Union[int, Sequence[int]]] = None,
         jit_compile: Optional[bool] = None,
+        **kws: Any
     ) -> Callable[..., Any]:
         """
         Return the jitted version of function ``f``.
 
         :param f: function to be jitted
         :type f: Callable[..., Any]
         :param static_argnums: index of args that doesn't regarded as tensor,
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/cupy_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # pylint: disable=invalid-name
 
 import logging
 import warnings
 from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 import numpy as np
+import scipy
 
 try:  # old version tn compatiblity
     from tensornetwork.backends import base_backend
 
     tnbackend = base_backend.BaseBackend
 
 except ImportError:
@@ -58,14 +59,26 @@
         self: Any,
         a: Tensor,
         axis: Optional[Sequence[int]] = None,
         keepdims: bool = False,
     ) -> Tensor:
         return cp.sum(a, axis=axis, keepdims=keepdims)
 
+    def conj(self, tensor: Tensor) -> Tensor:
+        return tensor.conj()
+
+    def sign(self, tensor: Tensor) -> Tensor:
+        return cp.sign(tensor)
+
+    def multiply(self, tensor1: Tensor, tensor2: Tensor) -> Tensor:
+        return tensor1 * tensor2
+
+    def norm(self, tensor: Tensor) -> Tensor:
+        return cp.linalg.norm(tensor)
+
     def shape_tuple(self, tensor: Tensor) -> Tuple[int]:
         return tensor.shape  # type:ignore
 
     def tensordot(
         self, a: Tensor, b: Tensor, axes: Union[int, Sequence[Sequence[int]]]
     ) -> Tensor:
         return cp.tensordot(a, b, axes)
@@ -96,15 +109,15 @@
             dtype = dtypestr
         return cp.zeros(shape, dtype=dtype)
 
     def copy(self, a: Tensor) -> Tensor:
         return a.copy()
 
     def expm(self, a: Tensor) -> Tensor:
-        raise NotImplementedError
+        return self.convert_to_tensor(scipy.linalg.expm(self.numpy(a)))
 
     def abs(self, a: Tensor) -> Tensor:
         return cp.abs(a)
 
     def sin(self, a: Tensor) -> Tensor:
         return cp.sin(a)
 
@@ -258,15 +271,15 @@
     def left_shift(self, x: Tensor, y: Tensor) -> Tensor:
         return cp.left_shift(x, y)
 
     def solve(self, A: Tensor, b: Tensor, assume_a: str = "gen") -> Tensor:  # type: ignore
         raise NotImplementedError
 
     def searchsorted(self, a: Tensor, v: Tensor, side: str = "left") -> Tensor:
-        return cp.searchsorted(a, v, side=side)  # type: ignore
+        return cp.searchsorted(a, v, side=side)
 
     def set_random_state(
         self, seed: Optional[int] = None, get_only: bool = False
     ) -> Any:
         g = cp.random.default_rng(seed)  # None auto supported
         if get_only is False:
             self.g = g
@@ -303,15 +316,15 @@
         high: float = 1,
         dtype: str = "32",
     ) -> Tensor:
         if isinstance(dtype, str):
             dtype = dtype[-2:]
         if isinstance(shape, int):
             shape = (shape,)
-        r = g.uniform(low=low, high=high, size=shape)
+        r = g.random(shape) * (high - low) + low
         if dtype == "32":
             r = r.astype(np.float32)
         elif dtype == "64":
             r = r.astype(np.float64)
         elif not isinstance(dtype, str):
             r = r.astype(dtype)
         else:
@@ -364,30 +377,30 @@
             return true_fun()
         return false_fun()
 
     def switch(self, index: Tensor, branches: Sequence[Callable[[], Tensor]]) -> Tensor:
         return branches[index]()
 
     def device(self, a: Tensor) -> str:
-        return "gpu"
+        return self._dev2str(a.device)
 
     def device_move(self, a: Tensor, dev: Any) -> Tensor:
-        if dev == "gpu":
-            return a
-        raise ValueError("CuPy backend only support GPU device")
+        if isinstance(dev, str):
+            dev = self._str2dev(dev)
+        with dev:
+            return cp.asarray(a)
 
     def _dev2str(self, dev: Any) -> str:
-        if dev == "gpu":
-            return "gpu"
-        raise ValueError("CuPy backend only support GPU device")
+        return f"gpu:{dev.id}"
 
     def _str2dev(self, str_: str) -> Any:
-        if str_ == "gpu":
-            return "gpu"
-        raise ValueError("CuPy backend only support GPU device")
+        if str_ == "cpu":
+            raise ValueError("CuPy backend only support GPU device")
+        else:
+            return cp.cuda.Device(int(str_.split(":")[-1]))
 
     def stop_gradient(self, a: Tensor) -> Tensor:
         raise NotImplementedError("CuPy backend doesn't support AD")
 
     def grad(
         self,
         f: Callable[..., Any],
@@ -405,14 +418,15 @@
         raise NotImplementedError("CuPy backend doesn't support AD")
 
     def jit(
         self,
         f: Callable[..., Any],
         static_argnums: Optional[Union[int, Sequence[int]]] = None,
         jit_compile: Optional[bool] = None,
+        **kws: Any,
     ) -> Callable[..., Any]:
         logger.warning("CuPy backend has no jit interface, just do nothing")
         return f
         # raise NotImplementedError("numpy backend doesn't support jit compiling")
 
     def vmap(
         self, f: Callable[..., Any], vectorized_argnums: Union[int, Sequence[int]] = 0
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/jax_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,14 +573,24 @@
 
     def switch(self, index: Tensor, branches: Sequence[Callable[[], Tensor]]) -> Tensor:
         # branches_null = [lambda _: b() for b in branches]
         # see https://stackoverflow.com/a/34021333 for weird behavior of lambda with list comprehension
         branches_null = [lambda _, f=b: f() for b in branches]
         return libjax.lax.switch(index, branches_null, None)
 
+    def scan(
+        self, f: Callable[[Tensor, Tensor], Tensor], xs: Tensor, init: Tensor
+    ) -> Tensor:
+        def f_jax(*args: Any, **kws: Any) -> Any:
+            r = f(*args, **kws)
+            return r, None
+
+        carry, _ = libjax.lax.scan(f_jax, init, xs)
+        return carry
+
     def scatter(self, operand: Tensor, indices: Tensor, updates: Tensor) -> Tensor:
         rank = len(operand.shape)
         dnums = libjax.lax.ScatterDimensionNumbers(
             update_window_dims=(),
             inserted_window_dims=tuple([i for i in range(rank)]),
             scatter_dims_to_operand_dims=tuple([i for i in range(rank)]),
         )
@@ -682,14 +692,15 @@
         return value, vjpv
 
     def jit(
         self,
         f: Callable[..., Any],
         static_argnums: Optional[Union[int, Sequence[int]]] = None,
         jit_compile: Optional[bool] = None,
+        **kws: Any,
     ) -> Any:
         return libjax.jit(f, static_argnums=static_argnums)
 
     def vmap(
         self, f: Callable[..., Any], vectorized_argnums: Union[int, Sequence[int]] = 0
     ) -> Any:
         if isinstance(vectorized_argnums, int):
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/jax_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 def jaxqr_bwd(res: Sequence[Array], tangents: Sequence[Array]) -> Tuple[Array]:
     a, q, r = res
     dq, dr = tangents
     dq = dq.conj()
     dr = dr.conj()
 
     def _TriangularSolve(x: Array, r: Array) -> Array:
-        return jax.scipy.linalg.solve_triangular(  # type: ignore
+        return jax.scipy.linalg.solve_triangular(
             r, x.T.conj(), lower=False, trans=0
         ).T.conj()
 
     def _QrGradSquareAndDeepMatrices(q: Array, r: Array, dq: Array, dr: Array) -> Array:
         # Modification begins
         rdiag = jnp.diag(r)
         rdiag = (jnp.abs(rdiag) < qr_epsilon) * qr_epsilon + (
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/numpy_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,14 +373,15 @@
         raise NotImplementedError("numpy backend doesn't support AD")
 
     def jit(
         self,
         f: Callable[..., Any],
         static_argnums: Optional[Union[int, Sequence[int]]] = None,
         jit_compile: Optional[bool] = None,
+        **kws: Any
     ) -> Callable[..., Any]:
         logger.warning("numpy backend has no jit interface, just do nothing")
         return f
         # raise NotImplementedError("numpy backend doesn't support jit compiling")
 
     def vmap(
         self, f: Callable[..., Any], vectorized_argnums: Union[int, Sequence[int]] = 0
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/pytorch_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Backend magic inherited from tensornetwork: pytorch backend
 """
 # pylint: disable=invalid-name
 
 import logging
 from typing import Any, Callable, Optional, Sequence, Tuple, Union
 from operator import mul
-from functools import reduce
+from functools import reduce, partial
 
 import tensornetwork
 from tensornetwork.backends.pytorch import pytorch_backend
 from .abstract_backend import ExtendedBackend
 
 dtypestr: str
 Tensor = Any
@@ -22,14 +22,32 @@
 
 # TODO(@refraction-ray): lack stateful random methods implementation for now
 # TODO(@refraction-ray): lack scatter impl for now
 # TODO(@refraction-ray): lack sparse relevant methods for now
 # To be added once pytorch backend is ready
 
 
+class torch_jit_func:
+    """
+    Delay the tracing of torch jit to the first run time:
+    consistent with tf and jax mechanism
+    """
+
+    def __init__(self, f: Callable[..., Any]):
+        self.compiled = False
+        self.f = f
+
+    def __call__(self, *args: Any, **kws: Any) -> Any:
+        if self.compiled is False:
+            self.f = torchlib.jit.trace(self.f, example_inputs=args)
+            self.compiled = True
+
+        return self.f(*args, **kws)
+
+
 class torch_optimizer:
     def __init__(self, optimizer: Any) -> None:
         self.optimizer = optimizer
         self.is_init = False
 
     def update(self, grads: pytree, params: pytree) -> pytree:
         # flatten grad and param
@@ -510,45 +528,51 @@
 
     def value_and_grad(
         self,
         f: Callable[..., Any],
         argnums: Union[int, Sequence[int]] = 0,
         has_aux: bool = False,
     ) -> Callable[..., Tuple[Any, Any]]:
-        def ask_require(t: Tensor) -> Any:
-            t.requires_grad_(True)
-            return t
-
-        def get_grad(t: Tensor) -> Tensor:
-            return t.grad
-
         def wrapper(*args: Any, **kws: Any) -> Any:
-            x = []
-            if isinstance(argnums, int):
-                argnumsl = [argnums]
-                # if you also call lhs as argnums, something weird may happen
-                # the reason is that python then take it as local vars
-            else:
-                argnumsl = argnums  # type: ignore
-            for i, arg in enumerate(args):
-                if i in argnumsl:
-                    x.append(self.tree_map(ask_require, arg))
-                else:
-                    x.append(arg)
-            y = f(*x, **kws)
-            if has_aux:
-                y[0].backward()
-            else:
-                y.backward()
-            gs = [self.tree_map(get_grad, x[i]) for i in argnumsl]
-            if len(gs) == 1:
-                gs = gs[0]
-            return y, gs
+            gavf = torchlib.func.grad_and_value(f, argnums=argnums, has_aux=has_aux)
+            g, v = gavf(*args, **kws)
+            return v, g
 
         return wrapper
+        # def ask_require(t: Tensor) -> Any:
+        #     t.requires_grad_(True)
+        #     return t
+
+        # def get_grad(t: Tensor) -> Tensor:
+        #     return t.grad
+
+        # def wrapper(*args: Any, **kws: Any) -> Any:
+        #     # x = []
+        #     if isinstance(argnums, int):
+        #         argnumsl = [argnums]
+        #         # if you also call lhs as argnums, something weird may happen
+        #         # the reason is that python then take it as local vars
+        #     else:
+        #         argnumsl = argnums  # type: ignore
+        #     args = list(args)
+        #     for i, arg in enumerate(args):
+        #         if i in argnumsl:
+        #             args[i] = self.tree_map(ask_require, arg)
+        #     args = tuple(args)
+        #     y = f(*args, **kws)
+        #     if has_aux:
+        #         y[0].backward()
+        #     else:
+        #         y.backward()
+        #     gs = [self.tree_map(get_grad, x[i]) for i in argnumsl]
+        #     if len(gs) == 1:
+        #         gs = gs[0]
+        #     return y, gs
+
+        # return wrapper
 
     def vjp(
         self,
         f: Callable[..., Any],
         inputs: Union[Tensor, Sequence[Tensor]],
         v: Union[Tensor, Sequence[Tensor]],
     ) -> Tuple[Union[Tensor, Sequence[Tensor]], Union[Tensor, Sequence[Tensor]]]:
@@ -573,72 +597,111 @@
         # to be investigate whether the overhead issue remains as in
         # https://github.com/renmengye/tensorflow-forward-ad/issues/2
         return torchlib.autograd.functional.jvp(f, inputs, v)  # type: ignore
 
     def vmap(
         self,
         f: Callable[..., Any],
-        vectorized_argnums: Optional[Union[int, Sequence[int]]] = None,
+        vectorized_argnums: Union[int, Sequence[int]] = 0,
     ) -> Any:
-        logger.warning(
-            "pytorch backend has no intrinsic vmap like interface"
-            ", use plain for loop for compatibility"
-        )
-        # the vmap support is vey limited, f must return one tensor
-        # nested list of tensor as return is not supported
         if isinstance(vectorized_argnums, int):
             vectorized_argnums = (vectorized_argnums,)
 
         def wrapper(*args: Any, **kws: Any) -> Tensor:
-            results = []
-            for barg in zip(*[args[i] for i in vectorized_argnums]):  # type: ignore
-                narg = []
-                j = 0
-                for k in range(len(args)):
-                    if k in vectorized_argnums:  # type: ignore
-                        narg.append(barg[j])
-                        j += 1
-                    else:
-                        narg.append(args[k])
-                results.append(f(*narg, **kws))
-            return torchlib.stack(results)
+            in_axes = tuple([0 if i in vectorized_argnums else None for i in range(len(args))])  # type: ignore
+            return torchlib.vmap(f, in_axes, 0)(*args, **kws)
 
         return wrapper
+        # v3
+        # logger.warning(
+        #     "pytorch backend has no intrinsic vmap like interface"
+        #     ", use plain for loop for compatibility"
+        # )
+        # # the vmap support is vey limited, f must return one tensor
+        # # nested list of tensor as return is not supported
+        # if isinstance(vectorized_argnums, int):
+        #     vectorized_argnums = (vectorized_argnums,)
+
+        # def wrapper(*args: Any, **kws: Any) -> Tensor:
+        #     results = []
+        #     for barg in zip(*[args[i] for i in vectorized_argnums]):  # type: ignore
+        #         narg = []
+        #         j = 0
+        #         for k in range(len(args)):
+        #             if k in vectorized_argnums:  # type: ignore
+        #                 narg.append(barg[j])
+        #                 j += 1
+        #             else:
+        #                 narg.append(args[k])
+        #         results.append(f(*narg, **kws))
+        #     return torchlib.stack(results)
+
+        # return wrapper
 
+        # v2
         # def vmapf(*args: Tensor, **kws: Any) -> Tensor:
         #     r = []
         #     for i in range(args[0].shape[0]):
         #         nargs = [arg[i] for arg in args]
         #         r.append(f(*nargs, **kws))
         #     return torchlib.stack(r)
 
         # return vmapf
 
+        # v1
         # raise NotImplementedError("pytorch backend doesn't support vmap")
         # There seems to be no map like architecture in pytorch for now
         # see https://discuss.pytorch.org/t/fast-way-to-use-map-in-pytorch/70814
 
     def jit(
         self,
         f: Callable[..., Any],
         static_argnums: Optional[Union[int, Sequence[int]]] = None,
         jit_compile: Optional[bool] = None,
+        **kws: Any
     ) -> Any:
-        return f  # do nothing here until I figure out what torch.jit is for and how does it work
+        if jit_compile is True:
+            # experimental feature reusing the jit_compile flag for tf
+            return torch_jit_func(f)
+        return f
+        # return f  # do nothing here until I figure out what torch.jit is for and how does it work
         # see https://github.com/pytorch/pytorch/issues/36910
 
     def vectorized_value_and_grad(
         self,
         f: Callable[..., Any],
         argnums: Union[int, Sequence[int]] = 0,
         vectorized_argnums: Union[int, Sequence[int]] = 0,
         has_aux: bool = False,
     ) -> Callable[..., Tuple[Any, Any]]:
         # [WIP], not a consistent impl compared to tf and jax backend, but pytorch backend is not fully supported anyway
-        f = self.value_and_grad(f, argnums=argnums, has_aux=has_aux)
-        f = self.vmap(f, vectorized_argnums=vectorized_argnums)
-        # f = self.jit(f)
-        return f
+        if isinstance(vectorized_argnums, int):
+            vectorized_argnums = (vectorized_argnums,)
+
+        def wrapper(
+            *args: Any, **kws: Any
+        ) -> Tuple[Tensor, Union[Tensor, Tuple[Tensor, ...]]]:
+            jf = self.value_and_grad(f, argnums=argnums, has_aux=has_aux)
+            jf = self.vmap(jf, vectorized_argnums=vectorized_argnums)
+            vs, gs = jf(*args, **kws)
+
+            if isinstance(argnums, int):
+                argnums_list = [argnums]
+                gs = [gs]
+            else:
+                argnums_list = argnums  # type: ignore
+                gs = list(gs)
+            for i, (j, g) in enumerate(zip(argnums_list, gs)):
+                if j not in vectorized_argnums:  # type: ignore
+                    gs[i] = self.tree_map(partial(torchlib.sum, dim=0), g)
+            if isinstance(argnums, int):
+                gs = gs[0]
+            else:
+                gs = tuple(gs)
+
+            return vs, gs
+
+        return wrapper
 
     vvag = vectorized_value_and_grad
 
     optimizer = torch_optimizer
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/tf_ops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,102 @@
 """
 Customized ops for ML framework
 """
 # pylint: disable=invalid-name
 
 from typing import Any
 
-import torch  # type: ignore
+import tensorflow as tf
 
-Array = Any  # torch Tensor
+Array = Any  # tensorflow Tensor
 
 qr_epsilon = 1e-8
 
 
-def torchqr_grad(
-    a: Array,
-    q: Array,
-    r: Array,
-    dq: Array,
-    dr: Array,
-) -> Array:
+def tfqr_grad(a: Array, q: Array, r: Array, dq: Array, dr: Array) -> Array:
     """Get the gradient for Qr."""
 
-    if r.shape[-2] > r.shape[-1] and q.shape[-2] == q.shape[-1]:
+    if (
+        r.shape.ndims is None
+        or r.shape.as_list()[-2] is None
+        or r.shape.as_list()[-1] is None
+    ):
+        raise NotImplementedError(
+            "QrGrad not implemented with dynamic shapes. "
+            f"Received r.shape: {r.shape}"
+        )
+    if (
+        r.shape.dims[-2].value > r.shape.dims[-1].value
+        and q.shape.dims[-2].value == q.shape.dims[-1].value
+    ):
         raise NotImplementedError(
             "QrGrad not implemented when nrows > ncols "
             "and full_matrices is true. Received r.shape="
-            f"{r.shape} with nrows={r.shape[-2]}"
-            f"and ncols={r.shape[-1]}."
+            f"{r.shape} with nrows={r.shape.dims[-2]}"
+            f"and ncols={r.shape.dims[-1]}."
         )
 
     def _TriangularSolve(x: Array, r: Array) -> Array:
         """Equivalent to matmul(x, adjoint(matrix_inverse(r))) if r is upper-tri."""
-        return torch.linalg.solve_triangular(
-            r, x.adjoint(), upper=True, unitriangular=False
-        ).adjoint()
+        return tf.linalg.adjoint(
+            tf.linalg.triangular_solve(
+                r, tf.linalg.adjoint(x), lower=False, adjoint=False
+            )
+        )
 
     def _QrGradSquareAndDeepMatrices(q: Array, r: Array, dq: Array, dr: Array) -> Array:
         """
         Get the gradient for matrix orders num_rows >= num_cols and full_matrices is false.
         """
 
         # Modification begins
-        rdiag = torch.linalg.diagonal(r)
-        # if abs(rdiag[i]) < qr_epsilon then rdiag[i] = qr_epsilon otherwise keep the old value
-        qr_epsilon_diag = torch.ones_like(rdiag) * qr_epsilon
-        rdiag = torch.where(rdiag.abs() < qr_epsilon, qr_epsilon_diag, rdiag)
-        r = torch.diagonal_scatter(r, rdiag, dim1=-2, dim2=-1)
+        rdiag = tf.linalg.diag_part(r)
+        small_indices = tf.where(tf.math.abs(rdiag) < qr_epsilon)
+        length = tf.shape(small_indices)[0]
+        newvalues = tf.ones((length,), dtype=rdiag.dtype) * qr_epsilon
+        rdiag = tf.tensor_scatter_nd_update(rdiag, small_indices, newvalues)
+        delta_r = tf.linalg.set_diag(r, rdiag) - r
+        r = r + delta_r
         # delta_dq = math_ops.matmul(q, math_ops.matmul(dr, tf.linalg.adjoint(delta_r)))
         # dq = dq + delta_dq
         # Modification ends
 
-        qdq = torch.matmul(q.adjoint(), dq)
-        qdq_ = qdq - qdq.adjoint()
-        rdr = torch.matmul(r, dr.adjoint())
-        rdr_ = rdr - rdr.adjoint()
-        tril = torch.tril(qdq_ + rdr_)
+        qdq = tf.matmul(q, dq, adjoint_a=True)
+        qdq_ = qdq - tf.linalg.adjoint(qdq)
+        rdr = tf.matmul(r, dr, adjoint_b=True)
+        rdr_ = rdr - tf.linalg.adjoint(rdr)
+        tril = tf.linalg.band_part(qdq_ + rdr_, -1, 0)
 
-        grad_a = torch.matmul(q, dr + _TriangularSolve(tril, r))
-        grad_b = _TriangularSolve(dq - torch.matmul(q, qdq), r)
+        grad_a = tf.matmul(q, dr + _TriangularSolve(tril, r))
+        grad_b = _TriangularSolve(dq - tf.matmul(q, qdq), r)
         ret = grad_a + grad_b
 
-        if q.is_complex():
-            m = rdr - qdq.adjoint()
-            eyem = torch.diagonal_scatter(
-                torch.zeros_like(m), torch.linalg.diagonal(m), dim1=-2, dim2=-1
-            )
-            correction = eyem - torch.real(eyem).to(dtype=q.dtype)
-            ret = ret + _TriangularSolve(torch.matmul(q, correction.adjoint()), r)
+        if q.dtype.is_complex:
+            m = rdr - tf.linalg.adjoint(qdq)
+            eyem = tf.linalg.set_diag(tf.zeros_like(m), tf.linalg.diag_part(m))
+            correction = eyem - tf.cast(tf.math.real(eyem), q.dtype)
+            ret = ret + _TriangularSolve(tf.matmul(q, tf.linalg.adjoint(correction)), r)
 
         return ret
 
-    num_rows, num_cols = q.shape[-2], r.shape[-1]
+    num_rows, num_cols = q.shape.dims[-2].value, r.shape.dims[-1]
 
     if num_rows >= num_cols:
         return _QrGradSquareAndDeepMatrices(q, r, dq, dr)
 
     y = a[..., :, num_rows:]
     u = r[..., :, :num_rows]
     dv = dr[..., :, num_rows:]
     du = dr[..., :, :num_rows]
-    dy = torch.matmul(q, dv)
-    dx = _QrGradSquareAndDeepMatrices(q, u, dq + torch.matmul(y, dv.adjoint()), du)
-    return torch.cat([dx, dy], dim=-1)
-
-
-class torchqr(torch.autograd.Function):
-    """
-    Customized backward of qr for better numerical stability
-    """
-
-    @staticmethod
-    def forward(ctx, a: Array) -> Any:
-        q, r = torch.linalg.qr(a, mode="reduced")
-        ctx.save_for_backward(a, q, r)
-        return q, r
-
-    @staticmethod
-    def backward(ctx, dq: Array, dr: Array) -> Any:
-        a, q, r = ctx.saved_tensors
-        return torchqr_grad(a, q, r, dq, dr)
+    dy = tf.matmul(q, dv)
+    dx = _QrGradSquareAndDeepMatrices(q, u, dq + tf.matmul(y, dv, adjoint_b=True), du)
+    return tf.concat([dx, dy], axis=-1)
+
+
+@tf.custom_gradient  # type: ignore
+def tfqr(A: Array) -> Any:
+    q, r = tf.linalg.qr(A)
+
+    def grad(dq: Array, dr: Array) -> Any:
+        return tfqr_grad(A, q, r, dq, dr)
+
+    return (q, r), grad
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-0.9.0/tensorcircuit/backends/tensorflow_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,19 +578,22 @@
         self,
         pred: bool,
         true_fun: Callable[[], Tensor],
         false_fun: Callable[[], Tensor],
     ) -> Tensor:
         return tf.cond(pred, true_fun, false_fun)
 
-    def switch(
-        self: Any, index: Tensor, branches: Sequence[Callable[[], Tensor]]
-    ) -> Tensor:
+    def switch(self, index: Tensor, branches: Sequence[Callable[[], Tensor]]) -> Tensor:
         return tf.switch_case(index, branches)
 
+    def scan(
+        self, f: Callable[[Tensor, Tensor], Tensor], xs: Tensor, init: Tensor
+    ) -> Tensor:
+        return tf.scan(f, xs, init)[-1]
+
     def device(self, a: Tensor) -> str:
         dev = a.device
         return self._dev2str(dev)
 
     def device_move(self, a: Tensor, dev: Any) -> Tensor:
         if isinstance(dev, str):
             dev = self._str2dev(dev)
@@ -718,24 +721,30 @@
             t.watch(inputs)
             y = f(*inputs)
         g = t.gradient(y, inputs, v)
         g = list(g)
         for i, gi in enumerate(g):
             if gi is None:
                 g[i] = tf.zeros_like(inputs[i])
+            if isinstance(gi, tf.IndexedSlices):
+                # gradient can return sth weird
+                # TODO(@refraction-ray): check whether other AD tf methods have such issues
+                # shape is still unkown, dense_shape attr doesn't work?
+                g[i] = tf.convert_to_tensor(gi)
         g = tuple(g)
         if one_input:
             g = g[0]
         return y, g
 
     def jit(
         self,
         f: Callable[..., Any],
         static_argnums: Optional[Union[int, Sequence[int]]] = None,
         jit_compile: Optional[bool] = None,
+        **kws: Any
     ) -> Any:
         # static_argnums not supported in tf case, this is only for a consistent interface
         # for more on static_argnums in tf.function, see issue: https://github.com/tensorflow/tensorflow/issues/52193
         # tf.function works with dict pytree but fails at list pytree, hmm...
         # no full jittable pytree support in tf
         # another difference from jax.jit
         if self.minor < 5:
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/basecircuit.py` & `tensorcircuit-0.9.0/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/channels.py` & `tensorcircuit-0.9.0/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/circuit.py` & `tensorcircuit-0.9.0/tensorcircuit/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,15 +770,15 @@
         if with_prob:
             return sample, p
         else:
             return sample, -1.0
 
     # TODO(@refraction-ray): more _before function like state_before? and better API?
 
-    def expectation(  # type: ignore
+    def expectation(
         self,
         *ops: Tuple[tn.Node, List[int]],
         reuse: bool = True,
         enable_lightcone: bool = False,
         noise_conf: Optional[Any] = None,
         nmc: int = 1000,
         status: Optional[Tensor] = None,
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-0.9.0/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-0.9.0/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/cons.py` & `tensorcircuit-0.9.0/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/densitymatrix.py` & `tensorcircuit-0.9.0/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/experimental.py` & `tensorcircuit-0.9.0/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/gates.py` & `tensorcircuit-0.9.0/tensorcircuit/gates.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import warnings
 
 import numpy as np
 import tensornetwork as tn
 from scipy.stats import unitary_group
 
 from .cons import backend, dtypestr, npdtype
-from .backends import get_backend
 from .utils import arg_alias
 
 thismodule = sys.modules[__name__]
 
 Tensor = Any
 Array = Any
 Operator = Any  # QuOperator
@@ -253,30 +252,26 @@
         if not n:
             n = "unknowngate"
         self.m = m
         self.n = n
         self.ctrl = ctrl
 
     def __call__(self, *args: Any, **kws: Any) -> Gate:
-        # m = array_to_tensor(self.m)
+        m1 = array_to_tensor(self.m)
         # m = backend.cast(m, dtypestr)
-        m = self.m.astype(npdtype)
-        return Gate(deepcopy(m), name=self.n)
+        m1 = backend.cast(m1, dtypestr)
+        return Gate(m1, name=self.n)
 
     def adjoint(self) -> "GateF":
         m = self.__call__()
-        npb = get_backend("numpy")
-        shape0 = npb.shape_tuple(m.tensor)
-        m0 = npb.reshapem(m.tensor)
-        ma = npb.adjoint(m0)
-        if np.allclose(m0, ma, atol=1e-5):
-            name = self.n
-        else:
-            name = self.n + "d"
-        ma = npb.reshape(ma, shape0)
+        shape0 = backend.shape_tuple(m.tensor)
+        m0 = backend.reshapem(m.tensor)
+        ma = backend.adjoint(m0)
+        name = self.n + "d"
+        ma = backend.reshape(ma, shape0)
         return GateF(ma, name, self.ctrl)
 
     # TODO(@refraction-ray): adjoint gate convention finally determined
     def ided(self, before: bool = True) -> "GateF":
         def f(*args: Any, **kws: Any) -> Any:
             m = self.__call__(*args, **kws)
             u = m.tensor
@@ -808,15 +803,15 @@
     :type unitary: Tensor
     :param theta: angle in radians
     :type theta: float
     :param name: suffix of Gate name
     :return: Exponential Gate
     :rtype: Gate
     """
-    theta = num_to_tensor(theta)
+    theta, unitary = num_to_tensor(theta, unitary)
     mat = backend.expm(-backend.i() * theta * unitary)
     dimension = reduce(mul, mat.shape)
     nolegs = int(np.log(dimension) / np.log(2))
     mat = backend.reshape(mat, shape=[2 for _ in range(nolegs)])
     return Gate(mat, name="exp-" + name)
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-0.9.0/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-0.9.0/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-0.9.0/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-0.9.0/tensorcircuit/interfaces/tensortrans.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,18 +46,20 @@
         return t
     if t is None:
         return
     return which_backend(t).numpy(t)
 
 
 def tensor_to_backend_jittable(t: Tensor) -> Tensor:
-    if which_backend(t, return_backend=False) == backend.name:
-        return t
     if isinstance(t, int) or isinstance(t, float):
         return t
+    if isinstance(t, QuOperator):
+        return t
+    if which_backend(t, return_backend=False) == backend.name:
+        return t
     return backend.convert_to_tensor(which_backend(t).numpy(t))
 
 
 def numpy_to_tensor(t: Array, backend: Any) -> Tensor:
     if isinstance(t, int) or isinstance(t, float):
         return t
     return backend.convert_to_tensor(t)
@@ -272,22 +274,33 @@
                 else:
                     is_krauslist = False
 
                 if gate_to_tensor:
                     arg = backend.tree_map(
                         partial(gate_to_matrix, is_reshapem=gate_as_matrix), arg
                     )
-                if qop_to_matrix:
+                if qop_as_matrix:
                     arg = backend.tree_map(
                         partial(qop_to_matrix, is_reshapem=qop_as_matrix), arg
                     )
                 arg = backend.tree_map(tensor_to_backend_jittable, arg)
+
                 # arg = backend.tree_map(backend.convert_to_tensor, arg)
+                def _cast(a: Tensor, dtype: str) -> Tensor:
+                    if isinstance(a, QuOperator):
+                        return a
+                    return backend.cast(a, dtype)
+
+                def _reshapem(a: Tensor) -> Tensor:
+                    if isinstance(a, QuOperator):
+                        return a
+                    return backend.reshapem(a)
+
                 if cast_dtype:
-                    arg = backend.tree_map(partial(backend.cast, dtype=dtypestr), arg)
+                    arg = backend.tree_map(partial(_cast, dtype=dtypestr), arg)
                 if tensor_as_matrix:
                     arg = backend.tree_map(backend.reshapem, arg)
 
                 if is_krauslist is True:
                     arg = KrausList(arg, name, is_unitary)
             nargs.append(arg)
         return f(*nargs, **kws)
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/interfaces/torch.py` & `tensorcircuit-0.9.0/tensorcircuit/interfaces/torch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Interface wraps quantum function as a torch function
 """
 
-from typing import Any, Callable, Tuple
+from typing import Any, Callable, Dict, Tuple
+from functools import partial
 
 from ..cons import backend
 from ..utils import is_sequence
 from .tensortrans import general_args_to_backend
 
 
 Tensor = Any
@@ -104,11 +105,59 @@
             )
             r = backend.tree_map(lambda s: s.to(device=ctx.device), r)
             if not is_sequence(r):
                 return (r,)
             return r
 
     # currently, memory transparent dlpack in these ML framework has broken support on complex dtypes
-    return Fun.apply  # type: ignore
+    return Fun.apply
 
 
 pytorch_interface = torch_interface
+
+
+def torch_interface_kws(
+    f: Callable[..., Any], jit: bool = True, enable_dlpack: bool = False
+) -> Callable[..., Any]:
+    """
+    similar to py:meth:`tensorcircuit.interfaces.torch.torch_interface`,
+    but now the interface support static arguments for function ``f``,
+    which is not a tensor and can be used with keyword arguments
+
+    :Example:
+
+    .. code-block:: python
+
+        tc.set_backend("tensorflow")
+
+        def f(tensor, integer):
+            r = 0.
+            for i in range(integer):
+                r += tensor
+            return r
+
+        fnew = tc.interfaces.torch_interface_kws(f)
+
+        print(fnew(torch.ones([2]), integer=3))
+        print(fnew(torch.ones([2]), integer=4))
+
+    :param f: _description_
+    :type f: Callable[..., Any]
+    :param jit: _description_, defaults to True
+    :type jit: bool, optional
+    :param enable_dlpack: _description_, defaults to False
+    :type enable_dlpack: bool, optional
+    :return: _description_
+    :rtype: Callable[..., Any]
+    """
+    cache_dict: Dict[Tuple[Any, ...], Callable[..., Any]] = {}
+
+    def wrapper(*args: Any, **kws: Any) -> Any:
+        key = tuple([(k, v) for k, v in kws.items()])
+        if key not in cache_dict:
+            fnew = torch_interface(
+                partial(f, **kws), jit=jit, enable_dlpack=enable_dlpack
+            )
+            cache_dict[key] = fnew
+        return cache_dict[key](*args)
+
+    return wrapper
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/keras.py` & `tensorcircuit-0.9.0/tensorcircuit/keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     #     base_config = super().get_config()
     #     return dict(list(base_config.items()) + list(config.items()))
 
 
 KerasLayer = QuantumLayer
 
 
-class HardwareLayer(QuantumLayer):  # type: ignore
+class HardwareLayer(QuantumLayer):
     @tf.autograph.experimental.do_not_convert  # type: ignore
     def call(
         self,
         inputs: tf.Tensor,
         training: Optional[bool] = None,
         mask: Optional[tf.Tensor] = None,
         **kwargs: Any
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/mps_base.py` & `tensorcircuit-0.9.0/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/mpscircuit.py` & `tensorcircuit-0.9.0/tensorcircuit/mpscircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,16 +518,16 @@
         # TODO(@SUSYUSTC): jax autograd is wrong on this function
         """
         Apply a n-qubit gate by transforming the gate to MPO
         """
         ordered = np.all(np.diff(index) > 0)
         if not ordered:
             order = np.argsort(index)
-            order2 = order + len(index)  # type: ignore
-            order_all = order.tolist() + order2.tolist()  # type: ignore
+            order2 = order + len(index)
+            order_all = order.tolist() + order2.tolist()
             newgate = backend.transpose(gate.tensor, order_all)
             index = np.sort(index).tolist()
             self.apply_nqubit_gate(newgate, *index, split=split)
             return
         if split is None:
             split = self.split
         MPO, index_left = self.gate_to_MPO(gate, *index)
@@ -810,15 +810,15 @@
             nqubits,
             tensors=tensors,
             center_position=center_position,
             split=self.split.copy(),
         )
         return mps
 
-    def expectation(  # type: ignore
+    def expectation(
         self,
         *ops: Tuple[Gate, List[int]],
         reuse: bool = True,
         other: Optional["MPSCircuit"] = None,
         conj: bool = True,
         normalize: bool = False,
         split: Optional[Dict[str, Any]] = None,
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/noisemodel.py` & `tensorcircuit-0.9.0/tensorcircuit/noisemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         noise_conf = NoiseConf()
 
     readout_error = noise_conf.readout_error
 
     if noise_conf.has_quantum:
         # density matrix
         if isinstance(c, DMCircuit):
-            cnoise = circuit_with_noise(c, noise_conf)  #  type: ignore
+            cnoise = circuit_with_noise(c, noise_conf)
             return cnoise.sample_expectation_ps(
                 x=x, y=y, z=z, shots=shots, status=status, readout_error=readout_error
             )
 
         # monte carlo
         else:
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/quantum.py` & `tensorcircuit-0.9.0/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/results/counts.py` & `tensorcircuit-0.9.0/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-0.9.0/tensorcircuit/results/readout_mitigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,15 +545,15 @@
                 )
             )
 
         if not given_list:
             r = quasi_out[0]
             r = sort_count(r)
             r = {k: v * shots for k, v in r.items()}
-            return sort_count(r)  # type: ignore
+            return sort_count(r)
             # return quasi_out[0]  # type: ignore
         mitcounts = QuasiCollection(quasi_out)
         return sort_count(mitcounts.nearest_probability_distribution())  # type: ignore
 
     def _apply_correction(  # type: ignore
         self,
         counts,
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/simplify.py` & `tensorcircuit-0.9.0/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/templates/blocks.py` & `tensorcircuit-0.9.0/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/templates/chems.py` & `tensorcircuit-0.9.0/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/templates/dataset.py` & `tensorcircuit-0.9.0/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/templates/ensemble.py` & `tensorcircuit-0.9.0/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/templates/graphs.py` & `tensorcircuit-0.9.0/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/templates/measurements.py` & `tensorcircuit-0.9.0/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/torchnn.py` & `tensorcircuit-0.9.0/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit/translation.py` & `tensorcircuit-0.9.0/tensorcircuit/translation.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,15 +437,15 @@
     :rtype: Any
     """
     if circuit_constructor is not None:
         Circ = circuit_constructor
     elif is_dm:
         Circ = DMCircuit2
     else:
-        Circ = Circuit  # type: ignore
+        Circ = Circuit
     if circuit_params is None:
         circuit_params = {}
     if "nqubits" not in circuit_params:
         circuit_params["nqubits"] = n
     if (
         len(qcdata) > 0
         and qcdata[0][0].name == "initialize"
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/utils.py` & `tensorcircuit-0.9.0/tensorcircuit/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 """
 Helper functions
 """
 
 from typing import Any, Callable, Union, Sequence, Tuple, Dict
 from functools import wraps
+import os
 import platform
 import re
 import time
 
 
+def gpu_memory_share(flag: bool = True) -> None:
+    # TODO(@refraction-ray): the default torch behavior should be True
+    # preallocate behavior for torch to be investigated
+    if flag is True:
+        os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = "true"
+        os.environ["XLA_PYTHON_CLIENT_PREALLOCATE"] = "false"
+    else:
+        os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = "false"
+        os.environ["XLA_PYTHON_CLIENT_PREALLOCATE"] = "true"
+
+
 def return_partial(
     f: Callable[..., Any], return_argnums: Union[int, Sequence[int]] = 0
 ) -> Callable[..., Any]:
     r"""
     Return a callable function for output ith parts of the original output along the first axis.
     Original output supports List and Tensor.
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit/vis.py` & `tensorcircuit-0.9.0/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tensorcircuit.egg-info/PKG-INFO` & `tensorcircuit-0.9.0/tensorcircuit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: tensorcircuit
-Version: 0.8.0
+Version: 0.9.0
 Summary: Quantum circuits on top of tensor network
 Home-page: https://github.com/tencent-quantum-lab/tensorcircuit
 Author: TensorCircuit Authors
 Author-email: shixinzhang@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: jax
 Provides-Extra: torch
 Provides-Extra: qiskit
+Provides-Extra: cloud
 License-File: LICENSE
 
 <p align="center">
   <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
     <img width=90% src="docs/source/statics/logov2.jpg">
   </a>
 </p>
@@ -186,14 +187,15 @@
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/buwantaiji"><img src="https://avatars.githubusercontent.com/u/25216189?v=4?s=100" width="100px;" alt="Hao Xie"/><br /><sub><b>Hao Xie</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=buwantaiji" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/pramitsingh0"><img src="https://avatars.githubusercontent.com/u/52959209?v=4?s=100" width="100px;" alt="Pramit Singh"/><br /><sub><b>Pramit Singh</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=pramitsingh0" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/JAllcock"><img src="https://avatars.githubusercontent.com/u/26302022?v=4?s=100" width="100px;" alt="Jonathan Allcock"/><br /><sub><b>Jonathan Allcock</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=JAllcock" title="Documentation">📖</a> <a href="#ideas-JAllcock" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-JAllcock" title="Talks">📢</a></td>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/nealchen2003"><img src="https://avatars.githubusercontent.com/u/45502551?v=4?s=100" width="100px;" alt="nealchen2003"/><br /><sub><b>nealchen2003</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=nealchen2003" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="16.66%"><a href="https://github.com/eurethia"><img src="https://avatars.githubusercontent.com/u/84611606?v=4?s=100" width="100px;" alt="隐公观鱼"/><br /><sub><b>隐公观鱼</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/WiuYuan"><img src="https://avatars.githubusercontent.com/u/108848998?v=4?s=100" width="100px;" alt="WiuYuan"/><br /><sub><b>WiuYuan</b></sub></a><br /><a href="#example-WiuYuan" title="Examples">💡</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `tensorcircuit-0.8.0/tensorcircuit.egg-info/SOURCES.txt` & `tensorcircuit-0.9.0/tensorcircuit.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 examples/variational_dynamics.py
 examples/vqe_extra.py
 examples/vqe_extra_mpo.py
 examples/vqe_extra_mpo_spopt.py
 examples/vqeh2o_benchmark.py
 examples/vqnhe_h6.py
 tensorcircuit/__init__.py
+tensorcircuit/about.py
 tensorcircuit/abstractcircuit.py
 tensorcircuit/asciiart.py
 tensorcircuit/basecircuit.py
 tensorcircuit/channels.py
 tensorcircuit/circuit.py
 tensorcircuit/cons.py
 tensorcircuit/densitymatrix.py
@@ -95,14 +96,23 @@
 tensorcircuit/backends/jax_backend.py
 tensorcircuit/backends/jax_ops.py
 tensorcircuit/backends/numpy_backend.py
 tensorcircuit/backends/pytorch_backend.py
 tensorcircuit/backends/pytorch_ops.py
 tensorcircuit/backends/tensorflow_backend.py
 tensorcircuit/backends/tf_ops.py
+tensorcircuit/cloud/__init__.py
+tensorcircuit/cloud/abstraction.py
+tensorcircuit/cloud/apis.py
+tensorcircuit/cloud/config.py
+tensorcircuit/cloud/local.py
+tensorcircuit/cloud/quafu_provider.py
+tensorcircuit/cloud/tencent.py
+tensorcircuit/cloud/utils.py
+tensorcircuit/cloud/wrapper.py
 tensorcircuit/compiler/__init__.py
 tensorcircuit/compiler/composed_compiler.py
 tensorcircuit/compiler/qiskit_compiler.py
 tensorcircuit/interfaces/__init__.py
 tensorcircuit/interfaces/numpy.py
 tensorcircuit/interfaces/scipy.py
 tensorcircuit/interfaces/tensorflow.py
@@ -120,14 +130,15 @@
 tensorcircuit/templates/measurements.py
 tests/__init__.py
 tests/conftest.py
 tests/test_backends.py
 tests/test_calibrating.py
 tests/test_channels.py
 tests/test_circuit.py
+tests/test_cloud.py
 tests/test_compiler.py
 tests/test_dmcircuit.py
 tests/test_ensemble.py
 tests/test_gates.py
 tests/test_interfaces.py
 tests/test_keras.py
 tests/test_miscs.py
```

### Comparing `tensorcircuit-0.8.0/tests/conftest.py` & `tensorcircuit-0.9.0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,11 +45,23 @@
     except ImportError as e:
         print(e)
         tc.set_backend("numpy")
         pytest.skip("****** No torch backend found, skipping test suit *******")
 
 
 @pytest.fixture(scope="function")
+def cpb():
+    try:
+        tc.set_backend("cupy")
+        yield
+        tc.set_backend("numpy")
+    except ImportError as e:
+        print(e)
+        tc.set_backend("numpy")
+        pytest.skip("****** No cupy backend found, skipping test suit *******")
+
+
+@pytest.fixture(scope="function")
 def highp():
     tc.set_dtype("complex128")
     yield
     tc.set_dtype("complex64")
```

### Comparing `tensorcircuit-0.8.0/tests/test_backends.py` & `tensorcircuit-0.9.0/tests/test_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 thisfile = os.path.abspath(__file__)
 modulepath = os.path.dirname(os.path.dirname(thisfile))
 
 sys.path.insert(0, modulepath)
 import tensorcircuit as tc
 
 dtype = np.complex64
-ii = np.eye(4, dtype=dtype)
-iir = ii.reshape([2, 2, 2, 2])
-ym = np.array([[0, -1.0j], [1.0j, 0]], dtype=dtype)
-zm = np.array([[1.0, 0.0], [0.0, -1.0]], dtype=dtype)
-yz = np.kron(ym, zm)
-yzr = yz.reshape([2, 2, 2, 2])
 
 
 def universal_vmap():
     def sum_real(x, y):
         return tc.backend.real(x + y)
 
     vop = tc.backend.vmap(sum_real, vectorized_argnums=(0, 1))
@@ -46,25 +40,26 @@
 
 
 def test_vmap_tf(tfb):
     r = universal_vmap()
     assert r.numpy()[0, 0] == 3.0
 
 
-@pytest.mark.skip(
-    reason="pytorch backend to be fixed with newly added complex dtype support"
-)
+# @pytest.mark.skip(
+#     reason="pytorch backend to be fixed with newly added complex dtype support"
+# )
 def test_vmap_torch(torchb):
     r = universal_vmap()
     assert r.numpy()[0, 0] == 3.0
 
 
 def test_grad_torch(torchb):
     a = tc.backend.ones([2], dtype="float32")
 
+    # @partial(tc.backend.jit, jit_compile=True)
     @tc.backend.grad
     def f(x):
         return tc.backend.sum(x)
 
     np.testing.assert_allclose(f(a), np.ones([2]), atol=1e-5)
 
 
@@ -173,14 +168,20 @@
             tc.array_to_tensor(np.array([0, 1, 2])),
             tc.array_to_tensor(np.array([2, 1, 0]), dtype="int32"),
         ),
         np.array([2, 1, 0]),
         atol=1e-5,
     )
 
+    def sum_(carry, x):
+        return carry + x
+
+    r = tc.backend.scan(sum_, tc.backend.ones([10, 2]), tc.backend.zeros([2]))
+    np.testing.assert_allclose(r, 10 * np.ones([2]), atol=1e-5)
+
 
 @pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb"), lf("torchb")])
 def test_backend_methods_2(backend):
     np.testing.assert_allclose(tc.backend.mean(tc.backend.ones([10])), 1.0, atol=1e-5)
     # acos acosh asin asinh atan atan2 atanh cosh (cos) tan tanh sinh (sin)
     np.testing.assert_allclose(
         tc.backend.acos(tc.backend.ones([2], dtype="float32")),
@@ -301,15 +302,15 @@
     )
 
 
 @pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb"), lf("torchb")])
 def test_device_cpu_only(backend):
     a = tc.backend.ones([])
     dev_str = tc.backend.device(a)
-    assert dev_str == "cpu"
+    assert dev_str in ["cpu", "gpu:0"]
     tc.backend.device_move(a, dev_str)
 
 
 @pytest.mark.skipif(
     len(tf.config.list_physical_devices()) == 1, reason="no GPU detected"
 )
 @pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb"), lf("torchb")])
@@ -415,51 +416,53 @@
     c = tc.Circuit(n, inputs=inputs)
     paramc = tc.backend.cast(param, "complex64")
 
     for i in range(n):
         c.H(i)
     for j in range(nlayers):
         for i in range(n - 1):
-            c.any(
-                i,
-                i + 1,
-                unitary=tc.backend.cos(paramc[2 * j, i]) * iir
-                + tc.backend.sin(paramc[2 * j, i]) * 1.0j * yzr,
-            )
+            c.ryy(i, i + 1, theta=paramc[2 * j, i])
+            # c.any(
+            #     i,
+            #     i + 1,
+            #     unitary=tc.backend.cos(paramc[2 * j, i]) * iir
+            #     + tc.backend.sin(paramc[2 * j, i]) * 1.0j * yzr,
+            # )
         for i in range(n):
             c.rx(i, theta=paramc[2 * j + 1, i])
     e = 0.0
     for i in range(n):
         e += c.expectation((tc.gates.x(), [i]))
     for i in range(n - 1):  # OBC
         e += c.expectation((tc.gates.z(), [i]), (tc.gates.z(), [(i + 1) % n]))
     e = tc.backend.real(e)
     return e
 
 
-@pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb")])
+@pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb"), lf("torchb")])
 def test_vvag(backend):
     n = 4
     nlayers = 3
     inp = tc.backend.ones([2**n]) / 2 ** (n / 2)
     param = tc.backend.ones([2 * nlayers, n])
-    inp = tc.backend.cast(inp, "complex64")
-    param = tc.backend.cast(param, "complex64")
+    # inp = tc.backend.cast(inp, "complex64")
+    # param = tc.backend.cast(param, "complex64")
 
     vqe_energy_p = partial(vqe_energy, n=n, nlayers=nlayers)
 
     vg = tc.backend.value_and_grad(vqe_energy_p, argnums=(0, 1))
     v0, (g00, g01) = vg(inp, param)
 
     batch = 8
     inps = tc.backend.ones([batch, 2**n]) / 2 ** (n / 2)
     inps = tc.backend.cast(inps, "complex64")
 
     pvag = tc.backend.vvag(vqe_energy_p, argnums=(0, 1))
     v1, (g10, g11) = pvag(inps, param)
+    print(v1.shape, g10.shape, g11.shape)
     np.testing.assert_allclose(v1[0], v0, atol=1e-4)
     np.testing.assert_allclose(g10[0], g00, atol=1e-4)
     np.testing.assert_allclose(g11 / batch, g01, atol=1e-4)
 
 
 @pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb")])
 def test_vvag_dict(backend):
```

### Comparing `tensorcircuit-0.8.0/tests/test_calibrating.py` & `tensorcircuit-0.9.0/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_channels.py` & `tensorcircuit-0.9.0/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_circuit.py` & `tensorcircuit-0.9.0/tests/test_circuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 thisfile = os.path.abspath(__file__)
 modulepath = os.path.dirname(os.path.dirname(thisfile))
 
 sys.path.insert(0, modulepath)
 import tensorcircuit as tc
 
 
-def test_wavefunction():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_wavefunction(backend):
     qc = tc.Circuit(2)
     qc.unitary(
         0,
         1,
         unitary=tc.gates.Gate(np.arange(16).reshape(2, 2, 2, 2).astype(np.complex64)),
     )
     assert np.real(qc.wavefunction()[2]) == 8
@@ -37,23 +38,25 @@
     qc.unitary(
         0, unitary=tc.gates.Gate(np.arange(4).reshape(2, 2).astype(np.complex64))
     )
     qc.wavefunction()
     assert np.real(qc.wavefunction()[2]) == 2
 
 
-def test_basics():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_basics(backend):
     c = tc.Circuit(2)
     c.x(0)
-    np.testing.assert_allclose(c.amplitude("10"), np.array(1.0))
+    np.testing.assert_allclose(tc.backend.numpy(c.amplitude("10")), np.array(1.0))
     c.CNOT(0, 1)
-    np.testing.assert_allclose(c.amplitude("11"), np.array(1.0))
+    np.testing.assert_allclose(tc.backend.numpy(c.amplitude("11")), np.array(1.0))
 
 
-def test_measure():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_measure(backend):
     c = tc.Circuit(3)
     c.H(0)
     c.h(1)
     c.toffoli(0, 1, 2)
     assert c.measure(2)[0] in [0, 1]
 
 
@@ -228,21 +231,24 @@
                 tc.backend.norm(f(jax.random.PRNGKey(23))), 1.0, atol=1e-4
             )
             np.testing.assert_allclose(
                 tc.backend.norm(f(jax.random.PRNGKey(24))), 1.0, atol=1e-4
             )
 
 
-def test_expectation():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_expectation(backend):
     c = tc.Circuit(2)
     c.H(0)
-    np.testing.assert_allclose(c.expectation((tc.gates.z(), [0])), 0, atol=1e-7)
+    np.testing.assert_allclose(
+        tc.backend.numpy(c.expectation((tc.gates.z(), [0]))), 0, atol=1e-7
+    )
 
 
-@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb")])
+@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb"), lf("cpb")])
 def test_exp1(backend):
     @partial(tc.backend.jit, jit_compile=True)
     def sf():
         c = tc.Circuit(2)
         xx = np.array(
             [[0, 0, 0, 1], [0, 0, 1, 0], [0, 1, 0, 0], [1, 0, 0, 0]], dtype=np.complex64
         )
@@ -256,16 +262,16 @@
         xx = np.array(
             [[0, 0, 0, 1], [0, 0, 1, 0], [0, 1, 0, 0], [1, 0, 0, 0]], dtype=np.complex64
         )
         c.exp(0, 1, unitary=xx, theta=tc.num_to_tensor(0.2))
         s1 = c.state()
         return s1
 
-    s = sf()
-    s1 = s1f()
+    s = tc.backend.numpy(sf())
+    s1 = tc.backend.numpy(s1f())
     np.testing.assert_allclose(s, s1, atol=1e-4)
 
 
 def test_complex128(highp, tfb):
     c = tc.Circuit(2)
     c.H(1)
     c.rx(0, theta=tc.gates.num_to_tensor(1j))
@@ -312,58 +318,59 @@
 def test_single_qubit():
     c = tc.Circuit(1)
     c.H(0)
     w = c.state()[0]
     np.testing.assert_allclose(w, np.array([1, 1]) / np.sqrt(2), atol=1e-4)
 
 
-def test_expectation_between_two_states():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_expectation_between_two_states(backend):
     zp = np.array([1.0, 0.0])
     zd = np.array([0.0, 1.0])
     assert tc.expectation((tc.gates.y(), [0]), ket=zp, bra=zd) == 1j
 
     c = tc.Circuit(3)
     c.H(0)
     c.ry(1, theta=tc.num_to_tensor(0.8))
     c.cnot(1, 2)
 
     state = c.wavefunction()
     x1z2 = [(tc.gates.x(), [0]), (tc.gates.z(), [1])]
     e1 = c.expectation(*x1z2)
     e2 = tc.expectation(*x1z2, ket=state, bra=state, normalization=True)
-    np.testing.assert_allclose(e2, e1)
+    np.testing.assert_allclose(tc.backend.numpy(e2), tc.backend.numpy(e1))
 
     c = tc.Circuit(3)
     c.H(0)
     c.ry(1, theta=tc.num_to_tensor(0.8 + 0.7j))
     c.cnot(1, 2)
 
     state = c.wavefunction()
     x1z2 = [(tc.gates.x(), [0]), (tc.gates.z(), [1])]
     e1 = c.expectation(*x1z2) / tc.backend.norm(state) ** 2
     e2 = tc.expectation(*x1z2, ket=state, normalization=True)
-    np.testing.assert_allclose(e2, e1)
+    np.testing.assert_allclose(tc.backend.numpy(e2), tc.backend.numpy(e1))
 
     c = tc.Circuit(2)
     c.X(1)
     s1 = c.state()
     c2 = tc.Circuit(2)
     c2.X(0)
     s2 = c2.state()
     c3 = tc.Circuit(2)
     c3.H(1)
     s3 = c3.state()
     x1x2 = [(tc.gates.x(), [0]), (tc.gates.x(), [1])]
     e = tc.expectation(*x1x2, ket=s1, bra=s2)
-    np.testing.assert_allclose(e, 1.0)
+    np.testing.assert_allclose(tc.backend.numpy(e), 1.0)
     e2 = tc.expectation(*x1x2, ket=s3, bra=s2)
-    np.testing.assert_allclose(e2, 1.0 / np.sqrt(2))
+    np.testing.assert_allclose(tc.backend.numpy(e2), 1.0 / np.sqrt(2))
 
 
-@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb")])
+@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb"), lf("cpb")])
 def test_any_inputs_state(backend):
     c = tc.Circuit(2, inputs=tc.array_to_tensor(np.array([0.0, 0.0, 0.0, 1.0])))
     c.X(0)
     z0 = c.expectation((tc.gates.z(), [0]))
     assert z0 == 1.0
     c = tc.Circuit(2, inputs=tc.array_to_tensor(np.array([0.0, 0.0, 1.0, 0.0])))
     c.X(0)
@@ -375,46 +382,50 @@
     assert z0 == -1.0
     c = tc.Circuit(
         2,
         inputs=tc.array_to_tensor(np.array([1 / np.sqrt(2), 0.0, 1 / np.sqrt(2), 0.0])),
     )
     c.X(0)
     z0 = c.expectation((tc.gates.z(), [0]))
-    np.testing.assert_allclose(z0, 0.0, rtol=1e-4, atol=1e-4)
+    np.testing.assert_allclose(tc.backend.numpy(z0), 0.0, rtol=1e-4, atol=1e-4)
 
 
-@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb")])
+@pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("cpb")])
 def test_postselection(backend):
     c = tc.Circuit(3)
     c.H(1)
     c.H(2)
     c.mid_measurement(1, 1)
     c.mid_measurement(2, 1)
     s = c.wavefunction()
-    np.testing.assert_allclose(tc.backend.real(s[3]), 0.5)
+    np.testing.assert_allclose(tc.backend.numpy(s[3]).real, 0.5)
 
 
-def test_unitary():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_unitary(backend):
     c = tc.Circuit(2, inputs=np.eye(4))
     c.X(0)
     c.Y(1)
-    answer = np.kron(tc.gates.x().tensor, tc.gates.y().tensor)
-    np.testing.assert_allclose(c.wavefunction().reshape([4, 4]), answer, atol=1e-4)
+    answer = tc.backend.numpy(np.kron(tc.gates.x().tensor, tc.gates.y().tensor))
+    np.testing.assert_allclose(
+        tc.backend.numpy(c.wavefunction().reshape([4, 4])), answer, atol=1e-4
+    )
 
 
-def test_expectation_ps():
+@pytest.mark.parametrize("backend", [lf("npb"), lf("cpb")])
+def test_expectation_ps(backend):
     c = tc.Circuit(2)
     c.X(0)
     r = c.expectation_ps(z=[0, 1])
-    np.testing.assert_allclose(r, -1, atol=1e-5)
+    np.testing.assert_allclose(tc.backend.numpy(r), -1, atol=1e-5)
 
     c = tc.Circuit(2)
     c.H(0)
     r = c.expectation_ps(z=[1], x=[0])
-    np.testing.assert_allclose(r, 1, atol=1e-5)
+    np.testing.assert_allclose(tc.backend.numpy(r), 1, atol=1e-5)
 
 
 def test_probability():
     for c_cls in [tc.Circuit, tc.DMCircuit]:
         c = c_cls(2)
         c.h(0)
         c.h(1)
@@ -1500,7 +1511,28 @@
     assert c.get_positional_logical_mapping() == {0: 0, 1: 1, 2: 2}
     c = tc.Circuit(3)
     c.cx(0, 1)
     c.h(1)
     c.measure_instruction(2)
     c.measure_instruction(0)
     assert c.get_positional_logical_mapping() == {0: 2, 1: 0}
+
+
+@pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb")])
+def test_inverse_jit(backend):
+    K = tc.backend
+
+    def simple_ansatz(param):
+        c = tc.Circuit(3)
+        for i in range(3):
+            c.cx(i, (i + 1) % 3)
+            c.rzz(i, (i + 1) % 3, theta=param[i])
+        c1 = c.inverse()
+        c2 = tc.Circuit(3)
+        c2.x(1)
+        c1.append(c2)
+        return tc.backend.real(c1.expectation_ps(z=[1]))
+
+    v_ansatz = K.jit(K.vvag(simple_ansatz))
+    vs, gs = v_ansatz(K.ones([2, 3], dtype="float32"))
+    assert K.shape_tuple(gs) == (2, 3)
+    np.testing.assert_allclose(K.numpy(vs), -1.0 * K.ones([2]), atol=1e-5)
```

### Comparing `tensorcircuit-0.8.0/tests/test_compiler.py` & `tensorcircuit-0.9.0/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_dmcircuit.py` & `tensorcircuit-0.9.0/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_ensemble.py` & `tensorcircuit-0.9.0/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_gates.py` & `tensorcircuit-0.9.0/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_interfaces.py` & `tensorcircuit-0.9.0/tests/test_interfaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -105,14 +105,82 @@
     l3 = torch.sum(l3)
     l3.backward()
     pg = param3.grad
     np.testing.assert_allclose(pg, 2 * np.ones([2]).astype(np.complex64), atol=1e-5)
 
 
 @pytest.mark.skipif(is_torch is False, reason="torch not installed")
+@pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb")])
+def test_torch_interface_kws(backend):
+    def f(param, n):
+        c = tc.Circuit(n)
+        c = tc.templates.blocks.example_block(c, param)
+        loss = c.expectation(
+            [
+                tc.gates.x(),
+                [
+                    1,
+                ],
+            ]
+        )
+        return tc.backend.real(loss)
+
+    f_jit_torch = tc.interfaces.torch_interface_kws(f, jit=True, enable_dlpack=True)
+
+    param = torch.ones([4, 4], requires_grad=True)
+    l = f_jit_torch(param, n=4)
+    l = l**2
+    l.backward()
+
+    pg = param.grad
+    np.testing.assert_allclose(pg.shape, [4, 4])
+    np.testing.assert_allclose(pg[0, 1], -2.146e-3, atol=1e-5)
+
+    def f2(paramzz, paramx, n, nlayer):
+        c = tc.Circuit(n)
+        for i in range(n):
+            c.H(i)
+        for j in range(nlayer):  # 2
+            for i in range(n - 1):
+                c.exp1(i, i + 1, unitary=tc.gates._zz_matrix, theta=paramzz[j, i])
+            for i in range(n):
+                c.rx(i, theta=paramx[j, i])
+        loss1 = c.expectation(
+            [
+                tc.gates.x(),
+                [
+                    1,
+                ],
+            ]
+        )
+        loss2 = c.expectation(
+            [
+                tc.gates.x(),
+                [
+                    2,
+                ],
+            ]
+        )
+        return tc.backend.real(loss1), tc.backend.real(loss2)
+
+    f2_torch = tc.interfaces.torch_interface_kws(f2, jit=True, enable_dlpack=True)
+
+    paramzz = torch.ones([2, 4], requires_grad=True)
+    paramx = torch.ones([2, 4], requires_grad=True)
+
+    l1, l2 = f2_torch(paramzz, paramx, n=4, nlayer=2)
+    l = l1 - l2
+    l.backward()
+
+    pg = paramzz.grad
+    np.testing.assert_allclose(pg.shape, [2, 4])
+    np.testing.assert_allclose(pg[0, 0], -0.41609, atol=1e-5)
+
+
+@pytest.mark.skipif(is_torch is False, reason="torch not installed")
 @pytest.mark.xfail(
     (int(tf.__version__.split(".")[1]) < 9)
     or (int("".join(jax.__version__.split(".")[1:])) < 314),
     reason="version too low for tf or jax",
 )
 @pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb")])
 def test_torch_interface_dlpack_complex(backend):
@@ -293,14 +361,15 @@
         blist.append("pytorch")
     for b in blist:
         ans = tc.interfaces.general_args_to_backend(
             args=tc.backend.ones([2], dtype="float32"),
             target_backend=b,
             enable_dlpack=True,
         )
+        ans = tc.interfaces.which_backend(ans).device_move(ans, "cpu")
         np.testing.assert_allclose(ans, np.ones([2]))
 
 
 @pytest.mark.parametrize("backend", [lf("npb"), lf("tfb"), lf("jaxb")])
 def test_args_to_tensor(backend):
     @partial(
         tc.interfaces.args_to_tensor,
@@ -352,10 +421,9 @@
         [tc.Gate(np.ones([2, 2])), tc.Gate(np.ones([2, 2, 2, 2]))],
         tc.QuOperator.from_tensor(np.ones([2, 2, 2, 2, 2, 2])),
         np.ones([2, 2, 2, 2]),
     )
 
     assert tc.interfaces.which_backend(a[0], return_backend=False) == tc.backend.name
     assert tc.backend.shape_tuple(a[1]) == (2, 2, 2, 2)
-    assert tc.interfaces.which_backend(b, return_backend=False) == tc.backend.name
-    assert tc.backend.shape_tuple(b) == (2, 2, 2, 2, 2, 2)
+    assert tc.backend.shape_tuple(b.eval()) == (2, 2, 2, 2, 2, 2)
     assert tc.backend.shape_tuple(c) == (2, 2, 2, 2)
```

### Comparing `tensorcircuit-0.8.0/tests/test_keras.py` & `tensorcircuit-0.9.0/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_miscs.py` & `tensorcircuit-0.9.0/tests/test_miscs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     ([2, 1], np.kron(y, x)),
     ([3, 1], np.kron(z, x)),
     ([3, 2, 2, 0], np.kron(np.kron(np.kron(z, y), y), i)),
     ([0, 1, 1, 1], np.kron(np.kron(np.kron(i, x), x), x)),
 ]
 
 
+def test_about():
+    print(tc.about())
+
+
 def test_ps2coo(tfb):
     for l, a in check_pairs:
         r1 = PauliString2COO(tf.constant(l, dtype=tf.int64))
         np.testing.assert_allclose(tc.backend.to_dense(r1), a, atol=1e-5)
 
 
 def test_pss2coo(tfb):
```

### Comparing `tensorcircuit-0.8.0/tests/test_mpscircuit.py` & `tensorcircuit-0.9.0/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_noisemodel.py` & `tensorcircuit-0.9.0/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_qaoa.py` & `tensorcircuit-0.9.0/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_quantum.py` & `tensorcircuit-0.9.0/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_quantum_attr.py` & `tensorcircuit-0.9.0/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_results.py` & `tensorcircuit-0.9.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_simplify.py` & `tensorcircuit-0.9.0/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_templates.py` & `tensorcircuit-0.9.0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_torchnn.py` & `tensorcircuit-0.9.0/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.8.0/tests/test_van.py` & `tensorcircuit-0.9.0/tests/test_van.py`

 * *Files identical despite different names*

