# Comparing `tmp/QuantumIntelligence-0.0.6.tar.gz` & `tmp/QuantumIntelligence-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumIntelligence-0.0.6.tar", last modified: Fri Apr 28 05:27:26 2023, max compression
+gzip compressed data, was "QuantumIntelligence-0.0.7.tar", last modified: Fri May  5 09:43:58 2023, max compression
```

## Comparing `QuantumIntelligence-0.0.6.tar` & `QuantumIntelligence-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.138677 QuantumIntelligence-0.0.6/
--rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1763 2023-04-28 05:27:26.138251 QuantumIntelligence-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 05:27:26.138914 QuantumIntelligence-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     8844 2023-04-28 05:27:11.000000 QuantumIntelligence-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.101615 QuantumIntelligence-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.106491 QuantumIntelligence-0.0.6/src/QuantumIntelligence/
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.117843 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/
--rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
--rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/__init__.py
--rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
--rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
--rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.117843 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/
--rw-rw-rw-   0        0        0    48902 2023-04-28 05:17:22.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Circuit.py
--rw-rw-rw-   0        0        0     9960 2023-04-05 10:35:49.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Gate.py
--rw-rw-rw-   0        0        0    18240 2023-04-28 05:27:11.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Simulator.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.136565 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/
--rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/MPSclass.py
--rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/TEBD.py
--rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/TNclass.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/__init__.py
--rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.111528 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/
--rw-rw-rw-   0        0        0     1763 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.126597 QuantumIntelligence-0.0.7/
+-rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1763 2023-05-05 09:43:58.125792 QuantumIntelligence-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 09:43:58.126597 QuantumIntelligence-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     8844 2023-05-05 09:42:18.000000 QuantumIntelligence-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.102859 QuantumIntelligence-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.107309 QuantumIntelligence-0.0.7/src/QuantumIntelligence/
+drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.117930 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/
+-rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
+-rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/__init__.py
+-rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
+-rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
+-rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.121977 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/
+-rw-rw-rw-   0        0        0    48914 2023-05-04 19:29:25.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Circuit.py
+-rw-rw-rw-   0        0        0     9960 2023-04-28 05:24:32.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Gate.py
+-rw-rw-rw-   0        0        0    18277 2023-05-04 19:49:53.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Simulator.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.125208 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/
+-rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/MPSclass.py
+-rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/TEBD.py
+-rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/TNclass.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.112203 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/
+-rw-rw-rw-   0        0        0     1763 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/top_level.txt
```

### Comparing `QuantumIntelligence-0.0.6/LICENSE` & `QuantumIntelligence-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/PKG-INFO` & `QuantumIntelligence-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.6
+Version: 0.0.7
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.6/README.md` & `QuantumIntelligence-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/setup.py` & `QuantumIntelligence-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     name="QuantumIntelligence",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.6",  # Required
+    version="0.0.7",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Developing quantum intelligence.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Circuit.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,15 +723,15 @@
             circuit = self
             circuit.clear()
         else:
             circuit = Circuit(self.n_qubit, self.device, self.dtype, size=self.size)
         supported_name_no_params = ['x', 'y', 'z', 'h', 'cx', 'cy', 'cz', 'ccx', 'swap']
         supported_name_specific = ['sdg', 'tdg', 's', 't']
         supported_name_with_params = ['rx', 'ry', 'rz']
-        supported_name_with_complex_params = ['u3']
+        supported_name_with_complex_params = ['u3', 'u']
         qiskit_register = qiskit_circuit.qregs[0]
         for instruction in qiskit_circuit:
             operation = instruction.operation
             qubits = instruction.qubits
             name = operation.name
             position = []
             for qq in qubits:
@@ -757,15 +757,15 @@
                     # circuit.rz_gate(position=position, theta=np.pi/4)
                 elif name == 's':
                     circuit.append(Gate.s_gate(), position=position)
                     # circuit.rz_gate(position=position, theta=np.pi/2)
                 else:
                     raise ValueError('Please report this bug to deveploper. Error occurs in supported_name_specific.')
             elif name in supported_name_with_complex_params:
-                if name == 'u3':
+                if name in ['u3', 'u']:
                     params = tuple(float(ii) for ii in operation.params)
                     circuit.append(Gate.u3(theta=params), position=position)
                 else:
                     raise ValueError('Please report this bug to deveploper. Error occurs in supported_name_specific.')
             else:
                 raise ValueError('Does not support', name)
         if not replace:
```

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Gate.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Gate.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Simulator.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,16 @@
         self.state = tc.from_numpy(result.final_state_vector).to(self.device).to(self.dtype)
         if clear_circuit:
             self.circuit.clear()
 
     def qiskit_simulate(self, clear_circuit=True):
         self.circuit.regularize_all_position()
         if 'cuda' in self.device:
-            device = 'GPU'
+            # device = 'GPU'
+            device = 'CPU'
         else:
             device = 'CPU'
         if self.dtype == tc.complex128:
             precision = 'double'
         else:
             precision = 'single'
         double_precision = (tc.complex128 == self.dtype)
@@ -259,31 +260,28 @@
             raise ValueError('error in extend, check position')
         index = int(basis, 2)
         new_position = list(range(-m_p, 0))
         tmp_state = self.state.movedim(position, new_position).reshape(-1, 2 ** m_p)
         return tmp_state[:, index]
 
     def fake_local_measure(self, position, operator):
-
-        assert position == sorted(position), 'warning!!! The position should be in descending order.'
-        index_contract = list(range(self.n_qubit))
-        for pp in position:
-            index_contract.remove(pp)
-        reduce_rho = tc.tensordot(self._state, self._state.conj(), dims=[index_contract, index_contract])
-        measure_result = tc.einsum('ab,ba->', reduce_rho, operator)
-        # print(reduce_rho)
+        reduce_rho = self.fake_local_rho(position=position)
+        measure_result = tc.einsum('ab,ba->', reduce_rho, operator.to(self.device).to(self.dtype))
         return measure_result
 
     def fake_local_rho(self, position):
-
-        assert position == sorted(position), 'warning!!! The position should be in descending order.'
+        sorted_position = sorted(position)
         index_contract = list(range(self.n_qubit))
+        permute_index0 = [sorted_position.index(ii) for ii in position]
+        permute_index1 = [ii + len(position) for ii in permute_index0]
         for pp in position:
             index_contract.remove(pp)
         reduce_rho = tc.tensordot(self._state, self._state.conj(), dims=[index_contract, index_contract])
+        reduce_rho = reduce_rho.permute(permute_index0 + permute_index1)
+        # print(permute_index0 + permute_index1)
         return reduce_rho.reshape(2**len(position), -1)
 
     def fake_measure_circuit(self, circuit:Circuit):
         if len(self.circuit) > 0:
             print('warning, there are gates that are not simulated before this fake measure. '
                   'Measured results are based on the current state')
         backup_circuit = self.circuit
@@ -365,15 +363,15 @@
 
     @property
     def state(self):
         return self._state
 
     @state.setter
     def state(self, state):
-        raise ValueError('not support')
+        self._state = state
 
     def act_single_gate(self, gate, position, control=None, fast_mode=False):
         new_state = DVD(default_value=0)
         if len(position) == 1:
             # single qubit gate
             pp = position[0]
             gmatrix = gate.tensor
@@ -402,14 +400,16 @@
         self._state = new_state
 
     def sampling(self, n_shots=1024, position=None, if_print=True, rand_seed=None, return_weight=False):
         if rand_seed is None:
             rand_seed = self.rand_seed
         if rand_seed is not None:
             random.seed(rand_seed)
+        if position is None:
+            position = list(range(self.n_qubit))
         m_p = len(position)
         population = list()
         weight = 2**m_p *[0]
         for pp in range(2 ** m_p):
             element = bin(pp)[2:]
             element = (m_p - len(element)) * '0' + element
             population.append(element)
```

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/MPSclass.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/MPSclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/TEBD.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/TEBD.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/TNclass.py` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/TNclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/PKG-INFO` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.6
+Version: 0.0.7
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/SOURCES.txt` & `QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

