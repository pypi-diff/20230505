# Comparing `tmp/kiwigrad-0.26.tar.gz` & `tmp/kiwigrad-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.26.tar", last modified: Mon May  1 12:43:45 2023, max compression
+gzip compressed data, was "kiwigrad-0.27.tar", last modified: Thu May  4 22:36:50 2023, max compression
```

## Comparing `kiwigrad-0.26.tar` & `kiwigrad-0.27.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-01 12:43:45.944782 kiwigrad-0.26/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.26/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2128 2023-05-01 12:43:45.944530 kiwigrad-0.26/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1652 2023-04-29 16:01:59.000000 kiwigrad-0.26/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-01 12:43:45.940589 kiwigrad-0.26/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      297 2023-05-01 12:41:04.000000 kiwigrad-0.26/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10349 2023-05-01 12:19:55.000000 kiwigrad-0.26/kiwigrad/engine.c
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.26/kiwigrad/engine.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      968 2023-05-01 12:29:46.000000 kiwigrad-0.26/kiwigrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.26/kiwigrad/layers.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.26/kiwigrad/neurons.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.26/kiwigrad/nn.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.26/kiwigrad/skeleton.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-01 12:43:45.942997 kiwigrad-0.26/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2128 2023-05-01 12:43:45.000000 kiwigrad-0.26/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      355 2023-05-01 12:43:45.000000 kiwigrad-0.26/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-01 12:43:45.000000 kiwigrad-0.26/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-01 12:43:45.000000 kiwigrad-0.26/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-01 12:43:45.000000 kiwigrad-0.26/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-01 12:43:45.944864 kiwigrad-0.26/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      997 2023-05-01 12:41:42.000000 kiwigrad-0.26/setup.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-01 12:43:45.943514 kiwigrad-0.26/test/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1075 2023-05-01 10:14:41.000000 kiwigrad-0.26/test/test_value.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-04 22:36:50.938040 kiwigrad-0.27/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.27/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3223 2023-05-04 22:36:50.937201 kiwigrad-0.27/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2747 2023-05-01 22:05:50.000000 kiwigrad-0.27/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-04 22:36:50.928303 kiwigrad-0.27/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      297 2023-05-04 22:27:05.000000 kiwigrad-0.27/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11030 2023-05-04 22:29:02.000000 kiwigrad-0.27/kiwigrad/engine.c
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.27/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      968 2023-05-01 12:29:46.000000 kiwigrad-0.27/kiwigrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.27/kiwigrad/layers.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.27/kiwigrad/neurons.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.27/kiwigrad/nn.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.27/kiwigrad/skeleton.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-04 22:36:50.934769 kiwigrad-0.27/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3223 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      355 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-04 22:36:50.000000 kiwigrad-0.27/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-04 22:36:50.938305 kiwigrad-0.27/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      997 2023-05-04 22:27:00.000000 kiwigrad-0.27/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-04 22:36:50.936324 kiwigrad-0.27/test/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1075 2023-05-01 10:14:41.000000 kiwigrad-0.27/test/test_value.py
```

### Comparing `kiwigrad-0.26/LICENSE` & `kiwigrad-0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.26/PKG-INFO` & `kiwigrad-0.27/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,46 @@
-Metadata-Version: 2.1
-Name: kiwigrad
-Version: 0.26
-Summary: Mini deep learning framework
-Home-page: https://github.com/marcosalvalaggio/kiwigrad
-Author: Marco Salvalaggio
-Author-email: mar.salvalaggio@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Kiwigrad
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) 
 
