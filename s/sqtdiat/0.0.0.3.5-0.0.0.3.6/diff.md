# Comparing `tmp/sqtdiat-0.0.0.3.5.tar.gz` & `tmp/sqtdiat-0.0.0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqtdiat-0.0.0.3.5.tar", last modified: Fri Feb 10 06:57:53 2023, max compression
+gzip compressed data, was "sqtdiat-0.0.0.3.6.tar", last modified: Sat Feb 11 12:12:30 2023, max compression
```

## Comparing `sqtdiat-0.0.0.3.5.tar` & `sqtdiat-0.0.0.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 06:57:53.815163 sqtdiat-0.0.0.3.5/
--rw-rw-rw-   0        0        0     1072 2023-02-09 10:17:11.000000 sqtdiat-0.0.0.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0      576 2023-02-10 06:57:53.815163 sqtdiat-0.0.0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       91 2023-02-09 11:55:44.000000 sqtdiat-0.0.0.3.5/README.md
--rw-rw-rw-   0        0        0       86 2023-02-09 07:26:18.000000 sqtdiat-0.0.0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0      617 2023-02-10 06:57:53.815163 sqtdiat-0.0.0.3.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-10 06:57:53.751558 sqtdiat-0.0.0.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-02-10 06:57:53.751558 sqtdiat-0.0.0.3.5/src/sqtdiat/
--rw-rw-rw-   0        0        0        0 2023-02-09 09:34:26.000000 sqtdiat-0.0.0.3.5/src/sqtdiat/__init__.py
--rw-rw-rw-   0        0        0     8673 2023-02-10 06:55:51.000000 sqtdiat-0.0.0.3.5/src/sqtdiat/qops.py
-drwxrwxrwx   0        0        0        0 2023-02-10 06:57:53.815163 sqtdiat-0.0.0.3.5/src/sqtdiat.egg-info/
--rw-rw-rw-   0        0        0      576 2023-02-10 06:57:53.000000 sqtdiat-0.0.0.3.5/src/sqtdiat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-02-10 06:57:53.000000 sqtdiat-0.0.0.3.5/src/sqtdiat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 06:57:53.000000 sqtdiat-0.0.0.3.5/src/sqtdiat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-10 06:57:53.000000 sqtdiat-0.0.0.3.5/src/sqtdiat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-11 12:12:30.186058 sqtdiat-0.0.0.3.6/
+-rw-rw-rw-   0        0        0     1072 2023-02-09 10:17:11.000000 sqtdiat-0.0.0.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      576 2023-02-11 12:12:30.187058 sqtdiat-0.0.0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2023-02-09 11:55:44.000000 sqtdiat-0.0.0.3.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-02-09 07:26:18.000000 sqtdiat-0.0.0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0      617 2023-02-11 12:12:30.187058 sqtdiat-0.0.0.3.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-02-11 12:12:30.110266 sqtdiat-0.0.0.3.6/src/
+drwxrwxrwx   0        0        0        0 2023-02-11 12:12:30.146585 sqtdiat-0.0.0.3.6/src/sqtdiat/
+-rw-rw-rw-   0        0        0        0 2023-02-09 09:34:26.000000 sqtdiat-0.0.0.3.6/src/sqtdiat/__init__.py
+-rw-rw-rw-   0        0        0    11377 2023-02-11 12:11:28.000000 sqtdiat-0.0.0.3.6/src/sqtdiat/qops.py
+drwxrwxrwx   0        0        0        0 2023-02-11 12:12:30.186058 sqtdiat-0.0.0.3.6/src/sqtdiat.egg-info/
+-rw-rw-rw-   0        0        0      576 2023-02-11 12:12:30.000000 sqtdiat-0.0.0.3.6/src/sqtdiat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-02-11 12:12:30.000000 sqtdiat-0.0.0.3.6/src/sqtdiat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-11 12:12:30.000000 sqtdiat-0.0.0.3.6/src/sqtdiat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-02-11 12:12:30.000000 sqtdiat-0.0.0.3.6/src/sqtdiat.egg-info/top_level.txt
```

### Comparing `sqtdiat-0.0.0.3.5/LICENSE.txt` & `sqtdiat-0.0.0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqtdiat-0.0.0.3.5/PKG-INFO` & `sqtdiat-0.0.0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqtdiat
-Version: 0.0.0.3.5
+Version: 0.0.0.3.6
 Summary: Contains the code to perform certain mathematical operations involved in quantum computing.
 Author: Umesh, Ashish, Pavan, Aparajith
 Author-email: p.b.ashish786@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `sqtdiat-0.0.0.3.5/setup.cfg` & `sqtdiat-0.0.0.3.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7174 6469 6174 0d0a 7665 7273   = sqtdiat..vers
-00000020: 696f 6e20 3d20 302e 302e 302e 332e 350d  ion = 0.0.0.3.5.
+00000020: 696f 6e20 3d20 302e 302e 302e 332e 360d  ion = 0.0.0.3.6.
 00000030: 0a61 7574 686f 7220 3d20 556d 6573 682c  .author = Umesh,
 00000040: 2041 7368 6973 682c 2050 6176 616e 2c20   Ashish, Pavan, 
 00000050: 4170 6172 616a 6974 680d 0a61 7574 686f  Aparajith..autho
 00000060: 725f 656d 6169 6c20 3d20 702e 622e 6173  r_email = p.b.as
 00000070: 6869 7368 3738 3640 676d 6169 6c2e 636f  hish786@gmail.co
 00000080: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000090: 2043 6f6e 7461 696e 7320 7468 6520 636f   Contains the co
```

