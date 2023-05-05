# Comparing `tmp/qrisp-0.0.16.tar.gz` & `tmp/qrisp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrisp-0.0.16.tar", last modified: Fri May  5 09:23:02 2023, max compression
+gzip compressed data, was "qrisp-0.1.0.tar", last modified: Fri May  5 09:51:48 2023, max compression
```

## Comparing `qrisp-0.0.16.tar` & `qrisp-0.1.0.tar`

### file list

```diff
@@ -1,164 +1,162 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.770154 qrisp-0.0.16/
--rw-rw-rw-   0        0        0    14474 2023-04-24 14:39:30.000000 qrisp-0.0.16/LICENSE
--rw-rw-rw-   0        0        0     3120 2023-05-05 09:23:02.771153 qrisp-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0     2528 2023-05-04 15:01:28.000000 qrisp-0.0.16/README.md
--rw-rw-rw-   0        0        0      206 2023-05-03 15:23:04.000000 qrisp-0.0.16/pyproject.toml
--rw-rw-rw-   0        0        0      588 2023-05-05 09:23:02.774156 qrisp-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0     1518 2023-04-26 12:33:10.000000 qrisp-0.0.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:01.924755 qrisp-0.0.16/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:01.967676 qrisp-0.0.16/src/qrisp/
--rw-rw-rw-   0        0        0      715 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.059435 qrisp-0.0.16/src/qrisp/arithmetic/
--rw-rw-rw-   0        0        0    33229 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/arithmetic/SBP_arithmetic.py
--rw-rw-rw-   0        0        0      717 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/arithmetic/__init__.py
--rw-rw-rw-   0        0        0     6820 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/arithmetic/comparisons.py
--rw-rw-rw-   0        0        0     5350 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/arithmetic/incrementation.py
--rw-rw-rw-   0        0        0    26444 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/arithmetic/matrix_multiplication.py
--rw-rw-rw-   0        0        0     3293 2023-04-24 14:36:50.000000 qrisp-0.0.16/src/qrisp/arithmetic/poly_tools.py
--rw-rw-rw-   0        0        0    11049 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/arithmetic/ripple_carry_adder.py
--rw-rw-rw-   0        0        0    16425 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/arithmetic/ripple_division.py
--rw-rw-rw-   0        0        0     1137 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/arithmetic/ripple_mult.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.121772 qrisp-0.0.16/src/qrisp/circuit/
--rw-rw-rw-   0        0        0      759 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/circuit/__init__.py
--rw-rw-rw-   0        0        0     1237 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/circuit/clbit.py
--rw-rw-rw-   0        0        0     5906 2023-05-04 12:50:14.000000 qrisp-0.0.16/src/qrisp/circuit/controlled_operations.py
--rw-rw-rw-   0        0        0     3773 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/circuit/instruction.py
--rw-rw-rw-   0        0        0      504 2023-04-24 14:36:50.000000 qrisp-0.0.16/src/qrisp/circuit/library.py
--rw-rw-rw-   0        0        0    28278 2023-05-04 12:07:53.000000 qrisp-0.0.16/src/qrisp/circuit/operation.py
--rw-rw-rw-   0        0        0    68121 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/circuit/quantum_circuit.py
--rw-rw-rw-   0        0        0     1510 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/circuit/qubit.py
--rw-rw-rw-   0        0        0     5371 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/circuit/standard_operations.py
--rw-rw-rw-   0        0        0     5529 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/circuit/transpiler.py
--rw-rw-rw-   0        0        0     4119 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/circuit/transpiler_old.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.190731 qrisp-0.0.16/src/qrisp/core/
--rw-rw-rw-   0        0        0      782 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/core/__init__.py
--rw-rw-rw-   0        0        0    34131 2023-05-04 12:56:12.000000 qrisp-0.0.16/src/qrisp/core/compilation.py
--rw-rw-rw-   0        0        0    38339 2023-05-04 13:03:20.000000 qrisp-0.0.16/src/qrisp/core/library.py
--rw-rw-rw-   0        0        0    32223 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/core/quantum_array.py
--rw-rw-rw-   0        0        0     9072 2023-05-04 12:17:44.000000 qrisp-0.0.16/src/qrisp/core/quantum_dictionary.py
--rw-rw-rw-   0        0        0    41472 2023-05-04 12:13:38.000000 qrisp-0.0.16/src/qrisp/core/quantum_session.py
--rw-rw-rw-   0        0        0    47245 2023-05-04 12:22:18.000000 qrisp-0.0.16/src/qrisp/core/quantum_variable.py
--rw-rw-rw-   0        0        0    13528 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/core/session_merging_tools.py
--rw-rw-rw-   0        0        0      626 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/default_backend.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.300172 qrisp-0.0.16/src/qrisp/environments/
--rw-rw-rw-   0        0        0     6710 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/environments/GMS_environment.py
--rw-rw-rw-   0        0        0      803 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/environments/__init__.py
--rw-rw-rw-   0        0        0    11072 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/environments/control_environment.py
--rw-rw-rw-   0        0        0     5682 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/environments/gate_wrap_environment.py
--rw-rw-rw-   0        0        0    26090 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/environments/quantum_conditionals.py
--rw-rw-rw-   0        0        0    15094 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/environments/quantum_environments.py
--rw-rw-rw-   0        0        0    20097 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/environments/quantum_inversion.py
--rw-rw-rw-   0        0        0     4008 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/environments/temp_var_environment.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.320663 qrisp-0.0.16/src/qrisp/grover/
--rw-rw-rw-   0        0        0      465 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/grover/__init__.py
--rw-rw-rw-   0        0        0    13152 2023-05-04 12:46:08.000000 qrisp-0.0.16/src/qrisp/grover/grover_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.344581 qrisp-0.0.16/src/qrisp/interface/
--rw-rw-rw-   0        0        0      680 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/__init__.py
--rw-rw-rw-   0        0        0     8052 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/backends.py
--rw-rw-rw-   0        0        0    13521 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/circuit_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.373002 qrisp-0.0.16/src/qrisp/interface/openapi_interface/
--rw-rw-rw-   0        0        0      869 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/openapi_interface/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/openapi_interface/backend_client.py
--rw-rw-rw-   0        0        0     3878 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/openapi_interface/backend_server.py
--rw-rw-rw-   0        0        0     1184 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/openapi_interface/interface_types.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.414106 qrisp-0.0.16/src/qrisp/interface/thrift_interface/
--rw-rw-rw-   0        0        0      638 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/__init__.py
--rw-rw-rw-   0        0        0     3340 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/backend_client.py
--rw-rw-rw-   0        0        0     5900 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/backend_server.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.448330 qrisp-0.0.16/src/qrisp/interface/thrift_interface/codegen/
--rw-rw-rw-   0        0        0    16486 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/codegen/BackendService.py
--rw-rw-rw-   0        0        0      475 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/codegen/__init__.py
--rw-rw-rw-   0        0        0      835 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/codegen/constants.py
--rw-rw-rw-   0        0        0    28640 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/codegen/ttypes.py
--rw-rw-rw-   0        0        0     1068 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/interface_types.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.461677 qrisp-0.0.16/src/qrisp/iterators/
--rw-rw-rw-   0        0        0      492 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/iterators/__init__.py
--rw-rw-rw-   0        0        0     3616 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/iterators/qrange.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.486121 qrisp-0.0.16/src/qrisp/logic_synthesis/
--rw-rw-rw-   0        0        0      605 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/logic_synthesis/__init__.py
--rw-rw-rw-   0        0        0    19564 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/logic_synthesis/gray_synthesis.py
--rw-rw-rw-   0        0        0     2724 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/logic_synthesis/pprm_synthesis.py
--rw-rw-rw-   0        0        0    15282 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/logic_synthesis/truth_tables.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.515331 qrisp-0.0.16/src/qrisp/misc/
--rw-rw-rw-   0        0        0    17523 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/misc/GMS_tools.py
--rw-rw-rw-   0        0        0      500 2023-05-04 12:59:01.000000 qrisp-0.0.16/src/qrisp/misc/__init__.py
--rw-rw-rw-   0        0        0     3989 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/misc/depth_reduction.py
--rw-rw-rw-   0        0        0    20826 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/misc/multi_cx.py
--rw-rw-rw-   0        0        0    58870 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/misc/utility.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.539742 qrisp-0.0.16/src/qrisp/qtypes/
--rw-rw-rw-   0        0        0      618 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/qtypes/__init__.py
--rw-rw-rw-   0        0        0     6095 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/qtypes/quantum_bool.py
--rw-rw-rw-   0        0        0     2199 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/qtypes/quantum_char.py
--rw-rw-rw-   0        0        0    27432 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/qtypes/quantum_float.py
--rw-rw-rw-   0        0        0     4697 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/qtypes/quantum_string.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.567019 qrisp-0.0.16/src/qrisp/quantum_network/
--rw-rw-rw-   0        0        0      636 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.571411 qrisp-0.0.16/src/qrisp/quantum_network/interface/
--rw-rw-rw-   0        0        0      420 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.590633 qrisp-0.0.16/src/qrisp/quantum_network/interface/codegen/
--rw-rw-rw-   0        0        0    56700 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
--rw-rw-rw-   0        0        0      482 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/interface/codegen/__init__.py
--rw-rw-rw-   0        0        0      835 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/interface/codegen/constants.py
--rw-rw-rw-   0        0        0    23289 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/interface/codegen/ttypes.py
--rw-rw-rw-   0        0        0     1348 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/interface_connection_example.py
--rw-rw-rw-   0        0        0    13103 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/qn_client.py
--rw-rw-rw-   0        0        0     5468 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/qn_server.py
--rw-rw-rw-   0        0        0     5246 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/qn_simulator_server.py
--rw-rw-rw-   0        0        0     6427 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/quantum_network/quantum_network_session.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.640527 qrisp-0.0.16/src/qrisp/simulator/
--rw-rw-rw-   0        0        0      834 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/__init__.py
--rw-rw-rw-   0        0        0     9181 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/bi_array_helper.py
--rw-rw-rw-   0        0        0    49803 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/bi_arrays.py
--rw-rw-rw-   0        0        0    49731 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/bi_arrays_new.py
--rw-rw-rw-   0        0        0    27103 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/circuit_preprocessing.py
--rw-rw-rw-   0        0        0    13706 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/circuit_reordering.py
--rw-rw-rw-   0        0        0     7394 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/impure_quantum_state.py
--rw-rw-rw-   0        0        0      514 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/numerics_config.py
--rw-rw-rw-   0        0        0     6109 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/quantum_state.py
--rw-rw-rw-   0        0        0    13159 2023-05-04 11:22:09.000000 qrisp-0.0.16/src/qrisp/simulator/simulator.py
--rw-rw-rw-   0        0        0     7455 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/tensor_factor.py
--rw-rw-rw-   0        0        0    11931 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/simulator/unitary_management.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.655588 qrisp-0.0.16/src/qrisp/uncomputation/
--rw-rw-rw-   0        0        0      563 2023-05-03 15:23:04.000000 qrisp-0.0.16/src/qrisp/uncomputation/__init__.py
--rw-rw-rw-   0        0        0     5987 2023-05-04 11:07:25.000000 qrisp-0.0.16/src/qrisp/uncomputation/type_checker.py
--rw-rw-rw-   0        0        0     4223 2023-05-04 11:07:25.000000 qrisp-0.0.16/src/qrisp/uncomputation/uncomputation.py
--rw-rw-rw-   0        0        0    11619 2023-05-04 12:40:04.000000 qrisp-0.0.16/src/qrisp/uncomputation/unqomp.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:01.994176 qrisp-0.0.16/src/qrisp.egg-info/
--rw-rw-rw-   0        0        0     3120 2023-05-05 09:23:01.000000 qrisp-0.0.16/src/qrisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5225 2023-05-05 09:23:01.000000 qrisp-0.0.16/src/qrisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:23:01.000000 qrisp-0.0.16/src/qrisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-05 09:23:01.000000 qrisp-0.0.16/src/qrisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 09:23:01.000000 qrisp-0.0.16/src/qrisp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:02.768151 qrisp-0.0.16/tests/
--rw-rw-rw-   0        0        0     1127 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_GMS_environment_example.py
--rw-rw-rw-   0        0        0     1505 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_GXX_converter_example.py
--rw-rw-rw-   0        0        0     2391 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_GXX_gates_example.py
--rw-rw-rw-   0        0        0     3155 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_GZZ_gates_example.py
--rw-rw-rw-   0        0        0     2599 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_abstract_parameters.py
--rw-rw-rw-   0        0        0      915 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_array_entry_manipulation.py
--rw-rw-rw-   0        0        0     4089 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_comparisons.py
--rw-rw-rw-   0        0        0     3554 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_conditional_environments_example.py
--rw-rw-rw-   0        0        0     3168 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_controlled_gates.py
--rw-rw-rw-   0        0        0     4369 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_diagonal_hamiltonian_application.py
--rw-rw-rw-   0        0        0     1692 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_gray_synthesis_example.py
--rw-rw-rw-   0        0        0     4087 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_grovers_algorithm.py
--rw-rw-rw-   0        0        0      696 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_hello_world.py
--rw-rw-rw-   0        0        0     1721 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_inpl_matrix_multiplication_example.py
--rw-rw-rw-   0        0        0     1479 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_interface.py
--rw-rw-rw-   0        0        0     1006 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_loops.py
--rw-rw-rw-   0        0        0     2131 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_matrix_multiplication_example.py
--rw-rw-rw-   0        0        0     2424 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_mcx.py
--rw-rw-rw-   0        0        0      680 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_measurement_reduction.py
--rw-rw-rw-   0        0        0      658 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_outcome_array.py
--rw-rw-rw-   0        0        0     1948 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_qiskit_backend_client.py
--rw-rw-rw-   0        0        0      835 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_qompiler.py
--rw-rw-rw-   0        0        0     2963 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_quantum_arithmetic.py
--rw-rw-rw-   0        0        0     3016 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_quantum_dictionary.py
--rw-rw-rw-   0        0        0     1087 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_quantum_division.py
--rw-rw-rw-   0        0        0     5053 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_quantum_teleportation.py
--rw-rw-rw-   0        0        0     1255 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_state_preparation.py
--rw-rw-rw-   0        0        0      994 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_string_test.py
--rw-rw-rw-   0        0        0     5332 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_uncomputation_example.py
--rw-rw-rw-   0        0        0     1651 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/test_unitary_calculation.py
--rw-rw-rw-   0        0        0     4137 2023-05-03 15:23:04.000000 qrisp-0.0.16/tests/tests_doc_examples.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.753478 qrisp-0.1.0/
+-rw-rw-rw-   0        0        0    14474 2023-04-24 14:39:30.000000 qrisp-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3119 2023-05-05 09:51:48.754479 qrisp-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2528 2023-05-04 15:01:28.000000 qrisp-0.1.0/README.md
+-rw-rw-rw-   0        0        0      206 2023-05-03 15:23:04.000000 qrisp-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      587 2023-05-05 09:51:48.756480 qrisp-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2023-04-26 12:33:10.000000 qrisp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.121717 qrisp-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.165257 qrisp-0.1.0/src/qrisp/
+-rw-rw-rw-   0        0        0      715 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.214098 qrisp-0.1.0/src/qrisp/arithmetic/
+-rw-rw-rw-   0        0        0    33229 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/arithmetic/SBP_arithmetic.py
+-rw-rw-rw-   0        0        0      717 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/arithmetic/__init__.py
+-rw-rw-rw-   0        0        0     6820 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/arithmetic/comparisons.py
+-rw-rw-rw-   0        0        0     5350 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/arithmetic/incrementation.py
+-rw-rw-rw-   0        0        0    26444 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/arithmetic/matrix_multiplication.py
+-rw-rw-rw-   0        0        0     3293 2023-04-24 14:36:50.000000 qrisp-0.1.0/src/qrisp/arithmetic/poly_tools.py
+-rw-rw-rw-   0        0        0    11049 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/arithmetic/ripple_carry_adder.py
+-rw-rw-rw-   0        0        0    16425 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/arithmetic/ripple_division.py
+-rw-rw-rw-   0        0        0     1137 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/arithmetic/ripple_mult.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.254205 qrisp-0.1.0/src/qrisp/circuit/
+-rw-rw-rw-   0        0        0      759 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/circuit/__init__.py
+-rw-rw-rw-   0        0        0     1237 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/circuit/clbit.py
+-rw-rw-rw-   0        0        0     5906 2023-05-04 12:50:14.000000 qrisp-0.1.0/src/qrisp/circuit/controlled_operations.py
+-rw-rw-rw-   0        0        0     3773 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/circuit/instruction.py
+-rw-rw-rw-   0        0        0      504 2023-04-24 14:36:50.000000 qrisp-0.1.0/src/qrisp/circuit/library.py
+-rw-rw-rw-   0        0        0    28278 2023-05-04 12:07:53.000000 qrisp-0.1.0/src/qrisp/circuit/operation.py
+-rw-rw-rw-   0        0        0    68121 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/circuit/quantum_circuit.py
+-rw-rw-rw-   0        0        0     1510 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/circuit/qubit.py
+-rw-rw-rw-   0        0        0     5371 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/circuit/standard_operations.py
+-rw-rw-rw-   0        0        0     5529 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/circuit/transpiler.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.289008 qrisp-0.1.0/src/qrisp/core/
+-rw-rw-rw-   0        0        0      782 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/core/__init__.py
+-rw-rw-rw-   0        0        0    34131 2023-05-04 12:56:12.000000 qrisp-0.1.0/src/qrisp/core/compilation.py
+-rw-rw-rw-   0        0        0    38339 2023-05-04 13:03:20.000000 qrisp-0.1.0/src/qrisp/core/library.py
+-rw-rw-rw-   0        0        0    32223 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/core/quantum_array.py
+-rw-rw-rw-   0        0        0     9072 2023-05-04 12:17:44.000000 qrisp-0.1.0/src/qrisp/core/quantum_dictionary.py
+-rw-rw-rw-   0        0        0    41472 2023-05-04 12:13:38.000000 qrisp-0.1.0/src/qrisp/core/quantum_session.py
+-rw-rw-rw-   0        0        0    47245 2023-05-04 12:22:18.000000 qrisp-0.1.0/src/qrisp/core/quantum_variable.py
+-rw-rw-rw-   0        0        0    13528 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/core/session_merging_tools.py
+-rw-rw-rw-   0        0        0      626 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/default_backend.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.323080 qrisp-0.1.0/src/qrisp/environments/
+-rw-rw-rw-   0        0        0     6710 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/environments/GMS_environment.py
+-rw-rw-rw-   0        0        0      803 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/environments/__init__.py
+-rw-rw-rw-   0        0        0    11072 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/environments/control_environment.py
+-rw-rw-rw-   0        0        0     5682 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/environments/gate_wrap_environment.py
+-rw-rw-rw-   0        0        0    26090 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/environments/quantum_conditionals.py
+-rw-rw-rw-   0        0        0    15094 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/environments/quantum_environments.py
+-rw-rw-rw-   0        0        0    20097 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/environments/quantum_inversion.py
+-rw-rw-rw-   0        0        0     4008 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/environments/temp_var_environment.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.331102 qrisp-0.1.0/src/qrisp/grover/
+-rw-rw-rw-   0        0        0      465 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/grover/__init__.py
+-rw-rw-rw-   0        0        0    13152 2023-05-04 12:46:08.000000 qrisp-0.1.0/src/qrisp/grover/grover_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.341560 qrisp-0.1.0/src/qrisp/interface/
+-rw-rw-rw-   0        0        0      680 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/__init__.py
+-rw-rw-rw-   0        0        0     8052 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/backends.py
+-rw-rw-rw-   0        0        0    13521 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/circuit_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.359854 qrisp-0.1.0/src/qrisp/interface/openapi_interface/
+-rw-rw-rw-   0        0        0      869 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/openapi_interface/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/openapi_interface/backend_client.py
+-rw-rw-rw-   0        0        0     3878 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/openapi_interface/backend_server.py
+-rw-rw-rw-   0        0        0     1184 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/openapi_interface/interface_types.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.381960 qrisp-0.1.0/src/qrisp/interface/thrift_interface/
+-rw-rw-rw-   0        0        0      638 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/__init__.py
+-rw-rw-rw-   0        0        0     3340 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/backend_client.py
+-rw-rw-rw-   0        0        0     5900 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/backend_server.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.400311 qrisp-0.1.0/src/qrisp/interface/thrift_interface/codegen/
+-rw-rw-rw-   0        0        0    16486 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/codegen/BackendService.py
+-rw-rw-rw-   0        0        0      475 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    28640 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0     1068 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/interface_types.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.409458 qrisp-0.1.0/src/qrisp/iterators/
+-rw-rw-rw-   0        0        0      492 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/iterators/__init__.py
+-rw-rw-rw-   0        0        0     3616 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/iterators/qrange.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.429400 qrisp-0.1.0/src/qrisp/logic_synthesis/
+-rw-rw-rw-   0        0        0      605 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/logic_synthesis/__init__.py
+-rw-rw-rw-   0        0        0    19564 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/logic_synthesis/gray_synthesis.py
+-rw-rw-rw-   0        0        0     2724 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/logic_synthesis/pprm_synthesis.py
+-rw-rw-rw-   0        0        0    15282 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/logic_synthesis/truth_tables.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.450971 qrisp-0.1.0/src/qrisp/misc/
+-rw-rw-rw-   0        0        0    17523 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/misc/GMS_tools.py
+-rw-rw-rw-   0        0        0      500 2023-05-04 12:59:01.000000 qrisp-0.1.0/src/qrisp/misc/__init__.py
+-rw-rw-rw-   0        0        0     3989 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/misc/depth_reduction.py
+-rw-rw-rw-   0        0        0    20826 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/misc/multi_cx.py
+-rw-rw-rw-   0        0        0    58870 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/misc/utility.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.475044 qrisp-0.1.0/src/qrisp/qtypes/
+-rw-rw-rw-   0        0        0      618 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/qtypes/__init__.py
+-rw-rw-rw-   0        0        0     6095 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/qtypes/quantum_bool.py
+-rw-rw-rw-   0        0        0     2199 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/qtypes/quantum_char.py
+-rw-rw-rw-   0        0        0    27432 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/qtypes/quantum_float.py
+-rw-rw-rw-   0        0        0     4697 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/qtypes/quantum_string.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.499353 qrisp-0.1.0/src/qrisp/quantum_network/
+-rw-rw-rw-   0        0        0      636 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.502343 qrisp-0.1.0/src/qrisp/quantum_network/interface/
+-rw-rw-rw-   0        0        0      420 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.538774 qrisp-0.1.0/src/qrisp/quantum_network/interface/codegen/
+-rw-rw-rw-   0        0        0    56700 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
+-rw-rw-rw-   0        0        0      482 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    23289 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0     1348 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/interface_connection_example.py
+-rw-rw-rw-   0        0        0    13103 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/qn_client.py
+-rw-rw-rw-   0        0        0     5468 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/qn_server.py
+-rw-rw-rw-   0        0        0     5246 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/qn_simulator_server.py
+-rw-rw-rw-   0        0        0     6427 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/quantum_network/quantum_network_session.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.610465 qrisp-0.1.0/src/qrisp/simulator/
+-rw-rw-rw-   0        0        0      834 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/__init__.py
+-rw-rw-rw-   0        0        0     9181 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/bi_array_helper.py
+-rw-rw-rw-   0        0        0    49803 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/bi_arrays.py
+-rw-rw-rw-   0        0        0    27103 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/circuit_preprocessing.py
+-rw-rw-rw-   0        0        0    13706 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/circuit_reordering.py
+-rw-rw-rw-   0        0        0     7394 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/impure_quantum_state.py
+-rw-rw-rw-   0        0        0      514 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/numerics_config.py
+-rw-rw-rw-   0        0        0     6109 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/quantum_state.py
+-rw-rw-rw-   0        0        0    13159 2023-05-04 11:22:09.000000 qrisp-0.1.0/src/qrisp/simulator/simulator.py
+-rw-rw-rw-   0        0        0     7455 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/tensor_factor.py
+-rw-rw-rw-   0        0        0    11931 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/simulator/unitary_management.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.627604 qrisp-0.1.0/src/qrisp/uncomputation/
+-rw-rw-rw-   0        0        0      563 2023-05-03 15:23:04.000000 qrisp-0.1.0/src/qrisp/uncomputation/__init__.py
+-rw-rw-rw-   0        0        0     5987 2023-05-04 11:07:25.000000 qrisp-0.1.0/src/qrisp/uncomputation/type_checker.py
+-rw-rw-rw-   0        0        0     4223 2023-05-04 11:07:25.000000 qrisp-0.1.0/src/qrisp/uncomputation/uncomputation.py
+-rw-rw-rw-   0        0        0    11619 2023-05-04 12:40:04.000000 qrisp-0.1.0/src/qrisp/uncomputation/unqomp.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.181323 qrisp-0.1.0/src/qrisp.egg-info/
+-rw-rw-rw-   0        0        0     3119 2023-05-05 09:51:48.000000 qrisp-0.1.0/src/qrisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5152 2023-05-05 09:51:48.000000 qrisp-0.1.0/src/qrisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:51:48.000000 qrisp-0.1.0/src/qrisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-05 09:51:48.000000 qrisp-0.1.0/src/qrisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 09:51:48.000000 qrisp-0.1.0/src/qrisp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 09:51:48.749479 qrisp-0.1.0/tests/
+-rw-rw-rw-   0        0        0     1127 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_GMS_environment_example.py
+-rw-rw-rw-   0        0        0     1505 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_GXX_converter_example.py
+-rw-rw-rw-   0        0        0     2391 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_GXX_gates_example.py
+-rw-rw-rw-   0        0        0     3155 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_GZZ_gates_example.py
+-rw-rw-rw-   0        0        0     2599 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_abstract_parameters.py
+-rw-rw-rw-   0        0        0      915 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_array_entry_manipulation.py
+-rw-rw-rw-   0        0        0     4089 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_comparisons.py
+-rw-rw-rw-   0        0        0     3554 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_conditional_environments_example.py
+-rw-rw-rw-   0        0        0     3168 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_controlled_gates.py
+-rw-rw-rw-   0        0        0     4369 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_diagonal_hamiltonian_application.py
+-rw-rw-rw-   0        0        0     1692 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_gray_synthesis_example.py
+-rw-rw-rw-   0        0        0     4087 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_grovers_algorithm.py
+-rw-rw-rw-   0        0        0      696 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_hello_world.py
+-rw-rw-rw-   0        0        0     1721 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_inpl_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     1479 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_interface.py
+-rw-rw-rw-   0        0        0     1006 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_loops.py
+-rw-rw-rw-   0        0        0     2131 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     2424 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_mcx.py
+-rw-rw-rw-   0        0        0      680 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_measurement_reduction.py
+-rw-rw-rw-   0        0        0      658 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_outcome_array.py
+-rw-rw-rw-   0        0        0     1948 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_qiskit_backend_client.py
+-rw-rw-rw-   0        0        0      835 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_qompiler.py
+-rw-rw-rw-   0        0        0     2963 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_quantum_arithmetic.py
+-rw-rw-rw-   0        0        0     3016 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_quantum_dictionary.py
+-rw-rw-rw-   0        0        0     1087 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_quantum_division.py
+-rw-rw-rw-   0        0        0     5053 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_quantum_teleportation.py
+-rw-rw-rw-   0        0        0     1255 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_state_preparation.py
+-rw-rw-rw-   0        0        0      994 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_string_test.py
+-rw-rw-rw-   0        0        0     5332 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_uncomputation_example.py
+-rw-rw-rw-   0        0        0     1651 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/test_unitary_calculation.py
+-rw-rw-rw-   0        0        0     4137 2023-05-03 15:23:04.000000 qrisp-0.1.0/tests/tests_doc_examples.py
```

### Comparing `qrisp-0.0.16/LICENSE` & `qrisp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/PKG-INFO` & `qrisp-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.0.16
+Version: 0.1.0
 Summary: Qrisp - A high level language for gate-based quantum computing
 Home-page: https://github.com/fraunhoferfokus/Qrisp
 Author: Raphael Seidel
 Author-email: raphael.seidel@fokus.fraunhofer.de
 Project-URL: Bug Tracker, https://github.com/fraunhoferfokus/Qrisp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
