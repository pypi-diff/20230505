# Comparing `tmp/kiwigrad-0.27.tar.gz` & `tmp/kiwigrad-0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.27.tar", last modified: Thu May  4 22:36:50 2023, max compression
+gzip compressed data, was "kiwigrad-0.28.tar", last modified: Fri May  5 13:28:27 2023, max compression
```

## Comparing `kiwigrad-0.27.tar` & `kiwigrad-0.28.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-04 22:36:50.938040 kiwigrad-0.27/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.27/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3223 2023-05-04 22:36:50.937201 kiwigrad-0.27/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2747 2023-05-01 22:05:50.000000 kiwigrad-0.27/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-04 22:36:50.928303 kiwigrad-0.27/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      297 2023-05-04 22:27:05.000000 kiwigrad-0.27/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11030 2023-05-04 22:29:02.000000 kiwigrad-0.27/kiwigrad/engine.c
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.27/kiwigrad/engine.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      968 2023-05-01 12:29:46.000000 kiwigrad-0.27/kiwigrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.27/kiwigrad/layers.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.27/kiwigrad/neurons.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.27/kiwigrad/nn.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.27/kiwigrad/skeleton.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-04 22:36:50.934769 kiwigrad-0.27/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3223 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      355 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-04 22:36:50.938305 kiwigrad-0.27/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      997 2023-05-04 22:27:00.000000 kiwigrad-0.27/setup.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-04 22:36:50.936324 kiwigrad-0.27/test/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1075 2023-05-01 10:14:41.000000 kiwigrad-0.27/test/test_value.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-05 13:28:27.769001 kiwigrad-0.28/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.28/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3209 2023-05-05 13:28:27.768567 kiwigrad-0.28/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2733 2023-05-05 13:24:24.000000 kiwigrad-0.28/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-05 13:28:27.762970 kiwigrad-0.28/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      297 2023-05-05 13:20:50.000000 kiwigrad-0.28/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11668 2023-05-05 13:18:44.000000 kiwigrad-0.28/kiwigrad/engine.c
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.28/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      968 2023-05-01 12:29:46.000000 kiwigrad-0.28/kiwigrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.28/kiwigrad/layers.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.28/kiwigrad/neurons.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1521 2023-05-05 13:21:19.000000 kiwigrad-0.28/kiwigrad/nn.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.28/kiwigrad/skeleton.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-05 13:28:27.766176 kiwigrad-0.28/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3209 2023-05-05 13:28:27.000000 kiwigrad-0.28/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      355 2023-05-05 13:28:27.000000 kiwigrad-0.28/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-05 13:28:27.000000 kiwigrad-0.28/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-05 13:28:27.000000 kiwigrad-0.28/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-05 13:28:27.000000 kiwigrad-0.28/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-05 13:28:27.769163 kiwigrad-0.28/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      997 2023-05-05 13:20:45.000000 kiwigrad-0.28/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-05 13:28:27.767194 kiwigrad-0.28/test/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1120 2023-05-04 22:47:44.000000 kiwigrad-0.28/test/test_value.py
```

### Comparing `kiwigrad-0.27/LICENSE` & `kiwigrad-0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.27/PKG-INFO` & `kiwigrad-0.28/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.27
+Version: 0.28
 Summary: Mini deep learning framework
 Home-page: https://github.com/marcosalvalaggio/kiwigrad
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Kiwigrad
+## Kiwigrad
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) 
 
 *Despite lacking the ability to fly through the skies like **PyTorch** and **TensorFlow**, the Kiwigrad is still a formidable bird that is teeming with untapped potential waiting to be uncovered.* :wink:
 
 - [Kiwigrad](#kiwigrad)
-  - [Install](#install)
-  - [Functionalities](#functionalities)
-    - [Examples](#examples)
-  - [Todos](#todos)
+- [Install](#install)
+- [Functionalities](#functionalities)
+  - [Examples](#examples)
+- [Running test](#running-test)
 
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
 
 To install the current release,
 
@@ -89,11 +89,14 @@
 g.backward()
 print(f'{a.grad:.4f}') # prints 138.8338, i.e. the numerical value of dg/da
 print(f'{b.grad:.4f}') # prints 645.5773, i.e. the numerical value of dg/db
 
 draw_dot(g)
 ```
 
-## Todos
+## Running test
 
-* Include the activation functions tanh in the Value object.
+```console
+cd test 
+pytest .
+```
```

### Comparing `kiwigrad-0.27/README.md` & `kiwigrad-0.28/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Kiwigrad
+## Kiwigrad
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) 
 
 *Despite lacking the ability to fly through the skies like **PyTorch** and **TensorFlow**, the Kiwigrad is still a formidable bird that is teeming with untapped potential waiting to be uncovered.* :wink:
 
 - [Kiwigrad](#kiwigrad)
-  - [Install](#install)
-  - [Functionalities](#functionalities)
-    - [Examples](#examples)
-  - [Todos](#todos)
+- [Install](#install)
+- [Functionalities](#functionalities)
+  - [Examples](#examples)
+- [Running test](#running-test)
 
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
 
 To install the current release,
 
@@ -73,10 +73,13 @@
 g.backward()
 print(f'{a.grad:.4f}') # prints 138.8338, i.e. the numerical value of dg/da
 print(f'{b.grad:.4f}') # prints 645.5773, i.e. the numerical value of dg/db
 
 draw_dot(g)
 ```
 
-## Todos
+## Running test
 
-* Include the activation functions tanh in the Value object.
+```console
+cd test 
+pytest .
+```
```

### Comparing `kiwigrad-0.27/kiwigrad/engine.c` & `kiwigrad-0.28/kiwigrad/engine.c`

 * *Files 3% similar despite different names*

```diff
@@ -142,14 +142,22 @@
   Value *child = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 0));
   double x = ((Value *)self)->data;
   child->grad += (1 - pow(x, 2)) * ((Value *)self)->grad;
   Py_RETURN_NONE;
 }
 
 static PyObject *
+exp_backward(PyObject *self) {
+  Value *child = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 0));
+  double x = ((Value *)self)->data;
+  child->grad += x * ((Value *)self)->grad;
+  Py_RETURN_NONE;
+}
+
+static PyObject *
 add_backward(PyObject *self) {
   Value *child_1 = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 0));
   Value *child_2 = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 1));
   
   child_1->grad += ((Value *)self)->grad;
   child_2->grad += ((Value *)self)->grad;
   Py_RETURN_NONE;
@@ -178,15 +186,16 @@
 static BackwardFunction backward_methods[] = {
    &add_backward,
    &mul_backward,
    &pow_backward,
    &relu_backward,
    &sigmoid_backward,
    &log_backward,
-   &tanh_backward
+   &tanh_backward,
+   &exp_backward
   };
 
 static PyObject * Value_relu(PyObject *self) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   if (((Value *)self)->data < 0.0) {
     value->data = 0.0;
   } else {
@@ -231,14 +240,26 @@
   value->grad = 0.0;
   value->prev = PyTuple_Pack(1, self);
   value->op = PyUnicode_FromString("tanh");
   value->func_idx = 6;
   return (PyObject *)value;
 }
 
+static PyObject * Value_exp(PyObject *self) {
+  Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
+  double x = ((Value *)self)->data;
+  double t = exp(x);
+  value->data = t;
+  value->grad = 0.0;
+  value->prev = PyTuple_Pack(1, self);
+  value->op = PyUnicode_FromString("exp");
+  value->func_idx = 7;
+  return (PyObject *)value;
+}
+
 static void list_append(List *list, PyObject *value) {
   Node *node = malloc(sizeof(Node));
   node->value = ((Value *)value);
   node->next = NULL;
   if (!(list->head)) {
     node->prev = NULL;
     list->head = node;
@@ -290,14 +311,15 @@
 }
 
 static PyMethodDef Value_methods[] = {
     {"relu", (PyCFunction)Value_relu, METH_NOARGS, "ReLU"},
     {"sigmoid", (PyCFunction)Value_sigmoid, METH_NOARGS, "Sigmoid"},
     {"log", (PyCFunction)Value_log, METH_NOARGS, "Log"},
     {"tanh", (PyCFunction)Value_tanh, METH_NOARGS, "Tanh"},
+    {"exp", (PyCFunction)Value_exp, METH_NOARGS, "Exp"},
     // {"_backward", (PyCFunction)_backward, METH_NOARGS, "Backward"}, // DEBUG
     {"backward", (PyCFunction)backward, METH_NOARGS, "Backward"},
     {NULL}  /* Sentinel */
 };
 
 static PyMemberDef Value_members[] = {
    {"data", T_DOUBLE, offsetof(Value, data), 0, "Data"},
```

### Comparing `kiwigrad-0.27/kiwigrad/engine.py` & `kiwigrad-0.28/kiwigrad/engine.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.27/kiwigrad/graph.py` & `kiwigrad-0.28/kiwigrad/graph.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.27/kiwigrad/layers.py` & `kiwigrad-0.28/kiwigrad/layers.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.27/kiwigrad/neurons.py` & `kiwigrad-0.28/kiwigrad/neurons.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.27/kiwigrad/nn.py` & `kiwigrad-0.28/kiwigrad/nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,16 @@
             for neuron in layer.neurons:
                 weights.append([i.data for i in neuron.w])
                 weights.append(neuron.b.data)
         file_name = f'{save_name}.pkl'
         with open(file_name, 'wb') as f:
             pickle.dump(weights, f)
     
-    def load(self, save_name: str = "weights"):
-        file_name = f'{save_name}.pkl'
-        with open(file_name, 'rb') as f:
+    def load(self, path: str = "weights.pkl"):
+        with open(path, 'rb') as f:
             params = pickle.load(f)
         load_weights = []
         for param in params:
             if isinstance(param, list):
                 load_param = [Value(i) for i in param]
                 load_weights.append(load_param)
             else:
```

### Comparing `kiwigrad-0.27/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.28/kiwigrad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.27
+Version: 0.28
 Summary: Mini deep learning framework
 Home-page: https://github.com/marcosalvalaggio/kiwigrad
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Kiwigrad
+## Kiwigrad
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) 
 
 *Despite lacking the ability to fly through the skies like **PyTorch** and **TensorFlow**, the Kiwigrad is still a formidable bird that is teeming with untapped potential waiting to be uncovered.* :wink:
 
 - [Kiwigrad](#kiwigrad)
-  - [Install](#install)
-  - [Functionalities](#functionalities)
-    - [Examples](#examples)
-  - [Todos](#todos)
+- [Install](#install)
+- [Functionalities](#functionalities)
+  - [Examples](#examples)
+- [Running test](#running-test)
 
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
 
 To install the current release,
 
@@ -89,11 +89,14 @@
 g.backward()
 print(f'{a.grad:.4f}') # prints 138.8338, i.e. the numerical value of dg/da
 print(f'{b.grad:.4f}') # prints 645.5773, i.e. the numerical value of dg/db
 
 draw_dot(g)
 ```
 
-## Todos
+## Running test
 
-* Include the activation functions tanh in the Value object.
+```console
+cd test 
+pytest .
+```
```

### Comparing `kiwigrad-0.27/setup.py` & `kiwigrad-0.28/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools.extension import Extension
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='kiwigrad',
-      version='0.27',
+      version='0.28',
       description='Mini deep learning framework',
       author='Marco Salvalaggio',
       author_email='mar.salvalaggio@gmail.com',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/marcosalvalaggio/kiwigrad',
```

### Comparing `kiwigrad-0.27/test/test_value.py` & `kiwigrad-0.28/test/test_value.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from kiwigrad import Value
 import torch
 import unittest
 
 class TestValue(unittest.TestCase):
 
-    def test_activation_function(self):
+    def test_activation_functions(self):
         #kiwigrad
         a = Value(2.)
         b = a.sigmoid()
         c = b.relu()
-        c.backward()
+        d = c.tanh()
+        d.backward()
         #pytorch
         at = torch.tensor([2.], requires_grad=True)
         bt = at.sigmoid()
         ct = bt.relu()
-        ct.backward()
+        dt = ct.tanh()
+        dt.backward()
         at_g = float(at.grad)
         #test
         self.assertAlmostEqual(a.grad, at_g)
 
     def test_more_ops(self):
         #kiwigrad
         a = Value(3.)
```

