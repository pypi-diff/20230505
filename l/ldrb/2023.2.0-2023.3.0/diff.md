# Comparing `tmp/ldrb-2023.2.0.tar.gz` & `tmp/ldrb-2023.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldrb-2023.2.0.tar", last modified: Fri Mar 31 13:16:10 2023, max compression
+gzip compressed data, was "ldrb-2023.3.0.tar", last modified: Fri May  5 09:46:34 2023, max compression
```

## Comparing `ldrb-2023.2.0.tar` & `ldrb-2023.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-03-31 13:16:10.794079 ldrb-2023.2.0/
--rw-r--r--   0 finsberg   (501) staff       (20)     7652 2022-06-04 16:58:47.000000 ldrb-2023.2.0/LICENSE
--rw-r--r--   0 finsberg   (501) staff       (20)     3651 2023-03-31 13:16:10.794157 ldrb-2023.2.0/PKG-INFO
--rw-r--r--   0 finsberg   (501) staff       (20)     3005 2023-01-27 11:15:56.000000 ldrb-2023.2.0/README.md
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-03-31 13:16:10.792208 ldrb-2023.2.0/ldrb/
--rw-r--r--   0 finsberg   (501) staff       (20)      562 2023-03-28 08:03:45.000000 ldrb-2023.2.0/ldrb/__init__.py
--rw-r--r--   0 finsberg   (501) staff       (20)    12667 2023-03-28 08:03:25.000000 ldrb-2023.2.0/ldrb/calculus.py
--rw-r--r--   0 finsberg   (501) staff       (20)    24592 2023-03-28 08:03:25.000000 ldrb-2023.2.0/ldrb/ldrb.py
--rw-r--r--   0 finsberg   (501) staff       (20)     9552 2023-02-27 13:17:56.000000 ldrb-2023.2.0/ldrb/save.py
--rw-r--r--   0 finsberg   (501) staff       (20)     8660 2023-03-28 08:03:25.000000 ldrb-2023.2.0/ldrb/utils.py
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-03-31 13:16:10.793580 ldrb-2023.2.0/ldrb.egg-info/
--rw-r--r--   0 finsberg   (501) staff       (20)     3651 2023-03-31 13:16:10.000000 ldrb-2023.2.0/ldrb.egg-info/PKG-INFO
--rw-r--r--   0 finsberg   (501) staff       (20)      314 2023-03-31 13:16:10.000000 ldrb-2023.2.0/ldrb.egg-info/SOURCES.txt
--rw-r--r--   0 finsberg   (501) staff       (20)        1 2023-03-31 13:16:10.000000 ldrb-2023.2.0/ldrb.egg-info/dependency_links.txt
--rw-r--r--   0 finsberg   (501) staff       (20)        1 2022-11-16 10:23:38.000000 ldrb-2023.2.0/ldrb.egg-info/not-zip-safe
--rw-r--r--   0 finsberg   (501) staff       (20)      237 2023-03-31 13:16:10.000000 ldrb-2023.2.0/ldrb.egg-info/requires.txt
--rw-r--r--   0 finsberg   (501) staff       (20)        5 2023-03-31 13:16:10.000000 ldrb-2023.2.0/ldrb.egg-info/top_level.txt
--rw-r--r--   0 finsberg   (501) staff       (20)     1397 2023-03-31 13:16:10.794556 ldrb-2023.2.0/setup.cfg
--rw-r--r--   0 finsberg   (501) staff       (20)      109 2023-03-28 08:03:45.000000 ldrb-2023.2.0/setup.py
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-03-31 13:16:10.793923 ldrb-2023.2.0/tests/
--rw-r--r--   0 finsberg   (501) staff       (20)     6614 2023-03-28 08:03:25.000000 ldrb-2023.2.0/tests/test_ldrb.py
--rw-r--r--   0 finsberg   (501) staff       (20)     1680 2023-02-27 13:17:56.000000 ldrb-2023.2.0/tests/test_save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:46:34.698913 ldrb-2023.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-05 09:46:20.000000 ldrb-2023.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 09:46:34.698913 ldrb-2023.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-05 09:46:20.000000 ldrb-2023.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:46:34.698913 ldrb-2023.3.0/ldrb/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24675 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/ldrb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:46:34.698913 ldrb-2023.3.0/ldrb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-05 09:46:34.702913 ldrb-2023.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 09:46:20.000000 ldrb-2023.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:46:34.698913 ldrb-2023.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-05 09:46:20.000000 ldrb-2023.3.0/tests/test_ldrb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-05 09:46:20.000000 ldrb-2023.3.0/tests/test_save.py
```

### Comparing `ldrb-2023.2.0/LICENSE` & `ldrb-2023.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ldrb-2023.2.0/PKG-INFO` & `ldrb-2023.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldrb
-Version: 2023.2.0
+Version: 2023.3.0
 Summary: Laplace-Dirichlet Rule-based algorithm for assigning myocardial fiber orientations.
 Home-page: https://github.com/finsberg/ldrb
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: LGPL-3.0
 Keywords: cardiac modeling,fiber orientations
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `ldrb-2023.2.0/README.md` & `ldrb-2023.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ldrb-2023.2.0/ldrb/__init__.py` & `ldrb-2023.3.0/ldrb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .ldrb import dolfin_ldrb
 from .ldrb import project_gradients
 from .ldrb import scalar_laplacians
 from .save import fiber_to_xdmf
 from .save import fun_to_xdmf
 from .utils import space_from_string
 
-__version__ = "2023.2.0"
+__version__ = "2023.3.0"
 __author__ = "Henrik Finsberg (henriknf@simula.no)"
 
 __all__ = [
     "save",
     "fun_to_xdmf",
     "fiber_to_xdmf",
     "ldrb",
```