+*Despite lacking the ability to fly through the skies like **PyTorch** and **TensorFlow**, the Kiwigrad is still a formidable bird that is teeming with untapped potential waiting to be uncovered.* :wink:
+
 - [Kiwigrad](#kiwigrad)
   - [Install](#install)
-  - [Kiwigrad Library](#kiwigrad-library)
+  - [Functionalities](#functionalities)
     - [Examples](#examples)
-  - [TODOS](#todos)
+  - [Todos](#todos)
 
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
 
 To install the current release,
 
 ```console
 pip install kiwigrad
 ```
 
-## Kiwigrad Library
+## Functionalities 
 
-Kiwigrad library is a modified version of the [micrograd](https://github.com/karpathy/micrograd) and the [minigrad](https://github.com/goktug97/minigrad) packages with additional features. The main features added to Kiwigrad are:
+Kiwigrad is a modified version of the [micrograd](https://github.com/karpathy/micrograd) and the [minigrad](https://github.com/goktug97/minigrad) packages with additional features. The main features added to Kiwigrad are:
 
 * Training is faster due to the C implementation of the Value object.
+* Tracing functionalities like the original [micrograd](https://github.com/karpathy/micrograd) package were added. An example of this can be seen in the [ops](examples/ops.ipynb) notebook.
 * Methods for saving and loading the weights of a trained model.
 * Support for RNN(1) feedforward neural networks.
 
 ### Examples
 
 * In the [examples](examples/) folder, you can find examples of models trained using the Kiwigrad library.
-* Here is a declaration example of an MLP net using Kiwigrad:
+* A declaration example of an MLP net using Kiwigrad:
   
 ```python 
 from kiwigrad import MLP, Layer
 
 class PotNet(MLP):
     def __init__(self):
         layers = [
@@ -61,12 +48,35 @@
             Layer(nin=16, nout=16, bias=True, activation="relu"),
             Layer(nin=16, nout=1, bias=True, activation="linear")
         ]
         super().__init__(layers=layers)
 
 model = PotNet()
 ```
+* Kiwigrad like [micrograd](https://github.com/karpathy/micrograd) and the [minigrad](https://github.com/goktug97/minigrad) comes with support for a number of possible operations:
+
+```python 
+from kiwigrad import Value, draw_dot
+
+a = Value(-4.0)
+b = Value(2.0)
+c = a + b
+d = a * b + b**3
+c += c + Value(1.)
+c += Value(1.) + c + (-a)
+d += d * Value(2) + (b + a).relu()
+d += Value(3.) * d + (b - a).relu()
+e = c - d
+f = e**2
+g = f / Value(2.0)
+g += Value(10.0) / f
+print(f'{g.data:.4f}') # prints 24.7041, the outcome of this forward pass
+g.backward()
+print(f'{a.grad:.4f}') # prints 138.8338, i.e. the numerical value of dg/da
+print(f'{b.grad:.4f}') # prints 645.5773, i.e. the numerical value of dg/db
 
-## TODOS
+draw_dot(g)
+```
 
-* Include the activation functions tanh in the Value object.
+## Todos
 
+* Include the activation functions tanh in the Value object.
```

### Comparing `kiwigrad-0.26/kiwigrad/engine.c` & `kiwigrad-0.27/kiwigrad/engine.c`

 * *Files 6% similar despite different names*

```diff
@@ -134,14 +134,22 @@
   double x = ((Value *)self)->data;
   double t = exp(x);
   child->grad += (pow(t, -1)) * ((Value *)self)->grad;
   Py_RETURN_NONE;
 }
 
 static PyObject *
+tanh_backward(PyObject *self) {
+  Value *child = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 0));
+  double x = ((Value *)self)->data;
+  child->grad += (1 - pow(x, 2)) * ((Value *)self)->grad;
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
@@ -169,15 +177,16 @@
 typedef PyObject * (*BackwardFunction)(PyObject *);
 static BackwardFunction backward_methods[] = {
    &add_backward,
    &mul_backward,
    &pow_backward,
    &relu_backward,
    &sigmoid_backward,
-   &log_backward
+   &log_backward,
+   &tanh_backward
   };
 
 static PyObject * Value_relu(PyObject *self) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   if (((Value *)self)->data < 0.0) {
     value->data = 0.0;
   } else {
@@ -210,14 +219,25 @@
   value->grad = 0.0;
   value->prev = PyTuple_Pack(1, self);
   value->op = PyUnicode_FromString("log");
   value->func_idx = 5;
   return (PyObject *)value;
 }
 
+static PyObject * Value_tanh(PyObject *self) {
+  Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
+  double x = ((Value *)self)->data;
+  double t = (exp(2*x) - 1)/(exp(2*x) + 1);
+  value->data = t;
+  value->grad = 0.0;
+  value->prev = PyTuple_Pack(1, self);
+  value->op = PyUnicode_FromString("tanh");
+  value->func_idx = 6;
+  return (PyObject *)value;
+}
 
 static void list_append(List *list, PyObject *value) {
   Node *node = malloc(sizeof(Node));
   node->value = ((Value *)value);
   node->next = NULL;
   if (!(list->head)) {
     node->prev = NULL;
@@ -269,14 +289,15 @@
   Py_RETURN_NONE;
 }
 
 static PyMethodDef Value_methods[] = {
     {"relu", (PyCFunction)Value_relu, METH_NOARGS, "ReLU"},
     {"sigmoid", (PyCFunction)Value_sigmoid, METH_NOARGS, "Sigmoid"},
     {"log", (PyCFunction)Value_log, METH_NOARGS, "Log"},
+    {"tanh", (PyCFunction)Value_tanh, METH_NOARGS, "Tanh"},
     // {"_backward", (PyCFunction)_backward, METH_NOARGS, "Backward"}, // DEBUG
     {"backward", (PyCFunction)backward, METH_NOARGS, "Backward"},
     {NULL}  /* Sentinel */
 };
 
 static PyMemberDef Value_members[] = {
    {"data", T_DOUBLE, offsetof(Value, data), 0, "Data"},
```

### Comparing `kiwigrad-0.26/kiwigrad/engine.py` & `kiwigrad-0.27/kiwigrad/engine.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.26/kiwigrad/graph.py` & `kiwigrad-0.27/kiwigrad/graph.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.26/kiwigrad/layers.py` & `kiwigrad-0.27/kiwigrad/layers.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.26/kiwigrad/neurons.py` & `kiwigrad-0.27/kiwigrad/neurons.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.26/kiwigrad/nn.py` & `kiwigrad-0.27/kiwigrad/nn.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.26/setup.py` & `kiwigrad-0.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools.extension import Extension
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='kiwigrad',
-      version='0.26',
+      version='0.27',
       description='Mini deep learning framework',
       author='Marco Salvalaggio',
       author_email='mar.salvalaggio@gmail.com',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/marcosalvalaggio/kiwigrad',
```

### Comparing `kiwigrad-0.26/test/test_value.py` & `kiwigrad-0.27/test/test_value.py`

 * *Files identical despite different names*