```

### Comparing `qrisp-0.0.16/README.md` & `qrisp-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/setup.cfg` & `qrisp-0.1.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7269 7370 0d0a 7665 7273 696f   = qrisp..versio
-00000020: 6e20 3d20 302e 302e 3136 0d0a 6175 7468  n = 0.0.16..auth
-00000030: 6f72 203d 2052 6170 6861 656c 2053 6569  or = Raphael Sei
-00000040: 6465 6c0d 0a61 7574 686f 725f 656d 6169  del..author_emai
-00000050: 6c20 3d20 7261 7068 6165 6c2e 7365 6964  l = raphael.seid
-00000060: 656c 4066 6f6b 7573 2e66 7261 756e 686f  el@fokus.fraunho
-00000070: 6665 722e 6465 0d0a 6465 7363 7269 7074  fer.de..descript
-00000080: 696f 6e20 3d20 4120 736d 616c 6c20 6578  ion = A small ex
-00000090: 616d 706c 6520 7061 636b 6167 650d 0a6c  ample package..l
-000000a0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000b0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000c0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000d0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000e0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000f0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000100: 6769 7468 7562 2e63 6f6d 2f66 7261 756e  github.com/fraun
-00000110: 686f 6665 7266 6f6b 7573 2f51 7269 7370  hoferfokus/Qrisp
-00000120: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
-00000130: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
-00000140: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000150: 2e63 6f6d 2f66 7261 756e 686f 6665 7266  .com/fraunhoferf
-00000160: 6f6b 7573 2f51 7269 7370 2f69 7373 7565  okus/Qrisp/issue
-00000170: 730d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  s....[options]..
-00000180: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000190: 093d 7372 630d 0a70 6163 6b61 6765 7320  .=src..packages 
-000001a0: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-000001b0: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
-000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-000001d0: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-000001e0: 7265 203d 2073 7263 0d0a 0d0a 5b74 6f6f  re = src....[too
-000001f0: 6c3a 7079 7465 7374 5d0d 0a74 6573 7470  l:pytest]..testp
-00000200: 6174 6873 203d 202e 2f74 6573 7473 0d0a  aths = ./tests..
-00000210: 7079 7468 6f6e 7061 7468 203d 202e 0d0a  pythonpath = ...
-00000220: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000230: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000240: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000020: 6e20 3d20 302e 312e 300d 0a61 7574 686f  n = 0.1.0..autho
+00000030: 7220 3d20 5261 7068 6165 6c20 5365 6964  r = Raphael Seid
+00000040: 656c 0d0a 6175 7468 6f72 5f65 6d61 696c  el..author_email
+00000050: 203d 2072 6170 6861 656c 2e73 6569 6465   = raphael.seide
+00000060: 6c40 666f 6b75 732e 6672 6175 6e68 6f66  l@fokus.fraunhof
+00000070: 6572 2e64 650d 0a64 6573 6372 6970 7469  er.de..descripti
+00000080: 6f6e 203d 2041 2073 6d61 6c6c 2065 7861  on = A small exa
+00000090: 6d70 6c65 2070 6163 6b61 6765 0d0a 6c6f  mple package..lo
+000000a0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+000000b0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+000000c0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000d0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+000000e0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+000000f0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+00000100: 6974 6875 622e 636f 6d2f 6672 6175 6e68  ithub.com/fraunh
+00000110: 6f66 6572 666f 6b75 732f 5172 6973 700d  oferfokus/Qrisp.
+00000120: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
+00000130: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
+00000140: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000150: 636f 6d2f 6672 6175 6e68 6f66 6572 666f  com/fraunhoferfo
+00000160: 6b75 732f 5172 6973 702f 6973 7375 6573  kus/Qrisp/issues
+00000170: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000180: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000190: 3d73 7263 0d0a 7061 636b 6167 6573 203d  =src..packages =
+000001a0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+000001b0: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
+000001c0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+000001d0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+000001e0: 6520 3d20 7372 630d 0a0d 0a5b 746f 6f6c  e = src....[tool
+000001f0: 3a70 7974 6573 745d 0d0a 7465 7374 7061  :pytest]..testpa
+00000200: 7468 7320 3d20 2e2f 7465 7374 730d 0a70  ths = ./tests..p
+00000210: 7974 686f 6e70 6174 6820 3d20 2e0d 0a0d  ythonpath = ....
+00000220: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+00000230: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+00000240: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `qrisp-0.0.16/setup.py` & `qrisp-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/__init__.py` & `qrisp-0.1.0/src/qrisp/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/SBP_arithmetic.py` & `qrisp-0.1.0/src/qrisp/arithmetic/SBP_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/__init__.py` & `qrisp-0.1.0/src/qrisp/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/comparisons.py` & `qrisp-0.1.0/src/qrisp/arithmetic/comparisons.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/incrementation.py` & `qrisp-0.1.0/src/qrisp/arithmetic/incrementation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/matrix_multiplication.py` & `qrisp-0.1.0/src/qrisp/arithmetic/matrix_multiplication.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/poly_tools.py` & `qrisp-0.1.0/src/qrisp/arithmetic/poly_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/ripple_carry_adder.py` & `qrisp-0.1.0/src/qrisp/arithmetic/ripple_carry_adder.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/ripple_division.py` & `qrisp-0.1.0/src/qrisp/arithmetic/ripple_division.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/arithmetic/ripple_mult.py` & `qrisp-0.1.0/src/qrisp/arithmetic/ripple_mult.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/__init__.py` & `qrisp-0.1.0/src/qrisp/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/clbit.py` & `qrisp-0.1.0/src/qrisp/circuit/clbit.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/controlled_operations.py` & `qrisp-0.1.0/src/qrisp/circuit/controlled_operations.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/instruction.py` & `qrisp-0.1.0/src/qrisp/circuit/instruction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/operation.py` & `qrisp-0.1.0/src/qrisp/circuit/operation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/quantum_circuit.py` & `qrisp-0.1.0/src/qrisp/circuit/quantum_circuit.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/qubit.py` & `qrisp-0.1.0/src/qrisp/circuit/qubit.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/standard_operations.py` & `qrisp-0.1.0/src/qrisp/circuit/standard_operations.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/circuit/transpiler.py` & `qrisp-0.1.0/src/qrisp/circuit/transpiler.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/core/__init__.py` & `qrisp-0.1.0/src/qrisp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/core/compilation.py` & `qrisp-0.1.0/src/qrisp/core/compilation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/core/library.py` & `qrisp-0.1.0/src/qrisp/core/library.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/core/quantum_array.py` & `qrisp-0.1.0/src/qrisp/core/quantum_array.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/core/quantum_dictionary.py` & `qrisp-0.1.0/src/qrisp/core/quantum_dictionary.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/core/quantum_session.py` & `qrisp-0.1.0/src/qrisp/core/quantum_session.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/core/quantum_variable.py` & `qrisp-0.1.0/src/qrisp/core/quantum_variable.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/core/session_merging_tools.py` & `qrisp-0.1.0/src/qrisp/core/session_merging_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/default_backend.py` & `qrisp-0.1.0/src/qrisp/default_backend.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/environments/GMS_environment.py` & `qrisp-0.1.0/src/qrisp/environments/GMS_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/environments/__init__.py` & `qrisp-0.1.0/src/qrisp/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/environments/control_environment.py` & `qrisp-0.1.0/src/qrisp/environments/control_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/environments/gate_wrap_environment.py` & `qrisp-0.1.0/src/qrisp/environments/gate_wrap_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/environments/quantum_conditionals.py` & `qrisp-0.1.0/src/qrisp/environments/quantum_conditionals.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/environments/quantum_environments.py` & `qrisp-0.1.0/src/qrisp/environments/quantum_environments.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/environments/quantum_inversion.py` & `qrisp-0.1.0/src/qrisp/environments/quantum_inversion.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/environments/temp_var_environment.py` & `qrisp-0.1.0/src/qrisp/environments/temp_var_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/grover/grover_tools.py` & `qrisp-0.1.0/src/qrisp/grover/grover_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/__init__.py` & `qrisp-0.1.0/src/qrisp/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/backends.py` & `qrisp-0.1.0/src/qrisp/interface/backends.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/circuit_converter.py` & `qrisp-0.1.0/src/qrisp/interface/circuit_converter.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/openapi_interface/__init__.py` & `qrisp-0.1.0/src/qrisp/interface/openapi_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/openapi_interface/backend_client.py` & `qrisp-0.1.0/src/qrisp/interface/openapi_interface/backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/openapi_interface/backend_server.py` & `qrisp-0.1.0/src/qrisp/interface/openapi_interface/backend_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/openapi_interface/interface_types.py` & `qrisp-0.1.0/src/qrisp/interface/openapi_interface/interface_types.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/thrift_interface/__init__.py` & `qrisp-0.1.0/src/qrisp/interface/thrift_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/thrift_interface/backend_client.py` & `qrisp-0.1.0/src/qrisp/interface/thrift_interface/backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/thrift_interface/backend_server.py` & `qrisp-0.1.0/src/qrisp/interface/thrift_interface/backend_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/thrift_interface/codegen/BackendService.py` & `qrisp-0.1.0/src/qrisp/interface/thrift_interface/codegen/BackendService.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/thrift_interface/codegen/constants.py` & `qrisp-0.1.0/src/qrisp/interface/thrift_interface/codegen/constants.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/thrift_interface/codegen/ttypes.py` & `qrisp-0.1.0/src/qrisp/interface/thrift_interface/codegen/ttypes.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/thrift_interface/interface_types.py` & `qrisp-0.1.0/src/qrisp/interface/thrift_interface/interface_types.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py` & `qrisp-0.1.0/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/iterators/qrange.py` & `qrisp-0.1.0/src/qrisp/iterators/qrange.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/logic_synthesis/__init__.py` & `qrisp-0.1.0/src/qrisp/logic_synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/logic_synthesis/gray_synthesis.py` & `qrisp-0.1.0/src/qrisp/logic_synthesis/gray_synthesis.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/logic_synthesis/pprm_synthesis.py` & `qrisp-0.1.0/src/qrisp/logic_synthesis/pprm_synthesis.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/logic_synthesis/truth_tables.py` & `qrisp-0.1.0/src/qrisp/logic_synthesis/truth_tables.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/misc/GMS_tools.py` & `qrisp-0.1.0/src/qrisp/misc/GMS_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/misc/depth_reduction.py` & `qrisp-0.1.0/src/qrisp/misc/depth_reduction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/misc/multi_cx.py` & `qrisp-0.1.0/src/qrisp/misc/multi_cx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/misc/utility.py` & `qrisp-0.1.0/src/qrisp/misc/utility.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/qtypes/__init__.py` & `qrisp-0.1.0/src/qrisp/qtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/qtypes/quantum_bool.py` & `qrisp-0.1.0/src/qrisp/qtypes/quantum_bool.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/qtypes/quantum_char.py` & `qrisp-0.1.0/src/qrisp/qtypes/quantum_char.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/qtypes/quantum_float.py` & `qrisp-0.1.0/src/qrisp/qtypes/quantum_float.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/qtypes/quantum_string.py` & `qrisp-0.1.0/src/qrisp/qtypes/quantum_string.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/__init__.py` & `qrisp-0.1.0/src/qrisp/quantum_network/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py` & `qrisp-0.1.0/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/interface/codegen/constants.py` & `qrisp-0.1.0/src/qrisp/quantum_network/interface/codegen/constants.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/interface/codegen/ttypes.py` & `qrisp-0.1.0/src/qrisp/quantum_network/interface/codegen/ttypes.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/interface_connection_example.py` & `qrisp-0.1.0/src/qrisp/quantum_network/interface_connection_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/qn_client.py` & `qrisp-0.1.0/src/qrisp/quantum_network/qn_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/qn_server.py` & `qrisp-0.1.0/src/qrisp/quantum_network/qn_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/qn_simulator_server.py` & `qrisp-0.1.0/src/qrisp/quantum_network/qn_simulator_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/quantum_network/quantum_network_session.py` & `qrisp-0.1.0/src/qrisp/quantum_network/quantum_network_session.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/__init__.py` & `qrisp-0.1.0/src/qrisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/bi_array_helper.py` & `qrisp-0.1.0/src/qrisp/simulator/bi_array_helper.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/bi_arrays.py` & `qrisp-0.1.0/src/qrisp/simulator/bi_arrays.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/circuit_preprocessing.py` & `qrisp-0.1.0/src/qrisp/simulator/circuit_preprocessing.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/circuit_reordering.py` & `qrisp-0.1.0/src/qrisp/simulator/circuit_reordering.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/impure_quantum_state.py` & `qrisp-0.1.0/src/qrisp/simulator/impure_quantum_state.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/numerics_config.py` & `qrisp-0.1.0/src/qrisp/simulator/numerics_config.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/quantum_state.py` & `qrisp-0.1.0/src/qrisp/simulator/quantum_state.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/simulator.py` & `qrisp-0.1.0/src/qrisp/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/tensor_factor.py` & `qrisp-0.1.0/src/qrisp/simulator/tensor_factor.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/simulator/unitary_management.py` & `qrisp-0.1.0/src/qrisp/simulator/unitary_management.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/uncomputation/__init__.py` & `qrisp-0.1.0/src/qrisp/uncomputation/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/uncomputation/type_checker.py` & `qrisp-0.1.0/src/qrisp/uncomputation/type_checker.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/uncomputation/uncomputation.py` & `qrisp-0.1.0/src/qrisp/uncomputation/uncomputation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp/uncomputation/unqomp.py` & `qrisp-0.1.0/src/qrisp/uncomputation/unqomp.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/src/qrisp.egg-info/PKG-INFO` & `qrisp-0.1.0/src/qrisp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.0.16
+Version: 0.1.0
 Summary: Qrisp - A high level language for gate-based quantum computing
 Home-page: https://github.com/fraunhoferfokus/Qrisp
 Author: Raphael Seidel
 Author-email: raphael.seidel@fokus.fraunhofer.de
 Project-URL: Bug Tracker, https://github.com/fraunhoferfokus/Qrisp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
```