### Comparing `ldrb-2023.2.0/ldrb/calculus.py` & `ldrb-2023.3.0/ldrb/calculus.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,48 +2,32 @@
 import numpy as np
 
 
 _float_1D_array = numba.types.Array(numba.float64, 1, "C")
 _float_2D_array = numba.types.Array(numba.float64, 2, "C")
 
 
-@numba.njit(numba.float64(_float_1D_array, _float_1D_array))
-def quat_dot(q1: np.ndarray, q2: np.ndarray) -> float:
-    """Quaternion dot product
-
-    Parameters
-    ----------
-    q1 : np.ndarray
-        First quaternion
-    q2 : np.ndarray
-        Second quaternion
-
-    Returns
-    -------
-    float
-        The quaternion dot product
-    """
-    return q1[0] * q2[0] + q1[1] * q2[1] + q1[2] * q2[2] + q1[3] * q2[3]
-
-
 @numba.njit(_float_1D_array(_float_1D_array))
 def normalize(u: np.ndarray) -> np.ndarray:
     """L2-Normalize vector with
 
     Parameters
     ----------
     u : np.ndarray
         Vector
 
     Returns
     -------
     np.ndarray
         Normalized vector
     """
-    return u / np.linalg.norm(u)
+    u_norm = np.linalg.norm(u)
+    if u_norm > 0.0:
+        return u / u_norm
+    return u
 
 
 @numba.njit(_float_1D_array(_float_1D_array, _float_1D_array, numba.float64))
 def slerp(q1: np.ndarray, q2: np.ndarray, t: float) -> np.ndarray:
     """Spherical linear interpolation from `q1` to `q2` at `t`
 
     Parameters
@@ -56,83 +40,68 @@
         Interpolation factor, between 0 and 1
 
     Returns
     -------
     np.ndarray
         The spherical linear interpolation between `q1` and `q2` at `t`
     """
-    dot = quat_dot(q1, q2)
-    if dot > 1 - 1e-12:
+    dot = q1.dot(q2)
+    q3 = q2
+    if dot < 0.0:
+        dot = -dot
+        q3 = -q2
+
+    if dot < 0.9999:
         angle = np.arccos(dot)
         a = np.sin(angle * (1 - t)) / np.sin(angle)
         b = np.sin(angle * t) / np.sin(angle)
+        return a * q1 + b * q3
 
-        q = q2
-        q *= b
-        q1a = q1
-        q1a *= a
-        q += q1a
-    else:
-        q = q1
-        q *= 1 - t
-        q2t = q2
-        q2t *= t
-        q += q2t
-    return q
+    # Angle is close to zero - do linear interpolation
+    return q1 * (1 - t) + q3 * t
 
 
 @numba.njit(_float_1D_array(_float_2D_array))
 def rot2quat(Q: np.ndarray) -> np.ndarray:
-    """Convert rotation matrix to quaternion
+    t = Q[0][0] + Q[1][1] + Q[2][2]
 
-    Parameters
-    ----------
-    Q : np.ndarray
-        Rotation matrix
+    if t > 0:
+        r = np.sqrt(1.0 + t)
+        s = 0.5 / r
+
+        a = 0.5 * r
+        b = (Q[2][1] - Q[1][2]) * s
+        c = (Q[0][2] - Q[2][0]) * s
+        d = (Q[1][0] - Q[0][1]) * s
+
+    elif Q[0][0] > Q[1][1] and Q[0][0] > Q[2][2]:
+        s = 2 * np.sqrt(1.0 + Q[0][0] - Q[1][1] - Q[2][2])
+
+        a = (Q[2][1] - Q[1][2]) / s
+        b = 0.25 * s
+        c = (Q[0][1] + Q[1][0]) / s
+        d = (Q[0][2] + Q[2][0]) / s
+
+    elif Q[1][1] > Q[0][0] and Q[1][1] > Q[2][2]:
+        s = 2 * np.sqrt(1.0 + Q[1][1] - Q[0][0] - Q[2][2])
+
+        a = (Q[0][2] - Q[2][0]) / s
+        b = (Q[0][1] + Q[1][0]) / s
+        c = 0.25 * s
+        d = (Q[1][2] + Q[2][1]) / s
 
-    Returns
-    -------
-    np.ndarray
-        Quaternion
-    """
-    M11 = Q[0][0]
-    M12 = Q[1][0]
-    M13 = Q[2][0]
-    M21 = Q[0][1]
-    M22 = Q[1][1]
-    M23 = Q[2][1]
-    M31 = Q[0][2]
-    M32 = Q[1][2]
-    M33 = Q[2][2]
-
-    w2 = 0.25 * (1 + M11 + M22 + M33)
-    err = 1e-15
-
-    if w2 > err:
-        w = np.sqrt(w2)
-        x = (M23 - M32) / (4.0 * w)
-        y = (M31 - M13) / (4.0 * w)
-        z = (M12 - M21) / (4.0 * w)
     else:
-        w = 0.0
-        x2 = -0.5 * (M22 + M33)
-        if x2 > err:
-            x = np.sqrt(x2)
-            y = M12 / (2.0 * x)
-            z = M13 / (2.0 * x)
-        else:
-            x = 0.0
-            y2 = 0.5 * (1 - M33)
-            if y2 > err:
-                y = np.sqrt(y2)
-                z = M23 / (2.0 * y)
-            else:
-                y = 0.0
-                z = 1.0
-    return normalize(np.array([w, x, y, z]))
+        s = 2 * np.sqrt(1.0 + Q[2][2] - Q[0][0] - Q[1][1])
+
+        a = (Q[1][0] - Q[0][1]) / s
+        b = (Q[0][2] + Q[2][0]) / s
+        c = (Q[1][2] + Q[2][1]) / s
+        d = 0.25 * s
+
+    return normalize(np.array([a, b, c, d]))
 
 
 @numba.njit(_float_2D_array(_float_1D_array))
 def quat2rot(q: np.ndarray) -> np.ndarray:
     """Convert quaternion to rotation matrix
 
     Parameters
@@ -187,68 +156,69 @@
     Linear interpolation of two orthogonal matrices.
     Assume that :math:`Q_a` and :math:`Q_b` refers to
     timepoint :math:`0` and :math:`1` respectively.
     Using spherical linear interpolation (slerp) find the
     orthogonal matrix at timepoint :math:`t`.
     """
 
-    if ~Qa.any() and ~Qb.any():
-        return np.zeros((3, 3))
-    if ~Qa.any():
-        return Qb
-    if ~Qb.any():
-        return Qa
+    # if ~Qa.any() and ~Qb.any():
+    #     return np.zeros((3, 3))
+    # if ~Qa.any():
+    #     return Qb
+    # if ~Qb.any():
+    #     return Qa
+
+    # tol = 1e-5
+
+    # if t < tol:
+    #     return Qa
+    # if t > 1 - tol:
+    #     return Qb
 
-    tol = 1e-12
-    qa = rot2quat(Qb)
+    qa = rot2quat(Qa)
     qb = rot2quat(Qb)
 