### Comparing `sqtdiat-0.0.0.3.5/src/sqtdiat/qops.py` & `sqtdiat-0.0.0.3.6/src/sqtdiat/qops.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,27 @@
     if type(state_vec) != np.array:
         state_vec = np.array(state_vec)
     norm_fact = 0
     for x in state_vec:
         norm_fact += x * np.conj(x)
     return 1 / np.sqrt(np.real(norm_fact)) * state_vec
 
+def gram_schmidt(basis_set):
+    if type(basis_set) != np.array:
+        basis_set = np.array(basis_set)
+    u = np.ones(basis_set.shape)
+    u[0] = basis_set[0]
+    for i in range(0, basis_set.shape[0]):
+        subt = np.zeros(basis_set.shape[1])
+        for j in range(0, i):
+            subt = subt + proj(basis_set[i], u[j])
+        u[i] = basis_set[i] - subt
+        u[i] = u[i] / np.sqrt(np.dot(u[i], np.conj(u[i])))
+    return u
+
 def trace(sqr_mat):
     """Returns the trace of a given square matrix"""
     if type(sqr_mat) != np.array:
         sqr_mat = np.array(sqr_mat)
     if sqr_mat.shape[0] == sqr_mat.shape[1]:
         return np.sum([sqr_mat[i][i] for i in range(sqr_mat.shape[0])])
     else:
@@ -88,14 +101,15 @@
         else: 
             return lin_en
 
 def partial_transpose(dens_mat, qubit, n):
     """Returns a partially transposed density matrix with the partial transpose performed in the nth qubit.
         Requires : dens_mat = a valid density matrix
                    qubit = integer, the position of the qubit to be flipped.
+                   n = dimension of the density matrix either row or column
 
     """
     if nxn_valid_quantum(dens_mat):
         n = int(np.log2(dens_mat.shape[0]))
         all_binary = generate_bin(n)
         all_binary_2 = generate_bin(n)
         part_qubit = n - qubit - 1
@@ -193,8 +207,67 @@
     # Stokes = Stokes.reshape(16, 1) 
     b = np.zeros((4, 4))
     for i in range(4):
         for j in range(4):
             b = b + Stokes[4 * i + j] * np.kron(s[i], s[j])
             # print(Stokes[4 * i + j], i, j)
     b = b / 4
-    return np.round(np.real(b), 3)
+    return np.round(np.real(b), 3)
+
+def ppt(dens_mat, qubit):
+    if type(dens_mat) != np.array:
+        dens_mat = np.array(dens_mat) 
+    n = dens_mat.shape[0]
+    new_mat = partial_transpose(dens_mat, qubit, n)
+    eig_vals_dm = np.linalg.eigvals(new_mat)
+    for x in np.round(eig_vals_dm, 4):
+        if x < 1e-4:
+            return True
+    return False
+
+def ideal_one_q_tomography(N_H, N_V, N_D, N_R):
+    N_t = N_H + N_V
+    P_H = N_H / N_t
+    P_V = N_V / N_t
+    P_D = N_D / N_t
+    P_R = N_R / N_t
+    return np.array([[2 * P_H, (2 * P_D - 1) - 1j * (1 - 2 * P_R)], [(2 * P_D - 1) + 1j * (1 - 2 * P_R), 2 * P_V]]) * 0.5
+
+def sqrt_dens_mat(dens_mat):
+    # if nxn_valid_quantum(dens_mat):
+    eig_vals, eig_vecs = np.linalg.eig(dens_mat)
+    eig_vals = np.real(eig_vals)
+    iden = np.eye(len(eig_vals))
+    for i in range(len(eig_vals)):
+        if np.abs(eig_vals[i]) < 10e-4:
+            val = 0
+        else:
+            val = np.sqrt(eig_vals[i])
+        iden[i] = val * iden[i]
+    print(iden)
+    return eig_vecs.T @ iden @ np.linalg.inv(eig_vecs.T)
+
+def fidelity(rho1, rho2):
+    if type(rho1) != np.array:
+        rho1 = np.array(rho1)
+    if type(rho2) != np.array:
+        rho2 = np.array(rho1)
+    if rho1.shape == rho2.shape:
+        if nxn_valid_quantum(rho1) and nxn_valid_quantum(rho2):
+            sqrt_rho1 = sqrt_dens_mat(rho1)
+            val = sqrt_rho1 @ rho2 @ sqrt_rho1
+            if np.imag(trace(val)) < 10e-4:
+                return np.round(np.real((trace(sqrt_dens_mat(val)))**2), 4)
+    else:
+        raise ValueError(f"Given density matrices are not of same dimension {rho1.shape}, {rho2.shape}")
+
+def stokes_two_qubit(dens_mat):
+    if nxn_valid_quantum(dens_mat):
+        if type(dens_mat) != np.array:
+            dens_mat = np.array(dens_mat)
+        pauli = [np.array([[1, 0], [0, 1]]), np.array([[0, 1], [1, 0]]), np.array([[0, -1j], [1j, 0]]), np.array([[1, 0], [0, -1]])]
+        stokes_vec = []
+        for x in pauli:
+            for y in pauli:
+                stokes_vec.append(np.round(np.real(trace(np.kron(x, y) @ dens_mat)), 5))
+                # print(np.kron(x, y))
+        return stokes_vec
```

### Comparing `sqtdiat-0.0.0.3.5/src/sqtdiat.egg-info/PKG-INFO` & `sqtdiat-0.0.0.3.6/src/sqtdiat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqtdiat
-Version: 0.0.0.3.5
+Version: 0.0.0.3.6
 Summary: Contains the code to perform certain mathematical operations involved in quantum computing.
 Author: Umesh, Ashish, Pavan, Aparajith
 Author-email: p.b.ashish786@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