### Comparing `qrisp-0.0.16/src/qrisp.egg-info/SOURCES.txt` & `qrisp-0.1.0/src/qrisp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 src/qrisp/circuit/instruction.py
 src/qrisp/circuit/library.py
 src/qrisp/circuit/operation.py
 src/qrisp/circuit/quantum_circuit.py
 src/qrisp/circuit/qubit.py
 src/qrisp/circuit/standard_operations.py
 src/qrisp/circuit/transpiler.py
-src/qrisp/circuit/transpiler_old.py
 src/qrisp/core/__init__.py
 src/qrisp/core/compilation.py
 src/qrisp/core/library.py
 src/qrisp/core/quantum_array.py
 src/qrisp/core/quantum_dictionary.py
 src/qrisp/core/quantum_session.py
 src/qrisp/core/quantum_variable.py
@@ -90,15 +89,14 @@
 src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
 src/qrisp/quantum_network/interface/codegen/__init__.py
 src/qrisp/quantum_network/interface/codegen/constants.py
 src/qrisp/quantum_network/interface/codegen/ttypes.py
 src/qrisp/simulator/__init__.py
 src/qrisp/simulator/bi_array_helper.py
 src/qrisp/simulator/bi_arrays.py
-src/qrisp/simulator/bi_arrays_new.py
 src/qrisp/simulator/circuit_preprocessing.py
 src/qrisp/simulator/circuit_reordering.py
 src/qrisp/simulator/impure_quantum_state.py
 src/qrisp/simulator/numerics_config.py
 src/qrisp/simulator/quantum_state.py
 src/qrisp/simulator/simulator.py
 src/qrisp/simulator/tensor_factor.py