-    quat_i = np.array([0, 1, 0, 0])
-    quat_j = np.array([0, 0, 1, 0])
-    quat_k = np.array([0, 0, 0, 1])
+    a = qa[0]
+    b = qa[1]
+    c = qa[2]
+    d = qa[3]
+
+    # i_qa = np.array([-b, a, -d, c])
+    # j_qa = np.array([-c, d, a, -b])
+    # k_qa = np.array([-d, -c, b, a])
+
+    qa_i = np.array([-b, a, d, -c])
+    qa_j = np.array([-c, -d, a, b])
+    qa_k = np.array([-d, c, -b, a])
+
+    # quat_array = [
+    #     qa,
+    #     i_qa,
+    #     j_qa,
+    #     k_qa,
+    # ]
 
     quat_array = [
         qa,
-        -qa,
-        quat_i * qa,
-        -quat_i * qa,
-        quat_j * qa,
-        -quat_j * qa,
-        quat_k * qa,
-        -quat_k * qa,
+        qa_i,
+        qa_j,
+        qa_k,
     ]
 
-    max_idx = 0
-    max_dot = 0.0
+    qm = quat_array[0]
+    max_dot = abs(qm.dot(qb))
 
-    idx = 0
-    for qm in [
-        qa,
-        -qa,
-        quat_i * qa,
-        -quat_i * qa,
-        quat_j * qa,
-        -quat_j * qa,
-        quat_k * qa,
-        -quat_k * qa,
-    ]:
-        dot = quat_dot(qm, qb)
+    for v in quat_array[1:]:
+        dot = abs(v.dot(qb))
         if dot > max_dot:
             max_dot = dot
-            max_idx = idx
-        idx += 1
+            qm = v
 
-    if max_dot > 1 - tol:
-        return Qb
-
-    qm = quat_array[max_idx]
     qm_slerp = slerp(qm, qb, t)
-    qm_norm = normalize(qm_slerp)
-
-    return quat2rot(qm_norm)
+    return quat2rot(qm_slerp)
 
 
 @numba.njit(_float_2D_array(_float_1D_array, _float_1D_array))
 def axis(u: np.ndarray, v: np.ndarray) -> np.ndarray:
     r"""
     Construct the fiber orientation coordinate system.
 
@@ -256,17 +226,15 @@
     and transmural direction respectively return a matrix that
     represents an orthonormal basis in the circumferential (first),
     apicobasal (second) and transmural (third) direction.
     """
 
     e1 = normalize(u)
 
-    # Create an initial guess for e0
-    e2 = normalize(v)
-    e2 -= e1.dot(e2) * e1
+    e2 = v - (e1.dot(v)) * e1
     e2 = normalize(e2)
 
     e0 = np.cross(e1, e2)
     e0 = normalize(e0)
 
     Q = np.zeros((3, 3))
     Q[:, 0] = e0
@@ -296,109 +264,14 @@
     B[1, :] = [0, np.cos(np.radians(beta)), np.sin(np.radians(beta))]
     B[2, :] = [0, -np.sin(np.radians(beta)), np.cos(np.radians(beta))]
 
     C = np.dot(Q.real, A).dot(B)
     return C
 
 
-@numba.njit(
-    _float_2D_array(
-        numba.float64,
-        numba.float64,
-        numba.float64,
-        _float_1D_array,
-        _float_1D_array,
-        _float_1D_array,
-        _float_1D_array,
-        numba.float64,
-        numba.float64,
-        numba.float64,
-        numba.float64,
-        numba.float64,
-    ),
-)
-def system_at_dof(
-    lv: float,
-    rv: float,
-    epi: float,
-    grad_lv: np.ndarray,
-    grad_rv: np.ndarray,
-    grad_epi: np.ndarray,
-    grad_ab: np.ndarray,
-    alpha_endo: float,
-    alpha_epi: float,
-    beta_endo: float,
-    beta_epi: float,
-    tol: float = 1e-7,
-) -> np.ndarray:
-    """
-    Compte the fiber, sheet and sheet normal at a
-    single degree of freedom
-
-    Arguments
-    ---------
-    lv : float
-        Value of the Laplace solution for the LV at the dof.
-    rv : float
-        Value of the Laplace solution for the RV at the dof.
-    epi : float
-        Value of the Laplace solution for the EPI at the dof.
-    grad_lv : np.ndarray
-        Gradient of the Laplace solution for the LV at the dof.
-    grad_rv : np.ndarray
-        Gradient of the Laplace solution for the RV at the dof.
-    grad_epi : np.ndarray
-        Gradient of the Laplace solution for the EPI at the dof.
-    grad_epi : np.ndarray
-        Gradient of the Laplace solution for the apex to base.
-        at the dof
-    alpha_endo : scalar
-        Fiber angle at the endocardium.
-    alpha_epi : scalar
-        Fiber angle at the epicardium.
-    beta_endo : scalar
-        Sheet angle at the endocardium.
-    beta_epi : scalar
-        Sheet angle at the epicardium.
-    tol : scalar
-        Tolerance for whether to consider the scalar values.
-        Default: 1e-7
-    """
-
-    if lv + rv < tol:
-        depth = 0.5
-    else:
-        depth = rv / (lv + rv)
-
-    alpha_s = alpha_endo * (1 - depth) - alpha_endo * depth
-    alpha_w = alpha_endo * (1 - epi) + alpha_epi * epi
-    beta_s = beta_endo * (1 - depth) - beta_endo * depth
-    beta_w = beta_endo * (1 - epi) + beta_epi * epi
-
-    Q_lv = np.zeros((3, 3))
-    if lv > tol:
-        Q_lv = axis(grad_ab, -1 * grad_lv)
-        Q_lv = orient(Q_lv, alpha_s, beta_s)
-
-    Q_rv = np.zeros((3, 3))
-    if rv > tol:
-        Q_rv = axis(grad_ab, grad_rv)
-        Q_rv = orient(Q_rv, alpha_s, beta_s)
-
-    Q_endo = bislerp(Q_lv, Q_rv, depth)
-
-    Q_epi = np.zeros((3, 3))
-    if epi > tol:
-        Q_epi = axis(grad_ab, grad_epi)
-        Q_epi = orient(Q_epi, alpha_w, beta_w)
-
-    Q_fiber = bislerp(Q_endo, Q_epi, epi)
-    return Q_fiber
-
-
 @numba.njit
 def compute_fiber_sheet_system(
     f0,
     s0,
     n0,
     xdofs,
     ydofs,
@@ -421,15 +294,14 @@
     alpha_epi_sept,
     beta_endo_lv,
     beta_epi_lv,
     beta_endo_rv,
     beta_epi_rv,
     beta_endo_sept,
     beta_epi_sept,
-    tol,
 ):
     grad_lv = np.zeros(3)
     grad_rv = np.zeros(3)
     grad_epi = np.zeros(3)
     grad_ab = np.zeros(3)
 
     for i in range(len(xdofs)):
@@ -451,14 +323,15 @@
         grad_epi[2] = epi_gradient[zdofs[i]]
 
         grad_ab[0] = apex_gradient[xdofs[i]]
         grad_ab[1] = apex_gradient[ydofs[i]]
         grad_ab[2] = apex_gradient[zdofs[i]]
 
         if epi > 0.5:
+            # We are not in the septum
             if lv_rv >= 0.5:
                 # We are in the LV region
                 marker_scalar[sdofs[i]] = 1
                 alpha_endo = alpha_endo_lv
                 beta_endo = beta_endo_lv
                 alpha_epi = alpha_epi_lv
                 beta_epi = beta_epi_lv
@@ -466,50 +339,57 @@
                 # We are in the RV region
                 marker_scalar[sdofs[i]] = 2
                 alpha_endo = alpha_endo_rv
                 beta_endo = beta_endo_rv
                 alpha_epi = alpha_epi_rv
                 beta_epi = beta_epi_rv
         else:
-            if lv_rv >= 1 - tol:
+            if lv_rv >= 0.9:
                 # We are in the LV region
                 marker_scalar[sdofs[i]] = 1
                 alpha_endo = alpha_endo_lv
                 beta_endo = beta_endo_lv
                 alpha_epi = alpha_epi_lv
                 beta_epi = beta_epi_lv
-            elif lv_rv <= tol:
+            elif lv_rv <= 0.1:
                 # We are in the RV region
                 marker_scalar[sdofs[i]] = 2
                 alpha_endo = alpha_endo_rv
                 beta_endo = beta_endo_rv
                 alpha_epi = alpha_epi_rv
                 beta_epi = beta_epi_rv
             else:
                 # We are in the septum
                 marker_scalar[sdofs[i]] = 3
                 alpha_endo = alpha_endo_sept
                 beta_endo = beta_endo_sept
                 alpha_epi = alpha_epi_sept
                 beta_epi = beta_epi_sept
 