```

### Comparing `qrisp-0.0.16/tests/test_GMS_environment_example.py` & `qrisp-0.1.0/tests/test_GMS_environment_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_GXX_converter_example.py` & `qrisp-0.1.0/tests/test_GXX_converter_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_GXX_gates_example.py` & `qrisp-0.1.0/tests/test_GXX_gates_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_GZZ_gates_example.py` & `qrisp-0.1.0/tests/test_GZZ_gates_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_abstract_parameters.py` & `qrisp-0.1.0/tests/test_abstract_parameters.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_array_entry_manipulation.py` & `qrisp-0.1.0/tests/test_array_entry_manipulation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_comparisons.py` & `qrisp-0.1.0/tests/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_conditional_environments_example.py` & `qrisp-0.1.0/tests/test_conditional_environments_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_controlled_gates.py` & `qrisp-0.1.0/tests/test_controlled_gates.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_diagonal_hamiltonian_application.py` & `qrisp-0.1.0/tests/test_diagonal_hamiltonian_application.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_gray_synthesis_example.py` & `qrisp-0.1.0/tests/test_gray_synthesis_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_grovers_algorithm.py` & `qrisp-0.1.0/tests/test_grovers_algorithm.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_hello_world.py` & `qrisp-0.1.0/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_inpl_matrix_multiplication_example.py` & `qrisp-0.1.0/tests/test_inpl_matrix_multiplication_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_interface.py` & `qrisp-0.1.0/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_loops.py` & `qrisp-0.1.0/tests/test_loops.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_matrix_multiplication_example.py` & `qrisp-0.1.0/tests/test_matrix_multiplication_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_mcx.py` & `qrisp-0.1.0/tests/test_mcx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_measurement_reduction.py` & `qrisp-0.1.0/tests/test_measurement_reduction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_outcome_array.py` & `qrisp-0.1.0/tests/test_outcome_array.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_qiskit_backend_client.py` & `qrisp-0.1.0/tests/test_qiskit_backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_qompiler.py` & `qrisp-0.1.0/tests/test_qompiler.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_quantum_arithmetic.py` & `qrisp-0.1.0/tests/test_quantum_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_quantum_dictionary.py` & `qrisp-0.1.0/tests/test_quantum_dictionary.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_quantum_division.py` & `qrisp-0.1.0/tests/test_quantum_division.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_quantum_teleportation.py` & `qrisp-0.1.0/tests/test_quantum_teleportation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_state_preparation.py` & `qrisp-0.1.0/tests/test_state_preparation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_string_test.py` & `qrisp-0.1.0/tests/test_string_test.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_uncomputation_example.py` & `qrisp-0.1.0/tests/test_uncomputation_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/test_unitary_calculation.py` & `qrisp-0.1.0/tests/test_unitary_calculation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.16/tests/tests_doc_examples.py` & `qrisp-0.1.0/tests/tests_doc_examples.py`

 * *Files identical despite different names*