-        Q_fiber = system_at_dof(
-            lv=lv,
-            rv=rv,
-            epi=epi,
-            grad_lv=grad_lv,
-            grad_rv=grad_rv,
-            grad_epi=grad_epi,
-            grad_ab=grad_ab,
-            alpha_endo=alpha_endo,
-            alpha_epi=alpha_epi,
-            beta_endo=beta_endo,
-            beta_epi=beta_epi,
-            tol=tol,
-        )
+        if lv + rv < 1e-12:
+            depth = 0.5
+        else:
+            depth = rv / (lv + rv)
+
+        alpha_s = alpha_endo * (1 - depth) - alpha_endo * depth
+        alpha_w = alpha_endo * (1 - epi) + alpha_epi * epi
+        beta_s = beta_endo * (1 - depth) - beta_endo * depth
+        beta_w = beta_endo * (1 - epi) + beta_epi * epi
+
+        Q_lv = axis(grad_ab, -grad_lv)
+        Q_lv = orient(Q_lv, alpha_s, beta_s)
+
+        Q_rv = axis(grad_ab, grad_rv)
+        Q_rv = orient(Q_rv, alpha_s, beta_s)
+
+        Q_epi = axis(grad_ab, grad_epi)
+        Q_epi = orient(Q_epi, alpha_w, beta_w)
+
+        Q_endo = bislerp(Q_lv, Q_rv, depth)
+        Q_fiber = bislerp(Q_endo, Q_epi, epi)
 
         f0[xdofs[i]] = Q_fiber[0, 0]
         f0[ydofs[i]] = Q_fiber[1, 0]
         f0[zdofs[i]] = Q_fiber[2, 0]
 
         s0[xdofs[i]] = Q_fiber[0, 1]
         s0[ydofs[i]] = Q_fiber[1, 1]
```

### Comparing `ldrb-2023.2.0/ldrb/ldrb.py` & `ldrb-2023.3.0/ldrb/ldrb.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,14 @@
 
     f0 = np.zeros_like(lv_gradient)
     s0 = np.zeros_like(lv_gradient)
     n0 = np.zeros_like(lv_gradient)
     if marker_scalar is None:
         marker_scalar = np.zeros_like(lv_scalar)
 
-    tol = 0.1
-
     from .calculus import compute_fiber_sheet_system as _compute_fiber_sheet_system
 
     _compute_fiber_sheet_system(
         f0,
         s0,
         n0,
         dofs[:, 0],
@@ -189,15 +187,14 @@
         alpha_epi_sept,
         beta_endo_lv,
         beta_epi_lv,
         beta_endo_rv,
         beta_epi_rv,
         beta_endo_sept,
         beta_epi_sept,
-        tol,
     )
 
     return FiberSheetSystem(fiber=f0, sheet=s0, sheet_normal=n0)
 
 
 def dofs_from_function_space(mesh: df.Mesh, fiber_space: str) -> np.ndarray:
     """
@@ -533,14 +530,17 @@
             gradient_cg = df.Function(V_cg)
             projector(gradient_cg, df.grad(scalar_solution))
             gradient = df.interpolate(gradient_cg, Vv)
 
             # Add gradient data
             data[case + "_gradient"] = gradient.vector().get_local()
 
+            df.File(f"{case}.pvd") << scalar_solution_int
+            df.File(f"{case}_grad.pvd") << gradient
+
         # Add scalar data
         if case != "apex":
             data[case + "_scalar"] = scalar_solution_int.vector().get_local()
 
     # Return data
     return data
```

### Comparing `ldrb-2023.2.0/ldrb/save.py` & `ldrb-2023.3.0/ldrb/save.py`

 * *Files identical despite different names*

### Comparing `ldrb-2023.2.0/ldrb/utils.py` & `ldrb-2023.3.0/ldrb/utils.py`

 * *Files identical despite different names*

### Comparing `ldrb-2023.2.0/ldrb.egg-info/PKG-INFO` & `ldrb-2023.3.0/ldrb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldrb
-Version: 2023.2.0
+Version: 2023.3.0
 Summary: Laplace-Dirichlet Rule-based algorithm for assigning myocardial fiber orientations.
 Home-page: https://github.com/finsberg/ldrb
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: LGPL-3.0
 Keywords: cardiac modeling,fiber orientations
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `ldrb-2023.2.0/setup.cfg` & `ldrb-2023.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ldrb-2023.2.0/tests/test_save.py` & `ldrb-2023.3.0/tests/test_save.py`

 * *Files identical despite different names*

